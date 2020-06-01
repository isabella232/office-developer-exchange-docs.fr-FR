---
title: DistinguishedFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DistinguishedFolderId
api_type:
- schema
ms.assetid: 50018162-2941-4227-8a5b-d6b4686bb32f
description: L’élément DistinguishedFolderId identifie les dossiers qui peuvent être référencés par leur nom. Si vous n’utilisez pas cet élément, vous devez utiliser l’élément FolderId pour identifier un dossier.
ms.openlocfilehash: be883cbca00910b24e4c45ba047803e5a5024566
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462695"
---
# <a name="distinguishedfolderid"></a>DistinguishedFolderId

L’élément **DistinguishedFolderId** identifie les dossiers qui peuvent être référencés par leur nom. Si vous n’utilisez pas cet élément, vous devez utiliser l’élément [FolderId](folderid.md) pour identifier un dossier. 
  
```XML
<DistinguishedFolderId Id="" ChangeKey="">
   <Mailbox/>
</DistinguishedFolderId>
```

 **DistinguishedFolderIdType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**Id** <br/> |Contient une chaîne qui identifie un dossier par défaut. Cet attribut est obligatoire.  <br/> |
|**ChangeKey** <br/> |Contient une chaîne qui identifie la version d’un dossier identifiée par l’attribut **ID** . Cet attribut est facultatif. Utilisez cet attribut pour vous assurer que la version correcte d’un dossier est utilisée.  <br/> |
   
#### <a name="id-attribute-values"></a>Valeurs de l’attribut ID

