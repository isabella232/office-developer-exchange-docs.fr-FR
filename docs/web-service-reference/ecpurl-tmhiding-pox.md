---
title: EcpUrl-tmHiding (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: 9b9ae15b-3ac1-45ac-85ba-38c7231fe508
description: L’élément EcpUrl-tmHiding spécifie une URL partielle qui peut être combinée avec la valeur de l’élément EcpUrl (POX) pour générer une URL qui peut être utilisée pour désabonner l’utilisateur d’une boîte aux lettres de site.
ms.openlocfilehash: d8e8ced554b96f1a0cd554d3d601970d5f47019b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59514732"
---
# <a name="ecpurl-tmhiding-pox"></a>EcpUrl-tmHiding (POX)

L’élément **EcpUrl-tmHiding** spécifie une URL partielle qui peut être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour désabonner l’utilisateur d’une boîte aux lettres de site. 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
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
|[Protocol (POX)](protocol-pox.md) <br/> |Contient les spécifications de connexion d’un client à l’ordinateur qui exécute Microsoft Exchange Server sur qui le rôle serveur d’accès au client est installé.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur de texte représente une URL partielle qui peut être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour désabonner l’utilisateur d’une boîte aux lettres de site. La valeur de l’élément **EcpUrl-tmHiding** contient les paramètres contenus dans les caractères « < » et « > » qui sont remplacés par le client, comme indiqué dans le tableau suivant. 
  
|**Paramètre**|**Remplacer par**|
|:-----|:-----|
| _Id_ <br/> |Adresse de messagerie SMTP ou nom X500 de la boîte aux lettres de site.  <br/> |
   
## <a name="remarks"></a>Remarques

**L’élément EcpUrl-tmHiding** est un élément enfant facultatif de **l’élément Protocol.** 
  
## <a name="see-also"></a>Voir aussi



[Éléments XML de découverte automatique POX pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

