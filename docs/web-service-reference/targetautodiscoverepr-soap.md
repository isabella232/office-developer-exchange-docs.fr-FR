---
title: TargetAutodiscoverEpr (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: fdb9cc7a-cf0a-431b-9f6f-5f1db1792db7
description: L’élément TargetAutodiscoverEpr représente la propriété TargetAutodiscoverEpr. L’élément TargetAutodiscoverEpr est à usage interne uniquement. Cet élément n’est pas utilisé par les clients.
ms.openlocfilehash: f49d7b0acc59d638f2fca993ec7d8f182cd7380a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59545803"
---
# <a name="targetautodiscoverepr-soap"></a>TargetAutodiscoverEpr (SOAP)

**L’élément TargetAutodiscoverEpr** représente la **propriété TargetAutodiscoverEpr.** **L’élément TargetAutodiscoverEpr est** à usage interne uniquement. Cet élément n’est pas utilisé par les clients. 
  
```XML
<TargetAutodiscoverEpr/>
```

 **anyURI**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[OrganizationRelationshipSettings (SOAP)](organizationrelationshipsettings-soap.md) <br/> |Représente une liste de relations organisationnelles pour une seule organisation.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur de texte de cet élément est un URI (Uniform Resource Identifier) pour la relation d’organisation.
  
## <a name="remarks"></a>Remarques

Cet élément spécifie l’URL de découverte automatique du serveur pour l’organisation externe. 
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nom du schéma  <br/> |Schéma de découverte automatique  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetOrganizationRelationshipSettings (SOAP)](getorganizationrelationshipsettings-operation-soap.md)

