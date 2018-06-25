---
title: EcpUrl-tmHiding (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 9b9ae15b-3ac1-45ac-85ba-38c7231fe508
description: L’élément EcpUrl-tmHiding spécifie une URL partielle peut être combinée avec la valeur de l’élément EcpUrl (POX) pour générer une URL qui peut être utilisée pour annuler l’abonnement de l’utilisateur à partir d’une boîte aux lettres du site.
ms.openlocfilehash: 461e9780dbd657ba0ba8b9ce9ea4fe902cba9698
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756074"
---
# <a name="ecpurl-tmhiding-pox"></a>EcpUrl-tmHiding (POX)

L’élément **EcpUrl-tmHiding** spécifie une URL partielle peut être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour annuler l’abonnement de l’utilisateur à partir d’une boîte aux lettres du site. 
  
[Découverte automatique (POX)](autodiscover-pox.md)
  
[Réponse (POX)](response-pox.md)
  
[Compte (POX)](account-pox.md)
  
[Protocole (POX)](protocol-pox.md)
  
[EcpUrl-tmHiding (POX)](ecpurl-tmhiding-pox.md)
  
```XML
<EcpUrl-tmHiding/>
```

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Protocole (POX)](protocol-pox.md) <br/> |Contient les spécifications pour connecter un client à l’ordinateur qui exécute Microsoft Exchange Server qui a le rôle de serveur d’accès au Client est installé.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

La valeur de texte représente une URL partielle peut être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour annuler l’abonnement de l’utilisateur à partir d’une boîte aux lettres du site. La valeur de l’élément **EcpUrl-tmHiding** contient les paramètres contenus dans « < » et « > » caractères sont remplacés par le client, comme indiqué dans le tableau suivant. 
  
|**Paramètre**|**Remplacer par**|
|:-----|:-----|
| 
  _Id_ <br/> |L’adresse de messagerie SMTP ou la X500 le nom de la boîte aux lettres de site unique.  <br/> |
   
## <a name="remarks"></a>Remarques

L’élément **EcpUrl-tmHiding** est un élément enfant facultatif de l’élément de **protocole** . 
  
## <a name="see-also"></a>Voir aussi



[Éléments du fichier XML Autodiscover variole pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

