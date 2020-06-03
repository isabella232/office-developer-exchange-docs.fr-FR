---
title: SubscriptionStatus
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SubscriptionStatus
api_type:
- schema
ms.assetid: 2d64ebb7-f26a-4d02-b7ef-d9d7da75f0c3
description: L’élément SubscriptionStatus décrit l’état d’un abonnement envoyé.
ms.openlocfilehash: 195ab229380f4386b39e5c3fd48208cf66e224f0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530943"
---
# <a name="subscriptionstatus"></a>SubscriptionStatus

L’élément **SubscriptionStatus** décrit l’état d’un abonnement envoyé. 
  
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
|[SendNotificationResult](sendnotificationresult.md) <br/> |Contient la réponse de l’application cliente à une notification de type transmission.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte est requise. Voici les valeurs de texte possibles pour cet élément :
  
- OK
    
- Se désinscrire
    
## <a name="remarks"></a>Remarques

Cet élément décrit l’état de l’abonnement. L’application cliente d’abonnement poussé renvoie l’État à l’ordinateur qui exécute Exchange 2007 sur lequel le rôle de serveur d’accès au client est installé après chaque notification de transmission. Si la valeur **SubscriptionStatus** est **unsubscribe**, le serveur d’accès au client cesse d’envoyer des notifications et met fin à l’abonnement. Si la valeur **SubscriptionStatus** est définie sur **OK**, le serveur d’accès au client continuera à envoyer des notifications.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

