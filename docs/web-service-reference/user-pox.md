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
description: L’élément User fournit des informations spécifiques à l’utilisateur.
ms.openlocfilehash: 8f53319bcf34595305748adafc9aa1e25283611e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530217"
---
# <a name="user-pox"></a>Utilisateur (POX)

L’élément **User** fournit des informations spécifiques à l’utilisateur. 
  
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

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[DisplayName (chaîne)](displayname-string.md) <br/> |Représente le nom d’affichage de l’utilisateur.  <br/> |
|[LegacyDN (POX)](legacydn-pox.md) <br/> |Identifie la boîte aux lettres d’un utilisateur par le nom unique hérité.  <br/> |
|[DeploymentId (POX)](deploymentid-pox.md) <br/> |Identifie de manière unique la forêt Exchange.  <br/> |
|[AutoDiscoverSMTPAddress (POX)](autodiscoversmtpaddress-pox.md) <br/> |Contient l’adresse SMTP de l’utilisateur qui est utilisée pour le processus de découverte automatique.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Réponse (POX)](response-pox.md) <br/> |Contient la réponse du service de découverte automatique.  <br/> |
   
## <a name="remarks"></a>Remarques

Les demandes et les réponses de découverte automatique doivent être codées au format UTF-8.
  
## <a name="see-also"></a>Voir aussi



[Éléments XML de découverte automatique de la VARIOle pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

