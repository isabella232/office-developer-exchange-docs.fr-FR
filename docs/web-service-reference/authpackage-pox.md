---
title: AuthPackage (POX)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 709dbe53-6141-41f8-a2b9-a399bae47991
description: L’élément AuthPackage spécifie le schéma d’authentification utilisé lors de l’authentification sur le serveur Exchange sur qui le rôle serveur de boîtes aux lettres est installé.
ms.openlocfilehash: aff4e84cd44d76c2c5a913b6627e1b0c87bab4dc
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513023"
---
# <a name="authpackage-pox"></a>AuthPackage (POX)

**L’élément AuthPackage** spécifie le schéma d’authentification utilisé lors de l’authentification sur le serveur Exchange sur qui le rôle serveur de boîtes aux lettres est installé. 
  
- [AutoDiscover (POX)](autodiscover-pox.md)
  
- [Response (POX)](response-pox.md)
  
- [Account (POX)](account-pox.md)
  
- [Protocol (POX)](protocol-pox.md)
  
- [AuthPackage (POX)](authpackage-pox.md)
  
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
|[Protocol (POX)](protocol-pox.md) <br/> |Contient les spécifications de connexion d’un client au serveur d’accès au client.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur de texte spécifie le schéma d’authentification utilisé lors de l’authentification sur le serveur de boîtes aux lettres. Les valeurs possibles sont les suivantes :
  
- basic
- kerb
- kerbntlm
- ntlm
- certificat
- négocier
- nego2
    
## <a name="remarks"></a>Remarques

**L’élément AuthPackage est** utilisé uniquement lorsque l’élément [Type (POX)](type-pox.md) a une valeur de texte EXCH ou EXPR. 
  
### <a name="version-differences"></a>Différences entre les versions

Office 365, les versions Exchange Online et sur site de Exchange à partir de la build 15.00.0995.014 retournent la valeur « négocier » uniquement si le serveur est configuré pour utiliser l’authentification Negotiate et que le client inclut un [en-tête X-ClientCanHandle](pox-autodiscover-request-for-exchange.md) contenant « Negotiate ». 
  
## <a name="see-also"></a>Voir aussi

- [Éléments XML de découverte automatique POX pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

