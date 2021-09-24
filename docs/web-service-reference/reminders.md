---
title: Reminders
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 19294300-ab84-4784-8aa7-3395a08de640
description: L’élément Reminders spécifie les rappels renvoyés dans la réponse à une demande GetReminders.
ms.openlocfilehash: 0b760e93bf27f0fdaad9464580fad924367dea32
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513408"
---
# <a name="reminders"></a>Reminders

**L’élément Reminders** spécifie les rappels renvoyés dans la réponse à **une demande GetReminders.** 
  
```XML
<Reminders>
   <Reminder></Reminder>
</Reminders>
```

 **ArrayOfRemindersType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

[Reminder](reminder.md)
  
### <a name="parent-elements"></a>Éléments parents

[GetRemindersResponse](getremindersresponse.md)
  
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



[GetRemindersResponse](getremindersresponse.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

