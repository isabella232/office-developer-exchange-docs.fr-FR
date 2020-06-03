---
title: EmwsUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: cad0fa91-8d75-4dde-a484-518c837ae063
description: L’élément EmwsUrl spécifie l’URL de la meilleure instance de point de terminaison pour les services Web Exchange (EWS) pour un utilisateur à extension messagerie.
ms.openlocfilehash: 19e1078ae8d08513e85d75d87e960a910986f727
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530669"
---
# <a name="emwsurl-pox"></a>EmwsUrl (POX)

L’élément **EmwsUrl** spécifie l’URL de la meilleure instance de point de terminaison pour les services Web Exchange (EWS) pour un utilisateur à extension messagerie. 
  
- [Découverte automatique (POX)](autodiscover-pox.md) 
- [Réponse (POX)](response-pox.md) 
- [Compte (POX)](account-pox.md) 
- [Protocol (POX)](protocol-pox.md) 
- [EmwsUrl (POX)](emwsurl-pox.md)
  
```XML
<EmwsUrl/>
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
|[Protocol (POX)](protocol-pox.md) <br/> |Contient les spécifications relatives à la connexion d’un client à l’ordinateur qui exécute Microsoft Exchange Server sur lequel le rôle de serveur d’accès au client est installé.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur de texte représente l’URL du point de terminaison EWS de l’utilisateur. Elle est équivalente à l’élément [EwsUrl (POX)](ewsurl-pox.md) . 
  
## <a name="remarks"></a>Remarques

L’élément **EmwsUrl** est un élément enfant facultatif de l’élément **Protocol** . 
  
## <a name="see-also"></a>Voir aussi

- [Éléments XML de découverte automatique de la VARIOle pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

