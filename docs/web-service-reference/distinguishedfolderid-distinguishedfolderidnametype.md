---
title: DistinguishedFolderId (DistinguishedFolderIdNameType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 915b2ee9-8284-4bf6-8995-1fd0785e9e48
description: L’élément DistinguishedFolderId identifie les dossiers qui peuvent être référencés par un nom.
ms.openlocfilehash: 1f5b97fc7ee7b93989762c26e4b979a8dfb884be
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756016"
---
# <a name="distinguishedfolderid-distinguishedfolderidnametype"></a>DistinguishedFolderId (DistinguishedFolderIdNameType)

L’élément **DistinguishedFolderId** identifie les dossiers qui peuvent être référencés par un nom. 
  
```XML
<DistinguishedFolderId> calendar | contacts | deleteditems | drafts | inbox | journal | notes | outbox | sentitems | tasks | msgfolderroot | publicfoldersroot | root | junkemail | searchfolders | voicemail | recoverableitemsroot | recoverableitemsdeletions | recoverableitemsversions | recoverableitemspurges | archiveroot | archivemsgfolderroot | archivedeleteditems | archiverecoverableitemsroot | archiverecoverableitemsdeletions | archiverecoverableitemsversions | archiverecoverableitemspurges | syncissues | conflicts | localfailures | serverfailures | recipientcache | quickcontacts | conversationhistory | adminauditlogs | todosearch | mycontacts | directory | imcontactlist | peopleconnect</DistinguishedFolderId>
```

 **DistinguishedFolderIdNameType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Folder](folder.md) <br/> |Spécifie un dossier générique.  <br/> |
|[CalendarFolder](calendarfolder.md) <br/> |Spécifie un dossier de calendrier.  <br/> |
|[ContactsFolder](contactsfolder.md) <br/> |Spécifie un dossier contacts.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

**Valeurs de texte des éléments DistinguishedFolderId**

|**Valeur**|**Description**|
|:-----|:-----|
|calendrier  <br/> |Indique l’URL du dossier calendrier.  <br/> |
|contacts  <br/> |Indique l’URL du dossier contacts.  <br/> |
|deleteditems  <br/> |Indique l’URL du dossier éléments supprimés.  <br/> |
|brouillons  <br/> |Indique l’URL du dossier Brouillons.  <br/> |
|boîte de réception  <br/> |Indique l’URL du dossier boîte de réception.  <br/> |
|journal  <br/> |Indique l’URL du dossier journal.  <br/> |
|notes  <br/> |Indique l’URL du dossier notes.  <br/> |
|la boîte d’envoi  <br/> |Indique l’URL du dossier boîte d’envoi.  <br/> |
|éléments envoyés  <br/> |Indique l’URL du dossier éléments envoyés.  <br/> |
|tasks  <br/> |Indique l’URL du dossier tâches.  <br/> |
|msgfolderroot  <br/> |Indique l’URL du dossier racine message.  <br/> |
|publicfoldersroot  <br/> |Indique l’URL du dossier racine des dossiers publics.  <br/> |
|root  <br/> |Indique l’URL du dossier racine.  <br/> |
|junkemail  <br/> |Indique l’URL du dossier courrier indésirable.  <br/> |
|SearchFolders  <br/> |Indique l’URL des dossiers de recherche.  <br/> |
|messagerie vocale  <br/> |Indique l’URL du dossier de messagerie vocale.  <br/> |
|recoverableitemsroot  <br/> |Indique l’URL du dossier racine éléments récupérables.  <br/> |
|recoverableitemsdeletions  <br/> |Indique l’URL du dossier éléments récupérables supprimés.  <br/> |
|recoverableitemsversions  <br/> |Indique l’URL du dossier éléments récupérables versions.  <br/> |
|recoverableitemspurges  <br/> |Indique l’URL du dossier éléments récupérables purgés.  <br/> |
|archiveroot  <br/> |Indique l’URL du dossier racine archive.  <br/> |
|archivemsgfolderroot  <br/> |Indique l’URL du dossier racine dossier message archivé.  <br/> |
|archivedeleteditems  <br/> |Indique l’URL du dossier éléments supprimés archivées.  <br/> |
|archiverecoverableitemsroot  <br/> |Indique l’URL du dossier racine des éléments récupérables archivés.  <br/> |
|archiverecoverableitemsdeletions  <br/> |Indique l’URL du dossier éléments supprimés récupérables archivés.  <br/> |
|archiverecoverableitemsversions  <br/> |Indique l’URL du dossier versions archivées des éléments récupérables.  <br/> |
|archiverecoverableitemspurges  <br/> |Indique l’URL du dossier éléments récupérables purgés archivés.  <br/> |
|syncissues  <br/> |Indique l’URL du dossier de problèmes de synchronisation.  <br/> |
|conflits  <br/> |Indique l’URL du dossier conflits.  <br/> |
|localfailures  <br/> |Indique l’URL du dossier Défaillances locales.  <br/> |
|serverfailures  <br/> |Indique l’URL du dossier d’échecs du serveur.  <br/> |
|recipientcache  <br/> |Indique l’URL du dossier de cache de destinataires.  <br/> |
|QuickContacts  <br/> |Indique l’URL du dossier contacts rapides.  <br/> |
|conversationhistory  <br/> |Indique l’URL du dossier historique des conversations.  <br/> |
|adminauditlogs  <br/> |Indique l’URL du dossier du journal d’audit d’administration.  <br/> |
|todosearch  <br/> |Indique l’URL du dossier des tâches de recherche.  <br/> |
|mescontacts  <br/> |Indique l’URL de la mon dossier contacts.  <br/> |
|répertoire  <br/> |Indique une URL du dossier de répertoire.  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma type  <br/> |
|Validation File  <br/> |types.xsd  <br/> |
|Peut être vide  <br/> ||
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

