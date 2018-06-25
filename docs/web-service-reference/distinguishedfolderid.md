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
description: L’élément DistinguishedFolderId identifie les dossiers qui peuvent être référencés par un nom. Si vous n’utilisez pas cet élément, vous devez utiliser l’élément FolderId pour identifier un dossier.
ms.openlocfilehash: 834166be3d882fa8c0533cfcc2999600430b82ce
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756018"
---
# <a name="distinguishedfolderid"></a>DistinguishedFolderId

L’élément **DistinguishedFolderId** identifie les dossiers qui peuvent être référencés par un nom. Si vous n’utilisez pas cet élément, vous devez utiliser l’élément [FolderId](folderid.md) pour identifier un dossier. 
  
```XML
<DistinguishedFolderId Id="" ChangeKey="">
   <Mailbox/>
</DistinguishedFolderId>
```

 **DistinguishedFolderIdType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|
  **Id** <br/> |Contient une chaîne qui identifie un dossier par défaut. Cet attribut est requis.  <br/> |
|**ChangeKey** <br/> |Contient une chaîne qui identifie une version d’un dossier qui est identifié par l’attribut **Id** . Cet attribut est facultatif. Utilisez cet attribut pour vous assurer que la version correcte d’un dossier est utilisée.  <br/> |
   
#### <a name="id-attribute-values"></a>Valeurs d’attribut ID

