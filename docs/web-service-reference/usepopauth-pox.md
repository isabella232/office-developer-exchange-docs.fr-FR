---
title: UsePOPAuth (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 28f552d8-6bb8-49b4-a45c-b2053670f1cc
description: L’élément UsePOPAuth indique si les informations d’authentification fournies pour un type de compte POP3 sont également utilisées pour le protocole SMTP (Simple Mail Transfer Protocol).
ms.openlocfilehash: 8d5bfffaab31c382ad43915e18b8a7a2b2737c21
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466506"
---
# <a name="usepopauth-pox"></a>UsePOPAuth (POX)

L’élément **UsePOPAuth** indique si les informations d’authentification fournies pour un type de compte POP3 sont également utilisées pour le protocole SMTP (Simple Mail Transfer Protocol). 
  
[Découverte automatique (POX)](autodiscover-pox.md)
  
[Réponse (POX)](response-pox.md)
  
[Compte (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[UsePOPAuth (POX)](usepopauth-pox.md)
  
```xml
<UsePOPAuth>on or off</UsePOPAuth>
```

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Protocol (POX)](protocol-pox.md) <br/> |Contient les spécifications relatives à la connexion d’un client à l’ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d’accès au client est installé.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur Text indique si les informations d’authentification fournies pour un type de compte POP3 sont également utilisées pour SMTP. Les valeurs possibles sont **on** et **off**.
  
## <a name="remarks"></a>Remarques

L’élément **UsePOPAuth** est utilisé uniquement lorsque [type (POX)](type-pox.md) est SMTP. 
  
## <a name="see-also"></a>Voir aussi



[Éléments XML de découverte automatique de la VARIOle pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

