---
title: EwsPartnerUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 2ebae21c-3efa-4239-9b49-4a3a8871449b
description: L’élément EwsPartnerUrl Spécifie l’URL de l’instance de point de terminaison meilleures pour Exchange Web Services (EWS) pour un utilisateur à extension messagerie.
ms.openlocfilehash: 97c33e1fed4adc8a9e8542d85e67c942118f6096
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756240"
---
# <a name="ewspartnerurl-pox"></a>EwsPartnerUrl (POX)

L’élément **EwsPartnerUrl** Spécifie l’URL de l’instance de point de terminaison meilleures pour Exchange Web Services (EWS) pour un utilisateur à extension messagerie. 
  
[Découverte automatique (POX)](autodiscover-pox.md)
  
[Réponse (POX)](response-pox.md)
  
[Compte (POX)](account-pox.md)
  
[Protocole (POX)](protocol-pox.md)
  
[EwsPartnerUrl (POX)](ewspartnerurl-pox.md)
  
```XML
<EwsPartnerUrl/>
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

La valeur de text représente l’URL du point de terminaison EWS pour l’utilisateur.
  
## <a name="remarks"></a>Remarques

L’élément **EwsPartnerUrl** est un élément enfant facultatif de l’élément de **protocole** . Elle est équivalente à l’élément [EwsUrl (POX)](ewsurl-pox.md) . 
  
## <a name="see-also"></a>Voir aussi



[Éléments du fichier XML Autodiscover variole pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

