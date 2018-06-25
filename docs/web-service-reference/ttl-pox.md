---
title: TTL (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 178eefa1-995c-4bea-930b-e51293961191
description: L’élément de durée de vie spécifie la durée de vie, en heures, pendant laquelle les paramètres restent valides.
ms.openlocfilehash: 5fecf3103553a82ed2aeeecfc1e4e1b9fe38583c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838781"
---
# <a name="ttl-pox"></a>TTL (POX)

L’élément de **durée de vie** spécifie la durée de vie, en heures, pendant laquelle les paramètres restent valides. 
  
[Découverte automatique (POX)](autodiscover-pox.md)
  
[Réponse (POX)](response-pox.md)
  
[Compte (POX)](account-pox.md)
  
[Protocole (POX)](protocol-pox.md)
  
[TTL (POX)](ttl-pox.md)
  
```xml
<TTL/>
```

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Protocole (POX)](protocol-pox.md) <br/> |Contient les spécifications pour connecter un client à l’ordinateur Exchange Server 2007 sur lequel est installé le rôle de serveur d’accès au Client.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

La valeur de texte représente la durée de vie, en heures, pendant laquelle les paramètres restent valides. La valeur zéro indique que redécouverte n’est pas obligatoire. Si aucune valeur n’est pas spécifié, la valeur par défaut de cet élément est 1 heure.
  
## <a name="remarks"></a>Remarques

Une fois le temps qui est représenté par l’élément de **durée de vie** écoulée, doivent identifier les paramètres à l’aide d’une requête de découverte automatique. 
  
## <a name="see-also"></a>Voir aussi



[Éléments du fichier XML Autodiscover variole pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

