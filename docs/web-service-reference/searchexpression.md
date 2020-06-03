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
description: L’élément SearchExpression est un élément abstrait qui représente l’élément substitué dans une restriction. Toutes les expressions de recherche dérivent de ce type de base. Cet élément n’est pas utilisé dans un document d’instance XML.
ms.openlocfilehash: db06ce8e2faa0f2589963d58aab55073c618c171
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530351"
---
# <a name="searchexpression"></a>SearchExpression

L’élément **SearchExpression** est un élément abstrait qui représente l’élément substitué dans une restriction. Toutes les expressions de recherche dérivent de ce type de base. Cet élément n’est pas utilisé dans un document d’instance XML. 
  
```xml
<SearchExpression/>
```

 **SearchExpressionType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Restriction](restriction.md) <br/> |Représente la restriction ou la requête qui est utilisée pour filtrer des éléments ou des dossiers dans les opérations FindItem/FindFolder et Search Folder.  <br/> |
|[Not](not.md) <br/> |Représente une expression de recherche qui nie la valeur booléenne de l’expression de recherche qu’elle contient.  <br/> |
|[And](and.md) <br/> |Représente une expression de recherche qui vous permet d’effectuer une opération booléenne **et** une opération entre deux ou plusieurs expressions de recherche. Le résultat de l’opération **and** est **true** si toutes les expressions de recherche contenues dans l’élément **and** sont **true**.  <br/> |
|[Or](or.md) <br/> |Représente une expression de recherche qui effectue une opération **or** logique sur l’expression de recherche qu’elle contient. **Ou** renverra **true** si l’un de ses enfants renvoie la **valeur true**. **Ou** il doit avoir au moins deux enfants.  <br/> |
   
## <a name="remarks"></a>Remarques

Tout élément Filter qui fait partie du groupe de substitution SearchExpression peut apparaître à la place de l’élément SearchExpression.
  
> [!NOTE]
> Cet élément ne se produira jamais directement dans un document d’instance. 
  
Les éléments suivants sont membres du groupe de substitution SearchExpression :
  
- [Exists](exists.md)
    
- [Exclut](excludes.md)
    
- [IsEqualTo](isequalto.md)
    
- [IsNotEqualTo](isnotequalto.md)
    
- [IsGreaterThan](isgreaterthan.md)
    
- [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md)
    
- [IsLessThan](islessthan.md)
    
- [IsLessThanOrEqualTo](islessthanorequalto.md)
    
- [Contains](contains.md)
    
- [Not](not.md)
    
- [And](and.md)
    
- [Or](or.md)
    
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

