---
title: ReminderType
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: bfaf84eb-271a-4728-84fc-a20205a100bd
description: L’élément ReminderType spécifie le type de rappels à renvoyer.
ms.openlocfilehash: ab10db372efb935b335868f5d212ded84b29e6eb
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518000"
---
# <a name="remindertype"></a>ReminderType

**L’élément ReminderType** spécifie le type de rappels à renvoyer. 
  
```XML
<ReminderType> All | Current | Old </ReminderType>
```

 **chaîne**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[GetReminders](getreminders.md)
  
## <a name="text-value"></a>Valeur texte

La valeur de texte de **l’élément ReminderType** est le type de rappels à renvoyer, **tous,** **actuels** ou **anciens**. **Tout** est la valeur recommandée pour cet élément. Pour plus d’informations sur la relation entre l’élément **ReminderType** et les éléments [BeginTime](begintime.md) et [EndTime,](endtime-remindermessagedatatype.md) voir [l’opération GetReminders](getreminders-operation.md).
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[GetReminders](getreminders.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

