---
title: TargetAutodiscoverEpr (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: fdb9cc7a-cf0a-431b-9f6f-5f1db1792db7
description: L’élément TargetAutodiscoverEpr représente la propriété TargetAutodiscoverEpr. L’élément TargetAutodiscoverEpr est à usage interne uniquement. Cet élément n’est pas utilisé par les clients.
ms.openlocfilehash: 0b28444727e21a98925b6d1062bcbbac62c68981
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838670"
---
# <a name="targetautodiscoverepr-soap"></a>TargetAutodiscoverEpr (SOAP)

L’élément **TargetAutodiscoverEpr** représente la propriété **TargetAutodiscoverEpr** . L’élément **TargetAutodiscoverEpr** est à usage interne uniquement. Cet élément n’est pas utilisé par les clients. 
  
```XML
<TargetAutodiscoverEpr/>
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
|[OrganizationRelationshipSettings (SOAP)](organizationrelationshipsettings-soap.md) <br/> |Représente une liste des relations d’organisation pour une organisation unique.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

La valeur de texte pour cet élément est un identificateur uniform resource identifier (URI) pour la relation d’organisation.
  
## <a name="remarks"></a>Remarques

Cet élément spécifie l’URL de découverte automatique du serveur pour l’organisation externe. 
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nom du schéma  <br/> |Schéma de découverte automatique  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetOrganizationRelationshipSettings (SOAP)](getorganizationrelationshipsettings-operation-soap.md)

