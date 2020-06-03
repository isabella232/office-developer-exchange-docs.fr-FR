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
description: Trouvez des informations sur l’opération EWS ConvertId.
ms.openlocfilehash: 36bd47d3fc7c7ca7cea7b38222abb25fba6074ac
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44452551"
---
# <a name="convertid-operation"></a>Opération ConvertId

Trouvez des informations sur l’opération EWS **ConvertId** . 
  
L’opération EWS (Exchange Web Services) **ConvertId** convertit les identificateurs d’élément et de dossier entre les formats acceptés par Exchange Online, Exchange Online dans le cadre d’Office 365 et les versions locales d’Exchange à partir d’exchange Server 2013. 
  
## <a name="using-the-convertid-operation"></a>Utilisation de l’opération ConvertId
<a name="bk_usingConvertId"> </a>

Vous pouvez convertir les identificateurs suivants à l’aide de l’opération **ConvertId** : 
  
- Format d’identificateur pour EWS dans la version initiale d’Exchange 2007. Cette valeur est représentée par la `EwsLegacyId` valeur d’énumération dans l’énumération [IdFormat](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx) . 
    
- Format d’identificateur pour EWS dans Exchange 2007 SP1 ou Exchange 2010. Cette valeur est représentée par la `EwsId` valeur d’énumération dans [IdFormat](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx).
    
- Identificateur MAPI, comme dans la propriété **PR_ENTRYID** . Cette valeur est représentée par la `EntryId` valeur d’énumération dans l’énumération [IdFormat](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx) . 
    
- Identificateur d’événement de calendrier de disponibilité. Il s’agit d’une représentation codée en hexadécimal de la propriété **PR_ENTRYID** . Cette valeur est représentée par la `HexEntryId` valeur d’énumération dans [IdFormat](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx).
    
- Identificateur de la banque Exchange. Cette valeur est représentée par la `StoreId` valeur d’énumération dans [IdFormat](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx). L’opération **ConvertId** ne convertit pas les identificateurs de dossiers publics de l’identificateur EWS en identificateur de magasin. 
    
- Identificateur d’Outlook Web App. Cette valeur est représentée par la `OwaId` valeur d’énumération dans [IdFormat](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx)
    
    La transmission des URL créées à partir de cet identificateur vers Outlook Web App n’est pas prise en charge. L’identificateur d’Outlook Web App est applicable à Exchange 2007 et Exchange 2010. Outlook Web App pour Exchange Online et les versions d’Exchange commençant par Exchange Server 2013 utilisent des identificateurs EWS.
    
L’opération **ConvertId** ne fonctionne pas comme prévu lors de la conversion d’identificateurs de dossiers publics de l’identificateur EWS en identificateur de magasin dans Exchange Online et Exchange 2013. Vous pouvez mettre à jour manuellement l’identificateur renvoyé sous forme de solution de contournement. Pour mettre à jour manuellement l’identificateur : 
  
1. Dans le code de votre application, déterminez si l’élément/dossier cible se trouve dans un dossier public. 
    
2. Décodez la chaîne d’identificateur codée en base64.
    
3. Vérifiez que le type Byte (21ème octet) a la valeur 7. Une valeur de 7 indique que l’identificateur est dans un format incorrect.
    
4. Ignorez les quatre premiers octets. Elles doivent être définies sur zéro.
    
5. Mettez à jour les 16 octets suivants avec le GUID suivant : 1A447390AA6611CD9BC800AA002FC45A
    
6. Mettez à jour l’octet suivant (type Byte) avec une valeur de 9.
    
7. Remplacez l’identificateur par une chaîne codée en base 64.
    
> [!NOTE]
> L’opération **ConvertId** vérifie qu’une adresse SMTP donnée a un format valide. L’opération ne détermine pas si une adresse SMTP représente une boîte aux lettres valide. 
  
L’opération **ConvertId** peut utiliser les en-têtes SOAP répertoriés dans le tableau suivant. 
  
**Tableau 1. En-têtes SOAP d’opération ConvertId**

|**Header**|**Élément**|**Description**|
|:-----|:-----|:-----|
|Emprunt d’identité  <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Identifie l’utilisateur qui emprunte l’identité de l’application cliente. Ceci s’applique à une demande.  <br/> |
|RequestVersion  <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifie la version de schéma de la demande d’opération applicable à une demande.  <br/> |
|ServerVersion  <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifie la version du serveur qui a répondu à la demande. Ceci s’applique à une réponse.  <br/> |
   
## <a name="convertid-operation-request-example"></a>Exemple de requête d’opération ConvertId
<a name="bk_usingConvertId"> </a>

L’exemple de requête **ConvertId** suivant montre comment convertir un identificateur EWS en identificateur d’Outlook Web App. 
  
L’élément [RequestServerVersion](requestserverversion.md) de l’en-tête SOAP doit être défini sur Exchange2007_SP1 ou une version ultérieure pour que cette opération fonctionne. 
  
> [!NOTE]
> Identificateur de l'élément a été raccourcie afin de préserver la lisibilité. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010"/>
  </soap:Header>
  <soap:Body>
    <ConvertId xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               DestinationFormat="OwaId">
      <SourceIds>
        <t:AlternateId Format="EwsId" Id="AAMkAGZhN2IxYTA0LWNiNzItN="
                       Mailbox="user1@example.com"/>
      </SourceIds>
    </ConvertId>
  </soap:Body>
</soap:Envelope>
```

## <a name="convertid-operation-response-example"></a>Exemple de réponse d’opération ConvertId
<a name="bk_usingConvertId"> </a>

L’exemple suivant montre une réponse réussie à une demande **ConvertId** . Cet exemple de réponse contient un identificateur Outlook Web App. 
  
> [!NOTE]
> L’identificateur d’Outlook Web App a été raccourci pour conserver la lisibilité. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="1" 
                         MajorBuildNumber="191" MinorBuildNumber="0" 
                         Version="Exchange2010" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ConvertIdResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

## <a name="convertid-operation-error-response-example"></a>Exemple de réponse d’erreur d’opération ConvertId
<a name="bk_usingConvertId"> </a>

L’exemple suivant montre la réponse à une demande contenant un type de format d’identificateur incorrect.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <ServerVersionInfo MajorVersion="8" MinorVersion="1" 
                       MajorBuildNumber="206" MinorBuildNumber="0"
                       Version="Exchange2010" 
                       xmlns="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ConvertIdResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

Le format d’identificateur EWS a changé entre la version initiale d’Exchange 2007 et Exchange 2007 Service Pack 1 (SP1). Exchange Online dans le cadre d’Office 365, Exchange Online et les versions locales d’Exchange à partir d’Exchange 2010 utilisent le même format d’identificateur que celui utilisé par Exchange 2007 SP1.
  
L’opération **ConvertId** convertit des identificateurs de dossiers publics de l’identificateur EWS en identificateur de magasin dans Exchange 2007 et Exchange 2010. 
  
## <a name="see-also"></a>Voir aussi
<a name="bk_ConvertIdVersionDiff"> </a>

- [Conversion des identificateurs](https://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)
    
- [ConvertIdType](https://msdn.microsoft.com/library/ExchangeWebServices.ConvertIdType.aspx)
    
- [ConvertId](https://msdn.microsoft.com/library/ExchangeWebServices.ExchangeServiceBinding.ConvertId.aspx)
    

