---
title: StatusEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- StatusEvent
api_type:
- schema
ms.assetid: d3901818-2640-4bed-aad8-21a61aee62a1
description: L’élément StatusEvent représente une notification qu’aucune nouvelle activité n’a eu lieu dans la boîte aux lettres.
ms.openlocfilehash: 777d5cd22e47fea6e7bf7432e58e5d58d1ef67a4
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543974"
---
# <a name="statusevent"></a>StatusEvent

**L’élément StatusEvent** représente une notification qu’aucune nouvelle activité n’a eu lieu dans la boîte aux lettres. 
  
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
|[Watermark](watermark.md) <br/> |Représente le dernier filigrane valide pour un abonnement.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Notification](notification-ex15websvcsotherref.md) <br/> |Contient des informations sur l’abonnement et les événements qui se sont produits depuis la dernière notification.  <br/> |
   
## <a name="remarks"></a>Remarques

**L’élément StatusEvent** est renvoyé dans une notification pour l’une des raisons suivantes : 
  
- Un client pull émettra une demande GetEvents sur un abonnement qui n’a aucune activité.
    
- Un client Push n’a aucun événement dans la file d’attente lorsque [statusFrequency](statusfrequency.md) a été atteint. 
    
Le **filigrane StatusEvent**[est](watermark.md) utilisé par une application cliente de la même manière que les autres filigranes de type d’événement. Toutefois, le filigrane de **StatusEvent** n’est pas identique aux filigranes utilisés pour d’autres événements. Par exemple, un abonnement a des événements avec des filigranes 1, 2 et 3 et ces événements ont été correctement communiqué dans une notification. Une période d’inactivité se produit et une **demande GetEvents** est envoyée. Le serveur d’accès au client (CAS) renvoie un événement d’état et inclut le dernier filigrane, 3, en tant que [PreviousMark](previouswatermark.md) et [le filigrane actuel.](watermark.md)
  
Le filigrane ne restera pas le même dans tous les cas. Les entrées d’événement sont conservées pendant 30 jours. Pour conserver un abonnement actif, le CAS met régulièrement à jour les filigranes des files d’attente d’abonnement. Les filigranes mis à jour sont envoyés aux clients pour conserver un abonnement actif.
  
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

