---
title: NetworkRequirements (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 1555fd2e-05b6-4b94-907b-dae9174049d9
description: L’élément NetworkRequirements contient les critères utilisés pour déterminer si l’ordinateur client se trouve sur un réseau qui répond aux exigences du fournisseur de services Internet (ISP) pour se connecter au serveur.
ms.openlocfilehash: 07a258ad48b74c614ce367db0f893ed884cf3f75
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59509512"
---
# <a name="networkrequirements-pox"></a>NetworkRequirements (POX)

**L’élément NetworkRequirements** contient les critères utilisés pour déterminer si l’ordinateur client se trouve sur un réseau qui répond aux exigences du fournisseur de services Internet (ISP) pour se connecter au serveur. 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
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
|[IPv4Start (POX)](ipv4start-pox.md) <br/> |Identifie le début d’une plage d’adresses IP de version 4 (IPv4) utilisées pour identifier un ordinateur sur un réseau.  <br/> |
|[IPv4End (POX)](ipv4end-pox.md) <br/> |Identifie la fin d’une plage d’adresses IP de version 4 (IPv4) utilisées pour identifier un ordinateur sur le réseau.  <br/> |
|[IPv6Start (POX)](ipv6start-pox.md) <br/> |Identifie le début d’une plage d’adresses IP de version 6 (IPv6) utilisées pour identifier un ordinateur sur un réseau.  <br/> |
|[IPv6End (POX)](ipv6end-pox.md) <br/> |Identifie la fin d’une plage d’adresses IP de version 6 (IPv6) utilisées pour identifier un ordinateur sur un réseau.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Protocol (POX)](protocol-pox.md) <br/> |Contient les spécifications de connexion d’un client à l’ordinateur qui exécute Microsoft Exchange Server 2007 où le rôle serveur d’accès au client est installé.  <br/> |
   
## <a name="remarks"></a>Remarques

Si le client de messagerie ne correspond pas à la demande réseau, il doit essayer d’autres types de protocole. Les fai peuvent fournir un ensemble de serveurs avec des balises de protocole [(POX)](protocol-pox.md) qui ne nécessitent pas d’authentification, mais qui doivent se trouver sur le réseau isp. Les fai peuvent lister un autre ensemble de serveurs qui nécessitent une authentification, mais qui ne doivent pas nécessairement se trouver sur un réseau spécifique. 
  
**L’élément NetworkRequirements est** facultatif. 
  
## <a name="see-also"></a>Voir aussi



[Éléments XML de découverte automatique POX pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

