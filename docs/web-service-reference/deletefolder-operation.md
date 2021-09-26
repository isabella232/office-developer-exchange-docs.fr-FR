---
title: Opération DeleteFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DeleteFolder
api_type:
- schema
ms.assetid: b0f92682-4895-4bcf-a4a1-e4c2e8403979
description: L’opération DeleteFolder supprime des dossiers d’une boîte aux lettres.
ms.openlocfilehash: fdd8519adbf9e0112f5fdd6a411dd6e7710f7d37
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59545432"
---
# <a name="deletefolder-operation"></a>Opération DeleteFolder

**L’opération DeleteFolder** supprime des dossiers d’une boîte aux lettres. 
  
## <a name="deletefolder-request-example"></a>Exemple de requête DeleteFolder

### <a name="description"></a>Description

L’exemple suivant **d’une demande DeleteFolder** montre comment former une demande de suppression d’un dossier. 
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <DeleteFolder xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                  DeleteType="HardDelete" >
      <FolderIds>
        <t:FolderId Id="AS4AUnVz=" />
      </FolderIds>
    </DeleteFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Commentaires

Cet exemple effectue une suppression en dur sur le dossier.
  
> [!NOTE]
> L’ID de dossier a été raccourci pour préserver la lisibilité. 
  
### <a name="request-elements"></a>Éléments de demande

Les éléments suivants sont utilisés dans la demande :
  
- [DeleteFolder](deletefolder.md)
    
- [FolderIds](folderids.md)
    
- [FolderId](folderid.md)
    
> [!NOTE]
> Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur exécutant Microsoft Exchange Server 2010 sur qui le rôle serveur d’accès au client est installé. 
  
Pour rechercher d’autres options pour le message de demande de **l’opération DeleteFolder,** explorez la hiérarchie de schéma. Commencez à [l’élément DeleteFolder.](deletefolder.md) 
  
## <a name="successful-deletefolder-response"></a>Réponse DeleteFolder réussie

### <a name="description"></a>Description

L’exemple suivant montre une réponse réussie à **la demande DeleteFolder.** 
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <DeleteFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:DeleteFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:DeleteFolderResponseMessage>
      </m:ResponseMessages>
    </DeleteFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="response-elements"></a>Éléments de réponse

Les éléments suivants sont utilisés dans la réponse :
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [DeleteFolderResponse](deletefolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [DeleteFolderResponseMessage](deletefolderresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
Pour rechercher d’autres options pour le message de réponse de **l’opération DeleteFolder,** explorez la hiérarchie de schéma. Commencez à [l’élément DeleteFolderResponse.](deletefolderresponse.md) 
  
## <a name="deletefolder-error-response"></a>Réponse d’erreur DeleteFolder

### <a name="description"></a>Description

L’exemple suivant montre une réponse d’erreur à **une demande DeleteFolder.** L’erreur est due à une demande de suppression d’un dossier qui n’était pas présent dans la boîte aux lettres. 
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <DeleteFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:DeleteFolderResponseMessage ResponseClass="Error">
          <m:MessageText>The specified object was not found in the store.</m:MessageText>
          <m:ResponseCode>ErrorItemNotFound</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:DeleteFolderResponseMessage>
      </m:ResponseMessages>
    </DeleteFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Commentaires

**L’opération DeleteFolder** ne peut pas être utilisée sur des dossiers spécifiques. 
  
### <a name="error-response-elements"></a>Éléments de réponse d’erreur

Les éléments suivants sont utilisés dans la réponse d'erreur :
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [DeleteFolderResponse](deletefolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [DeleteFolderResponseMessage](deletefolderresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
Pour rechercher d’autres options pour le message de réponse d’erreur de **l’opération DeleteFolder,** explorez la hiérarchie de schéma. Commencez à [l’élément DeleteFolderResponse.](deletefolderresponse.md) 
  
## <a name="see-also"></a>Voir aussi

- [Éléments XML EWS dans Exchange](ews-xml-elements-in-exchange.md)
- [Suppression de dossiers](https://msdn.microsoft.com/library/1958add5-5071-4239-adb2-40f7a7d74aee%28Office.15%29.aspx)

