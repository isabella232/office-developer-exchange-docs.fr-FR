---
title: IsNotEqualTo
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsNotEqualTo
api_type:
- schema
ms.assetid: e2eff26c-3403-45cd-bb74-1eb98c7dbfcd
description: L’élément IsNotEqualTo représente une expression de recherche qui compare une propriété avec une valeur constante ou une autre propriété et renvoie la valeur true si les valeurs ne sont pas identiques.
ms.openlocfilehash: c11f5ba5b8c0672bba0b9ae2a76211ac7d5d94ad
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828059"
---
# <a name="isnotequalto"></a>IsNotEqualTo

L’élément **IsNotEqualTo** représente une expression de recherche qui compare une propriété avec une valeur constante ou une autre propriété et renvoie **la valeur true** si les valeurs ne sont pas identiques. 
  
```xml
<IsNotEqualTo>
   <FieldURI/>
   <FieldURIOrConstant/>
</IsNotEqualTo>
```

 **IsNotEqualToType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[FieldURI](fielduri.md) <br/> |Identifie les propriétés fréquemment référencées par un URI.  <br/> |
|[IndexedFieldURI](indexedfielduri.md) <br/> |Identifie les membres individuels d’un dictionnaire.  <br/> |
|[ExtendedFieldURI](extendedfielduri.md) <br/> |Identifie les propriétés MAPI.  <br/> |
|[FieldURIOrConstant](fielduriorconstant.md) <br/> |Représente une propriété ou une constante à utiliser lors de la comparaison avec une autre propriété.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Restriction](restriction.md) <br/> |Représente la restriction ou la requête qui est utilisé pour filtrer des éléments ou des dossiers dans les opérations de dossier FindItem/FindFolder et la recherche.  <br/> |
|[Pas](not.md) <br/> |Représente une expression de recherche qui inverse la valeur booléenne de l’expression de recherche qu’il contient.  <br/> |
|[And](and.md) <br/> |Représente une expression de recherche qui vous permet d’effectuer une opération de type Boolean et entre deux ou plusieurs expressions de recherche. Le résultat de l’opération est **la valeur true** si toutes les expressions de recherche contenues dans l’And sont **remplies**.  <br/> |
|[Or](or.md) <br/> |Représente une expression de recherche qui effectue une opération OR logique sur l’expression de recherche qu’il contient. [Ou](or.md) renvoie **la valeur true** si un de ses enfants retourne **true**. **Ou** doit disposer de deux ou plusieurs enfants.  <br/> |
   
## <a name="remarks"></a>Remarques

Pour effectuer des comparaisons de chaînes, envisagez d’utiliser l’élément [contient](contains.md) , car elle fournit des options pour les paramètres correspondants tels que la casse et les espaces. Utilisez l’élément [pas](not.md) en association avec l’élément [contient](contains.md) pour inverser le résultat. 
  
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

