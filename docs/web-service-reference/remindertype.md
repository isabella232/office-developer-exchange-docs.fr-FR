---
title: ReminderType
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bfaf84eb-271a-4728-84fc-a20205a100bd
description: L’élément ReminderType Spécifie le type de rappels à renvoyer.
ms.openlocfilehash: 11739d2068a1009b2840b2169e86b113151cbfa9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829077"
---
# <a name="remindertype"></a>ReminderType

L’élément **ReminderType** Spécifie le type de rappels à renvoyer. 
  
```XML
<ReminderType> All | Current | Old </ReminderType>
```

 **string**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[GetReminders](getreminders.md)
  
## <a name="text-value"></a>Valeur de texte

La valeur de texte de l’élément **ReminderType** est le type de rappels à renvoyer, **tous les**, **actuel**ou **ancien**. **All** est la valeur recommandée pour cet élément. Pour plus d’informations sur la relation entre l’élément **ReminderType** et les éléments [BeginTime](begintime.md) et [EndTime](endtime-remindermessagedatatype.md) , voir [opération GetReminders](getreminders-operation.md).
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[GetReminders](getreminders.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

