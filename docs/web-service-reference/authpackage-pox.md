---
title: Package (POX)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 709dbe53-6141-41f8-a2b9-a399bae47991
description: L’élément package spécifie le modèle d’authentification utilisé lors de l’authentification auprès du serveur Exchange sur lequel le rôle serveur de boîtes aux lettres est installé.
ms.openlocfilehash: 5317cf49d354a558417829e1d1b5b67cd6874309
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459103"
---
# <a name="authpackage-pox"></a>Package (POX)

L’élément **package** spécifie le modèle d’authentification utilisé lors de l’authentification auprès du serveur Exchange sur lequel le rôle serveur de boîtes aux lettres est installé. 
  
- [Découverte automatique (POX)](autodiscover-pox.md)
  
- [Réponse (POX)](response-pox.md)
  
- [Compte (POX)](account-pox.md)
  
- [Protocol (POX)](protocol-pox.md)
  
- [Package (POX)](authpackage-pox.md)
  
```xml
<AuthPackage>basic or kerb or kerbntlm or ntlm or certificate or negotiate or nego2</AuthPackage>
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
|[Protocol (POX)](protocol-pox.md) <br/> |Contient les spécifications relatives à la connexion d’un client au serveur d’accès au client.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur texte spécifie le modèle d’authentification utilisé lors de l’authentification auprès du serveur de boîtes aux lettres. Les valeurs possibles sont les suivantes :
  
- Basic
- kerb
- kerbntlm
- négociation
- certificat
- poursuivre
- nego2
    
## <a name="remarks"></a>Remarques

L’élément **package** est utilisé uniquement lorsque l’élément [type (POX)](type-pox.md) a une valeur de texte Exch ou Expr. 
  
### <a name="version-differences"></a>Différences entre les versions

Office 365, Exchange Online et les versions locales d’Exchange commençant par Build 15.00.0995.014 renvoient la valeur « Negotiate » uniquement si le serveur est configuré pour utiliser l’authentification par négociation et si le client inclut un en-tête [X-ClientCanHandle](pox-autodiscover-request-for-exchange.md) contenant « Negotiate ». 
  
## <a name="see-also"></a>Voir aussi

- [Éléments XML de découverte automatique de la VARIOle pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

