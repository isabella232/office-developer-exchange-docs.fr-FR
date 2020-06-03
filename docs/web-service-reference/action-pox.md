---
title: Action (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: a3462c6b-453c-462a-830d-f29ee4a2babb
description: L’élément action fournit des informations qui permettent de déterminer si une autre demande de découverte automatique est nécessaire pour renvoyer les informations de configuration de l’utilisateur.
ms.openlocfilehash: f6d542b908948d09020b850b60ca1bdb025dd342
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529692"
---
# <a name="action-pox"></a>Action (POX)

L’élément **action** fournit des informations qui permettent de déterminer si une autre demande de découverte automatique est nécessaire pour renvoyer les informations de configuration de l’utilisateur. 
  
- [Découverte automatique (POX)](autodiscover-pox.md)
  
- [Réponse (POX)](response-pox.md)
  
- [Compte (POX)](account-pox.md)
  
- [Action (POX)](action-pox.md)
  
```xml
<Action>redirectUrl or redirectAddr or settings</Action>
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
|[Compte (POX)](account-pox.md) <br/> |Spécifie les paramètres de compte de l’utilisateur.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur de texte indique si une autre demande de découverte automatique est nécessaire pour récupérer les informations de configuration de l’utilisateur. Le tableau suivant répertorie les valeurs possibles.
  
|**Valeur**|**Description**|
|:-----|:-----|
|redirectUrl  <br/> |Si cette valeur est spécifiée, l’élément [redirectUrl (POX)](redirecturl-pox.md) spécifie l’URL du serveur d’accès au client à utiliser dans la demande de découverte automatique suivante. L’application cliente doit arrêter la redirection après 10 redirections.  <br/> |
|redirectAddr  <br/> |Si cette valeur est spécifiée, l’élément [RedirectAddr (POX)](redirectaddr-pox.md) indique l’adresse de messagerie qui doit être utilisée pour une demande de découverte automatique ultérieure.  <br/> |
|paramètres  <br/> |Si cette valeur est spécifiée, la réponse de découverte automatique contient les paramètres qui sont utilisés pour configurer le compte. La plupart des paramètres seront disponibles dans l’élément [Protocol (POX)](protocol-pox.md) .  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de découverte automatique de la VARIOle pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

