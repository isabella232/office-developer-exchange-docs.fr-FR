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
description: L’élément Contains représente une expression de recherche qui détermine si une propriété donnée contient la valeur de chaîne de constante fournie.
ms.openlocfilehash: 79529bd752bcbce954ae3c8b0085c203b4eb8777
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527116"
---
# <a name="contains"></a>Contains

L’élément **Contains** représente une expression de recherche qui détermine si une propriété donnée contient la valeur de chaîne de constante fournie. 
  
```xml
<Contains ContainmentMode="" ContainmentComparison="">
   <FieldURI/>
   <Constant/>
</Contains>
```

```xml
<Contains ContainmentMode="" ContainmentComparison="">
   <ExtendedFieldURI/>
   <Constant/>
</Contains>
```

```xml
<Contains ContainmentMode="" ContainmentComparison="">
   <IndexedFieldURI/>
   <Constant/>
</Contains>
```


**ContainsExpressionType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**ContainmentMode** <br/> |Identifie les limites d’une recherche.  <br/> |
|**ContainmentComparison** <br/> |Détermine si la recherche ignore les cas et les espaces.  <br/> |
   
#### <a name="containmentmode-attribute-values"></a>Valeurs d’attribut ContainmentMode

|**Valeur**|**Description**|
|:-----|:-----|
|FullString  <br/> |La comparaison se fait entre la chaîne complète et la constante. La valeur de la propriété et la constante fournie sont rigoureusement identiques.  <br/> |
|Préfixe  <br/> |La comparaison se fait entre le préfixe de chaîne et la constante.  <br/> |
|Sous-chaîne  <br/> |La comparaison se fait entre une sous-chaîne de la chaîne et la constante.  <br/> |
|PrefixOnWords  <br/> |La comparaison se fait entre un préfixe sur des mots individuels dans la chaîne et la constante.  <br/> |
|ExactPhrase  <br/> |La comparaison se fait entre une expression exacte dans la chaîne et la constante.  <br/> |
   
#### <a name="containmentcomparison-attribute-values"></a>Valeurs d’attribut ContainmentComparison

|**Valeur**|**Description**|
|:-----|:-----|
|Orthographe  <br/> |La comparaison doit être exacte.  <br/> |
|IgnoreCase  <br/> |La comparaison ne tient pas compte de la casse.  <br/> |
|IgnoreNonSpacingCharacters  <br/> |La comparaison ne tient pas compte des caractères non-espacement.  <br/> |
|Espacé  <br/> |À supprimer.  <br/> |
|IgnoreCaseAndNonSpacingCharacters  <br/> |La comparaison ne tient pas compte des caractères de casse et de non-espacement.  <br/> |
|LooseAndIgnoreCase  <br/> |À supprimer.  <br/> |
|LooseAndIgnoreNonSpace  <br/> |À supprimer.  <br/> |
|LooseAndIgnoreCaseAndIgnoreNonSpace  <br/> |À supprimer.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[FieldURI](fielduri.md) <br/> |Identifie les propriétés référencées fréquemment par URI.  <br/> |
|[IndexedFieldURI](indexedfielduri.md) <br/> |Identifie les membres individuels d’un dictionnaire.  <br/> |
|[ExtendedFieldURI](extendedfielduri.md) <br/> |Identifie les propriétés MAPI.  <br/> |
|[Constante](constant.md) <br/> |Identifie une valeur constante dans une restriction.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Restriction](restriction.md) <br/> |Représente la restriction ou la requête qui est utilisée pour filtrer des éléments ou des dossiers dans les opérations FindItem/FindFolder et Search Folder.  <br/> |
|[Not](not.md) <br/> |Représente une expression de recherche qui nie la valeur booléenne de l’expression de recherche qu’elle contient.  <br/> |
|[And](and.md) <br/> |Représente une expression de recherche qui vous permet d’effectuer une opération booléenne et une opération entre deux ou plusieurs expressions de recherche. Le résultat de l’opération and est **true** si toutes les expressions de recherche contenues dans le et sont **vraies**.  <br/> |
|[Or](or.md) <br/> |Représente une expression de recherche qui effectue une ou logique sur l’expression de recherche qu’elle contient. L’élément [ou](or.md) renvoie la **valeur true** si l’un de ses enfants renvoie la **valeur true**.  <br/> |
   
## <a name="remarks"></a>Remarques

Les attributs sont utilisés pour déterminer comment les éléments sont mis en correspondance.
  
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

