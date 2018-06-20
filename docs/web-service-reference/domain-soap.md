---
title: Domaine (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 849629a0-0467-422f-88f6-3b8a95c17bba
description: L’élément de domaine contient un domaine fédéré dans une réponse GetFederationInformation ou un domaine pour lequel les paramètres de configuration sont demandées dans une requête GetDomainSettings.
ms.openlocfilehash: 411ca866800322ef06eeecc2ab92adc6f711917c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756029"
---
# <a name="domain-soap"></a>Domaine (SOAP)

L’élément de **domaine** contient un domaine fédéré dans une réponse **GetFederationInformation** ou un domaine pour lequel les paramètres de configuration sont demandées dans une requête **GetDomainSettings** . 
  
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
|[Domaines (SOAP)](domains-soap.md) <br/> |Représente les domaines pour lesquels les paramètres de configuration sont retournés dans une opération **GetDomainSettings** ou les domaines que l’organisation a fédérés dans une opération **GetFederationInformation** .  <br/> |
   
## <a name="text-value"></a>Valeur de texte

La valeur de texte de l’élément de **domaine** représente un nom de domaine. 
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nom du schéma  <br/> |Schéma de découverte automatique  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   

