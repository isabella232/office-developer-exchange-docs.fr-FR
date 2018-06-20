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
description: L’élément CertPrincipalName Spécifie le nom principal du certificat Secure Sockets Layer (SSL) qui est nécessaire pour se connecter à l’organisation Microsoft Exchange Server 2007 à l’aide de SSL.
ms.openlocfilehash: d2766b16a3e8a1bcd013de332d9c07f709fcf949
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755502"
---
# <a name="certprincipalname-pox"></a>CertPrincipalName (POX)

L’élément **CertPrincipalName** Spécifie le nom principal du certificat Secure Sockets Layer (SSL) qui est nécessaire pour se connecter à l’organisation Microsoft Exchange Server 2007 à l’aide de SSL. 
  
[Découverte automatique (POX)](autodiscover-pox.md)
  
[Réponse (POX)](response-pox.md)
  
[Compte (POX)](account-pox.md)
  
[Protocole (POX)](protocol-pox.md)
  
[CertPrincipalName (POX)](certprincipalname-pox.md)
  
```xml
<CertPrincipalName>none or servername</CertPrinicpalName>
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
|[Protocole (POX)](protocol-pox.md) <br/> |Contient les spécifications pour connecter un client à l’ordinateur qui exécute Exchange 2007 ayant le rôle de serveur d’accès au Client est installé.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

La valeur texte spécifie le nom principal du certificat SSL qui est requise pour se connecter à l’organisation Microsoft Exchange à l’aide de SSL.
  
## <a name="remarks"></a>Remarques

Si l’élément **CertPrincipalName** n’est pas spécifié, la valeur par défaut est définie à msstd:SERVER, où serveur est la valeur qui est spécifiée dans l’élément [Serveur (POX)](server-pox.md) . Par exemple, si le serveur est spécifié en tant qu’exemple.com et **CertPrincipalName** avec [SSL (POX)](ssl-pox.md) activée est vide, la valeur par défaut **CertPrincipalName** serait msstd:example.com. 
  
Si **aucun** n’est spécifié, Windows valide le nom principal du certificat en fonction des informations figurant dans la rubrique [Noms principaux](http://go.microsoft.com/fwlink/?LinkId=93417) sur MSDN. 
  
## <a name="see-also"></a>Voir aussi



[Éléments du fichier XML Autodiscover variole pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

