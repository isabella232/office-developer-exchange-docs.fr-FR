---
title: ParentFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ParentFolderId
api_type:
- schema
ms.assetid: 258f4b1f-367e-4c7d-9c29-eb775a2398c7
description: L’élément ParentFolderId représente l’identificateur du dossier parent qui contient l’élément ou le dossier.
ms.openlocfilehash: 3bad638aa21019472df8f487f1e065d2e725e750
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465750"
---
# <a name="parentfolderid"></a>ParentFolderId

L’élément **ParentFolderId** représente l’identificateur du dossier parent qui contient l’élément ou le dossier. 
  
```XML
<ParentFolderId Id="" ChangeKey=""/>
```

**FolderIdType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**Id** <br/> |Contient une chaîne qui identifie un dossier dans la Banque d’Exchange. Cet attribut est obligatoire.  <br/> |
|**ChangeKey** <br/> |Contient une chaîne qui identifie la version d’un dossier identifiée par l’attribut **ID** . Cet attribut est facultatif. Utilisez cet attribut pour vous assurer que la version correcte d’un dossier est utilisée.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[CalendarFolder](calendarfolder.md) <br/> |Représente un dossier de calendrier dans une boîte aux lettres.  <br/> |
|[CalendarItem](calendaritem.md) <br/> |Représente un élément de calendrier dans une boîte aux lettres.  <br/> |
|[Contact](contact.md) <br/> |Représente un élément de contact dans une boîte aux lettres.  <br/> |
|[ContactsFolder](contactsfolder.md) <br/> |Représente un dossier de contacts dans une boîte aux lettres.  <br/> |
|[CopiedEvent](copiedevent.md) <br/> |Représente un événement dans lequel un élément ou un dossier est copié.  <br/> |
|[CreatedEvent](createdevent.md) <br/> |Représente un événement dans lequel un élément ou un dossier est créé.  <br/> |
|[DeletedEvent](deletedevent.md) <br/> |Représente un événement dans lequel un élément ou un dossier est supprimé.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Représente une liste de distribution privée dans une boîte aux lettres.  <br/> |
|[Folder](folder.md) <br/> |Représente un dossier dans une boîte aux lettres.  <br/> |
|[Élément](item.md) <br/> |Représente un élément Exchange générique.  <br/> |
|[Élément (UploadItemType)](item-uploaditemtype.md) <br/> |Représente un élément unique à télécharger dans une boîte aux lettres.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Représente une annulation de réunion dans une boîte aux lettres.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Représente un message de réunion dans une boîte aux lettres.  <br/> |
|[Propriété meetingrequest](meetingrequest.md) <br/> |Représente une demande de réunion dans une boîte aux lettres.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Représente une réponse à une réunion dans une boîte aux lettres.  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Représente un message électronique dans une boîte aux lettres.  <br/> |
|[ModifiedEvent](modifiedevent.md) <br/> |Représente un événement dans lequel un élément ou un dossier est modifié.  <br/> |
|[MovedEvent](movedevent.md) <br/> |Représente un événement dans lequel un élément ou un dossier est déplacé d’un dossier parent vers un autre dossier parent.  <br/> |
|[NewMailEvent](newmailevent.md) <br/> |Représente un événement qui est déclenché par un nouvel élément de courrier dans une boîte aux lettres.  <br/> |
|[AcceptItem](acceptitem.md) <br/> |Représente une réponse à accepter à une demande de réunion.  <br/> |
|[TentativelyAcceptItem](tentativelyacceptitem.md) <br/> |Représente un provisoire répond à une demande de réunion.  <br/> |
|[DeclineItem](declineitem.md) <br/> |Représente une réponse de refus à une demande de réunion.  <br/> |
|[RemoveItem](removeitem.md) <br/> |Supprime un élément de la banque d'informations Exchange.  <br/> |
|[Task](task.md) <br/> |Représente un élément de tâche dans une boîte aux lettres.  <br/> |
|[ReplyToItem](replytoitem.md) <br/> |Contient une réponse à l'auteur d'un élément dans la banque d'informations Exchange.  <br/> |
|[ReplyAllToItem](replyalltoitem.md) <br/> |Contient une réponse destinée à tous les destinataires identifiés d'un élément dans la banque d'informations Exchange.  <br/> |
|[ForwardItem](forwarditem.md) <br/> |Contient un élément de la banque Exchange pour transférer à des destinataires.  <br/> |
|[CancelCalendarItem](cancelcalendaritem.md) <br/> |Représente l'objet de réponse qui est utilisé pour annuler une réunion.  <br/> |
|[TasksFolder](tasksfolder.md) <br/> |Représente un dossier de tâches dans une boîte aux lettres.  <br/> |
|[SearchFolder](searchfolder.md) <br/> |Représente un dossier de recherche dans une boîte aux lettres.  <br/> |
   
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

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

