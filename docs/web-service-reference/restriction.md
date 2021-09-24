---
title: Restriction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Restriction
api_type:
- schema
ms.assetid: 77f19014-d112-4999-8e83-ecc32a117a73
description: L’élément Restriction représente la restriction ou la requête utilisée pour filtrer des éléments ou des dossiers dans les opérations FindItem/FindFolder et des dossiers de recherche.
ms.openlocfilehash: 378c2d0ce7911638e5e58346de46759e7fdd87f1
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540565"
---
# <a name="restriction"></a>Restriction

**L’élément Restriction** représente la restriction ou la requête utilisée pour filtrer des éléments ou des dossiers dans les opérations FindItem/FindFolder et des dossiers de recherche. 
  
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
|[And](and.md) <br/> |Représente une expression de recherche qui vous permet d’effectuer une opération **BOOlean AND** entre deux ou plusieurs expressions de recherche.  <br/> |
|[Contains](contains.md) <br/> |Représente une expression de recherche qui détermine si une propriété donnée contient la valeur de chaîne constante fournie.  <br/> |
|[Excludes](excludes.md) <br/> |Effectue un masque de propriétés au sens du bit.  <br/> |
|[Exists](exists.md) <br/> |Représente une expression de recherche qui renvoie **la valeur true** si la propriété fournie existe sur un élément.  <br/> |
|[IsEqualTo](isequalto.md) <br/> |Représente une expression de recherche qui compare une propriété avec une valeur constante ou une autre propriété et qui est évaluée à **true** si elles sont égales.  <br/> |
|[IsGreaterThan](isgreaterthan.md) <br/> |Représente une expression de recherche qui compare une propriété avec une valeur constante ou une autre propriété et renvoie la valeur **true** si la première propriété est supérieure à la valeur ou à la propriété.  <br/> |
|[IsGreaterThanOrEqualTo](isgreaterthanorequalto.md) <br/> |Représente une expression de recherche qui compare une propriété avec une valeur constante ou une autre propriété et renvoie la valeur **true** si la première propriété est supérieure ou égale à la valeur ou à la propriété.  <br/> |
|[IsLessThan](islessthan.md) <br/> |Représente une expression de recherche qui compare une propriété avec une valeur constante ou une autre propriété et renvoie la valeur **true** si la première propriété est inférieure à la valeur ou à la propriété.  <br/> |
|[IsLessThanOrEqualTo](islessthanorequalto.md) <br/> |Représente une expression de recherche qui compare une propriété avec une valeur constante ou une autre propriété et renvoie **true** si la première propriété est inférieure ou égale à la valeur ou à la propriété.  <br/> |
|[IsNotEqualTo](isnotequalto.md) <br/> |Représente une expression de recherche qui compare une propriété avec une valeur constante ou une autre propriété et renvoie **true** si les valeurs ne sont pas identiques.  <br/> |
|[Not](not.md) <br/> |Représente une expression de recherche qui annule la valeur booléle de l’expression de recherche qu’elle contient.  <br/> |
|[Or](or.md) <br/> |Représente une expression de recherche qui effectue une opération **LOGIQUE OR** sur l’expression de recherche qu’elle contient. **L’élément Or** retourne **true si** l’un de ses enfants retourne **true**.  <br/> |
|[SearchExpression](searchexpression.md) <br/> |Représente l’élément remplacé dans une restriction. Cet élément n’est pas utilisé dans un document d’instance XML.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[FindFolder](findfolder.md) <br/> |Définit une demande d’identification des dossiers dans une boîte aux lettres.  <br/> |
|[FindItem](finditem.md) <br/> |Définit une demande de recherche d’éléments dans une boîte aux lettres.  <br/> |
|[SearchParameters](searchparameters.md) <br/> |Représente les paramètres qui définissent un dossier de recherche.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

