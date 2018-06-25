---
title: Valeur
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Value
api_type:
- schema
ms.assetid: 9a30cadd-909e-41b1-b4e9-291643dd89c6
description: L’élément Value contient la valeur d’une propriété étendue.
ms.openlocfilehash: 4b8674d267b78f0384f9457e794e88ace8234826
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839008"
---
# <a name="value"></a>Valeur

L’élément **Value** contient la valeur d’une propriété étendue. 
  
```xml
<Value/>
```

**Chaîne**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Values](values.md) <br/> |Contient une collection de valeurs pour une propriété étendue.  <br/> |
|[ExtendedProperty](extendedproperty.md) <br/> |Identifie les propriétés étendues sur les dossiers et les éléments.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

La valeur de texte doit être compatible avec le type est indiqué par l’attribut PropertyType de la ExtendedFieldURI.
  
## <a name="remarks"></a>Remarques

Un élément de la **valeur** peut se produire dans les deux instances de la propriété étendue unique et à valeurs multiples. Pour les instances à valeur unique, il existe en tant qu’enfant de l’élément [ExtendedProperty](extendedproperty.md) direct. Pour l’instance à valeurs multiples, il existe en tant qu’un enfant direct de la collection de **valeurs** . 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

