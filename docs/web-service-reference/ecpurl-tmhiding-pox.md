---
title: EcpUrl-tmHiding (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 9b9ae15b-3ac1-45ac-85ba-38c7231fe508
description: L’élément EcpUrl-tmHiding spécifie une URL partielle qui peut être combinée avec la valeur de l’élément EcpUrl (POX) pour générer une URL qui peut être utilisée pour annuler l’abonnement de l’utilisateur à partir d’une boîte aux lettres de site.
ms.openlocfilehash: 68b949db8b8d98caddbac3b9f96c5d5e55b104b7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463530"
---
# <a name="ecpurl-tmhiding-pox"></a>EcpUrl-tmHiding (POX)

L’élément **EcpUrl-tmHiding** spécifie une URL partielle qui peut être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour annuler l’abonnement de l’utilisateur à partir d’une boîte aux lettres de site. 
  
[Découverte automatique (POX)](autodiscover-pox.md)
  
[Réponse (POX)](response-pox.md)
  
[Compte (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[EcpUrl-tmHiding (POX)](ecpurl-tmhiding-pox.md)
  
```XML
<EcpUrl-tmHiding/>
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

La valeur de texte représente une URL partielle qui peut être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour annuler l’abonnement de l’utilisateur à partir d’une boîte aux lettres de site. La valeur de l’élément **EcpUrl-tmHiding** contient les paramètres contenus dans les caractères « < » et « > » qui sont remplacés par le client, comme indiqué dans le tableau suivant. 
  
|**Parameter**|**Remplacer par**|
|:-----|:-----|
| _Id_ <br/> |Adresse de messagerie SMTP ou nom unique X500 de la boîte aux lettres de site.  <br/> |
   
## <a name="remarks"></a>Remarques

L’élément **EcpUrl-tmHiding** est un élément enfant facultatif de l’élément **Protocol** . 
  
## <a name="see-also"></a>Voir aussi



[Éléments XML de découverte automatique de la VARIOle pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

