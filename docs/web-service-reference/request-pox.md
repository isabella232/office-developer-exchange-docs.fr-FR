---
title: Demande (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: da54eb32-7ce5-4384-9893-255a2243a959
description: L’élément de demande contient la demande au service de découverte automatique.
ms.openlocfilehash: ed6b0a80e83e160287f382a881dc5405bfb47a37
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829124"
---
# <a name="request-pox"></a>Demande (POX)

L’élément de **demande** contient la demande au service de découverte automatique. 
  
[Découverte automatique (POX)](autodiscover-pox.md)
  
[Demande (POX)](request-pox.md)
  
```xml
<Request>
   <AcceptableResponseSchema/>
   <EMailAddress/>
</Request>
```

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[AcceptableResponseSchema (POX)](acceptableresponseschema-pox.md) <br/> |Identifie le schéma d’une réponse de découverte automatique.  <br/> |
|[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) <br/> |Identifie l’adresse de messagerie de l’utilisateur.  <br/> |
|[LegacyDN (POX)](legacydn-pox.md) <br/> |Identifie la boîte aux lettres d’un utilisateur par un nom unique hérité.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Découverte automatique (POX)](autodiscover-pox.md) <br/> |L’élément racine dans une requête de découverte automatique.  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Éléments du fichier XML Autodiscover variole pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

