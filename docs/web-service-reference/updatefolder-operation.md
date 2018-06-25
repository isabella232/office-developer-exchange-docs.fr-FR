---
title: Opération UpdateFolder
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateFolder
api_type:
- schema
ms.assetid: 3494c996-b834-4813-b1ca-d99642d8b4e7
description: 'L’opération UpdateFolder est utilisée pour modifier les propriétés d’un élément existant dans la banque d’informations Exchange. Chaque opération UpdateFolder comprend les éléments suivants :'
ms.openlocfilehash: b33937bb09f0dcbe3d3ed61bbf5233423f320d9c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838860"
---
# <a name="updatefolder-operation"></a>Opération UpdateFolder

L’opération UpdateFolder est utilisée pour modifier les propriétés d’un élément existant dans la banque d’informations Exchange. Chaque opération UpdateFolder comprend les éléments suivants :
  
- Élément [FolderId](folderid.md) qui spécifie un dossier à mettre à jour. 
    
- Chemin d’accès interne d’un élément dans le dossier, tel que spécifié par la forme de dossier, qui spécifie les données à mettre à jour.
    
- Un dossier qui contient la nouvelle valeur du champ mise à jour, si la mise à jour n’est pas une suppression.
    
## <a name="remarks"></a>Remarques

Trois actions de mise à jour de base peuvent être effectuées sur un élément. Ces actions sont répertoriées dans le tableau suivant.
  
|**Action**|**Description**|
|:-----|:-----|
|Ajout  <br/> |L’action d’ajout ajoute des données à une propriété existante. Il conserve les données qui s’y trouve. Ajouter n’est pas applicable à toutes les propriétés.  <br/> |
|Set  <br/> |L’action Définir remplace les données d’une propriété s’il contient des données, ou crée la propriété et lui affecte la valeur s’il n’existe pas. L’action Définir concerne uniquement les propriétés accessibles en écriture.  <br/> |
|Suppression  <br/> |L’action Supprimer Supprime une propriété d’un dossier. Cela diffère de la définition d’une valeur vide. Lorsque vous avez terminé, la propriété n’existe pas pour le dossier. Supprimer n’est pas applicable aux propriétés accessibles en écriture.  <br/> |
   
## <a name="updatefolder-request-example"></a>Exemple de requête UpdateFolder

### <a name="description"></a>Description

Une demande UpdateFolder l’exemple suivant montre comment mettre à jour un nom complet du dossier. 
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateFolder xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

Cet exemple modifie le nom complet du dossier pour le nouveau nom de dossier.
  
> [!NOTE]
> Les valeurs de l' **Id** et les attributs de l’élément [FolderId](folderid.md) **ChangeKey** ont été raccourcies pour des raisons de lisibilité. 
  
### <a name="request-elements"></a>Éléments de la demande

Les éléments suivants sont utilisés dans la demande :
  
- [UpdateFolder](updatefolder.md)
    
- [FolderChanges](folderchanges.md)
    
- [FolderChange](folderchange.md)
    
- [FolderId](folderid.md)
    
- [Mises à jour (élément)](updates-item.md)
    
- [SetFolderField](setfolderfield.md)
    
- [FieldURI](fielduri.md)
    
- [Folder](folder.md)
    
- [DisplayName (chaîne)](displayname-string.md)
    
Voir le schéma pour les éléments supplémentaires que vous pouvez utiliser pour créer une demande UpdateFolder.
  
> [!NOTE]
> L’emplacement par défaut du schéma est dans le répertoire virtuel EWS sur l’ordinateur sur lequel le rôle de serveur d’accès au Client est installé. 
  
## <a name="updatefolder-response-example"></a>Exemple de réponse UpdateFolder

### <a name="description"></a>Description

L’exemple suivant montre une réponse positive à la demande UpdateFolder. Dans cet exemple, la nouvelle clé de modification est retournée pour refléter l’état de mise à jour du dossier.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <UpdateFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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
> L’ID de dossier et la clé de modification ont été réduits afin de préserver la lisibilité. 
  
L’ID de dossier est renvoyé dans la réponse représente le dossier mises à jour.
  
### <a name="successful-response-elements"></a>Éléments de réponse réussie

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

L’exemple suivant montre une réponse d’erreur à une demande de UpdateFolder.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <UpdateFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

Cet exemple montre une réponse d’erreur est dû à un attribut **ChangeKey** non valide dans la demande. 
  
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

