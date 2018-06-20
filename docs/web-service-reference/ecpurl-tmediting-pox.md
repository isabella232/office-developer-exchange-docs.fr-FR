---
title: EcpUrl-tmEditing (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 1fbc2ea9-3f94-441b-ab42-647326bf0021
description: L’élément EcpUrl-tmEditing spécifie une URL partielle peut être combinée avec la valeur de l’élément EcpUrl (POX) pour générer une URL qui peut être utilisée pour modifier une boîte aux lettres de site existante.
ms.openlocfilehash: 29b27ffe9ef3c18a3b6471ca4a42956a43a5aaa6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756072"
---
# <a name="ecpurl-tmediting-pox"></a>EcpUrl-tmEditing (POX)

L’élément **EcpUrl-tmEditing** spécifie une URL partielle peut être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour modifier une boîte aux lettres de site existante. 
  
[Découverte automatique (POX)](autodiscover-pox.md)
  
[Réponse (POX)](response-pox.md)
  
[Compte (POX)](account-pox.md)
  
[Protocole (POX)](protocol-pox.md)
  
[EcpUrl-tmEditing (POX)](ecpurl-tmediting-pox.md)
  
```XML
<EcpUrl-tmEditing/>
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

La valeur de texte représente une URL partielle peut être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour modifier une boîte aux lettres de site existante. La valeur de l’élément **EcpUrl-tmEditing** contient les paramètres contenus dans « < » et « > » caractères sont remplacés par le client, comme indiqué dans le tableau suivant. 
  
|**Paramètre**|**Remplacer par**|
|:-----|:-----|
| 
  _Id_ <br/> |L’adresse de messagerie SMTP ou la X500 le nom de la boîte aux lettres de site unique.  <br/> |
   
## <a name="remarks"></a>Remarques

L’élément **EcpUrl-tmEditing** est un élément enfant facultatif de l’élément de **protocole** . 
  
## <a name="see-also"></a>Voir aussi



[Éléments du fichier XML Autodiscover variole pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

