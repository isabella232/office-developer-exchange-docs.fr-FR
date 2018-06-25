---
title: Délai d’expiration (durée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bb15f9a7-8ea5-4765-9877-762c3f98bf50
description: L’élément Timeout spécifie l’intervalle de temps avant un abonnement est dépassé par le serveur.
ms.openlocfilehash: 23b210dcdd87f2388aecec246068f12ec6c69a78
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838698"
---
# <a name="timeout-duration"></a>Délai d’expiration (durée)

L’élément **Timeout** Spécifie l’intervalle de temps avant un abonnement est dépassé par le serveur. 
  
```XML
<Timeout></Timeout>
```

 **SubscriptionTimeoutType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[PullSubscriptionRequest](pullsubscriptionrequest.md)
  
## <a name="text-value"></a>Valeur de texte

La valeur de texte de l’élément de **délai d’attente** est la durée, en minutes, avant qu’un abonnement est dépassé par le serveur. La valeur minimale est 1 ; la valeur maximale est de 1440. 
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> ||
   

