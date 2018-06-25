---
title: SearchExpression
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SearchExpression
api_type:
- schema
ms.assetid: daa179b6-8c7f-4268-a312-c2acc67fa7c3
description: L’élément SearchExpression est un élément abstrait qui représente l’élément substitué au sein d’une restriction. Toutes les expressions de recherche dérivent de ce type de base. Cet élément n’est pas utilisé dans un document d’instance XML.
ms.openlocfilehash: 8e0d09aec079280816cd9dfe2c1a55c88bb959a7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829286"
---
# <a name="searchexpression"></a>SearchExpression

L’élément **SearchExpression** est un élément abstrait qui représente l’élément substitué au sein d’une restriction. Toutes les expressions de recherche dérivent de ce type de base. Cet élément n’est pas utilisé dans un document d’instance XML. 
  
```xml
<SearchExpression/>
```

 **SearchExpressionType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Restriction](restriction.md) <br/> |Représente la restriction ou la requête qui est utilisé pour filtrer des éléments ou des dossiers dans les opérations de dossier FindItem/FindFolder et la recherche.  <br/> |
|[Pas](not.md) <br/> |Représente une expression de recherche qui inverse la valeur booléenne de l’expression de recherche qu’il contient.  <br/> |
|[And](and.md) <br/> |Représente une expression de recherche qui vous permet d’effectuer une opération type Boolean **et** entre deux ou plusieurs expressions de recherche. Le résultat de **l’opération** est **la valeur true** si toutes les expressions de recherche contenues dans l’élément **et** sont **remplies**.  <br/> |
|[Or](or.md) <br/> |Représente une expression de recherche qui effectue une opération **OR** logique sur l’expression de recherche qu’il contient. **Ou** renvoie **la valeur true** si un de ses enfants retourne **true**. **Ou** doit disposer de deux ou plusieurs enfants.  <br/> |
   
## <a name="remarks"></a>Remarques

N’importe quel élément de filtre qui fait partie d’un groupe de substitution SearchExpression peut s’afficher à la place de l’élément SearchExpression.
  
> [!NOTE]
> Cet élément se produira jamais directement au sein d’une instance de document. 
  
Les éléments suivants sont les membres du groupe de substitution SearchExpression :
  
- [Exists](exists.md)
    
- [Exclut](excludes.md)
    
- [Plutôt IsEqualTo](isequalto.md)
    
- [IsNotEqualTo](isnotequalto.md)
    
- [IsGreaterThan](isgreaterthan.md)
    
- [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md)
    
- [IsLessThan](islessthan.md)
    
- [IsLessThanOrEqualTo](islessthanorequalto.md)
    
- [Contient](contains.md)
    
- [Pas](not.md)
    
- [And](and.md)
    
- [Or](or.md)
    
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

