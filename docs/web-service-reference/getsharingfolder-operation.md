---
title: Opération GetSharingFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- GetSharingFolder
api_type:
- schema
ms.assetid: 75fee92a-a7f8-4a62-ad2b-17acbaada186
description: L’opération GetSharingFolder obtient l’identificateur de dossier local d’un dossier partagé spécifié.
ms.openlocfilehash: 20ee49b85d026ec2c14794599e0713b9939384eb
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515823"
---
# <a name="getsharingfolder-operation"></a>Opération GetSharingFolder

**L’opération GetSharingFolder** obtient l’identificateur de dossier local d’un dossier partagé spécifié. 
  
## <a name="soap-headers"></a>En-têtes SOAP

**L’opération GetSharingFolder** peut utiliser les en-têtes SOAP répertoriés et décrits dans le tableau suivant. 
  
|**Header**|**Élément**|**Description**|
|:-----|:-----|:-----|
|RequestVersion  <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifie la version de schéma pour la demande d’opération.  <br/> |
|ServerVersion  <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifie la version du serveur qui a répondu à la demande.  <br/> |
   
## <a name="getsharingfolder-request-example"></a>Exemple de requête GetSharingFolder

### <a name="getting-the-local-folder-identifier-by-specifying-the-sharedfolderid-element-of-the-folder-being-shared"></a>Obtention de l’identificateur de dossier local en spécifiant l’élément SharedFolderId du dossier partagé

L’exemple de code suivant montre comment créer une demande pour obtenir l’identificateur du dossier local qui correspond au dossier partagé. Le dossier partagé est identifié par l’adresse SMTP de la boîte aux lettres qui contient le dossier partagé et par l’élément [SharedFolderId](sharedfolderid.md) qui représente l’identificateur de ce dossier. Dans cet exemple, le dossier partagé appartient à user1@contoso.com. 
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010"/>
  </soap:Header>
  <soap:Body>
    <m:GetSharingFolder>
      <m:SmtpAddress>user1@contoso.com</m:SmtpAddress>
      <m:SharedFolderId>AAMkA=</m:SharedFolderId>
    </m:GetSharingFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="getting-the-local-folder-identifier-by-specifying-the-datatype-element-of-the-folder-being-shared"></a>Obtention de l’identificateur de dossier local en spécifiant l’élément DataType du dossier partagé

L’exemple de code suivant montre comment créer une demande pour obtenir l’identificateur du dossier local qui correspond au dossier partagé. Le dossier partagé est identifié par l’adresse SMTP de la boîte aux lettres qui contient le dossier en cours de partage et par l’élément [DataType](datatype.md) qui représente le type de données dans ce dossier. Dans cet exemple, le dossier partagé est le dossier Contacts qui appartient à user1@contoso.com. 
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010"/>
  </soap:Header>
  <soap:Body>
    <m:GetSharingFolder>
      <m:SmtpAddress>user1@contoso.com</m:SmtpAddress>
      <m:DataType>Contacts</m:DataType>
    </m:GetSharingFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Commentaires

Pour plus d’informations sur les valeurs possibles de **l’élément DataType,** voir [DataType](datatype.md).
  
## <a name="successful-getsharingfolder-response"></a>Réponse GetSharingFolder réussie

### <a name="description"></a>Description

L’exemple suivant montre une réponse réussie à **une demande GetSharingFolder.** **L’attribut ID** de [l’élément SharingFolderId](sharingfolderid.md) représente l’identificateur du dossier local dans la relation de partage. 
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="0" 
                         MajorBuildNumber="639" 
                         MinorBuildNumber="11" 
                         Version="Exchange2010" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetSharingFolderResponseMessage ResponseClass="Success"
                                xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
                                xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                                xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseCode>NoError</m:ResponseCode>
      <m:SharingFolderId Id="AAMkAD=" ChangeKey="AwAAA=" />
    </GetSharingFolderResponseMessage>
  </soap:Body>
</soap:Envelope>
```

## <a name="getsharingfolder-error-response"></a>Réponse d’erreur GetSharingFolder

### <a name="description"></a>Description

L’exemple suivant montre une réponse d’erreur à **une demande GetSharingFolder.** Dans cet exemple, l’erreur s’est produite, car la demande spécifie à la fois les éléments [SharingFolderId](sharingfolderid.md) et [DataType.](datatype.md) Notez qu’un seul ou l’autre de ces deux éléments peut être spécifié, mais pas les deux. 
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="0" 
                         MajorBuildNumber="639" 
                         MinorBuildNumber="11" 
                         Version="Exchange2010" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetSharingFolderResponseMessage ResponseClass="Error" 
                                xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
                                xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                                xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:MessageText>Either DataType or SharedFolderId must be specified, but not both.</m:MessageText>
      <m:ResponseCode>ErrorInvalidGetSharingFolderRequest</m:ResponseCode>
      <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
    </GetSharingFolderResponseMessage>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>Voir aussi



[GetSharingFolder](getsharingfolder.md)
  
[GetSharingFolderType](https://msdn.microsoft.com/library/ExchangeWebServices.GetSharingFolderType.aspx)
  
[GetSharingFolderResponseMessage](getsharingfolderresponsemessage.md)
  
[GetSharingFolderResponseMessageType](https://msdn.microsoft.com/library/ExchangeWebServices.GetSharingFolderResponseMessageType.aspx)


[Opérations EWS dans Exchange](ews-operations-in-exchange.md)
  
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

