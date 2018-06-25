---
title: OriginalStart
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- OriginalStart
api_type:
- schema
ms.assetid: 4599dd34-15ee-4d57-b886-732081b50784
description: L’élément OriginalStart représente l’heure de début d’origine d’un élément de calendrier.
ms.openlocfilehash: 9e5facb3df87ab08e05f23258abdf1767fae64e4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828668"
---
# <a name="originalstart"></a>OriginalStart

L’élément **OriginalStart** représente l’heure de début d’origine d’un élément de calendrier. 
  
```xml
<OriginalStart/>
```

 **DateTime**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[CalendarItem](calendaritem.md) <br/> |Représente un élément de calendrier dans la banque d’informations Exchange.  <br/> |
|[FirstOccurrence](firstoccurrence.md) <br/> |Représente la première occurrence d’un élément de calendrier périodique.  <br/> |
|[LastOccurrence](lastoccurrence.md) <br/> |Représente la dernière occurrence d’un élément de calendrier périodique.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Représente une demande de réunion dans la banque d'informations Exchange.  <br/> |
|[Occurrence](occurrence.md) <br/> |Représente une seule occurrence de modification d’un élément de calendrier périodique.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Une valeur de texte qui représente une date et une heure est obligatoire si cet élément est utilisé.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

