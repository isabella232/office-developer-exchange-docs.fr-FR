---
title: Serveur (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 0ce51644-7f3a-408c-a398-814439b658dc
description: L’élément Server spécifie le nom du serveur de messagerie.
ms.openlocfilehash: 6b29b153bc75b8836bfa113e126d122d620c2984
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462009"
---
# <a name="server-pox"></a>Serveur (POX)

L’élément **Server** spécifie le nom du serveur de messagerie. 
  
[Découverte automatique (POX)](autodiscover-pox.md)
  
[Réponse (POX)](response-pox.md)
  
[Compte (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[Serveur (POX)](server-pox.md)
  
```xml
<Server/>
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

La valeur texte identifie le serveur. Pour les protocoles tels que POP3, SMTP, IMAP ou NNTP, il s’agit soit d’un nom d’hôte, soit d’une adresse IP. Pour les protocoles tels que DAV ou WEB, il s’agit d’une URL.
  
## <a name="see-also"></a>Voir aussi



[Éléments XML de découverte automatique de la VARIOle pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

