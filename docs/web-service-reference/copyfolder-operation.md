---
title: CopyFolder, opération
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CopyFolder
api_type:
- schema
ms.assetid: c7ea0d68-9793-4144-b378-d99536776db9
description: L’opération CopyFolder copie les dossiers d’une boîte aux lettres.
ms.openlocfilehash: 1f9a7a3f3ede2d3cf8f9d41677d8ce0487266f17
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468893"
---
# <a name="copyfolder-operation"></a>CopyFolder, opération

L’opération CopyFolder copie les dossiers d’une boîte aux lettres.
  
## <a name="using-the-copyfolder-operation"></a>Utilisation de l’opération CopyFolder

L’opération CopyFolder est semblable à l' [opération MoveFolder](movefolder-operation.md). Il copie les dossiers identifiés et renvoie l' **ID** et **ChangeKey** des dossiers copiés. 
  
## <a name="copyfolder-request-example"></a>Exemple de requête CopyFolder

### <a name="description"></a>Description

L’exemple de requête CopyFolder suivant montre comment copier des dossiers dans le dossier boîte de réception.
  
> [!NOTE]
> La valeur de l’attribut **ID** de l’élément [FolderId](folderid.md) a été raccourcie pour des raisons de lisibilité. 
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CopyFolder xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ToFolderId>
        <t:DistinguishedFolderId Id="inbox"/>
      </ToFolderId>
      <FolderIds>
        <t:FolderId Id="AS4A=" ChangeKey="fsVU4=="/>
        <t:FolderId Id="AS4AU=" ChangeKey="fsVU4o=="/>
      </FolderIds>
    </CopyFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Commentaires

Les dossiers peuvent être identifiés par l’élément [DistinguishedFolderId](distinguishedfolderid.md) ou l’élément [FolderId](folderid.md) pour une utilisation dans les éléments [ToFolderId](tofolderid.md) ou [FolderIds](folderids.md) . 
  
### <a name="request-elements"></a>Demander des éléments

Les éléments suivants sont utilisés dans la demande :
  
- [CopyFolder](copyfolder.md)
    
- [ToFolderId](tofolderid.md)
    
- [DistinguishedFolderId](distinguishedfolderid.md)
    
- [FolderIds](folderids.md)
    
- [FolderId](folderid.md)
    
> [!NOTE]
> Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé. 
  
Pour rechercher d’autres options pour le message de demande de l’opération CopyFolder, explorez la hiérarchie du schéma. Commencez par l’élément [CopyFolder](copyfolder.md) . 
  
## <a name="successful-copyfolder-response"></a>Réponse CopyFolder réussie

### <a name="description"></a>Description

L’exemple suivant montre une réponse réussie à la demande CopyFolder. 
  
> [!NOTE]
> L’ID de dossier et la clé de modification ont été raccourcies afin de préserver la lisibilité. 
  
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
    <CopyFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CopyFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="AS4AUn=" ChangeKey="fsVU4o==" />
            </t:Folder>
          </m:Folders>
        </m:CopyFolderResponseMessage>
      </m:ResponseMessages>
    </CopyFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comment"></a>Commentaire

L’élément [FolderId](folderid.md) renvoyé dans la réponse représente le dossier qui a été copié dans le nouvel emplacement de dossier. 
  
### <a name="response-elements"></a>Éléments Response

Les éléments suivants sont utilisés dans la réponse :
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [CopyFolderResponse](copyfolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [CopyFolderResponseMessage](copyfolderresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [Dossiers](folders-ex15websvcsotherref.md)
    
- [Folder](folder.md)
    
- [FolderId](folderid.md)
    
Pour rechercher d’autres options pour le message de réponse de l’opération CopyFolder, explorez la hiérarchie du schéma. Commencez par l’élément [CopyFolderResponse](copyfolderresponse.md) . 
  
## <a name="copyfolder-error-response"></a>Réponse d’erreur CopyFolder

### <a name="description"></a>Description

L’exemple suivant montre une réponse d’erreur à une demande CopyFolder. L’erreur s’est produite car un dossier portant le même nom d’affichage existe déjà.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CopyFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CopyFolderResponseMessage ResponseClass="Error">
          <m:MessageText>The move or copy operation failed.</m:MessageText>
          <m:ResponseCode>ErrorMoveCopyFailed</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Folders />
        </m:CopyFolderResponseMessage>
      </m:ResponseMessages>
    </CopyFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a>Éléments de réponse d’erreur

Les éléments suivants sont utilisés dans la réponse d'erreur :
  
- [CopyFolderResponse](copyfolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [CopyFolderResponseMessage](copyfolderresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
- [Dossiers](folders-ex15websvcsotherref.md)
    
Pour rechercher d’autres options pour le message d’erreur de l’opération CopyFolder, explorez la hiérarchie du schéma. Commencez par l’élément [CopyFolderResponse](copyfolderresponse.md) . 
  
## <a name="see-also"></a>Voir aussi

- [Opération MoveFolder](movefolder-operation.md)
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

