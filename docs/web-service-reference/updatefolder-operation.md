---
title: Opération UpdateFolder
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- UpdateFolder
api_type:
- schema
ms.assetid: 3494c996-b834-4813-b1ca-d99642d8b4e7
description: 'L’opération UpdateFolder est utilisée pour modifier les propriétés d’un élément existant dans la Exchange store. Chaque opération UpdateFolder se compose des opérations suivantes :'
ms.openlocfilehash: be8e39e13681cea34e312158c348c60a94374bec
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541762"
---
# <a name="updatefolder-operation"></a>Opération UpdateFolder

L’opération UpdateFolder est utilisée pour modifier les propriétés d’un élément existant dans la Exchange store. Chaque opération UpdateFolder se compose des opérations suivantes :
  
- Élément [FolderId](folderid.md) qui spécifie un dossier à mettre à jour. 
    
- Chemin d’accès interne d’un élément dans le dossier, tel que spécifié par la forme du dossier, qui spécifie les données à mettre à jour.
    
- Dossier qui contient la nouvelle valeur du champ mis à jour, si la mise à jour n’est pas une suppression.
    
## <a name="remarks"></a>Remarques

Trois actions de mise à jour de base peuvent être effectuées sur un élément. Ces actions sont répertoriées dans le tableau suivant.
  
|**Action**|**Description**|
|:-----|:-----|
|Ajout  <br/> |L’action Ajouter ajoute des données à une propriété existante. Il conserve les données qui sont actuellement là. Append n’est pas applicable à toutes les propriétés.  <br/> |
|Set  <br/> |L’action de jeu remplace les données d’une propriété si elle contient des données, ou crée la propriété et définit sa valeur si elle n’existe pas. L’action définie s’applique uniquement aux propriétés accessibles en writable.  <br/> |
|Supprimer  <br/> |L’action de suppression supprime une propriété d’un dossier. Cela est différent de la définition d’une valeur vide. Lorsque vous avez terminé, la propriété n’existe pas pour le dossier. La suppression s’applique uniquement aux propriétés accessibles en writable.  <br/> |
   
## <a name="updatefolder-request-example"></a>Exemple de requête UpdateFolder

### <a name="description"></a>Description

L’exemple suivant d’une demande UpdateFolder montre comment mettre à jour un nom complet de dossier. 
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateFolder xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <FolderChanges>
        <t:FolderChange>
          <t:FolderId Id="AScA" ChangeKey="GO3u/"/>
          <t:Updates>
            <t:SetFolderField>
              <t:FieldURI FieldURI="folder:DisplayName"/>
              <t:Folder>
                <t:DisplayName>NewFolderName</t:DisplayName>
              </t:Folder>
            </t:SetFolderField>
          </t:Updates>
        </t:FolderChange>
      </FolderChanges>
    </UpdateFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Commentaires

Cet exemple modifie le nom complet du dossier en NewFolderName.
  
> [!NOTE]
> Les valeurs des **attributs Id** et **ChangeKey** de l’élément [FolderId](folderid.md) ont été raccourcies pour des raisons de lisibilité. 
  
### <a name="request-elements"></a>Éléments de demande

Les éléments suivants sont utilisés dans la demande :
  
- [UpdateFolder](updatefolder.md)
    
- [FolderChanges](folderchanges.md)
    
- [FolderChange](folderchange.md)
    
- [FolderId](folderid.md)
    
- [Updates (Folder)](updates-folder.md)
    
- [SetFolderField](setfolderfield.md)
    
- [FieldURI](fielduri.md)
    
- [Folder](folder.md)
    
- [DisplayName (chaîne)](displayname-string.md)
    
Consultez le schéma pour obtenir des éléments supplémentaires que vous pouvez utiliser pour former une demande UpdateFolder.
  
> [!NOTE]
> L’emplacement par défaut du schéma se trouve dans le répertoire virtuel EWS sur l’ordinateur sur qui le rôle serveur d’accès au client est installé. 
  
## <a name="updatefolder-response-example"></a>Exemple de réponse UpdateFolder

### <a name="description"></a>Description

L’exemple suivant montre une réponse réussie à la demande UpdateFolder. Dans cet exemple, la nouvelle touche de modification est renvoyée pour refléter l’état mis à jour du dossier.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <UpdateFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:UpdateFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="AAAlAFVz" ChangeKey="AQAAAB" />
            </t:Folder>
          </m:Folders>
        </m:UpdateFolderResponseMessage>
      </m:ResponseMessages>
    </UpdateFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Commentaires

> [!NOTE]
> L’ID de dossier et la touche de modification ont été raccourcis pour préserver la lisibilité. 
  
L’ID de dossier renvoyé dans la réponse représente le dossier mis à jour.
  
### <a name="successful-response-elements"></a>Éléments de réponse réussis

Les éléments suivants sont utilisés dans la réponse :
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [UpdateFolderResponse](updatefolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [UpdateFolderResponseMessage](updatefolderresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [Dossiers](folders-ex15websvcsotherref.md)
    
- [Folder](folder.md)
    
- [FolderId](folderid.md)
    
## <a name="updatefolder-error-response-example"></a>Exemple de réponse d’erreur UpdateFolder

### <a name="description"></a>Description

L’exemple suivant montre une réponse d’erreur à une demande UpdateFolder.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <UpdateFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:UpdateFolderResponseMessage ResponseClass="Error">
          <m:MessageText>The change key is invalid.</m:MessageText>
          <m:ResponseCode>ErrorInvalidChangeKey</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Folders />
        </m:UpdateFolderResponseMessage>
      </m:ResponseMessages>
    </UpdateFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Commentaires

Cet exemple montre une réponse d’erreur causée par un attribut **ChangeKey** non valide dans la demande. 
  
### <a name="error-response-elements"></a>Éléments de réponse d’erreur

Les éléments suivants sont utilisés dans la réponse d'erreur :
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [UpdateFolderResponse](updatefolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [UpdateFolderResponseMessage](updatefolderresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
- [Dossiers](folders-ex15websvcsotherref.md)
    
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

