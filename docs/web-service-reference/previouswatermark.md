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
description: L’élément PreviousWatermark représente la limite du dernier événement qui a été correctement transmis au client pour l’abonnement.
ms.openlocfilehash: 93c6f90d0866ae13618391b8544ab593fe33922b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828886"
---
# <a name="previouswatermark"></a>PreviousWatermark

L’élément **PreviousWatermark** représente la limite du dernier événement qui a été correctement transmis au client pour l’abonnement. 
  
```xml
<PreviousWatermark/>
```

 **WatermarkType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Notification](notification-ex15websvcsotherref.md) <br/> |Contient des informations sur l’abonnement et les événements qui se sont produites depuis la dernière notification.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Une valeur texte est requise. La valeur de texte représente la limite le plus récent. La valeur de texte ne peut pas être une chaîne vide.
  
## <a name="remarks"></a>Remarques

La propriété **PreviousWatermark** est utile pour le client lors de la détermination de la dernière notification réussie. Par exemple, si un abonnement a trois événements avec des filigranes 1, 2 et 3, et la prochaine notification est envoyée avec la valeur **PreviousWatermark** 3, le client peut comparer cette valeur à la limite supérieure de la dernière notification reçue. Ainsi, le client à assurer la continuité des événements. 
  
Pour les clients push, le **PreviousWatermark** est comparé à la limite connue dernière locale, côté client. Si les valeurs sont différentes, le client a manqué une notification d’événement et doit rétablir un abonnement à l’aide de la dernière filigrane local. Par exemple, si un client push reçoit trois événements pour un abonnement avec filigranes 1, 2 et 3, et la notification suivante est fourni avec une valeur **PreviousWatermark** 5, le client a manqué au moins une notification et doit créer un nouvel abonnement en passant un 3 en tant que filigrane. 
  
Dans le cas d’un client extrait, la valeur de **PreviousWatermark** sera la même que le [filigrane](watermark.md) inclus par le client lors de l’appel GetEvents. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération d'abonnement](subscribe-operation.md)
  
[Opération de GetEvents](getevents-operation.md)
  
[Opération de résiliation d'abonnement](unsubscribe-operation.md)

