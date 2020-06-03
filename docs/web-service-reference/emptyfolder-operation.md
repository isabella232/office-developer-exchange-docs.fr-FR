---
title: Opération EmptyFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 98161486-e2f2-480f-8d5d-708ba81b208a
description: L’opération EmptyFolder vide les dossiers dans une boîte aux lettres. Si vous le souhaitez, cette opération vous permet de supprimer les sous-dossiers du dossier spécifié. Lors de la suppression d’un sous-dossier, le sous-dossier et les messages qu’il contient sont supprimés.
ms.openlocfilehash: 1913db74d33f1e6750cd158df5870f257d0e7839
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530683"
---
# <a name="emptyfolder-operation"></a>Opération EmptyFolder

L’opération **EmptyFolder** vide les dossiers dans une boîte aux lettres. Si vous le souhaitez, cette opération vous permet de supprimer les sous-dossiers du dossier spécifié. Lors de la suppression d’un sous-dossier, le sous-dossier et les messages qu’il contient sont supprimés. 
  
## <a name="emptyfolder-request-example"></a>Exemple de requête EmptyFolder

### <a name="description"></a>Description

L’exemple de requête **EmptyFolder** suivant montre comment créer une demande de vidage d’un dossier. Cet exemple supprime tous les sous-dossiers du dossier identifié. 
  
> [!NOTE]
> Les valeurs des attributs **ID** et **ChangeKey** de l’élément [FolderId](folderid.md) ont été raccourcies pour des raisons de lisibilité. 
  
### <a name="code"></a>Code

```XML
<soap:Envelope xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version ="Exchange2010_SP1"/>
    </soap:Header>
    <soap:Body>
      <m:EmptyFolder DeleteType="HardDelete" DeleteSubFolders="true">
        <m:FolderIds>
          <t:FolderId Id="AQMkADhhOGU0"  ChangeKey="AQAAABYAAABsMB" />
        </m:FolderIds>
      </m:EmptyFolder>
    </soap:Body>
</soap:Envelope>

```

### <a name="comments"></a>Commentaires

Cet exemple effectue une suppression définitive sur le dossier.
  
Les dossiers peuvent être identifiés par l’élément [DistinguishedFolderId](distinguishedfolderid.md) ou l’élément [FolderId](folderid.md) pour une utilisation dans l’élément [FolderIds](folderids.md) . 
  
### <a name="request-elements"></a>Demander des éléments

Les éléments suivants sont utilisés dans la demande :
  
- [EmptyFolder](emptyfolder.md)
    
- [FolderIds](folderids.md)
    
- [FolderId](folderid.md)
    
## <a name="successful-emptyfolder-response"></a>Réponse EmptyFolder réussie

### <a name="description"></a>Description

L’exemple suivant montre une réponse réussie à la demande **EmptyFolder** . 
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="1" 
                         MajorBuildNumber="164" 
                         MinorBuildNumber="0" 
                         Version="Exchange2010_SP1"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:EmptyFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                           xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:EmptyFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:EmptyFolderResponseMessage>
      </m:ResponseMessages>
    </m:EmptyFolderResponse>
  </s:Body>
</s:Envelope>

```

### <a name="successful-response-elements"></a>Éléments de réponse réussis

Les éléments suivants sont utilisés dans la réponse :
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [EmptyFolderResponse](emptyfolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [EmptyFolderResponseMessage](emptyfolderresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
## <a name="emptyfolder-error-response"></a>Réponse d’erreur EmptyFolder

### <a name="description"></a>Description

L’exemple suivant montre une réponse d’erreur à une demande **EmptyFolder** . L’erreur a été créée car l’opération a essayé de vider un dossier qui n’a pas été trouvé dans la Banque d’Exchange. 
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
            MinorVersion="1" 
            MajorBuildNumber="164" 
            MinorBuildNumber="0" 
            Version="Exchange2010_SP1" 
            xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
            xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
            xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
            xmlns:xsd="http://www.w3.org/2001/XMLSchema" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
            xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetFolderResponse 
          xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetFolderResponseMessage ResponseClass="Error">
          <m:MessageText>Id is malformed.</m:MessageText>
          <m:ResponseCode>ErrorInvalidIdMalformed</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Folders />
        </m:GetFolderResponseMessage>
      </m:ResponseMessages>
    </m:GetFolderResponse>
  </s:Body>
</s:Envelope>
```

### <a name="error-response-elements"></a>Éléments de réponse d’erreur

Les éléments suivants sont utilisés dans la réponse :
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [GetFolderResponse](getfolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [GetFolderResponseMessage](getfolderresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
- [Dossiers](folders-ex15websvcsotherref.md)
    
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

