---
title: NetworkRequirements (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 1555fd2e-05b6-4b94-907b-dae9174049d9
description: L’élément NetworkRequirements contient les critères utilisés pour déterminer si l’ordinateur client est sur un réseau qui répond aux exigences du fournisseur de services Internet pour se connecter au serveur.
ms.openlocfilehash: d588f7eb12a445fba9c997c4b9db0a6842105b4e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462723"
---
# <a name="networkrequirements-pox"></a>NetworkRequirements (POX)

L’élément **NetworkRequirements** contient les critères utilisés pour déterminer si l’ordinateur client est sur un réseau qui répond aux exigences du fournisseur de services Internet pour se connecter au serveur. 
  
[Découverte automatique (POX)](autodiscover-pox.md)
  
[Réponse (POX)](response-pox.md)
  
[Compte (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[NetworkRequirements (POX)](networkrequirements-pox.md)
  
```xml
<NetworkRequirements>
   <IPv4Start/>
   <IPv4End/>
   <IPv6Start/>
   <IPv6End/>
</NetworkRequirements>
```

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[IPv4Start (POX)](ipv4start-pox.md) <br/> |Identifie le début d’une plage d’adresses IP version 4 (IPv4) utilisées pour identifier un ordinateur sur un réseau.  <br/> |
|[IPv4End (POX)](ipv4end-pox.md) <br/> |Identifie la fin d’une plage d’adresses IP version 4 (IPv4) utilisées pour identifier un ordinateur sur le réseau.  <br/> |
|[IPv6Start (POX)](ipv6start-pox.md) <br/> |Identifie le début d’une plage d’adresses IP version 6 (IPv6) utilisées pour identifier un ordinateur sur un réseau.  <br/> |
|[IPv6End (POX)](ipv6end-pox.md) <br/> |Identifie la fin d’une plage d’adresses IP version 6 (IPv6) utilisées pour identifier un ordinateur sur un réseau.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Protocol (POX)](protocol-pox.md) <br/> |Contient les spécifications relatives à la connexion d’un client à l’ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d’accès au client est installé.  <br/> |
   
## <a name="remarks"></a>Remarques

Si le client de messagerie ne correspond pas à la configuration réseau requise, il doit essayer d’autres types de protocole. Les fournisseurs de services Internet peuvent fournir un ensemble de serveurs avec des balises de [protocole](protocol-pox.md) qui ne nécessitent pas d’authentification, mais qui doivent être sur le réseau du fournisseur de services Internet. Ils peuvent répertorier un autre ensemble de serveurs qui nécessitent une authentification, mais ils ne doivent pas nécessairement se trouver sur un réseau spécifique. 
  
L’élément **NetworkRequirements** est facultatif. 
  
## <a name="see-also"></a>Voir aussi



[Éléments XML de découverte automatique de la VARIOle pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

