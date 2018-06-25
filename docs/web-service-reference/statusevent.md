---
title: StatusEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StatusEvent
api_type:
- schema
ms.assetid: d3901818-2640-4bed-aad8-21a61aee62a1
description: L’élément StatusEvent représente une notification qu’aucune nouvelle activité se n’est produite dans la boîte aux lettres.
ms.openlocfilehash: e214918f9795e9e29061d4aac72ab144d2b24267
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829592"
---
# <a name="statusevent"></a>StatusEvent

L’élément **StatusEvent** représente une notification qu’aucune nouvelle activité se n’est produite dans la boîte aux lettres. 
  
```xml
<StatusEvent>
   <Watermark/>
</StatusEvent>
```

 **BaseNotificationEventType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Filigrane](watermark.md) <br/> |Représente le dernier filigrane valid pour un abonnement.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Notification](notification-ex15websvcsotherref.md) <br/> |Contient des informations sur l’abonnement et les événements qui se sont produites depuis la dernière notification.  <br/> |
   
## <a name="remarks"></a>Remarques

L’élément **StatusEvent** est retournée dans une notification pour les raisons suivantes : 
  
- Un client de type pull émet une demande de GetEvents sur un abonnement ayant aucune activité.
    
- Un client push a pas d’événements dans la file d’attente lors de la [StatusFrequency](statusfrequency.md) a été atteinte. 
    
**StatusEvent**[filigrane](watermark.md) est utilisé par une application cliente dans la même manière que les autres filigranes de type événement. Toutefois, la limite pour le **StatusEvent** n’est pas le même que les filigranes utilisés pour d’autres événements. Par exemple, un abonnement a des événements avec filigranes 1, 2 et 3 et les événements ont été communiquées correctement dans une notification. Cet événement se produit une période d’inactivité et une demande **GetEvents** est envoyée. Le serveur d’accès au Client (CAS) retourne un événement d’état et inclut le dernier filigrane, 3, comme le [PreviousWatermark](previouswatermark.md) et le cours [filigrane](watermark.md).
  
La limite pas restent les mêmes dans tous les cas. Entrées d’événements sont conservées pendant 30 jours. Pour maintenir un abonnement actif, les autorités de certification met régulièrement à jour les filigranes des files d’attente de l’abonnement. Les filigranes mis à jour sont envoyées aux clients pour mettre à jour d’un abonnement actif.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
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

