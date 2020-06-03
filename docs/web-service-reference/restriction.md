---
title: Restriction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Restriction
api_type:
- schema
ms.assetid: 77f19014-d112-4999-8e83-ecc32a117a73
description: L’élément restriction représente la restriction ou la requête utilisée pour filtrer des éléments ou des dossiers dans les opérations FindItem/FindFolder et Search Folder.
ms.openlocfilehash: 6037ba15417d67d393ca70f3edf2248749c396e1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465288"
---
# <a name="restriction"></a>Restriction

L’élément **restriction** représente la restriction ou la requête utilisée pour filtrer des éléments ou des dossiers dans les opérations FindItem/FindFolder et Search Folder. 
  
```xml
<Restriction>
   <SearchExpression/>
</Restriction>
```

 **RestrictionType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[And](and.md) <br/> |Représente une expression de recherche qui vous permet d’effectuer une opération booléenne **et** une opération entre deux ou plusieurs expressions de recherche.  <br/> |
|[Contains](contains.md) <br/> |Représente une expression de recherche qui détermine si une propriété donnée contient la valeur de chaîne de constante fournie.  <br/> |
|[Exclut](excludes.md) <br/> |Effectue un masque de bits des propriétés.  <br/> |
|[Exists](exists.md) <br/> |Représente une expression de recherche qui renvoie la **valeur true** si la propriété fournie existe sur un élément.  <br/> |
|[IsEqualTo](isequalto.md) <br/> |Représente une expression de recherche qui compare une propriété à une valeur de constante ou à une autre propriété et donne la **valeur true** si elles sont égales.  <br/> |
|[IsGreaterThan](isgreaterthan.md) <br/> |Représente une expression de recherche qui compare une propriété avec une valeur de constante ou une autre propriété et renvoie la **valeur true** si la première propriété est supérieure à la valeur ou à la propriété.  <br/> |
|[IsGreaterThanOrEqualTo](isgreaterthanorequalto.md) <br/> |Représente une expression de recherche qui compare une propriété avec une valeur de constante ou une autre propriété et renvoie la **valeur true** si la première propriété est supérieure ou égale à la valeur ou à la propriété.  <br/> |
|[IsLessThan](islessthan.md) <br/> |Représente une expression de recherche qui compare une propriété à une valeur constante ou à une autre propriété et renvoie la **valeur true** si la première propriété est inférieure à la valeur ou à la propriété.  <br/> |
|[IsLessThanOrEqualTo](islessthanorequalto.md) <br/> |Représente une expression de recherche qui compare une propriété à une valeur de constante ou à une autre propriété et renvoie la **valeur true** si la première propriété est inférieure ou égale à la valeur ou à la propriété.  <br/> |
|[IsNotEqualTo](isnotequalto.md) <br/> |Représente une expression de recherche qui compare une propriété à une valeur de constante ou à une autre propriété et renvoie la **valeur true** si les valeurs ne sont pas identiques.  <br/> |
|[Not](not.md) <br/> |Représente une expression de recherche qui nie la valeur booléenne de l’expression de recherche qu’elle contient.  <br/> |
|[Or](or.md) <br/> |Représente une expression de recherche qui effectue une opération **or** logique sur l’expression de recherche qu’elle contient. L’élément **ou** renvoie la **valeur true** si l’un de ses enfants renvoie la **valeur true**.  <br/> |
|[SearchExpression](searchexpression.md) <br/> |Représente l’élément substitué dans une restriction. Cet élément n’est pas utilisé dans un document d’instance XML.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[FindFolder](findfolder.md) <br/> |Définit une demande pour identifier les dossiers d’une boîte aux lettres.  <br/> |
|[FindItem](finditem.md) <br/> |Définit une requête pour rechercher des éléments dans une boîte aux lettres.  <br/> |
|[SearchParameters](searchparameters.md) <br/> |Représente les paramètres qui définissent un dossier de recherche.  <br/> |
   
## <a name="remarks"></a>Remarques

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

