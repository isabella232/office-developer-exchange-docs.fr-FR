---
title: EcpUrl-aggr (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: 0e7879e3-9b8f-4f23-8291-bacec0e479c0
description: L’élément EcpUrl-aggr spécifie une URL partielle qui peut être combinée avec la valeur de l’élément EcpUrl (POX) pour générer une URL qui peut être utilisée pour accéder aux paramètres d’agrégation de messagerie pour un utilisateur à extension messagerie.
ms.openlocfilehash: b959747f05f6921b43d3d50512202c6423e899aa
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59545277"
---
# <a name="ecpurl-aggr-pox"></a>EcpUrl-aggr (POX)

L’élément **EcpUrl-aggr** spécifie une URL partielle qui peut être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour accéder aux paramètres d’agrégation de messagerie pour un utilisateur à extension messagerie. 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[EcpUrl-aggr (POX)](ecpurl-aggr-pox.md)
  
```XML
<EcpUrl-aggr/>
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
|[Protocol (POX)](protocol-pox.md) <br/> |Contient les spécifications de connexion d’un client à l’ordinateur qui exécute Microsoft Exchange Server sur qui le rôle serveur d’accès au client est installé.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur de texte représente une URL partielle qui peut être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour accéder aux paramètres d’agrégation de messagerie pour l’utilisateur. 
  
## <a name="remarks"></a>Remarques

**L’élément EcpUrl-aggr** est un élément enfant facultatif de **l’élément Protocol.** 
  
## <a name="see-also"></a>Voir aussi



[Éléments XML de découverte automatique POX pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

