---
title: ReminderGroup
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 3e23c2a1-05d8-4fec-897c-f684a5b97e4c
description: L’élément ReminderGroup spécifie si le rappel est pour un élément de calendrier ou une tâche.
ms.openlocfilehash: 7ec19505e9237680aee1b3a31332db7fdc4c0dd4
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59512470"
---
# <a name="remindergroup"></a>ReminderGroup

**L’élément ReminderGroup** spécifie si le rappel est pour un élément de calendrier ou une tâche. 
  
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

La valeur de texte de **l’élément ReminderGroup** est le type de groupe du rappel. La valeur de texte **Calendar** spécifie que le rappel est pour un élément de calendrier. La valeur de texte **de Task** spécifie que le rappel est pour un élément de tâche. 
  
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

