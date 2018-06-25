---
title: AppointmentState
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AppointmentState
api_type:
- schema
ms.assetid: ab3f5d04-ace1-4a15-9107-cefa6c41abc7
description: L’élément AppointmentState Spécifie l’état du rendez-vous.
ms.openlocfilehash: 05e92a3fea10a84518b0680c425011a91bc43d93
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755306"
---
# <a name="appointmentstate"></a>AppointmentState

L’élément **AppointmentState** Spécifie l’état du rendez-vous. 
  
```XML
<AppointmentState/>
```

 **int**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[CalendarItem](calendaritem.md) <br/> |Représente un élément de calendrier Exchange.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Représente une réunion dans la banque d'informations Exchange.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Cet élément contient une valeur de texte que représente la valeur bits. Il s’agit de formulaire entier. Cet élément est en lecture seule. Il sera renvoyée uniquement dans une réponse.
  
## <a name="remarks"></a>Remarques

Valeur entière qui est renvoyée représente le masque de bits état rendez-vous. Le tableau suivant décrit chaque bit.
  
|**Name**|**Bit**|**Description**|
|:-----|:-----|:-----|
|None  <br/> |0x0000  <br/> |Aucun indicateur n’ont été définies. Il est uniquement utilisé pour un rendez-vous qui n’inclut pas les participants.  <br/> |
|Réunion  <br/> |0x0001  <br/> |Ce rendez-vous est une réunion.  <br/> |
|Received  <br/> |0x0002  <br/> |Ce rendez-vous a été reçu.  <br/> |
|Annulé  <br/> |0x0004  <br/> |Ce rendez-vous a été annulé.  <br/> |
   
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

