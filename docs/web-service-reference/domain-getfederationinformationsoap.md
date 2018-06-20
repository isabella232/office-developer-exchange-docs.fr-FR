---
title: Domaine (GetFederationInformation) (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 56aeb659-8309-47a6-8c41-9f8b0436438c
description: L’élément de domaine identifie le domaine qui possède une approbation de fédération.
ms.openlocfilehash: 240c0b7cc13257ee36833625125691d4e51a103d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756035"
---
# <a name="domain-getfederationinformation-soap"></a>Domaine (GetFederationInformation) (SOAP)

L’élément de **domaine** identifie le domaine qui possède une approbation de fédération. 
  
```XML
<Domain/>
```

 **string**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Demande (GetFederationInformation) (SOAP)](request-getfederationinformationsoap.md) <br/> |Représente une demande [d’opération GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md) .  <br/> |
   
## <a name="text-value"></a>Valeur de texte

La valeur de texte représente le nom de domaine du domaine qui contient l’approbation de fédération.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nom du schéma  <br/> |Schéma de découverte automatique  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md)

