---
title: ExtendedProperty
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExtendedProperty
api_type:
- schema
ms.assetid: f9701409-b620-4afe-b9ee-4c1e95507af7
description: L’élément ExtendedProperty identifie les propriétés MAPI étendues sur les dossiers et les éléments.
ms.openlocfilehash: 99ede097d803d6fbf534cde0e77c08cec054bfa3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530606"
---
# <a name="extendedproperty"></a>ExtendedProperty

L’élément **ExtendedProperty** identifie les propriétés MAPI étendues sur les dossiers et les éléments. 
  
```xml
<ExtendedProperty>
   <ExtendedFieldURI/>
   <Values/>
</ExtendedProperty>
```

```xml
<ExtendedProperty>
   <ExtendedFieldURI/>
   <Value/>
</ExtendedProperty>
```

**ExtendedPropertyType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[ExtendedFieldURI](extendedfielduri.md) <br/> |Identifie une propriété MAPI étendue à obtenir, définir ou créer.  <br/> |
|[Valeurs](values.md) <br/> |Contient une collection de valeurs pour une propriété MAPI étendue à valeurs multiples.  <br/> |
|[Valeur](value.md) <br/> |Contient la valeur de la propriété étendue MAPI à valeur unique.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[CalendarItem](calendaritem.md) <br/> |Représente un élément de calendrier Exchange.  <br/> |
|[Contact](contact.md) <br/> |Représente un élément de contact Exchange.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Représente une liste de distribution.  <br/> |
|[Élément](item.md) <br/> |Représente un élément dans la banque d'informations Exchange.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Représente une annulation de réunion dans la banque d'informations Exchange.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Représente une réunion dans la banque d'informations Exchange.  <br/> |
|[Propriété meetingrequest](meetingrequest.md) <br/> |Représente une demande de réunion dans la banque d'informations Exchange.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Représente une réponse à une réunion dans la banque d'informations Exchange.  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Représente un message électronique Exchange.  <br/> |
|[RemoveItem](removeitem.md) <br/> |Supprime un élément de la banque d'informations Exchange.  <br/> |
|[Tâche](task.md) <br/> |Représente une tâche dans la banque d'informations Exchange.  <br/> |
|[CalendarFolder](calendarfolder.md) <br/> |Représente un dossier qui contient principalement des éléments de calendrier.  <br/> |
|[ContactsFolder](contactsfolder.md) <br/> |Représente un dossier de contacts dans une boîte aux lettres.  <br/> |
|[Folder](folder.md) <br/> |Représente un dossier à créer, obtenir, Rechercher, synchroniser ou mettre à jour.  <br/> |
|[SearchFolder](searchfolder.md) <br/> |Représente un dossier de recherche contenu dans une boîte aux lettres.  <br/> |
|[TasksFolder](tasksfolder.md) <br/> |Représente un dossier tâches contenu dans une boîte aux lettres.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

