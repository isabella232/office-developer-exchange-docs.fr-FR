---
title: DistinguishedFolderId (DistinguishedFolderIdNameType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 915b2ee9-8284-4bf6-8995-1fd0785e9e48
description: L’élément DistinguishedFolderId identifie les dossiers qui peuvent être référencés par leur nom.
ms.openlocfilehash: ac239ec63f78322f6c82ab4be269d6fe4380dd8d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456191"
---
# <a name="distinguishedfolderid-distinguishedfolderidnametype"></a>DistinguishedFolderId (DistinguishedFolderIdNameType)

L’élément **DistinguishedFolderId** identifie les dossiers qui peuvent être référencés par leur nom. 
  
```XML
<DistinguishedFolderId> calendar | contacts | deleteditems | drafts | inbox | journal | notes | outbox | sentitems | tasks | msgfolderroot | publicfoldersroot | root | junkemail | searchfolders | voicemail | recoverableitemsroot | recoverableitemsdeletions | recoverableitemsversions | recoverableitemspurges | archiveroot | archivemsgfolderroot | archivedeleteditems | archiverecoverableitemsroot | archiverecoverableitemsdeletions | archiverecoverableitemsversions | archiverecoverableitemspurges | syncissues | conflicts | localfailures | serverfailures | recipientcache | quickcontacts | conversationhistory | adminauditlogs | todosearch | mycontacts | directory | imcontactlist | peopleconnect</DistinguishedFolderId>
```

 **DistinguishedFolderIdNameType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Folder](folder.md) <br/> |Spécifie un dossier générique.  <br/> |
|[CalendarFolder](calendarfolder.md) <br/> |Spécifie un dossier de calendrier.  <br/> |
|[ContactsFolder](contactsfolder.md) <br/> |Spécifie un dossier de contacts.  <br/> |
   
## <a name="text-value"></a>Valeur texte

**Valeurs de texte de l’élément DistinguishedFolderId**

|**Valeur**|**Description**|
|:-----|:-----|
|calendrier  <br/> |Indique l’URL du dossier de calendrier.  <br/> |
|contacts  <br/> |Indique l’URL du dossier contacts.  <br/> |
|deleteditems  <br/> |Indique l’URL du dossier éléments supprimés.  <br/> |
|brouillons  <br/> |Indique l’URL du dossier Brouillons.  <br/> |
|boîtederéception  <br/> |Indique l’URL du dossier boîte de réception.  <br/> |
|n  <br/> |Indique l’URL du dossier journal.  <br/> |
|notes  <br/> |Indique l’URL du dossier Notes.  <br/> |
|Boîte d’envoi  <br/> |Indique l’URL du dossier boîte d’envoi.  <br/> |
|sentitems  <br/> |Indique l’URL du dossier éléments envoyés.  <br/> |
|tasks  <br/> |Indique l’URL du dossier tâches.  <br/> |
|msgfolderroot  <br/> |Indique l’URL du dossier racine du message.  <br/> |
|publicfoldersroot  <br/> |Indique l’URL du dossier racine des dossiers publics.  <br/> |
|root  <br/> |Indique l’URL du dossier racine.  <br/> |
|junkemail  <br/> |Indique l’URL du dossier courrier indésirable.  <br/> |
|searchfolders  <br/> |Indique l’URL des dossiers de recherche.  <br/> |
|voicemail  <br/> |Indique l’URL du dossier de messagerie vocale.  <br/> |
|recoverableitemsroot  <br/> |Indique l’URL du dossier racine des éléments récupérables.  <br/> |
|recoverableitemsdeletions  <br/> |Indique l’URL du dossier éléments récupérables supprimés.  <br/> |
|recoverableitemsversions  <br/> |Indique l’URL du dossier des versions de l’élément récupérable.  <br/> |
|recoverableitemspurges  <br/> |Indique l’URL du dossier éléments récupérables purgés.  <br/> |
|archiveroot  <br/> |Indique l’URL du dossier racine d’archivage.  <br/> |
|archivemsgfolderroot  <br/> |Indique l’URL du dossier racine du dossier de messages archivé.  <br/> |
|archivedeleteditems  <br/> |Indique l’URL du dossier éléments supprimés archivés.  <br/> |
|archiverecoverableitemsroot  <br/> |Indique l’URL du dossier racine des éléments récupérables archivés.  <br/> |
|archiverecoverableitemsdeletions  <br/> |Indique l’URL du dossier éléments supprimés récupérables archivés.  <br/> |
|archiverecoverableitemsversions  <br/> |Indique l’URL du dossier des éléments récupérables des éléments récupérables.  <br/> |
|archiverecoverableitemspurges  <br/> |Indique l’URL du dossier éléments récupérables purgés archivés.  <br/> |
|syncissues  <br/> |Indique l’URL du dossier problèmes de synchronisation.  <br/> |
|conflits  <br/> |Indique l’URL du dossier conflits.  <br/> |
|localfailures  <br/> |Indique l’URL du dossier défaillances locales.  <br/> |
|serverfailures  <br/> |Indique l’URL du dossier défaillances du serveur.  <br/> |
|recipientcache  <br/> |Indique l’URL du dossier du cache de destinataires.  <br/> |
|QuickContacts  <br/> |Indique l’URL du dossier contacts rapides.  <br/> |
|conversationhistory  <br/> |Indique l’URL du dossier historique des conversations.  <br/> |
|adminauditlogs  <br/> |Indique l’URL du dossier du journal d’audit administratif.  <br/> |
|todosearch  <br/> |Indique l’URL du dossier de recherche.  <br/> |
|MyContacts  <br/> |Indique l’URL du dossier Mes contacts.  <br/> |
|Active  <br/> |Indique une URL du dossier Directory.  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma type  <br/> |
|Validation File  <br/> |types. xsd  <br/> |
|Peut être vide  <br/> ||
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

