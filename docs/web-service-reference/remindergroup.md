---
title: ReminderGroup
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3e23c2a1-05d8-4fec-897c-f684a5b97e4c
description: L’élément ReminderGroup spécifie si le rappel est destiné à un élément de calendrier ou à une tâche.
ms.openlocfilehash: be6f4a7d7e9d495ed7b42ed40c60f016468e8c2c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529867"
---
# <a name="remindergroup"></a>ReminderGroup

L’élément **ReminderGroup** spécifie si le rappel est destiné à un élément de calendrier ou à une tâche. 
  
```XML
<ReminderGroup> Calendar | Task </ReminderGroup>
```

 **ReminderGroupType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[Reminder](reminder.md)
  
## <a name="text-value"></a>Valeur texte

La valeur de texte de l’élément **ReminderGroup** est le type de groupe du rappel. La valeur texte de **Calendar** spécifie que le rappel est destiné à un élément de calendrier. La valeur texte de **Task** spécifie que le rappel est destiné à un élément de tâche. 
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Reminder](reminder.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

