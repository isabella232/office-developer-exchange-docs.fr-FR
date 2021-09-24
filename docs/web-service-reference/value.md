---
title: Valeur
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Value
api_type:
- schema
ms.assetid: 9a30cadd-909e-41b1-b4e9-291643dd89c6
description: L’élément Value contient la valeur d’une propriété étendue.
ms.openlocfilehash: dc9d81a17896e730a5140a097574faa7619576d1
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513947"
---
# <a name="value"></a>Valeur

**L’élément Value** contient la valeur d’une propriété étendue. 
  
```xml
<Value/>
```

**String**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Valeurs](values.md) <br/> |Contient une collection de valeurs pour une propriété étendue.  <br/> |
|[ExtendedProperty](extendedproperty.md) <br/> |Identifie les propriétés étendues sur les dossiers et les éléments.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur de texte doit être compatible avec le type indiqué par l’attribut PropertyType de l’extendedFieldURI.
  
## <a name="remarks"></a>Remarques

Un **élément Value** peut se produire dans les instances de propriétés étendues à valeurs multiples et à valeurs multiples. Pour les instances à valeur unique, il existe en tant qu’enfant direct de [l’élément ExtendedProperty.](extendedproperty.md) Pour l’instance à valeurs multiples, il existe en tant qu’enfant direct de la collection **Values.** 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

