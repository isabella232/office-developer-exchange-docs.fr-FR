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
description: L’élément Domain contient un domaine fédéré dans une réponse GetFederationInformation ou contient un domaine dont les paramètres de configuration sont demandés dans une demande GetDomainSettings.
ms.openlocfilehash: f90c608ee1fc3356a227bca6411eaeff0c1e8b22
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456982"
---
# <a name="domain-soap"></a>Domaine (SOAP)

L’élément **Domain** contient un domaine fédéré dans une réponse **GetFederationInformation** ou contient un domaine dont les paramètres de configuration sont demandés dans une demande **GetDomainSettings** . 
  
```XML
<Domain/> 
```

 **chaîne**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Domaines (SOAP)](domains-soap.md) <br/> |Représente les domaines pour lesquels les paramètres de configuration sont renvoyés dans une opération **GetDomainSettings** ou les domaines que l’organisation a fédérés dans une opération **GetFederationInformation** .  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur de texte de l’élément de **domaine** représente un nom de domaine. 
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nom du schéma  <br/> |Schéma de découverte automatique  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   

