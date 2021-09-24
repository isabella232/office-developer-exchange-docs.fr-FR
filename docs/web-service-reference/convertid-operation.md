---
title: Opération ConvertId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ConvertId
api_type:
- schema
ms.assetid: 47d96cf6-9e2f-4fc0-9682-7258d3fbf918
description: Trouvez des informations sur l’opération ConvertId EWS.
ms.openlocfilehash: 04f20d8446ab3117adb3f00ea17f93c068eeffb9
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59536630"
---
# <a name="convertid-operation"></a>Opération ConvertId

Trouvez des informations sur **l’opération ConvertId** EWS. 
  
L’opération **ConvertId** Exchange Web Services (EWS) convertit les identificateurs d’élément et de dossier entre les formats acceptés par Exchange Online, Exchange Online dans le cadre de Office 365 et les versions sur site de Exchange à partir de Exchange Server 2013. 
  
## <a name="using-the-convertid-operation"></a>Utilisation de l’opération ConvertId
<a name="bk_usingConvertId"> </a>

Vous pouvez convertir les identificateurs suivants à l’aide de **l’opération ConvertId** : 
  
- Format d’identificateur pour EWS dans la version initiale de Exchange 2007. Cela est représenté par la valeur `EwsLegacyId` d’éumération dans [l’éumération IdFormat.](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx) 
    
- Format d’identificateur pour EWS Exchange 2007 SP1 ou Exchange 2010. Ceci est représenté par la valeur  `EwsId` d’éumération [dans IdFormat](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx).
    
- Identificateur MAPI, comme dans la **PR_ENTRYID** propriété. Cela est représenté par la valeur `EntryId` d’éumération dans [l’éumération IdFormat.](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx) 
    
- Identificateur d’événement de calendrier de disponibilité. Il s’agit d’une représentation codée hexadécimale de la **propriété PR_ENTRYID.** Ceci est représenté par la valeur  `HexEntryId` d’éumération [dans IdFormat](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx).
    
- Identificateur Exchange store. Ceci est représenté par la valeur  `StoreId` d’éumération [dans IdFormat](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx). **L’opération ConvertId** ne convertit pas les identificateurs de dossier public de l’identificateur EWS en identificateur de la boutique. 
    
- Identificateur Outlook Web App. Ceci est représenté par la valeur  `OwaId` d’éumération [dans IdFormat](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx)
    
    La transmission des URL créées à partir de cet identificateur vers Outlook Web App n’est pas prise en charge. L Outlook’identificateur Web App est applicable Exchange 2007 et Exchange 2010. Outlook Web App pour Exchange Online et les versions de Exchange à partir de Exchange Server 2013 utilise des identificateurs EWS.
    
L’opération **ConvertId** ne fonctionne pas comme prévu lors de la conversion des identificateurs de dossier public de l’identificateur EWS en identificateur de magasin dans Exchange Online et Exchange 2013. Vous pouvez mettre à jour manuellement l’identificateur renvoyé comme solution de contournement. Pour mettre à jour manuellement l’identificateur : 
  
1. Dans le code de votre application, déterminez si l’élément/dossier cible se trouve dans un dossier public. 
    
2. Décodez la chaîne d’identificateur codée en Base64.
    
3. Vérifiez que le type d’byte (21e byte) a une valeur de 7. La valeur 7 indique que l’identificateur est au format incorrect.
    
4. Ignorez les quatre premiers octets. Elles doivent être définies sur zéro.
    
5. Mettez à jour les 16 octets suivants avec le GUID suivant : 1A447390AA6611CD9BC800AA002FC45A
    
6. Mettez à jour l’byte suivant (type byte) avec la valeur 9.
    
7. Changez l’identificateur en chaîne codée en Base64.
    
> [!NOTE]
> **L’opération ConvertId** valide qu’une adresse SMTP donnée a un format valide. L’opération ne détermine pas si une adresse SMTP représente une boîte aux lettres valide. 
  
**L’opération ConvertId** peut utiliser les en-têtes SOAP répertoriés dans le tableau suivant. 
  
**Tableau 1. En-têtes SOAP d’opération ConvertId**

|**Header**|**Élément**|**Description**|
|:-----|:-----|:-----|
|Emprunt d’identité  <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Identifie l’utilisateur dont l’application cliente usurpe l’identité. Ceci s’applique à une demande.  <br/> |
|RequestVersion  <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifie la version de schéma de la demande d’opération Applicable à une demande.  <br/> |
|ServerVersion  <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifie la version du serveur qui a répondu à la demande. Ceci s’applique à une réponse.  <br/> |
   
## <a name="convertid-operation-request-example"></a>Exemple de demande d’opération ConvertId
<a name="bk_usingConvertId"> </a>

L’exemple suivant **d’une demande ConvertId** montre comment convertir un identificateur EWS en identificateur Outlook Web App. 
  
[L’élément RequestServerVersion](requestserverversion.md) dans l’en-tête SOAP doit être Exchange2007_SP1 ou version ultérieure pour que cette opération fonctionne. 
  
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

L’exemple suivant montre une réponse réussie à **une demande ConvertId.** Cet exemple de réponse contient un identificateur Outlook Web App. 
  
> [!NOTE]
> L’Outlook Web App a été raccourci pour préserver la lisibilité. 
  
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

L’exemple suivant montre la réponse à une demande qui contient le mauvais type de format d’identificateur.
  
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

Le format d’identificateur EWS a changé entre la version initiale de Exchange 2007 et Exchange 2007 Service Pack 1 (SP1). Exchange Online dans le cadre des versions Office 365, Exchange Online et sur site de Exchange à partir de Exchange 2010 utilisent le même format d’identificateur que Exchange 2007 SP1.
  
**L’opération ConvertId** convertit les identificateurs de dossier public de l’identificateur EWS en identificateur de magasin dans Exchange 2007 et Exchange 2010. 
  
## <a name="see-also"></a>Voir aussi
<a name="bk_ConvertIdVersionDiff"> </a>

- [Conversion d’identificateurs](https://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)
    
- [ConvertIdType](https://msdn.microsoft.com/library/ExchangeWebServices.ConvertIdType.aspx)
    
- [ConvertId](https://msdn.microsoft.com/library/ExchangeWebServices.ExchangeServiceBinding.ConvertId.aspx)
    

