---
title: EmwsUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: cad0fa91-8d75-4dde-a484-518c837ae063
description: L’élément EmwsUrl Spécifie l’URL de l’instance de point de terminaison meilleures pour Exchange Web Services (EWS) pour un utilisateur à extension messagerie.
ms.openlocfilehash: d8905d098c9978c3413f67e9a1b2443a52fb0d1f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756154"
---
# <a name="emwsurl-pox"></a>EmwsUrl (POX)

L’élément **EmwsUrl** Spécifie l’URL de l’instance de point de terminaison meilleures pour Exchange Web Services (EWS) pour un utilisateur à extension messagerie. 
  
- [Découverte automatique (POX)](autodiscover-pox.md) 
- [Réponse (POX)](response-pox.md) 
- [Compte (POX)](account-pox.md) 
- [Protocole (POX)](protocol-pox.md) 
- [EmwsUrl (POX)](emwsurl-pox.md)
  
```XML
<EmwsUrl/>
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

La valeur de text représente l’URL du point de terminaison EWS pour l’utilisateur. Elle est équivalente à l’élément [EwsUrl (POX)](ewsurl-pox.md) . 
  
## <a name="remarks"></a>Remarques

L’élément **EmwsUrl** est un élément enfant facultatif de l’élément de **protocole** . 
  
## <a name="see-also"></a>Voir aussi

- [Éléments du fichier XML Autodiscover variole pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

