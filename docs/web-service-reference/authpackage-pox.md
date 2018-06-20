---
title: AuthPackage (POX)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 709dbe53-6141-41f8-a2b9-a399bae47991
description: L’élément AuthPackage Spécifie le schéma d’authentification utilisé lors de l’authentification auprès du serveur Exchange qui a le rôle serveur de boîtes aux lettres.
ms.openlocfilehash: 120ec00ac82166ae2002a8fbac0edf9a1e23afc7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755352"
---
# <a name="authpackage-pox"></a>AuthPackage (POX)

L’élément **AuthPackage** Spécifie le schéma d’authentification utilisé lors de l’authentification auprès du serveur Exchange qui a le rôle serveur de boîtes aux lettres. 
  
- [Découverte automatique (POX)](autodiscover-pox.md)
  
- [Réponse (POX)](response-pox.md)
  
- [Compte (POX)](account-pox.md)
  
- [Protocole (POX)](protocol-pox.md)
  
- [AuthPackage (POX)](authpackage-pox.md)
  
```xml
<AuthPackage>basic or kerb or kerbntlm or ntlm or certificate or negotiate or nego2</AuthPackage>
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
|[Protocole (POX)](protocol-pox.md) <br/> |Contient les spécifications pour la connexion d’un client vers le serveur d’accès au Client.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

La valeur texte spécifie le schéma d’authentification utilisé lors de l’authentification auprès du serveur de boîtes aux lettres. Les valeurs possibles sont les suivantes :
  
- base
- marche
- kerbntlm
- NTLM
- certificat
- négocier
- nego2
    
## <a name="remarks"></a>Remarques

L’élément **AuthPackage** est uniquement utilisé lorsque l’élément de [Type (POX)](type-pox.md) a pour valeur texte EXCH ou EXPR. 
  
### <a name="version-differences"></a>Différences entre les versions

Office 365, Exchange Online et les versions locales d’Exchange commençant par créer 15.00.0995.014 retour une valeur de « négocier » uniquement si le serveur est configuré pour utiliser l’authentification par négociation et le client inclut un en-tête [X-ClientCanHandle](pox-autodiscover-request-for-exchange.md) qui contient « Négocier ». 
  
## <a name="see-also"></a>Voir aussi

- [Éléments du fichier XML Autodiscover variole pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

