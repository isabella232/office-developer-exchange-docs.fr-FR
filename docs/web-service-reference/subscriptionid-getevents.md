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
ms.openlocfilehash: e103386f466d65717878b4a6c811f3c3ad6e7c7d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465351"
---
# <a name="subscriptionid-getevents"></a>SubscriptionId (GetEvents)

L’élément **SubscriptionId** représente l’identificateur d’un abonnement. 
  
```xml
<SubscriptionId/>
```

 **SubscriptionIdType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetEvents](getevents.md) <br/> |Représente l’opération utilisée par les clients de type pull pour demander des notifications à partir du serveur.  <br/> |
|[Notification](notification-ex15websvcsotherref.md) <br/> |Contient des informations sur l’abonnement et les événements qui se sont produits depuis la dernière notification.  <br/> |
|[SubscribeResponseMessage](subscriberesponsemessage.md) <br/> |Contient l’État et le résultat d’une demande subscribe.  <br/> |
|[Se désabonner](unsubscribe.md) <br/> |Contient les propriétés utilisées pour annuler l’abonnement à un abonnement.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte est requise. La valeur texte est un GUID.
  
## <a name="remarks"></a>Remarques

Le GUID qui représente l’identificateur d’abonnement est généré par le serveur d’accès au client lors de la création de l’abonnement.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |schéma des messages  <br/> |
|Fichier de validation  <br/> |messages. xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération d'abonnement](subscribe-operation.md)
  
[Opération de GetEvents](getevents-operation.md)
  
[Opération de résiliation d'abonnement](unsubscribe-operation.md)

