---
title: Délai d’expiration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Timeout
api_type:
- schema
ms.assetid: c2e1ca5a-6667-4f6f-aac4-89de33bddc54
description: L’élément Timeout représente la durée, en minutes, pendant qui l’abonnement peut rester inactif sans demande GetEvents du client.
ms.openlocfilehash: d0b5945f5d116e0ebb7a24a23970e785761fb0c9
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59534166"
---
# <a name="timeout"></a>Délai d’expiration

**L’élément Timeout** représente la durée, en minutes, pendant qui l’abonnement peut rester inactif sans demande GetEvents du client. 
  
```xml
<Timeout/>
```

 **int**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[PullSubscriptionRequest](pullsubscriptionrequest.md) <br/> |Représente un abonnement à un abonnement de notification d’événement basé sur un pull.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte qui représente un integer est requise si cet élément est utilisé. Les valeurs possibles pour cet élément sont de 1 à 1 440 inclus. Cet élément est obligatoire.
  
## <a name="remarks"></a>Remarques

Le délai d’heure de l’abonnement est réinitialisé par une demande GetEvents réussie.
  
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

