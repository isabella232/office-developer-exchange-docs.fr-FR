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
description: L’élément IsNotEqualTo représente une expression de recherche qui compare une propriété à une valeur constante ou à une autre propriété et renvoie la valeur true si les valeurs ne sont pas identiques.
ms.openlocfilehash: 8c40fd1ce8c7c1f14b70f4fccfd3a24e4c99f1b5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464188"
---
# <a name="isnotequalto"></a>IsNotEqualTo

L’élément **IsNotEqualTo** représente une expression de recherche qui compare une propriété à une valeur constante ou à une autre propriété et renvoie la **valeur true** si les valeurs ne sont pas identiques. 
  
```xml
<IsNotEqualTo>
   <FieldURI/>
   <FieldURIOrConstant/>
</IsNotEqualTo>
```

```xml
<IsNotEqualTo>
   <ExtendedFieldURI/> 
   <FieldURIOrConstant/>
</IsNotEqualTo>
```

```xml
<IsNotEqualTo>
   <IndexedFieldURI/>
   <FieldURIOrConstant/>
</IsNotEqualTo>
```

**IsNotEqualToType**

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
|[FieldURIOrConstant](fielduriorconstant.md) <br/> |Représente une propriété ou une valeur constante à utiliser lors de la comparaison avec une autre propriété.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Restriction](restriction.md) <br/> |Représente la restriction ou la requête qui est utilisée pour filtrer des éléments ou des dossiers dans les opérations FindItem/FindFolder et Search Folder.  <br/> |
|[Not](not.md) <br/> |Représente une expression de recherche qui nie la valeur booléenne de l’expression de recherche qu’elle contient.  <br/> |
|[And](and.md) <br/> |Représente une expression de recherche qui vous permet d’effectuer une opération booléenne et une opération entre deux ou plusieurs expressions de recherche. Le résultat de l’opération and est **true** si toutes les expressions de recherche contenues dans le et sont **vraies**.  <br/> |
|[Or](or.md) <br/> |Représente une expression de recherche qui effectue une ou logique sur l’expression de recherche qu’elle contient. [Ou](or.md) renverra **true** si l’un de ses enfants renvoie la **valeur true**. **Ou** il doit avoir au moins deux enfants.  <br/> |
   
## <a name="remarks"></a>Remarques

Pour effectuer des comparaisons de chaînes, envisagez d’utiliser l’élément [Contains](contains.md) , car il fournit des options pour les paramètres correspondants tels que case et espace blanc. Utilisez l’élément [not](not.md) en combinaison avec l’élément [Contains](contains.md) pour inverser le résultat. 
  
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

