---
title: EwsPartnerUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 2ebae21c-3efa-4239-9b49-4a3a8871449b
description: L’élément EwsPartnerUrl spécifie l’URL de la meilleure instance de point de terminaison pour les services Web Exchange (EWS) pour un utilisateur à extension messagerie.
ms.openlocfilehash: a67eb17bb3db67a922c53ba5e37900ee0a9b956b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526108"
---
# <a name="ewspartnerurl-pox"></a>EwsPartnerUrl (POX)

L’élément **EwsPartnerUrl** spécifie l’URL de la meilleure instance de point de terminaison pour les services Web Exchange (EWS) pour un utilisateur à extension messagerie. 
  
[Découverte automatique (POX)](autodiscover-pox.md)
  
[Réponse (POX)](response-pox.md)
  
[Compte (POX)](account-pox.md)
  
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
|[Protocol (POX)](protocol-pox.md) <br/> |Contient les spécifications relatives à la connexion d’un client à l’ordinateur qui exécute Microsoft Exchange Server sur lequel le rôle de serveur d’accès au client est installé.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur de texte représente l’URL du point de terminaison EWS de l’utilisateur.
  
## <a name="remarks"></a>Remarques

L’élément **EwsPartnerUrl** est un élément enfant facultatif de l’élément **Protocol** . Elle est équivalente à l’élément [EwsUrl (POX)](ewsurl-pox.md) . 
  
## <a name="see-also"></a>Voir aussi



[Éléments XML de découverte automatique de la VARIOle pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

