---
title: NewReminderTime
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: ff1b6b1c-3557-41d4-8aa6-9528fdb3a21a
description: L’élément NewReminderTime spécifie une nouvelle heure pour un rappel.
ms.openlocfilehash: 9e6cb75396f35f606bcd974e374f24957ee5d1ec
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515445"
---
# <a name="newremindertime"></a>NewReminderTime

**L’élément NewReminderTime** spécifie une nouvelle heure pour un rappel. 
  
```XML
<NewReminderTime/>
```

 **chaîne**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[ReminderItemAction](reminderitemaction.md)
  
## <a name="text-value"></a>Valeur texte

La valeur de texte de **l’élément NewReminderTime** est une nouvelle heure pour le rappel. **L’élément NewReminderTime** est utilisé lorsque l’élément [ActionType](actiontype-reminderactiontype.md) est définie sur **Snooze**, afin de retarder le rappel. La valeur de **NewReminderTime doit** être supérieure à la [valeur ReminderTime](remindertime.md) renvoyée par l’opération [GetReminders](getreminders-operation.md).
  
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



[ReminderItemAction](reminderitemaction.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

