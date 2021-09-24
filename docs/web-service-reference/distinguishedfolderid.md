---
title: DistinguishedFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DistinguishedFolderId
api_type:
- schema
ms.assetid: 50018162-2941-4227-8a5b-d6b4686bb32f
description: L’élément DistinguishedFolderId identifie les dossiers qui peuvent être référencés par leur nom. Si vous n’utilisez pas cet élément, vous devez utiliser l’élément FolderId pour identifier un dossier.
ms.openlocfilehash: 309db925bb783c435320aeb283915ece39da2271
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521994"
---
# <a name="distinguishedfolderid"></a>DistinguishedFolderId

**L’élément DistinguishedFolderId** identifie les dossiers qui peuvent être référencés par leur nom. Si vous n’utilisez pas cet élément, vous devez utiliser l’élément [FolderId](folderid.md) pour identifier un dossier. 
  
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
|**ChangeKey** <br/> |Contient une chaîne qui identifie une version d’un dossier identifiée par **l’attribut ID.** Cet attribut est facultatif. Utilisez cet attribut pour vous assurer que la version correcte d’un dossier est utilisée.  <br/> |
   
#### <a name="id-attribute-values"></a>Valeurs d’attribut d’ID

|**Valeur**|**Description**|
|:-----|:-----|
|calendrier  <br/> |Représente le dossier Calendrier.  <br/> |
|contacts  <br/> |Représente le dossier Contacts.  <br/> |
|deleteditems  <br/> |Représente le dossier Éléments supprimés.  <br/> |
|brouillons  <br/> |Représente le dossier Brouillons.  <br/> |
|boîtederéception  <br/> |Représente le dossier Boîte de réception.  <br/> |
|journal  <br/> |Représente le dossier Journal.  <br/> |
|notes  <br/> |Représente le dossier Notes.  <br/> |
|Boîte d’envoi  <br/> |Représente le dossier Boîte d’envoi.  <br/> |
|sentitems  <br/> |Représente le dossier Éléments envoyés.  <br/> |
|tasks  <br/> |Représente le dossier Tâches.  <br/> |
|msgfolderroot  <br/> |Représente la racine du dossier de message.  <br/> |
|root  <br/> |Représente la racine de la boîte aux lettres.  <br/> |
|junkemail  <br/> |Représente le dossier Courrier indésirable.  <br/> |
|searchfolders  <br/> |Représente le dossier Dossiers de recherche.  <br/> |
|voicemail  <br/> |Représente le dossier Messagerie vocale.  <br/> |
|recoverableitemsroot  <br/> |Représente le dossier racine de la benne.  <br/> |
|recoverableitemsdeletions  <br/> |Représente le dossier des suppressions de bennes.  <br/> |
|recoverableitemsversions  <br/> |Représente le dossier des versions du benne.  <br/> |
|recoverableitemspurges  <br/> |Représente le dossier purges de la benne.  <br/> |
|archiveroot  <br/> |Représente le dossier d’archivage racine.  <br/> |
|archivemsgfolderroot  <br/> |Représente le dossier du message d’archivage racine.  <br/> |
|archivedeleteditems  <br/> |Représente le dossier d’archive des éléments supprimés.  <br/> |
|archiveinbox  <br/> |Représente le dossier boîte de réception d’archivage. Les versions Exchange à partir du numéro de build 15.00.0913.09 incluent cette valeur.  <br/> |
|archiverecoverableitemsroot  <br/> |Représente le dossier racine des éléments récupérables d’archivage.  <br/> |
|archiverecoverableitemsdeletions  <br/> |Représente le dossier des suppressions d’éléments récupérables d’archivage.  <br/> |
|archiverecoverableitemsversions  <br/> |Représente le dossier des versions des éléments récupérables d’archivage.  <br/> |
|archiverecoverableitemspurges  <br/> |Représente le dossier de purges des éléments récupérables d’archivage.  <br/> |
|syncissues  <br/> |Représente le dossier problèmes de synchronisation.  <br/> |
|conflits  <br/> |Représente le dossier conflits.  <br/> |
|localfailures  <br/> |Représente le dossier des défaillances locales.  <br/> |
|serverfailures  <br/> |Représente le dossier des défaillances du serveur.  <br/> |
|recipientcache  <br/> |Représente le dossier cache des destinataires.  <br/> |
|quickcontacts  <br/> |Représente le dossier contacts rapides.  <br/> |
|conversationhistory  <br/> |Représente le dossier d’historique des conversations.  <br/> |
|adminauditlogs  <br/> |Représente le dossier journaux d’audit de l’administrateur.  <br/> |
|todosearch  <br/> |Représente le dossier de recherche de todos.  <br/> |
|mycontacts  <br/> |Représente le dossier Mes contacts.  <br/> |
|répertoire  <br/> |Représente le dossier du répertoire.  <br/> |
|imcontactlist  <br/> |Représente le dossier de liste des contacts de messagerie instantanée.  <br/> |
|peopleconnect  <br/> |Représente le dossier de connexion des personnes.  <br/> |
|favoris  <br/> |Représente le dossier Favoris.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Boîte aux lettres](mailbox.md) <br/> |Identifie une adresse SMTP principale. Les adresses proxy ne sont pas autorisées.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ContextFolderId](contextfolderid.md) <br/> |Indique le dossier ciblé pour les actions de conversation qui utilisent des dossiers.  <br/> |
|[DestinationFolderId](destinationfolderid.md) <br/> |Indique le dossier de destination pour les actions de copie et de déplacement de conversation.  <br/> |
|[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) <br/> | Identifie le dossier dans lequel un dossier ou un élément est créé.  <br/><br/>Les expressions XPath de cet élément sont les suivantes :<br/><br/>  `/CreateItem/ParentFolderId` <br/><br/>`/CreateFolder/ParentFolderId` <br/> |
|[ParentFolderIds](parentfolderids.md) <br/> |Identifie les dossiers à rechercher pour [l’opération FindItem et](finditem-operation.md) [l’opération FindFolder](findfolder-operation.md).  <br/> |
|[BaseFolderIds](basefolderids.md) <br/> |Représente la collection de dossiers qui seront recherchés pour déterminer le contenu d’un dossier de recherche.  <br/> |
|[FolderIds](folderids.md) <br/> |Contient un tableau d’identificateurs de dossiers utilisés pour identifier les dossiers à copier, déplacer, obtenir, supprimer ou surveiller les notifications d’événement.  <br/> |
|[FolderChange](folderchange.md) <br/> |Représente une collection de modifications à effectuer sur un seul dossier.  <br/> <br/>Voici l’expression XPath de cet élément :<br/><br/>`/UpdateFolder/FolderChanges/FolderChange`<br/> |
|[ToFolderId](tofolderid.md) <br/> | Représente le dossier de destination d’un élément ou dossier copié ou déplacé.<br/><br/>Les expressions XPath de cet élément sont les suivantes :<br/><br/>`/MoveFolder/ToFolderId`<br/><br/>`/CopyFolder/ToFolderId`<br/><br/>`/MoveItem/ToFolderId`<br/><br/>`/CopyItem/ToFolderId` <br/> |
|[SavedItemFolderId](saveditemfolderid.md) <br/> | Identifie le dossier cible pour les opérations qui update, send et create items in the Exchange store.<br/><br/>Les expressions XPath de cet élément sont les suivantes :<br/><br/>`/CreateItem/SavedItemFolderId`<br/><br/>`/UpdateItem/SavedItemFolderId`<br/><br/>`/SendItem/SavedItemFolderId` <br/> |
|[SyncFolderId](syncfolderid.md) <br/> |Représente le dossier qui contient les éléments à synchroniser.  <br/> |
|[UserConfigurationName](userconfigurationname.md) <br/> |Représente le nom d’un objet de configuration utilisateur. Le nom de l’objet de configuration utilisateur est l’identificateur d’un objet de configuration utilisateur.  <br/> |
|[CopyToFolder](copytofolder.md) <br/> |Représente l’ID du dossier dans qui les éléments de courrier électronique seront copiés.  <br/> |
|[MoveToFolder](movetofolder.md) <br/> |Représente l’ID du dossier vers qui les éléments de courrier électronique seront déplacés.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

A **DistinguishedFolderId** resolves to a **FolderId**. 
  
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
- [Creating Folders (Exchange Web Services)](https://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

