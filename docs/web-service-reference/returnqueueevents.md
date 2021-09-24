---
title: ReturnQueueEvents
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ReturnQueueEvents
api_type:
- schema
ms.assetid: 69d22417-320c-4c6f-9fb4-2020f2480bb2
description: L’élément ReturnQueueEvents indique que la personne qui exécute la tâche est dans un rôle privilégié.
ms.openlocfilehash: d80513b8acdae04e447f63c5736622e577ece040
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59512260"
---
# <a name="returnqueueevents"></a>ReturnQueueEvents

**L’élément ReturnQueueEvents** indique que la personne qui exécute la tâche est dans un rôle privilégié. 
  
```XML
<ReturnQueueEvents>true | false</ReturnQueueEvents>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetMessageTrackingReport](getmessagetrackingreport.md) <br/> |Contient la demande de [l’opération GetMessageTrackingReport](getmessagetrackingreport-operation.md) pour récupérer le rapport de suivi des messages complet pour l’ID spécifié.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte qui représente une valeur Boolean est requise. La valeur **true indique** que la personne qui exécute la tâche est dans un rôle privilégié ; La valeur **false indique** que la personne qui exécute la tâche n’est pas dans un rôle privilégié. 
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération de GetMessageTrackingReport](getmessagetrackingreport-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

