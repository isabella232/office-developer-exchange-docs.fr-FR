---
title: Opération ConvertId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConvertId
api_type:
- schema
ms.assetid: 47d96cf6-9e2f-4fc0-9682-7258d3fbf918
description: Opération de recherche plus d’informations sur la ConvertId EWS.
ms.openlocfilehash: 5f1bcd8a9f0adc25b7c598ef10cc6bb139dfe02d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755652"
---
# <a name="convertid-operation"></a>Opération ConvertId

Trouvez des informations sur l’opération EWS **ConvertId** . 
  
L’opération de Exchange Web Services (EWS) **ConvertId** convertit les identificateurs d’éléments et dossiers entre les formats acceptés par Exchange Online, Exchange Online dans le cadre d’Office 365 et les versions d’Exchange commençant par le serveur Exchange local 2013. 
  
## <a name="using-the-convertid-operation"></a>Utilisation de l’opération ConvertId
<a name="bk_usingConvertId"> </a>

Vous pouvez convertir les identificateurs suivants à l’aide de l’opération **ConvertId** : 
  
- Le format d’identificateur pour EWS dans la version initiale d’Exchange 2007. Il est représenté par le `EwsLegacyId` valeur d’énumération dans l’énumération [IdFormat](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx) . 
    
- Le format d’identificateur pour EWS dans Exchange 2007 SP1 ou Exchange 2010. Il est représenté par le `EwsId` valeur d’énumération dans [IdFormat](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx).
    
- L’identificateur MAPI, comme illustré à la propriété **PR_ENTRYID** . Il est représenté par le `EntryId` valeur d’énumération dans l’énumération [IdFormat](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx) . 
    
- L’identificateur d’événement disponibilité de calendrier. Il s’agit d’une représentation de la propriété **PR_ENTRYID** codé en hexadécimal. Il est représenté par le `HexEntryId` valeur d’énumération dans [IdFormat](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx).
    
- L’identificateur de la banque Exchange. Il est représenté par le `StoreId` valeur d’énumération dans [IdFormat](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx). L’opération **ConvertId** ne convertit pas les identificateurs de dossier public à partir de l’identificateur EWS à l’identificateur de la banque. 
    
- L’identificateur d’Outlook Web App. Il est représenté par le `OwaId` valeur d’énumération dans [IdFormat](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx)
    
    Le passage d’URL qui sont créés à partir de cet identificateur à Outlook Web App n’est pas pris en charge. L’identificateur d’Outlook Web App s’applique à Exchange 2007 et Exchange 2010. Outlook Web App pour Exchange Online et les versions d’Exchange commençant par Exchange Server 2013 utilise les identificateurs EWS.
    
L’opération **ConvertId** ne fonctionne pas comme prévu lors de la conversion des identificateurs de dossier public à partir de l’identificateur EWS à l’identificateur de la banque dans Exchange Online et Exchange 2013. Vous pouvez mettre à jour manuellement l’identificateur qui est renvoyé sous la forme d’une solution de contournement. Mettre à jour manuellement l’identificateur : 
  
1. Dans votre code d’application, déterminez si le dossier cible élément est dans un dossier public. 
    
2. Décodez la chaîne d’identificateur codé en Base64.
    
3. Vérifiez que l’octet de type a la valeur 7 (21 octet). Une valeur de 7 indique que l’identificateur est dans un format incorrect.
    
4. Ignorer les quatre premiers octets. Elles doivent être définies sur zéro.
    
5. Mettre à jour les 16 octets avec le GUID suivant : 1A447390AA6611CD9BC800AA002FC45A
    
6. Mettre à jour le prochain octet (type octet) avec une valeur de 9.
    
7. Modifier l’identificateur d’une chaîne codée en Base64.
    
> [!NOTE]
> L’opération **ConvertId** valide qu’une adresse SMTP donnée a un format valide. L’opération ne détermine pas si une adresse SMTP représente une boîte aux lettres valide. 
  
L’opération **ConvertId** permettre utiliser les en-têtes SOAP qui sont répertoriés dans le tableau suivant. 
  
**Le tableau 1. En-têtes SOAP ConvertId opération**

