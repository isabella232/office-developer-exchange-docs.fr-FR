---
title: Opération CreateFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateFolder
api_type:
- schema
ms.assetid: 6f6c334c-b190-4e55-8f0a-38f2a018d1b3
description: L’opération CreateFolder crée des dossiers, des dossiers de calendrier, des dossiers de contacts, des dossiers de tâches et des dossiers de recherche.
ms.openlocfilehash: 125a6d212e5eaf85ace71c048de809f3a05ba9b6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457549"
---
# <a name="createfolder-operation"></a>Opération CreateFolder

L’opération CreateFolder crée des dossiers, des dossiers de calendrier, des dossiers de contacts, des dossiers de tâches et des dossiers de recherche.
  
## <a name="createfolder-request-example"></a>Exemple de demande CreateFolder

### <a name="description"></a>Description

L’exemple de requête CreateFolder suivant montre comment créer deux nouveaux dossiers dans la racine de la boîte aux lettres.
  
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

### <a name="request-elements"></a>Demander des éléments

Les éléments suivants sont utilisés dans la demande :
  
- [CreateFolder](createfolder.md)
    
- [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)
    
- [DistinguishedFolderId](distinguishedfolderid.md)
    
- [Dossiers](folders-ex15websvcsotherref.md)
    
- [Folder](folder.md)
    
- [DisplayName (chaîne)](displayname-string.md)
    
> [!NOTE]
> Le schéma qui décrit ces éléments se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute MicrosoftExchange Server 2007 sur lequel le rôle de serveur d’accès au client est installé. 
  
Pour rechercher d’autres options pour le message de demande de l’opération CreateFolder, explorez la hiérarchie du schéma. Commencez par l’élément [CreateFolder](createfolder.md) . 
  
> [!NOTE]
> Si vous créez un dossier de recherche avec une restriction à l’aide de la propriété **Calendar : Organizer** , un nouvel appel de dossier Get renverra la restriction avec la propriété **message : from** à sa place. Ces deux propriétés sont mappées sur la même propriété MAPI sous-jacente. 
  
L’opération CreateFolder prend en charge la création d’une classe de dossier personnalisée uniquement lorsque vous créez le dossier à l’aide d’un élément de type de dossier générique et que vous définissez l’élément **FolderClass** . 
  
## <a name="successful-createfolder-response-example"></a>Exemple de réponse CreateFolder réussie

### <a name="description"></a>Description

L’exemple suivant montre une réponse réussie à la demande CreateFolder. Dans cet exemple, la réponse renvoie les identificateurs des nouveaux dossiers.
  
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
    
Pour rechercher d’autres options pour le message de réponse de l’opération CreateFolder, explorez la hiérarchie du schéma. Commencez par l’élément [CreateFolderResponse](createfolderresponse.md) . 
  
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
    
Pour rechercher d’autres options pour le message d’erreur de réponse de l’opération CreateFolder, explorez la hiérarchie du schéma. Commencez par l’élément [CreateFolderResponse](createfolderresponse.md) . 
  
## <a name="see-also"></a>Voir aussi



[Opération FindItem](finditem-operation.md)
  
[Opération FindFolder](findfolder-operation.md)
  
 **CreateFolderType**


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)


[Création de dossiers (services Web Exchange)](https://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

