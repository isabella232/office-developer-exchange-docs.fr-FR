---
title: Timeout (Duration)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: bb15f9a7-8ea5-4765-9877-762c3f98bf50
description: L’élément Timeout spécifie la durée avant le délai d’un abonnement pull par le serveur.
ms.openlocfilehash: a5a9e094c25f609c0bcfa207ab96ae7f0877f43f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59545768"
---
# <a name="timeout-duration"></a>Timeout (Duration)

**L’élément Timeout** spécifie la durée avant le délai d’un abonnement pull par le serveur. 
  
```XML
<Timeout></Timeout>
```

 **SubscriptionTimeoutType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[PullSubscriptionRequest](pullsubscriptionrequest.md)
  
## <a name="text-value"></a>Valeur texte

La valeur texte de l’élément **Timeout** est la durée, en minutes, avant qu’un abonnement pull ne soit hors délai par le serveur. La valeur minimale est 1 ; la valeur maximale est 1 440. 
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> ||
   

