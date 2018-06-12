---
title: NewReminderTime
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ff1b6b1c-3557-41d4-8aa6-9528fdb3a21a
description: L’élément NewReminderTime spécifie une nouvelle heure pour un rappel.
ms.openlocfilehash: 9f3f509942c673c916cc646cd9519240aef6ea06
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828531"
---
# <a name="newremindertime"></a>NewReminderTime

L’élément **NewReminderTime** spécifie une nouvelle heure pour un rappel. 
  
```XML
<NewReminderTime/>
```

 **string**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[ReminderItemAction](reminderitemaction.md)
  
## <a name="text-value"></a>Valeur de texte

La valeur de texte de l’élément **NewReminderTime** est une nouvelle heure pour le rappel. L’élément **NewReminderTime** est utilisé lorsque l’élément [ActionType](actiontype-reminderactiontype.md) est défini sur **Répéter**, afin de différer le rappel. La valeur de la **NewReminderTime** doit être supérieure à la [ReminderTime](remindertime.md) retournées par l' [opération GetReminders](getreminders-operation.md).
  
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



[ReminderItemAction](reminderitemaction.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

