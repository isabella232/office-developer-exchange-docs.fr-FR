---
title: Utilisateur (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 7c42b516-77f6-4aee-99d8-b866d82d793a
description: L’élément de l’utilisateur fournit des informations spécifiques à l’utilisateur.
ms.openlocfilehash: 3f90ff0cc00170170c7304f2a19fe1d7abd9d1bc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838944"
---
# <a name="user-pox"></a>Utilisateur (POX)

L’élément de **l’utilisateur** fournit des informations spécifiques à l’utilisateur. 
  
[Découverte automatique (POX)](autodiscover-pox.md)
  
[Réponse (POX)](response-pox.md)
  
[Utilisateur (POX)](user-pox.md)
  
```xml
<User>
   <DisplayName/>
   <LegacyDN/>
   <DeploymentId/>
   <AutoDiscoverSMTPAddress/>
</User>
```

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[DisplayName (chaîne)](displayname-string.md) <br/> |Représente le nom complet de l’utilisateur.  <br/> |
|[LegacyDN (POX)](legacydn-pox.md) <br/> |Identifie la boîte aux lettres d’un utilisateur par un nom unique hérité.  <br/> |
|[DeploymentId (POX)](deploymentid-pox.md) <br/> |Identifie de manière unique la forêt Exchange.  <br/> |
|[AutoDiscoverSMTPAddress (POX)](autodiscoversmtpaddress-pox.md) <br/> |Contient l’adresse SMTP de l’utilisateur qui est utilisé pour le processus de découverte automatique.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Réponse (POX)](response-pox.md) <br/> |Contient la réponse du service de découverte automatique.  <br/> |
   
## <a name="remarks"></a>Remarques

Les réponses et les demandes de découverte automatique doivent être au format UTF-8.
  
## <a name="see-also"></a>Voir aussi



[Éléments du fichier XML Autodiscover variole pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

