---
title: EmwsUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: cad0fa91-8d75-4dde-a484-518c837ae063
description: L’élément EmwsUrl spécifie l’URL de la meilleure instance de point de terminaison pour Exchange Web Services (EWS) pour un utilisateur à messagerie.
ms.openlocfilehash: d46438f600e226bce95c5e479aca91bfa942535e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59538174"
---
# <a name="emwsurl-pox"></a>EmwsUrl (POX)

**L’élément EmwsUrl** spécifie l’URL de la meilleure instance de point de terminaison pour Exchange Web Services (EWS) pour un utilisateur à messagerie. 
  
- [AutoDiscover (POX)](autodiscover-pox.md) 
- [Response (POX)](response-pox.md) 
- [Account (POX)](account-pox.md) 
- [Protocol (POX)](protocol-pox.md) 
- [EmwsUrl (POX)](emwsurl-pox.md)
  
```XML
<EmwsUrl/>
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

La valeur de texte représente l’URL du point de terminaison EWS pour l’utilisateur. Elle équivaut à [l’élément EwsUrl (POX).](ewsurl-pox.md) 
  
## <a name="remarks"></a>Remarques

**L’élément EmwsUrl** est un élément enfant facultatif de **l’élément Protocol.** 
  
## <a name="see-also"></a>Voir aussi

- [Éléments XML de découverte automatique POX pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

