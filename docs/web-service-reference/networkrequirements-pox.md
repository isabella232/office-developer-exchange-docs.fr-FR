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
description: L’élément NetworkRequirements contient les critères utilisés pour déterminer si l’ordinateur client est sur un réseau qui répond aux exigences du fournisseur de services Internet (fournisseur de services Internet) pour se connecter au serveur.
ms.openlocfilehash: f3abcff04cd4121b8dcc7ceff7658ad389e6d0b0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828529"
---
# <a name="networkrequirements-pox"></a>NetworkRequirements (POX)

L’élément **NetworkRequirements** contient les critères utilisés pour déterminer si l’ordinateur client est sur un réseau qui répond aux exigences du fournisseur de services Internet (fournisseur de services Internet) pour se connecter au serveur. 
  
[Découverte automatique (POX)](autodiscover-pox.md)
  
[Réponse (POX)](response-pox.md)
  
[Compte (POX)](account-pox.md)
  
[Protocole (POX)](protocol-pox.md)
  
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

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[IPv4Start (POX)](ipv4start-pox.md) <br/> |Identifie le début d’une version de IP 4 (IPv4) adresses qui sont utilisés pour identifier un ordinateur sur un réseau.  <br/> |
|[IPv4End (POX)](ipv4end-pox.md) <br/> |Identifie la fin d’une version de IP 4 (IPv4) adresses qui sont utilisés pour identifier un ordinateur sur le réseau.  <br/> |
|[IPv6Start (POX)](ipv6start-pox.md) <br/> |Identifie le début d’une version 6 (IPv6) de la plage IP adresses qui sont utilisés pour identifier un ordinateur sur un réseau.  <br/> |
|[IPv6End (POX)](ipv6end-pox.md) <br/> |Identifie la fin d’une version 6 (IPv6) de la plage IP adresses qui sont utilisés pour identifier un ordinateur sur un réseau.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Protocole (POX)](protocol-pox.md) <br/> |Contient les spécifications pour connecter un client à l’ordinateur qui exécute Microsoft Exchange Server 2007 ayant le rôle de serveur d’accès au Client est installé.  <br/> |
   
## <a name="remarks"></a>Remarques

Si le client de messagerie ne correspond pas à la configuration réseau requise, il doit essayer d’autres types de protocoles. Fournisseurs de services Internet peuvent fournir un ensemble de serveurs avec des balises de [Protocole (POX)](protocol-pox.md) qui ne nécessitent pas d’authentification, mais sont nécessaires sur le réseau du fournisseur de services Internet. Fournisseurs de services Internet peuvent indiquer un autre ensemble de serveurs qui nécessitent une authentification, mais ne doivent pas se trouver sur un réseau spécifique. 
  
L’élément **NetworkRequirements** est facultative. 
  
## <a name="see-also"></a>Voir aussi



[Éléments du fichier XML Autodiscover variole pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

