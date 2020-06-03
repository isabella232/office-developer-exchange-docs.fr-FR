---
title: Exclut
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
description: L’élément excludes effectue un masque de bits de la propriété spécifiée et une valeur fournie.
ms.openlocfilehash: d5fcd8b86b454aa731bd43974b5b7d674fe76ed6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530613"
---
# <a name="excludes"></a>Exclut

L’élément **excludes** effectue un masque de bits de la propriété spécifiée et une valeur fournie. 
  
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

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[FieldURI](fielduri.md) <br/> |Identifie les propriétés référencées fréquemment par URI.  <br/> |
|[IndexedFieldURI](indexedfielduri.md) <br/> |Identifie les membres individuels d’un dictionnaire.  <br/> |
|[ExtendedFieldURI](extendedfielduri.md) <br/> |Identifie les propriétés MAPI.  <br/> |
|[Composé](bitmask.md) <br/> |Représente un masque hexadécimal ou décimal à utiliser pendant une opération de restriction [exclusions](excludes.md) . Si le masque binaire représente un nombre hexadécimal, il doit être préfixé par 0x ou 0X. Sinon, il est considéré comme un nombre décimal.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Restriction](restriction.md) <br/> |Représente la restriction ou la requête qui est utilisée pour filtrer des éléments ou des dossiers dans les opérations FindItem/FindFolder et Search Folder.  <br/> |
|[Not](not.md) <br/> |Représente une expression de recherche qui nie la valeur booléenne de l’expression de recherche qu’elle contient.  <br/> |
|[And](and.md) <br/> |Représente une expression de recherche qui vous permet d’effectuer une opération booléenne et une opération entre deux ou plusieurs expressions de recherche. Le résultat de l’opération and est **true** si toutes les expressions de recherche contenues dans le et sont **vraies**.  <br/> |
|[Or](or.md) <br/> |Représente une expression de recherche qui effectue une ou logique sur l’expression de recherche qu’elle contient. L’élément [ou](or.md) renvoie la **valeur true** si l’un de ses enfants renvoie la **valeur true**.  <br/> |
   
## <a name="remarks"></a>Remarques

**Exclusions** se traduit par la **valeur true** si une opération and effectuée sur les valeurs suivantes est résolue à 0 : 
  
1. Valeur de bits de la propriété
    
2. Valeur de masque de masque de la propriété
    
Les **exclusions** ne peuvent être appliquées qu’à une propriété qui a une valeur entière. Si le type de propriété n’est pas un entier, un code d’erreur **ErrorUnsupportedPathForQuery** est renvoyé dans la réponse. 
  
Vous pouvez effectuer l’opération inverse en appelant la méthode not (exclut).
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

