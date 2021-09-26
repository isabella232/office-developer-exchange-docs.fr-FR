---
title: SubscriptionStatus
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SubscriptionStatus
api_type:
- schema
ms.assetid: 2d64ebb7-f26a-4d02-b7ef-d9d7da75f0c3
description: L’élément SubscriptionStatus décrit l’état d’un abonnement Push.
ms.openlocfilehash: 6918a4965da2c075341c99581c3bd06c93da35fa
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546930"
---
# <a name="subscriptionstatus"></a>SubscriptionStatus

**L’élément SubscriptionStatus** décrit l’état d’un abonnement Push. 
  
```xml
<SubscriptionStatus>OK or Unsubscribe</SubscriptionStatus>
```

 **SubscriptionStatusType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[SendNotificationResult](sendnotificationresult.md) <br/> |Contient la réponse de l’application cliente à une notification Push.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte est requise. Voici les valeurs de texte possibles pour cet élément :
  
- OK
    
- Unsubscribe
    
## <a name="remarks"></a>Remarques

Cet élément décrit l’état de l’abonnement. L’application cliente d’abonnement Push renvoie l’état à l’ordinateur exécutant Exchange 2007 sur qui le rôle serveur d’accès au client est installé après chaque notification Push. Si la **valeur SubscriptionStatus** est égale **à Unsubscribe,** le serveur d’accès au client cesse d’envoyer des notifications et termine l’abonnement. Si la **valeur SubscriptionStatus** est égale à **OK,** le serveur d’accès au client continue d’envoyer des notifications.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

