---
title: Action (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: a3462c6b-453c-462a-830d-f29ee4a2babb
description: L’élément Action fournit des informations qui sont utilisées pour déterminer si une autre demande de découverte automatique est nécessaire pour renvoyer les informations de configuration de l’utilisateur.
ms.openlocfilehash: b1c07fefc6b8033b9b93bd044c04fb07ba289177
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513856"
---
# <a name="action-pox"></a>Action (POX)

**L’élément Action** fournit des informations qui sont utilisées pour déterminer si une autre demande de découverte automatique est nécessaire pour renvoyer les informations de configuration de l’utilisateur. 
  
- [AutoDiscover (POX)](autodiscover-pox.md)
  
- [Response (POX)](response-pox.md)
  
- [Account (POX)](account-pox.md)
  
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
|[Account (POX)](account-pox.md) <br/> |Spécifie les paramètres de compte de l’utilisateur.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur de texte représente si une autre demande de découverte automatique est nécessaire pour récupérer les informations de configuration de l’utilisateur. Le tableau suivant répertorie les valeurs possibles.
  
|**Valeur**|**Description**|
|:-----|:-----|
|redirectUrl  <br/> |Si cette valeur est spécifiée, l’élément [RedirectUrl (POX)](redirecturl-pox.md) spécifie l’URL du serveur d’accès au client à utiliser dans la demande de découverte automatique suivante. L’application cliente doit arrêter la redirection après 10 redirections.  <br/> |
|redirectAddr  <br/> |Si cette valeur est spécifiée, l’élément [RedirectAddr (POX)](redirectaddr-pox.md) spécifie l’adresse de messagerie à utiliser pour une demande de découverte automatique ultérieure.  <br/> |
|paramètres  <br/> |Si cette valeur est spécifiée, la réponse de découverte automatique contient les paramètres utilisés pour configurer le compte. La plupart des paramètres se trouvent dans l’élément [de protocole (POX).](protocol-pox.md)  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de découverte automatique POX pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

