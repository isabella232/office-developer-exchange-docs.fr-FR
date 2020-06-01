---
title: PreviousWatermark
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PreviousWatermark
api_type:
- schema
ms.assetid: 474f4f7c-47da-47d4-8126-230012172fb5
description: L’élément PreviousWatermark représente le filigrane du dernier événement qui a été correctement communiqué au client pour l’abonnement.
ms.openlocfilehash: 1b26a645a5ec6dbbd2874b118f968866aadc32af
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461652"
---
# <a name="previouswatermark"></a>PreviousWatermark

L’élément **PreviousWatermark** représente le filigrane du dernier événement qui a été correctement communiqué au client pour l’abonnement. 
  
```xml
<PreviousWatermark/>
```

 **WatermarkType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Notification](notification-ex15websvcsotherref.md) <br/> |Contient des informations sur l’abonnement et les événements qui se sont produits depuis la dernière notification.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte est requise. La valeur texte représente le dernier filigrane. La valeur de texte ne peut pas être une chaîne vide.
  
## <a name="remarks"></a>Remarques

La propriété **PreviousWatermark** est utile au client pour déterminer la dernière notification réussie. Par exemple, si un abonnement comporte trois événements avec les filigranes 1, 2 et 3, et que la notification suivante est envoyée avec une valeur **PreviousWatermark** de 3, le client peut comparer cette valeur à la valeur de filigrane de la dernière notification reçue. Cela permet au client de s’assurer de la continuité des événements. 
  
Pour les clients de type « poussé », le **PreviousWatermark** est comparé au dernier filigrane connu côté client et local. Si les valeurs sont différentes, le client a manqué une notification d’événement et doit rétablir un abonnement à l’aide de la dernière limite locale. Par exemple, si un client poussé reçoit trois événements pour un abonnement avec les filigranes 1, 2 et 3, et que la notification suivante est dotée d’une valeur **PreviousWatermark** de 5, le client a manqué au moins une notification et doit créer un nouvel abonnement, en passant un 3 comme filigrane. 
  
Dans le cas d’un client de type pull, la valeur de **PreviousWatermark** sera identique à celle du [filigrane](watermark.md) fourni par le client dans l’appel GetEvents. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération d'abonnement](subscribe-operation.md)
  
[Opération de GetEvents](getevents-operation.md)
  
[Opération de résiliation d'abonnement](unsubscribe-operation.md)

