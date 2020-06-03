---
title: CertPrincipalName (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: a24092c9-58be-4008-92c4-68ec5c6c0fa6
description: L’élément CertPrincipalName spécifie le nom de principal du certificat SSL (Secure Sockets Layer) qui est requis pour se connecter à l’organisation Microsoft Exchange Server 2007 à l’aide de SSL.
ms.openlocfilehash: fb2a1c8577bce41945b669be56f2a94a2c4dca26
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463341"
---
# <a name="certprincipalname-pox"></a>CertPrincipalName (POX)

L’élément **CertPrincipalName** spécifie le nom de principal du certificat SSL (Secure Sockets Layer) qui est requis pour se connecter à l’organisation Microsoft Exchange Server 2007 à l’aide de SSL. 
  
[Découverte automatique (POX)](autodiscover-pox.md)
  
[Réponse (POX)](response-pox.md)
  
[Compte (POX)](account-pox.md)
  
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
|[Protocol (POX)](protocol-pox.md) <br/> |Contient les spécifications relatives à la connexion d’un client à l’ordinateur qui exécute Exchange 2007 sur lequel le rôle de serveur d’accès au client est installé.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur texte spécifie le nom de principal du certificat SSL qui est requis pour se connecter à l’organisation Microsoft Exchange à l’aide de SSL.
  
## <a name="remarks"></a>Remarques

Si l’élément **CertPrincipalName** n’est pas spécifié, la valeur par défaut est définie sur msstd : serveur, où serveur est la valeur spécifiée dans l’élément [serveur (POX)](server-pox.md) . Par exemple, si le serveur est spécifié en tant que example.com et que la valeur de **CertPrincipalName** est laissée vide avec le [protocole SSL (POX)](ssl-pox.md) activé, la valeur par défaut de **CertPrincipalName** serait msstd :example. com. 
  
Si **aucune** valeur n’est spécifiée, Windows valide le nom de principal du certificat en fonction des informations figurant dans la rubrique [noms principaux](https://go.microsoft.com/fwlink/?LinkId=93417) sur MSDN. 
  
## <a name="see-also"></a>Voir aussi



[Éléments XML de découverte automatique de la VARIOle pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