|**Valeur**|**Description**|
|:-----|:-----|
|calendrier  <br/> |Représente le dossier de calendrier.  <br/> |
|contacts  <br/> |Représente le dossier contacts.  <br/> |
|deleteditems  <br/> |Représente le dossier éléments supprimés.  <br/> |
|brouillons  <br/> |Représente le dossier Brouillons.  <br/> |
|boîtederéception  <br/> |Représente le dossier boîte de réception.  <br/> |
|n  <br/> |Représente le dossier journal.  <br/> |
|notes  <br/> |Représente le dossier Notes.  <br/> |
|Boîte d’envoi  <br/> |Représente le dossier boîte d’envoi.  <br/> |
|sentitems  <br/> |Représente le dossier éléments envoyés.  <br/> |
|tasks  <br/> |Représente le dossier tâches.  <br/> |
|msgfolderroot  <br/> |Représente la racine du dossier de messages.  <br/> |
|root  <br/> |Représente la racine de la boîte aux lettres.  <br/> |
|junkemail  <br/> |Représente le dossier courrier indésirable.  <br/> |
|searchfolders  <br/> |Représente le dossier dossiers de recherche.  <br/> |
|voicemail  <br/> |Représente le dossier de messagerie vocale.  <br/> |
|recoverableitemsroot  <br/> |Représente le dossier racine de la benne.  <br/> |
|recoverableitemsdeletions  <br/> |Représente le dossier suppressions de benne.  <br/> |
|recoverableitemsversions  <br/> |Représente le dossier des versions de benne.  <br/> |
|recoverableitemspurges  <br/> |Représente le dossier purges de benne.  <br/> |
|archiveroot  <br/> |Représente le dossier d’archivage racine.  <br/> |
|archivemsgfolderroot  <br/> |Représente le dossier de messages d’archive racine.  <br/> |
|archivedeleteditems  <br/> |Représente le dossier éléments supprimés de l’archive.  <br/> |
|archiveinbox  <br/> |Représente le dossier boîte de réception d’archivage. Les versions d’Exchange commençant par le numéro de Build 15.00.0913.09 incluent cette valeur.  <br/> |
|archiverecoverableitemsroot  <br/> |Représente le dossier racine des éléments récupérables.  <br/> |
|archiverecoverableitemsdeletions  <br/> |Représente le dossier de suppression des éléments récupérables.  <br/> |
|archiverecoverableitemsversions  <br/> |Représente le dossier Archives des éléments récupérables.  <br/> |
|archiverecoverableitemspurges  <br/> |Représente le dossier purges d’éléments récupérables.  <br/> |
|syncissues  <br/> |Représente le dossier problèmes de synchronisation.  <br/> |
|conflits  <br/> |Représente le dossier conflits.  <br/> |
|localfailures  <br/> |Représente le dossier défaillances locales.  <br/> |
|serverfailures  <br/> |Représente le dossier défaillances du serveur.  <br/> |
|recipientcache  <br/> |Représente le dossier de cache de destinataires.  <br/> |
|QuickContacts  <br/> |Représente le dossier contacts rapides.  <br/> |
|conversationhistory  <br/> |Représente le dossier historique des conversations.  <br/> |
|adminauditlogs  <br/> |Représente le dossier journaux d’audit de l’administrateur.  <br/> |
|todosearch  <br/> |Représente le dossier de recherche todo.  <br/> |
|MyContacts  <br/> |Représente le dossier Mes contacts.  <br/> |
|Active  <br/> |Représente le dossier répertoire.  <br/> |
|imcontactlist  <br/> |Représente le dossier de liste de contacts de messagerie instantanée.  <br/> |
|peopleconnect  <br/> |Représente le dossier se connecter.  <br/> |
|favoris  <br/> |Représente le dossier Favoris.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Boîte aux lettres](mailbox.md) <br/> |Identifie une adresse SMTP principale. Les adresses proxy ne sont pas autorisées.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ContextFolderId](contextfolderid.md) <br/> |Indique le dossier ciblé pour les actions de conversation qui utilisent des dossiers.  <br/> |
|[DestinationFolderId](destinationfolderid.md) <br/> |Indique le dossier de destination pour les actions de conversation de copie et de déplacement.  <br/> |
|[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) <br/> | Identifie le dossier dans lequel un dossier ou un nouvel élément est créé.  <br/><br/>Voici les expressions XPath de cet élément :<br/><br/>  `/CreateItem/ParentFolderId` <br/><br/>`/CreateFolder/ParentFolderId` <br/> |
|[ParentFolderIds](parentfolderids.md) <br/> |Identifie les dossiers dans lesquels Rechercher l' [opération FindItem](finditem-operation.md) et l' [opération FindFolder](findfolder-operation.md).  <br/> |
|[BaseFolderIds](basefolderids.md) <br/> |Représente la collection de dossiers qui fera l’objet d’une recherche pour déterminer le contenu d’un dossier de recherche.  <br/> |
|[FolderIds](folderids.md) <br/> |Contient un tableau des identificateurs de dossier utilisés pour identifier les dossiers à copier, déplacer, obtenir, supprimer ou surveiller les notifications d’événement.  <br/> |
|[FolderChange](folderchange.md) <br/> |Représente une collection de modifications à effectuer sur un seul dossier.  <br/> <br/>Voici l’expression XPath de cet élément :<br/><br/>`/UpdateFolder/FolderChanges/FolderChange`<br/> |
|[ToFolderId](tofolderid.md) <br/> | Représente le dossier de destination d’un élément ou d’un dossier copié ou déplacé.<br/><br/>Voici les expressions XPath de cet élément :<br/><br/>`/MoveFolder/ToFolderId`<br/><br/>`/CopyFolder/ToFolderId`<br/><br/>`/MoveItem/ToFolderId`<br/><br/>`/CopyItem/ToFolderId` <br/> |
|[SavedItemFolderId](saveditemfolderid.md) <br/> | Identifie le dossier cible pour les opérations de mise à jour, d’envoi et de création d’éléments dans la Banque d’Exchange.<br/><br/>Voici les expressions XPath de cet élément :<br/><br/>`/CreateItem/SavedItemFolderId`<br/><br/>`/UpdateItem/SavedItemFolderId`<br/><br/>`/SendItem/SavedItemFolderId` <br/> |
|[SyncFolderId](syncfolderid.md) <br/> |Représente le dossier qui contient les éléments à synchroniser.  <br/> |
|[UserConfigurationName](userconfigurationname.md) <br/> |Représente le nom d’un objet de configuration utilisateur. Le nom de l’objet de configuration de l’utilisateur est l’identificateur d’un objet de configuration utilisateur.  <br/> |
|[CopyToFolder](copytofolder.md) <br/> |Représente l’ID du dossier dans lequel les éléments de courrier seront copiés.  <br/> |
|[MoveToFolder](movetofolder.md) <br/> |Représente l’ID du dossier vers lequel les éléments de courrier seront déplacés.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Un **DistinguishedFolderId** est résolu en **FolderId**. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML EWS dans Exchange](ews-xml-elements-in-exchange.md)
- [Création de dossiers (services Web Exchange)](https://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

