---
title: ManagedFolderInformation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ManagedFolderInformation
api_type:
- schema
ms.assetid: dea980eb-8303-47fe-a380-20a8efc9ead6
description: L’élément ManagedFolderInformation contient des informations sur un dossier personnalisé géré.
ms.openlocfilehash: ce15dcb15cccdce253494beefd2f4a2a7a0c0ad8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44450948"
---
# <a name="managedfolderinformation"></a>ManagedFolderInformation

L’élément **ManagedFolderInformation** contient des informations sur un dossier personnalisé géré. 
  
```xml
<ManagedFolderInformation>
   <CanDelete/>
   <CanRenameOrMove/>
   <MustDisplayComment/>
   <HasQuota/>
   <IsManagedFoldersRoot/>
   <ManagedFolderId/>
   <Comment/>
   <StorageQuota/>
   <FolderSize/>
   <HomePage/>
</ManagedFolderInformation>
```

 **ManagedFolderInformationType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[CanDelete](candelete.md) <br/> |Indique si un dossier géré peut être supprimé par un client.  <br/> |
|[CanRenameOrMove](canrenameormove.md) <br/> |Indique si un dossier géré donné peut être renommé ou déplacé par le client.  <br/> |
|[MustDisplayComment](mustdisplaycomment.md) <br/> |Indique si le commentaire du dossier géré doit être affiché.  <br/> |
|[HasQuota](hasquota.md) <br/> |Indique si le dossier géré a un quota.  <br/> |
|[IsManagedFoldersRoot](ismanagedfoldersroot.md) <br/> |Indique si le dossier géré est la racine de tous les dossiers gérés.  <br/> |
|[ManagedFolderId](managedfolderid.md) <br/> |Contient l’ID de dossier du dossier géré.  <br/> |
|[Comment](comment.md) <br/> |Contient le commentaire associé à un dossier géré.  <br/> |
|[StorageQuota](storagequota.md) <br/> |Décrit le quota de stockage pour le dossier géré.  <br/> |
|[FolderSize](foldersize.md) <br/> |Décrit la taille totale de tout le contenu d’un dossier géré.  <br/> |
|[HomePage](homepage.md) <br/> |Spécifie l’URL qui sera la page d’accueil par défaut pour le dossier géré.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Folder](folder.md) <br/> |Représente un dossier dans la Banque d’Exchange. Les dossiers personnalisés gérés ne peuvent être que des sous-dossiers du dossier nommé **Managed Folders**.  <br/> |
|[CalendarFolder](calendarfolder.md) <br/> |Non applicable  <br/> |
|[ContactsFolder](contactsfolder.md) <br/> |Non applicable  <br/> |
|[SearchFolder](searchfolder.md) <br/> |Non applicable  <br/> |
|[TasksFolder](tasksfolder.md) <br/> |Non applicable  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération CreateManagedFolder](createmanagedfolder-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)


[Ajout de dossiers gérés](https://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