|**Valeur**|**Description**|
|:-----|:-----|
|calendrier  <br/> |Représente le dossier calendrier.  <br/> |
|contacts  <br/> |Représente le dossier Contacts.  <br/> |
|deleteditems  <br/> |Représente le dossier éléments supprimés.  <br/> |
|brouillons  <br/> |Représente le dossier Brouillons.  <br/> |
|boîte de réception  <br/> |Représente le dossier boîte de réception.  <br/> |
|journal  <br/> |Représente le dossier Journal.  <br/> |
|notes  <br/> |Représente le dossier Notes.  <br/> |
|la boîte d’envoi  <br/> |Représente le dossier boîte d’envoi.  <br/> |
|éléments envoyés  <br/> |Représente le dossier éléments envoyés.  <br/> |
|tasks  <br/> |Représente le dossier tâches.  <br/> |
|msgfolderroot  <br/> |Représente la racine du dossier du message.  <br/> |
|root  <br/> |Représente la racine de la boîte aux lettres.  <br/> |
|junkemail  <br/> |Représente le dossier courrier indésirable.  <br/> |
|SearchFolders  <br/> |Représente le dossier de dossiers de recherche.  <br/> |
|messagerie vocale  <br/> |Représente le dossier de messagerie vocale.  <br/> |
|recoverableitemsroot  <br/> |Représente la benne de dossier racine.  <br/> |
|recoverableitemsdeletions  <br/> |Représente la benne de dossier de suppressions.  <br/> |
|recoverableitemsversions  <br/> |Représente la benne de dossier de versions.  <br/> |
|recoverableitemspurges  <br/> |Représente la benne de purge du dossier.  <br/> |
|archiveroot  <br/> |Représente le dossier racine d’archivage.  <br/> |
|archivemsgfolderroot  <br/> |Représente le dossier messages d’archivage racine.  <br/> |
|archivedeleteditems  <br/> |Représente le dossier d’éléments supprimés des archives.  <br/> |
|archiveinbox  <br/> |Représente le dossier boîte de réception de l’archive. Versions d’Exchange commençant par le numéro de build 15.00.0913.09 incluent cette valeur.  <br/> |
|archiverecoverableitemsroot  <br/> |Représente le dossier racine d’archivage éléments récupérables.  <br/> |
|archiverecoverableitemsdeletions  <br/> |Représente le dossier de suppressions d’éléments récupérables archive.  <br/> |
|archiverecoverableitemsversions  <br/> |Représente le dossier de versions d’éléments récupérables archive.  <br/> |
|archiverecoverableitemspurges  <br/> |Représente le dossier de purge archive les éléments récupérables.  <br/> |
|syncissues  <br/> |Représente le dossier problèmes de synchronisation.  <br/> |
|conflits  <br/> |Représente le dossier conflits.  <br/> |
|localfailures  <br/> |Représente le dossier Pannes locales.  <br/> |
|serverfailures  <br/> |Représente le dossier échecs du serveur.  <br/> |
|recipientcache  <br/> |Représente le dossier de cache de destinataires.  <br/> |
|QuickContacts  <br/> |Représente le dossier contacts rapides.  <br/> |
|conversationhistory  <br/> |Représente le dossier historique des conversations.  <br/> |
|adminauditlogs  <br/> |Représente le dossier des journaux d’audit d’administration.  <br/> |
|todosearch  <br/> |Représente le dossier de recherche des tâches.  <br/> |
|mescontacts  <br/> |Représente le dossier Mes Contacts.  <br/> |
|répertoire  <br/> |Représente le dossier de répertoire.  <br/> |
|imcontactlist  <br/> |Représente le dossier de liste de contacts de messagerie instantanée.  <br/> |
|peopleconnect  <br/> |Représente les personnes connecter le dossier.  <br/> |
|favoris  <br/> |Représente le dossier Favoris.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Boîte aux lettres](mailbox.md) <br/> |Identifie une adresse SMTP principale. Adresses proxy ne sont pas autorisés.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ContextFolderId](contextfolderid.md) <br/> |Indique le dossier qui est destiné aux actions de conversation qui utilisent des dossiers.  <br/> |
|[DestinationFolderId](destinationfolderid.md) <br/> |Indique le dossier de destination de copie et déplacer les actions de conversation.  <br/> |
|[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) <br/> | Identifie le dossier dans lequel un nouveau dossier ou un élément est créé.  <br/><br/>Les expressions XPath pour cet élément sont les suivantes :<br/><br/>  `/CreateItem/ParentFolderId` <br/><br/>`/CreateFolder/ParentFolderId` <br/> |
|[ParentFolderIds](parentfolderids.md) <br/> |Identifie les dossiers de recherche de l' [opération FindItem](finditem-operation.md) et l' [opération FindFolder](findfolder-operation.md).  <br/> |
|[BaseFolderIds](basefolderids.md) <br/> |Représente la collection de dossiers portera pour déterminer le contenu d’un dossier de recherche.  <br/> |
|[FolderIds](folderids.md) <br/> |Contient un tableau d’identificateurs de dossier qui sont utilisés pour identifier les dossiers pour copier, déplacer, obtenir, supprimer ou contrôler les notifications d’événements.  <br/> |
|[FolderChange](folderchange.md) <br/> |Représente une collection des modifications à effectuer sur un seul dossier.  <br/> <br/>Vous trouverez ci-dessous l’expression XPath pour cet élément :<br/><br/>`/UpdateFolder/FolderChanges/FolderChange`<br/> |
|[ToFolderId](tofolderid.md) <br/> | Représente le dossier de destination pour un dossier ou un élément copié ou déplacé.<br/><br/>Les expressions XPath pour cet élément sont les suivantes :<br/><br/>`/MoveFolder/ToFolderId`<br/><br/>`/CopyFolder/ToFolderId`<br/><br/>`/MoveItem/ToFolderId`<br/><br/>`/CopyItem/ToFolderId` <br/> |
|[SavedItemFolderId](saveditemfolderid.md) <br/> | Identifie le dossier cible pour les opérations de mise à jour, d’envoyer et de créer des éléments dans la banque d’informations Exchange.<br/><br/>Les expressions XPath pour cet élément sont les suivantes :<br/><br/>`/CreateItem/SavedItemFolderId`<br/><br/>`/UpdateItem/SavedItemFolderId`<br/><br/>`/SendItem/SavedItemFolderId` <br/> |
|[SyncFolderId](syncfolderid.md) <br/> |Représente le dossier qui contient les éléments à synchroniser.  <br/> |
|[UserConfigurationName](userconfigurationname.md) <br/> |Représente le nom d’un objet de configuration utilisateur. Le nom d’objet de configuration utilisateur est l’identificateur pour un objet de configuration utilisateur.  <br/> |
|[CopyToFolder](copytofolder.md) <br/> |Représente l’ID du dossier e-mail éléments vont être copiés dans.  <br/> |
|[MoveToFolder](movetofolder.md) <br/> |Représente l’ID du dossier éléments seront déplacées vers e-mail.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Un **DistinguishedFolderId** résout un **FolderId**. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)
- [Création de dossiers (Exchange Web Services)](http://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

