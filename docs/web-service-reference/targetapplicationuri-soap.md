---
title: TargetApplicationUri (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: e13c0edd-2ab1-49bb-a993-54a8db2dfbb9
description: L’élément TargetApplicationUri définit l’URI d’application cible. L’élément TargetApplicationUri est à usage interne uniquement. Cet élément n’est pas utilisé par les clients.
ms.openlocfilehash: fa401d4c1e8c1460804f116d840fe21129957852
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838669"
---
# <a name="targetapplicationuri-soap"></a>TargetApplicationUri (SOAP)

L’élément **TargetApplicationUri** définit l’URI d’application cible. L’élément **TargetApplicationUri** est à usage interne uniquement. Cet élément n’est pas utilisé par les clients. 
  
```XML
<TargetApplicationUri/>
```

 **anyURI**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[OrganizationRelationshipSettings (SOAP)](organizationrelationshipsettings-soap.md) <br/> |Représente une liste des relations d’organisation pour une organisation unique  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément définit l’URI de l’organisation externe cible.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nom du schéma  <br/> |Schéma de découverte automatique  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetOrganizationRelationshipSettings (SOAP)](getorganizationrelationshipsettings-operation-soap.md)

