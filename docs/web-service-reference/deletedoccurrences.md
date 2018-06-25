---
title: DeletedOccurrences
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeletedOccurrences
api_type:
- schema
ms.assetid: 736fb305-9528-4be8-ad37-65d7556edbf2
description: L’élément DeletedOccurrences contient un tableau d’occurrences supprimés d’un élément de calendrier périodique.
ms.openlocfilehash: 269c1176913cd642f93987462286dd1fee3a7339
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755856"
---
# <a name="deletedoccurrences"></a>DeletedOccurrences

L’élément **DeletedOccurrences** contient un tableau d’occurrences supprimés d’un élément de calendrier périodique. 
  
```xml
<DeletedOccurrences>
   <DeletedOccurrence/>
</DeletedOccurrences>
```

 **NonEmptyArrayOfDeletedOccurrencesType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[DeletedOccurrence](deletedoccurrence.md) <br/> |Représente une occurrence d’un élément de calendrier périodique supprimée.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[CalendarItem](calendaritem.md) <br/> |Représente un élément de calendrier Exchange.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Représente une demande de réunion dans la banque d'informations Exchange.  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément n’est valide que si la valeur de texte RecurringMaster est utilisée pour l’élément [CalendarItemType](calendaritemtype.md) . 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)  
- [Référence EWS pour Exchange](ews-reference-for-exchange.md)

