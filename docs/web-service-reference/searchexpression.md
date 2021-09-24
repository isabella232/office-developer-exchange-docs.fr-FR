---
title: SearchExpression
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SearchExpression
api_type:
- schema
ms.assetid: daa179b6-8c7f-4268-a312-c2acc67fa7c3
description: L’élément SearchExpression est un élément abstrait qui représente l’élément remplacé dans une restriction. Toutes les expressions de recherche dérivent de ce type de base. Cet élément n’est pas utilisé dans un document d’instance XML.
ms.openlocfilehash: e8047d333b36d77bc6823efd6488a15a6d2501a4
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59517846"
---
# <a name="searchexpression"></a>SearchExpression

**L’élément SearchExpression** est un élément abstrait qui représente l’élément remplacé dans une restriction. Toutes les expressions de recherche dérivent de ce type de base. Cet élément n’est pas utilisé dans un document d’instance XML. 
  
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
|[Restriction](restriction.md) <br/> |Représente la restriction ou la requête utilisée pour filtrer des éléments ou des dossiers dans les opérations FindItem/FindFolder et des dossiers de recherche.  <br/> |
|[Not](not.md) <br/> |Représente une expression de recherche qui annule la valeur booléle de l’expression de recherche qu’elle contient.  <br/> |
|[And](and.md) <br/> |Représente une expression de recherche qui vous permet d’effectuer une opération **BOOlean AND** entre deux ou plusieurs expressions de recherche. Le résultat de **l’opération AND** est **true** si toutes les expressions de recherche contenues dans l’élément **And** sont **vraies.**  <br/> |
|[Or](or.md) <br/> |Représente une expression de recherche qui effectue une opération **LOGIQUE OR** sur l’expression de recherche qu’elle contient. **Ou** retournera **true si** l’un de ses enfants retourne **true**. **Ou** doit avoir au moins deux enfants.  <br/> |
   
## <a name="remarks"></a>Remarques

Tout élément de filtre faisant partie du groupe de substitution SearchExpression peut apparaître à la place de l’élément SearchExpression.
  
> [!NOTE]
> Cet élément ne se produit jamais directement dans un document d’instance. 
  
Les éléments suivants sont membres du groupe de substitution SearchExpression :
  
- [Exists](exists.md)
    
- [Excludes](excludes.md)
    
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

