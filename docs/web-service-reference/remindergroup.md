---
title: ReminderGroup
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3e23c2a1-05d8-4fec-897c-f684a5b97e4c
description: L’élément ReminderGroup indique si le rappel est pour un élément de calendrier ou d’une tâche.
ms.openlocfilehash: d9d31cdab482d04149428021ad44cc742108053a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829060"
---
# <a name="remindergroup"></a>ReminderGroup

L’élément **ReminderGroup** indique si le rappel est pour un élément de calendrier ou d’une tâche. 
  
```XML
<ReminderGroup> Calendar | Task </ReminderGroup>
```

 **ReminderGroupType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[Rappel](reminder.md)
  
## <a name="text-value"></a>Valeur de texte

La valeur de texte de l’élément **ReminderGroup** est le type de groupe du rappel. La valeur de texte du **calendrier** Spécifie que le rappel est destiné à un élément de calendrier. La valeur de texte de la **tâche** Spécifie que le rappel est destiné à un élément de tâche. 
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Rappel](reminder.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

