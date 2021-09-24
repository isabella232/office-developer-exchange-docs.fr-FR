---
title: CertPrincipalName (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: a24092c9-58be-4008-92c4-68ec5c6c0fa6
description: L’élément CertPrincipalName spécifie le nom principal du certificat SSL (Secure Sockets Layer) requis pour se connecter à l’organisation Microsoft Exchange Server 2007 à l’aide de SSL.
ms.openlocfilehash: 69ee49cdad09032c269ffbbcc918044daf61cb9b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523250"
---
# <a name="certprincipalname-pox"></a>CertPrincipalName (POX)

**L’élément CertPrincipalName** spécifie le nom principal du certificat SSL (Secure Sockets Layer) requis pour se connecter à l’organisation Microsoft Exchange Server 2007 à l’aide de SSL. 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[CertPrincipalName (POX)](certprincipalname-pox.md)
  
```xml
<CertPrincipalName>none or servername</CertPrinicpalName>
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
|[Protocol (POX)](protocol-pox.md) <br/> |Contient les spécifications de connexion d’un client à l’ordinateur qui exécute Exchange 2007 où le rôle serveur d’accès au client est installé.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur de texte spécifie le nom principal du certificat SSL requis pour se connecter à l’organisation Microsoft Exchange à l’aide de SSL.
  
## <a name="remarks"></a>Remarques

Si **l’élément CertPrincipalName** n’est pas spécifié, la valeur par défaut est msstd:SERVER, où SERVER est la valeur spécifiée dans l’élément [Server (POX).](server-pox.md) Par exemple, si SERVER est spécifié en tant que example.com et que **CertPrincipalName** est laissé vide avec [SSL (POX)](ssl-pox.md) allumé, la valeur par défaut de **CertPrincipalName** sera msstd:example.com. 
  
Si **aucun n’est** spécifié, Windows valide le nom principal du certificat en fonction des informations de la rubrique [Noms](https://go.microsoft.com/fwlink/?LinkId=93417) principaux sur MSDN. 
  
## <a name="see-also"></a>Voir aussi



[Éléments XML de découverte automatique POX pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

