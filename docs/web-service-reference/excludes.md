---
title: Excludes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Excludes
api_type:
- schema
ms.assetid: bbaeddf6-9a67-4ee0-af99-7a7a5bbdc0e1
description: L’élément exclut effectue un masque de bits de la propriété spécifiée et une valeur fournie.
ms.openlocfilehash: febd4171210319d8f7e475f9879c5f895f508713
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354385"
---
# <a name="excludes"></a>Excludes

L’élément **exclut** effectue un masque de bits de la propriété spécifiée et une valeur fournie. 
  
```xml
<Excludes>
   <FieldURI/>
   <Bitmask/>
</Excludes>
```

```xml
<Excludes>
   <ExtendedFieldURI/> 
   <Bitmask/>
</Excludes>
```

```xml
<Excludes>
   <IndexedFieldURI/> 
   <Bitmask/>
</Excludes>
```

**ExcludesType**

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
|[Bitmask](bitmask.md) <br/> |Représente un masque hexadécimal ou décimal à utiliser lors d’une opération de restriction des [exclusions](excludes.md) . Si le masque de bits représente un nombre hexadécimal, il doit être précédé 0 x ou 0 X. Dans le cas contraire, il sera considéré un nombre décimal.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Restriction](restriction.md) <br/> |Représente la restriction ou la requête qui est utilisé pour filtrer des éléments ou des dossiers dans les opérations de dossier FindItem/FindFolder et la recherche.  <br/> |
|[Pas](not.md) <br/> |Représente une expression de recherche qui inverse la valeur booléenne de l’expression de recherche qu’il contient.  <br/> |
|[And](and.md) <br/> |Représente une expression de recherche qui vous permet d’effectuer une opération de type Boolean et entre deux ou plusieurs expressions de recherche. Le résultat de l’opération est **la valeur true** si toutes les expressions de recherche contenues dans l’And sont **remplies**.  <br/> |
|[Or](or.md) <br/> |Représente une expression de recherche qui effectue une opération OR logique sur l’expression de recherche qu’il contient. L’élément [ou](or.md) renvoie **la valeur true** si un de ses enfants retourne **true**.  <br/> |
   
## <a name="remarks"></a>Remarques

**Exclut** permettra de résoudre **la valeur True** si une opération et effectuée sur les éléments suivants est résolu à 0 : 
  
1. La valeur de la propriété binaire
    
2. La valeur de masque de bits pour la propriété
    
**Exclut** peut uniquement être appliqué à une propriété qui a une valeur entière. Si le type de propriété n’est pas un entier, un code d’erreur de **ErrorUnsupportedPathForQuery** est renvoyé dans la réponse. 
  
Vous pouvez effectuer l’opération inverse en appelant Not(Excludes).
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

