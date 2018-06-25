---
title: Port (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 4046821a-d6f3-4764-82be-4011221ce7a3
description: L’élément Port Spécifie le port utilisé pour se connecter à la banque.
ms.openlocfilehash: f5a2155d97061a87fdf819549ec29898efe4d201
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828842"
---
# <a name="port-pox"></a>Port (POX)

L’élément **Port** Spécifie le port utilisé pour se connecter à la banque. 
  
[Découverte automatique (POX)](autodiscover-pox.md)
  
[Réponse (POX)](response-pox.md)
  
[Compte (POX)](account-pox.md)
  
[Protocole (POX)](protocol-pox.md)
  
[Port (POX)](port-pox.md)
  
```xml
<Port/>
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
|[Protocole (POX)](protocol-pox.md) <br/> |Contient les spécifications pour connecter un client à l’ordinateur qui exécute Microsoft Exchange Server 2007 ayant le rôle de serveur d’accès au Client est installé.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

La valeur de texte représente le port utilisé pour accéder au serveur Exchange.
  
## <a name="remarks"></a>Remarques

La valeur du **Port** n’est pas utilisée si l’élément de [Serveur (POX)](server-pox.md) contient une URL. 
  
## <a name="see-also"></a>Voir aussi



[Éléments du fichier XML Autodiscover variole pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

