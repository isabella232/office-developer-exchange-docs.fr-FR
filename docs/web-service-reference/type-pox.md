---
title: Type (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 9a627244-554f-4223-b9d8-a601b81a4a1a
description: L’élément type identifie le type du compte de messagerie configuré.
ms.openlocfilehash: ad3570094ebe28498dfdc375cf7fc255434ba20d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465099"
---
# <a name="type-pox"></a>Type (POX)

L’élément **type** identifie le type du compte de messagerie configuré. 
  
[Découverte automatique (POX)](autodiscover-pox.md)
  
[Réponse (POX)](response-pox.md)
  
[Compte (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[Type (POX)](type-pox.md)
  
```XML
<Type>WEB or EXCH or EXPR or EXHTTP</Type>
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
|[Protocol (POX)](protocol-pox.md) <br/> |Contient les spécifications relatives à la connexion d’un client au serveur Exchange.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur de texte représente le type de compte de messagerie. Le tableau suivant répertorie les valeurs possibles.
  
|**Valeur**|**Description**|
|:-----|:-----|
|EXCH  <br/> |Le protocole utilisé pour se connecter au serveur est Exchange RPC.  <br/> |
|HTTP  <br/> |Protocole utilisé pour se connecter aux connexions RPC/HTTP du serveur.  <br/> |
|ARGUMENT  <br/> |Le protocole utilisé pour se connecter au serveur est Exchange RPC sur HTTP à l’aide d’un serveur proxy RPC.  <br/> Ceci s’applique uniquement lorsque l’élément [AccountType (POX)](accounttype-pox.md) est défini sur courrier électronique.  <br/> |
|WEB  <br/> |Le courrier électronique est accessible à partir d’un navigateur Web à l’aide de l’URL spécifiée dans l’élément [serveur (POX)](server-pox.md) .  <br/> Ceci s’applique uniquement lorsque l’élément [AccountType (POX)](accounttype-pox.md) est défini sur courrier électronique.  <br/> |
   
### <a name="version-differences"></a>Différences entre les versions

Office 365, Exchange Online et les versions locales d’Exchange commençant par Build 15.00.0995.014 renvoient la valeur « exhttp » uniquement si le serveur est configuré pour accepter les connexions RPC/HTTP et si le client inclut un en-tête [X-ClientCanHandle](pox-autodiscover-request-for-exchange.md) contenant « ExHttpInfo ». 
  
## <a name="see-also"></a>Voir aussi



[Éléments XML de découverte automatique de la VARIOle pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

