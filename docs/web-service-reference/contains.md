---
title: Contains
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Contains
api_type:
- schema
ms.assetid: 476d059d-c243-43e9-b475-319fc413ade2
description: L’élément contient représente une expression de recherche qui détermine si une propriété donnée contient la valeur de chaîne constante fournie.
ms.openlocfilehash: 083efdf32cd32bea6964361b5b558480aa937280
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755584"
---
# <a name="contains"></a>Contains

L’élément **contient** représente une expression de recherche qui détermine si une propriété donnée contient la valeur de chaîne constante fournie. 
  
```xml
<Contains ContainmentMode="" ContainmentComparison="">
   <FieldURI/>
   <Constant/>
</Contains>
```

 **ContainsExpressionType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**ContainmentMode** <br/> |Identifie les limites d’une recherche.  <br/> |
|**ContainmentComparison** <br/> |Détermine si la recherche ignore les cas et les espaces.  <br/> |
   
#### <a name="containmentmode-attribute-values"></a>Valeurs des attributs ContainmentMode

|**Valeur**|**Description**|
|:-----|:-----|
|FullString  <br/> |La comparaison est comprise entre la chaîne complète et la constante. La valeur de la propriété et la constante fournie sont exactement les mêmes.  <br/> |
|Le préfixe  <br/> |La comparaison est comprise entre le préfixe de la chaîne et la constante.  <br/> |
|Sous-chaîne  <br/> |La comparaison est comprise entre une sous-chaîne de la chaîne et la constante.  <br/> |
|PrefixOnWords  <br/> |La comparaison est comprise entre un préfixe sur les mots individuels dans la chaîne et la constante.  <br/> |
|ExactPhrase  <br/> |La comparaison est comprise entre une expression exacte dans la chaîne et la constante.  <br/> |
   
#### <a name="containmentcomparison-attribute-values"></a>Valeurs des attributs ContainmentComparison

|**Valeur**|**Description**|
|:-----|:-----|
|Exact  <br/> |La comparaison doit être exacte.  <br/> |
|IgnoreCase  <br/> |La comparaison ignore la casse.  <br/> |
|IgnoreNonSpacingCharacters  <br/> |La comparaison ignore les caractères sans espace.  <br/> |
|Espacé  <br/> |À supprimer.  <br/> |
|IgnoreCaseAndNonSpacingCharacters  <br/> |La comparaison ignore la casse et non pas d’espacement des caractères.  <br/> |
|LooseAndIgnoreCase  <br/> |À supprimer.  <br/> |
|LooseAndIgnoreNonSpace  <br/> |À supprimer.  <br/> |
|LooseAndIgnoreCaseAndIgnoreNonSpace  <br/> |À supprimer.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[FieldURI](fielduri.md) <br/> |Identifie les propriétés fréquemment référencées par un URI.  <br/> |
|[IndexedFieldURI](indexedfielduri.md) <br/> |Identifie les membres individuels d’un dictionnaire.  <br/> |
|[ExtendedFieldURI](extendedfielduri.md) <br/> |Identifie les propriétés MAPI.  <br/> |
|[Constante](constant.md) <br/> |Identifie une valeur de constante dans une restriction.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Restriction](restriction.md) <br/> |Représente la restriction ou la requête qui est utilisé pour filtrer des éléments ou des dossiers dans les opérations de dossier FindItem/FindFolder et la recherche.  <br/> |
|[Pas](not.md) <br/> |Représente une expression de recherche qui inverse la valeur booléenne de l’expression de recherche qu’il contient.  <br/> |
|[And](and.md) <br/> |Représente une expression de recherche qui vous permet d’effectuer une opération de type Boolean et entre deux ou plusieurs expressions de recherche. Le résultat de l’opération est **la valeur true** si toutes les expressions de recherche contenues dans l’And sont **remplies**.  <br/> |
|[Or](or.md) <br/> |Représente une expression de recherche qui effectue une opération OR logique sur l’expression de recherche qu’il contient. L’élément [ou](or.md) renvoie **la valeur true** si un de ses enfants retourne **true**.  <br/> |
   
## <a name="remarks"></a>Remarques

Les attributs sont utilisés pour déterminer la façon dont les éléments sont mis en correspondance.
  
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

