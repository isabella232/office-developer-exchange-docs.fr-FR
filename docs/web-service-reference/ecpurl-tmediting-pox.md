---
title: EcpUrl-tmEditing (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 1fbc2ea9-3f94-441b-ab42-647326bf0021
description: L’élément EcpUrl-tmEditing spécifie une URL partielle qui peut être combinée avec la valeur de l’élément EcpUrl (POX) pour générer une URL qui peut être utilisée pour modifier une boîte aux lettres de site existante.
ms.openlocfilehash: 5d6c6b8e8f73d113cfde3570065435927ffbae05
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463537"
---
# <a name="ecpurl-tmediting-pox"></a>EcpUrl-tmEditing (POX)

L’élément **EcpUrl-tmEditing** spécifie une URL partielle qui peut être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour modifier une boîte aux lettres de site existante. 
  
[Découverte automatique (POX)](autodiscover-pox.md)
  
[Réponse (POX)](response-pox.md)
  
[Compte (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[EcpUrl-tmEditing (POX)](ecpurl-tmediting-pox.md)
  
```XML
<EcpUrl-tmEditing/>
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

La valeur de texte représente une URL partielle qui peut être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour modifier une boîte aux lettres de site existante. La valeur de l’élément **EcpUrl-tmEditing** contient les paramètres contenus dans les caractères « < » et « > » qui sont remplacés par le client, comme indiqué dans le tableau suivant. 
  
|**Parameter**|**Remplacer par**|
|:-----|:-----|
| _Id_ <br/> |Adresse de messagerie SMTP ou nom unique X500 de la boîte aux lettres de site.  <br/> |
   
## <a name="remarks"></a>Remarques

L’élément **EcpUrl-tmEditing** est un élément enfant facultatif de l’élément **Protocol** . 
  
## <a name="see-also"></a>Voir aussi



[Éléments XML de découverte automatique de la VARIOle pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

