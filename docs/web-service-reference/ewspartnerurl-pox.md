---
title: EwsPartnerUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: 2ebae21c-3efa-4239-9b49-4a3a8871449b
description: L’élément EwsPartnerUrl spécifie l’URL de la meilleure instance de point de terminaison pour Exchange Web Services (EWS) pour un utilisateur à messagerie.
ms.openlocfilehash: 88ee0abdc5b8db09a938fc5fdba717a166b42399
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59524321"
---
# <a name="ewspartnerurl-pox"></a>EwsPartnerUrl (POX)

**L’élément EwsPartnerUrl** spécifie l’URL de la meilleure instance de point de terminaison pour Exchange Web Services (EWS) pour un utilisateur à messagerie. 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[EwsPartnerUrl (POX)](ewspartnerurl-pox.md)
  
```XML
<EwsPartnerUrl/>
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

La valeur de texte représente l’URL du point de terminaison EWS pour l’utilisateur.
  
## <a name="remarks"></a>Remarques

**L’élément EwsPartnerUrl** est un élément enfant facultatif de **l’élément Protocol.** Elle équivaut à [l’élément EwsUrl (POX).](ewsurl-pox.md) 
  
## <a name="see-also"></a>Voir aussi



[Éléments XML de découverte automatique POX pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

