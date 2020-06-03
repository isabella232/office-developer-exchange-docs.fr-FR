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
description: L’élément AppointmentState spécifie l’état du rendez-vous.
ms.openlocfilehash: 8b0e827d02e9051f31d43199503dc286c50e2125
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463474"
---
# <a name="appointmentstate"></a>AppointmentState

L’élément **AppointmentState** spécifie l’état du rendez-vous. 
  
```XML
<AppointmentState/>
```

 **int**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[CalendarItem](calendaritem.md) <br/> |Représente un élément de calendrier Exchange.  <br/> |
|[Propriété meetingrequest](meetingrequest.md) <br/> |Représente une réunion dans la banque d'informations Exchange.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Cet élément contient une valeur de texte qui représente Set bits. Il s’agit d’une forme entière. Cet élément est en lecture seule. Elle sera renvoyée uniquement dans une réponse.
  
## <a name="remarks"></a>Remarques

La valeur entière renvoyée représente le masque de binaire d’état de rendez-vous. Le tableau suivant décrit chaque bit.
  
|**Name**|**Légèrement**|**Description**|
|:-----|:-----|:-----|
|Aucun  <br/> |0x0000  <br/> |Aucun indicateur n’a été défini. Il est utilisé uniquement pour un rendez-vous qui n’inclut pas de participants.  <br/> |
|Satisfaire  <br/> |0x0001  <br/> |Ce rendez-vous est une réunion.  <br/> |
|Received  <br/> |0x0002  <br/> |Ce rendez-vous a été reçu.  <br/> |
|Annulé  <br/> |0x0004  <br/> |Ce rendez-vous a été annulé.  <br/> |
   
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

