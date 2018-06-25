---
title: SubscriptionId (GetEvents)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SubscriptionId
api_type:
- schema
ms.assetid: 77c0abab-69e8-428e-8c20-22258e4ef71b
description: L’élément SubscriptionId représente l’identificateur d’un abonnement.
ms.openlocfilehash: 8867b7da7c75cfd9d41f708c0481627d5186cc14
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829622"
---
# <a name="subscriptionid-getevents"></a>SubscriptionId (GetEvents)

L’élément **SubscriptionId** représente l’identificateur d’un abonnement. 
  
```xml
<SubscriptionId/>
```

 **SubscriptionIdType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetEvents](getevents.md) <br/> |Représente l’opération utilisée par les clients de l’extraction pour demander des notifications à partir du serveur.  <br/> |
|[Notification](notification-ex15websvcsotherref.md) <br/> |Contient des informations sur l’abonnement et les événements qui se sont produites depuis la dernière notification.  <br/> |
|[SubscribeResponseMessage](subscriberesponsemessage.md) <br/> |Contient l’état et les résultats d’une demande Subscribe.  <br/> |
|[Annuler l’abonnement](unsubscribe.md) <br/> |Contient les propriétés utilisées pour annuler l’abonnement à partir d’un abonnement.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Une valeur texte est requise. La valeur de texte est un GUID.
  
## <a name="remarks"></a>Remarques

Le GUID qui représente l’identificateur d’abonnement est généré par le serveur d’accès au Client lors de la création de l’abonnement.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |schéma des messages  <br/> |
|Fichier de validation  <br/> |messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération d'abonnement](subscribe-operation.md)
  
[Opération de GetEvents](getevents-operation.md)
  
[Opération de résiliation d'abonnement](unsubscribe-operation.md)

