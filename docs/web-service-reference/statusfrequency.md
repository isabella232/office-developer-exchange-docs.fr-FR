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
description: L’élément StatusFrequency représente la valeur du délai d’attente maximale, en minutes, dans laquelle les nouvelles tentatives sont effectuées par le serveur.
ms.openlocfilehash: 402f8978c0ec6b377dfa020f23595c8954509a07
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829589"
---
# <a name="statusfrequency"></a>StatusFrequency

L’élément **StatusFrequency** représente la valeur du délai d’attente maximale, en minutes, dans laquelle les nouvelles tentatives sont effectuées par le serveur. 
  
[S’abonner](subscribe.md)
  
[PushSubscriptionRequest](pushsubscriptionrequest.md)
  
[StatusFrequency](statusfrequency.md)
  
```XML
<StatusFrequency/>
```

 **SubscriptionStatusFrequencyType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[PushSubscriptionRequest](pushsubscriptionrequest.md) <br/> |Représente un abonnement à un abonnement de notification push d’événements.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Une valeur de texte qui représente un entier est obligatoire si cet élément est utilisé. Les valeurs possibles de cet élément sont 1 et 1440 (inclus). Cet élément est facultatif. La valeur par défaut est 30 minutes.
  
## <a name="remarks"></a>Remarques

La valeur de **StatusFrequency** est utilisée par le serveur pour réessayer une notification push lorsqu’il ne reçoit pas une réponse à une notification push ou un état ping à partir du client. Si le serveur ne reçoit pas de réponse, il réessayer d’envoyer la notification plusieurs fois avant qu’elle cesse d’envoyer la notification. Dans les services EWS, l’intervalle entre tentatives par défaut est de 30 secondes et tentatives suivantes sont toujours double l’heure de la dernière période de nouvelle tentative. Temps de nouvelle tentative ne sont pas exactes comme ils peuvent être retardées en raison d’autres charges sur le serveur. Le tableau suivant indique comment les intervalles se produisent dans les 30 minutes alloués à la valeur de **StatusFrequency** par défaut (en supposant que le serveur n’a pas trouvé les retards). 
  
|**Réessayer**|**Secondes**|**Heure**|
|:-----|:-----|:-----|
|0  <br/> |0  <br/> |Synchronisation initiale  <br/> |
|1  <br/> |30  <br/> |00:30  <br/> |
|2  <br/> |60  <br/> |01:00  <br/> |
|3  <br/> |120  <br/> |02:00  <br/> |
|4  <br/> |240  <br/> |04:00  <br/> |
|5  <br/> |480  <br/> |08:00  <br/> |
|6  <br/> |960  <br/> |16:00  <br/> |
|7  <br/> |1920  <br/> |32:00 - valeur par défaut **StatusFrequency** 30 dépassé, nouvelle tentative ne pas envoyé  <br/> |
   
Si le client ne reçoit pas les messages de notification à partir du serveur pour une période de temps qui dépasse deux fois la durée spécifiée par **StatusFrequency**, le client doit effectuer une action tels que recréer l’abonnement. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
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
  
[Filigrane](watermark.md)

