---
title: StatusFrequency
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- StatusFrequency
api_type:
- schema
ms.assetid: 917474e2-a426-4166-b825-53783a41dad4
description: L’élément StatusFrequency représente la valeur de délai d’attente maximale, en minutes, pendant laquelle les tentatives de nouvelles tentatives sont tentées par le serveur.
ms.openlocfilehash: f0359bab58167bbe7be5cce8c250240bebc7cc08
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59525532"
---
# <a name="statusfrequency"></a>StatusFrequency

**L’élément StatusFrequency** représente la valeur de délai d’attente maximale, en minutes, pendant laquelle les tentatives de nouvelles tentatives sont tentées par le serveur. 
  
[Subscribe](subscribe.md)
  
[PushSubscriptionRequest](pushsubscriptionrequest.md)
  
[StatusFrequency](statusfrequency.md)
  
```XML
<StatusFrequency/>
```

 **SubscriptionStatusFrequencyType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[PushSubscriptionRequest](pushsubscriptionrequest.md) <br/> |Représente un abonnement à un abonnement de notification d’événements push.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte qui représente un integer est requise si cet élément est utilisé. Les valeurs possibles pour cet élément sont de 1 à 1 440 inclus. Cet élément est facultatif. La valeur par défaut est 30 minutes.
  
## <a name="remarks"></a>Remarques

La **valeur StatusFrequency** est utilisée par le serveur pour réessayer une notification Push lorsqu’il ne reçoit pas de réponse à une notification Push ou à un ping d’état du client. Si le serveur ne reçoit pas de réponse, il retente l’envoi de la notification plusieurs fois avant d’arrêter l’envoi de la notification. Dans EWS, l’intervalle de nouvelle tentative par défaut est de 30 secondes et les tentatives suivantes sont toujours deux fois plus longues que la dernière tentative. Les heures de nouvelle tentative ne sont pas exactes, car elles peuvent être retardées en raison d’autres charges sur le serveur. Le tableau suivant montre comment les intervalles de nouvelle tentative se produisent dans les 30 minutes allouées par la valeur **StatusFrequency** par défaut (en supposant que le serveur n’a rencontré aucun retard). 
  
|**Réessayer**|**Secondes**|**Time**|
|:-----|:-----|:-----|
|0  <br/> |0  <br/> |Synchronisation initiale  <br/> |
|1  <br/> |30  <br/> |00:30  <br/> |
|2  <br/> |60  <br/> |01:00  <br/> |
|3  <br/> |120  <br/> |02:00  <br/> |
|4   <br/> |240  <br/> |04:00  <br/> |
|5  <br/> |480  <br/> |08:00  <br/> |
|6   <br/> |960  <br/> |16:00  <br/> |
|7   <br/> |1920  <br/> |32:00 - La valeur par défaut **StatusFrequency** de 30 est dépassée, nouvelle tentative non envoyée  <br/> |
   
Si le client ne reçoit pas de messages de notification du serveur pendant une période qui dépasse le double du temps spécifié par **StatusFrequency,** le client doit prendre une action telle que la recréation de l’abonnement. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
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
  
[Watermark](watermark.md)

