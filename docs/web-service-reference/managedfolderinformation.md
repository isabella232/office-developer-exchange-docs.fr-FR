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
ms.openlocfilehash: ef46e2e0db440de2a8acae8316ce98d11bd6710e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828341"
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

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[CanDelete](candelete.md) <br/> |Indique si un dossier géré peut être supprimé par un client.  <br/> |
|[CanRenameOrMove](canrenameormove.md) <br/> |Indique si un dossier géré donné peut être renommé ou déplacé par le client.  <br/> |
|[MustDisplayComment](mustdisplaycomment.md) <br/> |Indique si le commentaire de dossier géré doit être affiché.  <br/> |
|[HasQuota](hasquota.md) <br/> |Indique si le dossier géré a un quota.  <br/> |
|[IsManagedFoldersRoot](ismanagedfoldersroot.md) <br/> |Indique si le dossier géré est la racine de tous les dossiers gérés.  <br/> |
|[ManagedFolderId](managedfolderid.md) <br/> |Contient l’ID de dossier du dossier géré.  <br/> |
|[Commentaire](comment.md) <br/> |Contient le commentaire qui est associé à un dossier géré.  <br/> |
|[StorageQuota](storagequota.md) <br/> |Décrit le quota de stockage pour le dossier géré.  <br/> |
|[FolderSize](foldersize.md) <br/> |Décrit la taille totale de tout le contenu d’un dossier géré.  <br/> |
|[Page d’accueil](homepage.md) <br/> |Spécifie l’URL qui sera la page d’accueil par défaut pour le dossier géré.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Folder](folder.md) <br/> |Représente un dossier dans la banque d’informations Exchange. Les dossiers personnalisés gérés peuvent être uniquement les sous-dossiers du dossier nommé **Dossiers gérés**.  <br/> |
|[CalendarFolder](calendarfolder.md) <br/> |Non applicable.  <br/> |
|[ContactsFolder](contactsfolder.md) <br/> |Non applicable.  <br/> |
|[SearchFolder](searchfolder.md) <br/> |Non applicable.  <br/> |
|[Dossier tâches](tasksfolder.md) <br/> |Non applicable.  <br/> |
   
## <a name="remarks"></a>Notes

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération CreateManagedFolder](createmanagedfolder-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)


[Ajout de dossiers gérés](http://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

