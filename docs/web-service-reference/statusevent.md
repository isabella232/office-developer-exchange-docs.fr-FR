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
description: L’élément StatusEvent représente une notification indiquant qu’aucune nouvelle activité n’a eu lieu dans la boîte aux lettres.
ms.openlocfilehash: 8158a47937a810be2ea22346384b4e61da56ac48
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/01/2020
ms.locfileid: "44468256"
---
# <a name="statusevent"></a>StatusEvent

L’élément **StatusEvent** représente une notification indiquant qu’aucune nouvelle activité n’a eu lieu dans la boîte aux lettres. 
  
```xml
<StatusEvent>
   <Watermark/>
</StatusEvent>
```

 **BaseNotificationEventType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Watermark](watermark.md) <br/> |Représente le dernier filigrane valide d’un abonnement.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Notification](notification-ex15websvcsotherref.md) <br/> |Contient des informations sur l’abonnement et les événements qui se sont produits depuis la dernière notification.  <br/> |
   
## <a name="remarks"></a>Remarques

L’élément **StatusEvent** est renvoyé dans une notification pour l’une des raisons suivantes : 
  
- Un client de réception émet une demande GetEvents sur un abonnement qui n’a aucune activité.
    
- Un client poussé n’a pas d’événements dans la file d’attente lorsque le [StatusFrequency](statusfrequency.md) est atteint. 
    
Le **StatusEvent**[filigrane](watermark.md) StatusEvent est utilisé par une application cliente de la même manière que les autres filigranes de type d’événement. Toutefois, le filigrane de l' **StatusEvent** n’est pas le même que les filigranes utilisés pour d’autres événements. Par exemple, un abonnement comporte des événements avec les filigranes 1, 2 et 3 et ces événements ont été correctement communiqués dans une notification. Une période d’inactivité se produit et une demande **GetEvents** est envoyée. Le serveur d’accès au client (CAS) renvoie un événement d’État et inclut le dernier filigrane, 3, à la fois [PreviousWatermark](previouswatermark.md) et le [filigrane](watermark.md)actuel.
  
Le filigrane ne reste pas le même dans tous les cas. Les entrées d’événement sont conservées pendant 30 jours. Pour maintenir un abonnement actif, le CAS met régulièrement à jour les filigranes pour les files d’attente des abonnements. Les filigranes mis à jour sont envoyés aux clients pour maintenir un abonnement actif.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
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

