---
title: Opération CreateFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CreateFolder
api_type:
- schema
ms.assetid: 6f6c334c-b190-4e55-8f0a-38f2a018d1b3
description: L’opération CreateFolder crée des dossiers, des dossiers de calendrier, des dossiers de contacts, des dossiers de tâches et des dossiers de recherche.
ms.openlocfilehash: 1b6259ba15e31ee9976c08afa8971ead9a1d5b16
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515851"
---
# <a name="createfolder-operation"></a>Opération CreateFolder

L’opération CreateFolder crée des dossiers, des dossiers de calendrier, des dossiers de contacts, des dossiers de tâches et des dossiers de recherche.
  
## <a name="createfolder-request-example"></a>Exemple de requête CreateFolder

### <a name="description"></a>Description

L’exemple suivant d’une demande CreateFolder montre comment former une demande pour créer deux nouveaux dossiers à la racine de la boîte aux lettres.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateFolder xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ParentFolderId>
        <t:DistinguishedFolderId Id="msgfolderroot"/>
      </ParentFolderId>
      <Folders>
        <t:Folder>
          <t:DisplayName>Folder1</t:DisplayName>
        </t:Folder>
        <t:Folder>
          <t:DisplayName>Folder2</t:DisplayName>
        </t:Folder>
      </Folders>
    </CreateFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a>Éléments de demande

Les éléments suivants sont utilisés dans la demande :
  
- [CreateFolder](createfolder.md)
    
- [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)
    
- [DistinguishedFolderId](distinguishedfolderid.md)
    
- [Dossiers](folders-ex15websvcsotherref.md)
    
- [Folder](folder.md)
    
- [DisplayName (chaîne)](displayname-string.md)
    
> [!NOTE]
> Le schéma qui décrit ces éléments se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute MicrosoftExchange Server 2007 sur qui le rôle serveur d’accès au client est installé. 
  
Pour rechercher d’autres options pour le message de demande de l’opération CreateFolder, explorez la hiérarchie de schéma. Commencez à [l’élément CreateFolder.](createfolder.md) 
  
> [!NOTE]
> Si vous créez un dossier de recherche avec une restriction à l’aide de la propriété **calendar:Organizer,** un appel de dossier Get ultérieur retournera la restriction avec la propriété **message:from** à sa place. Ces deux propriétés sont m mas ex la m me propri t MAPI sous-jacente. 
  
L’opération CreateFolder prend en charge la création d’une classe de dossier personnalisée uniquement lorsque vous créez le dossier à l’aide d’un élément de type de dossier générique et définissez **l’élément FolderClass.** 
  
## <a name="successful-createfolder-response-example"></a>Exemple de réponse CreateFolder réussie

### <a name="description"></a>Description

L’exemple suivant montre une réponse réussie à la demande CreateFolder. Dans cet exemple, la réponse renvoie les identificateurs des nouveaux dossiers.
  
> [!NOTE]
> L’ID de dossier et la touche de modification ont été raccourcis pour préserver la lisibilité. 
  
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
    <CreateFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="AS4AUn==" />
            </t:Folder>
          </m:Folders>
        </m:CreateFolderResponseMessage>
        <m:CreateFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="AS4AUn==" />
            </t:Folder>
          </m:Folders>
        </m:CreateFolderResponseMessage>
      </m:ResponseMessages>
    </CreateFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a>Éléments de réponse réussis

Les éléments suivants sont utilisés dans la réponse :
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [CreateFolderResponse](createfolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [CreateFolderResponseMessage](createfolderresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [Dossiers](folders-ex15websvcsotherref.md)
    
- [Folder](folder.md)
    
- [FolderId](folderid.md)
    
Pour rechercher d’autres options pour le message de réponse de l’opération CreateFolder, explorez la hiérarchie de schéma. Commencez à [l’élément CreateFolderResponse.](createfolderresponse.md) 
  
## <a name="createfolder-error-response"></a>Réponse d’erreur CreateFolder

### <a name="description"></a>Description

L’exemple suivant montre une réponse d’erreur à une demande CreateFolder.
  
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
    <CreateFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateFolderResponseMessage ResponseClass="Error">
          <m:MessageText>A folder with the specified name already exists.</m:MessageText>
          <m:ResponseCode>ErrorFolderExists</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Folders />
        </m:CreateFolderResponseMessage>
      </m:ResponseMessages>
    </CreateFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a>Éléments de réponse d’erreur

Les éléments suivants sont utilisés dans la réponse d'erreur :
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [CreateFolderResponse](createfolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [CreateFolderResponseMessage](createfolderresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
- [Dossiers](folders-ex15websvcsotherref.md)
    
Pour rechercher d’autres options pour le message de réponse d’erreur de l’opération CreateFolder, explorez la hiérarchie de schéma. Commencez à [l’élément CreateFolderResponse.](createfolderresponse.md) 
  
## <a name="see-also"></a>Voir aussi



[Opération FindItem](finditem-operation.md)
  
[Opération FindFolder](findfolder-operation.md)
  
 **CreateFolderType**


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)


[Création de dossiers (Exchange Web Services)](https://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

