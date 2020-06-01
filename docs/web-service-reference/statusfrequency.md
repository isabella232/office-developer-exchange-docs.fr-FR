---
title: StatusFrequency
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StatusFrequency
api_type:
- schema
ms.assetid: 917474e2-a426-4166-b825-53783a41dad4
description: L’élément StatusFrequency représente la valeur de délai d’expiration maximale, en minutes, pendant laquelle les nouvelles tentatives sont tentées par le serveur.
ms.openlocfilehash: db14ecfd54584188b3da16bb369db6c8089c70f4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/01/2020
ms.locfileid: "44468242"
---
# <a name="statusfrequency"></a>StatusFrequency

L’élément **StatusFrequency** représente la valeur de délai d’expiration maximale, en minutes, pendant laquelle les nouvelles tentatives sont tentées par le serveur. 
  
[S’abonner](subscribe.md)
  
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
|[PushSubscriptionRequest](pushsubscriptionrequest.md) <br/> |Représente un abonnement à un abonnement de notification d’événement basé sur un type de message.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte qui représente un entier est requise si cet élément est utilisé. Les valeurs possibles de cet élément sont comprises entre 1 et 1440 inclus. Cet élément est facultatif. La valeur par défaut est 30 minutes.
  
## <a name="remarks"></a>Remarques

La valeur **StatusFrequency** est utilisée par le serveur pour renouveler une notification de transmission lorsqu’il ne reçoit pas de réponse à une notification d’envoi ou à un ping d’État à partir du client. Si le serveur ne reçoit pas de réponse, il essaie d’envoyer la notification plusieurs fois avant d’arrêter l’envoi de la notification. Dans EWS, l’intervalle de nouvelle tentative par défaut est de 30 secondes et les tentatives suivantes sont toujours effectuées deux fois l’heure de la dernière tentative. Les durées de nouvelle tentative ne sont pas exactes car elles peuvent être retardées en raison d’autres charges sur le serveur. Le tableau suivant indique comment les intervalles de nouvelle tentative se produisent dans les 30 minutes allouées par la valeur **StatusFrequency** par défaut (en supposant que le serveur n’a rencontré aucun retard). 
  
|**Réessayer**|**Secondes**|**Time**|
|:-----|:-----|:-----|
|0  <br/> |0  <br/> |Synchronisation initiale  <br/> |
|1   <br/> |0,30  <br/> |00:30  <br/> |
|n°2  <br/> |60  <br/> |01:00  <br/> |
|3  <br/> |120  <br/> |02:00  <br/> |
|4   <br/> |240  <br/> |04:00  <br/> |
|5   <br/> |480  <br/> |08:00  <br/> |
|6   <br/> |960  <br/> |16:00  <br/> |
|7   <br/> |1920  <br/> |32:00- **StatusFrequency** valeur par défaut de 30 dépassée, nouvelle tentative non envoyée  <br/> |
   
Si le client ne reçoit pas de messages de notification du serveur pendant une période de temps qui dépasse le double de la durée spécifiée par **StatusFrequency**, le client doit effectuer une action telle que la recréation de l’abonnement. 
  
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