|**Header**|**Élément**|**Description**|
|:-----|:-----|:-----|
|Emprunt d’identité  <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Identifie l’utilisateur emprunte l’identité de l’application cliente. Ceci s’applique à une demande.  <br/> |
|RequestVersion  <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifie la version du schéma pour la requête d’opération qu'applicable à une demande.  <br/> |
|ServerVersion  <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifie la version du serveur qui a répondu à la demande. Cela s’applique à une réponse.  <br/> |
   
## <a name="convertid-operation-request-example"></a>Exemple de requête d’opération ConvertId
<a name="bk_usingConvertId"> </a>

Une demande de **ConvertId** l’exemple suivant montre comment convertir un identificateur EWS un identificateur d’Outlook Web App. 
  
L’élément [RequestServerVersion](requestserverversion.md) dans l’en-tête SOAP doit être défini à Exchange2007_SP1 ou version ultérieure pour cette opération. 
  
> [!NOTE]
> Identificateur de l'élément a été raccourcie afin de préserver la lisibilité. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010"/>
  </soap:Header>
  <soap:Body>
    <ConvertId xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               DestinationFormat="OwaId">
      <SourceIds>
        <t:AlternateId Format="EwsId" Id="AAMkAGZhN2IxYTA0LWNiNzItN="
                       Mailbox="user1@example.com"/>
      </SourceIds>
    </ConvertId>
  </soap:Body>
</soap:Envelope>
```

## <a name="convertid-operation-response-example"></a>Exemple de réponse ConvertId opération
<a name="bk_usingConvertId"> </a>

L’exemple suivant montre une réponse positive à une demande de **ConvertId** . Cet exemple montre comment réponse contient un identificateur d’Outlook Web App. 
  
> [!NOTE]
> L’identificateur d’Outlook Web App a été raccourcie afin de préserver la lisibilité. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="1" 
                         MajorBuildNumber="191" MinorBuildNumber="0" 
                         Version="Exchange2010" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ConvertIdResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseMessages>
        <ConvertIdResponseMessage ResponseClass="Success">
          <ResponseCode>NoError</ResponseCode>
          <AlternateId xsi:type="t:AlternateIdType" Format="OwaId" Id="RgAAAAAS2%2" 
                         Mailbox="user@example.com" />
        </ConvertIdResponseMessage>
      </ResponseMessages>
    </ConvertIdResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="convertid-operation-error-response-example"></a>Exemple de réponse d’erreur opération ConvertId
<a name="bk_usingConvertId"> </a>

L’exemple suivant montre la réponse à une demande qui contient un type de format de l’identificateur.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <ServerVersionInfo MajorVersion="8" MinorVersion="1" 
                       MajorBuildNumber="206" MinorBuildNumber="0"
                       Version="Exchange2010" 
                       xmlns="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ConvertIdResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseMessages>
        <ConvertIdResponseMessage ResponseClass="Error">
          <MessageText>Id is malformed.</MessageText>
          <ResponseCode>ErrorInvalidIdMalformed</ResponseCode>
          <DescriptiveLinkKey>0</DescriptiveLinkKey>
        </ConvertIdResponseMessage>
      </ResponseMessages>
    </ConvertIdResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="version-differences"></a>Différences entre les versions
<a name="bk_ConvertIdVersionDiff"> </a>

Le format d’identificateur EWS modifié entre la version initiale d’Exchange 2007 et Exchange 2007 Service Pack 1 (SP1). Versions locales d’Exchange commençant par Exchange 2010, Exchange Online dans le cadre d’Office 365 et Exchange Online utilisent le même format d’identificateur qui utilise Exchange 2007 SP1.
  
L’opération **ConvertId** convertit les identificateurs de dossier public à partir de l’identificateur EWS à l’identificateur de la banque dans Exchange 2007 et Exchange 2010. 
  
## <a name="see-also"></a>Voir aussi
<a name="bk_ConvertIdVersionDiff"> </a>

- [Conversion des identificateurs](http://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)
    
- [ConvertIdType](https://msdn.microsoft.com/library/ExchangeWebServices.ConvertIdType.aspx)
    
- [ConvertId](https://msdn.microsoft.com/library/ExchangeWebServices.ExchangeServiceBinding.ConvertId.aspx)
    

