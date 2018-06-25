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
description: L’élément Action fournit des informations qui sont utilisées pour déterminer si une autre requête de découverte automatique est requise pour retourner les informations de configuration utilisateur.
ms.openlocfilehash: 118bb59f2c929e3c74683dbf3f073da34d67a3e7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756325"
---
# <a name="action-pox"></a>Action (POX)

L’élément **Action** fournit des informations qui sont utilisées pour déterminer si une autre requête de découverte automatique est requise pour retourner les informations de configuration utilisateur. 
  
- [Découverte automatique (POX)](autodiscover-pox.md)
  
- [Réponse (POX)](response-pox.md)
  
- [Compte (POX)](account-pox.md)
  
- [Action (POX)](action-pox.md)
  
```xml
<Action>redirectUrl or redirectAddr or settings</Action>
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
|[Compte (POX)](account-pox.md) <br/> |Spécifie les paramètres de compte pour l’utilisateur.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

La valeur de texte indique si une autre requête de découverte automatique est nécessaire afin de récupérer les informations de configuration de l’utilisateur. Le tableau suivant répertorie les valeurs possibles.
  
|**Valeur**|**Description**|
|:-----|:-----|
|redirectUrl  <br/> |Si cette valeur est spécifiée, l’élément [RedirectUrl (POX)](redirecturl-pox.md) sera spécifier l’URL de serveur d’accès au Client à utiliser dans la requête suivante de la découverte automatique. L’application cliente doit s’arrêter redirection après 10 redirections.  <br/> |
|redirectAddr  <br/> |Si cette valeur est spécifiée, l’élément [RedirectAddr (POX)](redirectaddr-pox.md) devez spécifier l’adresse de messagerie qui doit être utilisé pour une requête de découverte automatique suivante.  <br/> |
|settings  <br/> |Si cette valeur est spécifiée, la réponse de découverte automatique contient les paramètres qui sont utilisés pour configurer le compte. Vous trouverez la plupart des paramètres dans l’élément de [Protocole (POX)](protocol-pox.md) .  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments du fichier XML Autodiscover variole pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

