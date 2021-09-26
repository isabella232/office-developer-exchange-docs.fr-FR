---
title: EcpUrl-extinstall (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: f81807e6-93de-4e47-afee-1e1ae6a85054
description: L’élément EcpUrl-extinstall spécifie une URL partielle qui peut être combinée avec la valeur de l’élément EcpUrl (POX) pour générer une URL qui peut être utilisée pour afficher ou modifier les applications de messagerie actuellement installées dans la boîte aux lettres de l’utilisateur.
ms.openlocfilehash: bf91b12cbcff3b08b3b13569eac9c957dea12757
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541419"
---
# <a name="ecpurl-extinstall-pox"></a>EcpUrl-extinstall (POX)

L’élément **EcpUrl-extinstall** spécifie une URL partielle qui peut être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour afficher ou modifier les applications de messagerie actuellement installées dans la boîte aux lettres de l’utilisateur. 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[EcpUrl-extinstall (POX)](ecpurl-extinstall-pox.md)
  
```XML
<EcpUrl-extinstall/>
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

La valeur de texte représente une URL partielle qui peut être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour afficher ou modifier les applications de messagerie actuellement installées dans la boîte aux lettres de l’utilisateur. 
  
## <a name="remarks"></a>Remarques

**L’élément EcpUrl-extinstall** est un élément enfant facultatif de **l’élément Protocol.** 
  
## <a name="see-also"></a>Voir aussi



[Éléments XML de découverte automatique POX pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

