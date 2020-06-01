---
title: Ou
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Or
api_type:
- schema
ms.assetid: 4876d83a-73a3-4953-9d95-3048e6b76ccb
description: L’élément ou représente une expression de recherche qui effectue une ou logique sur l’expression de recherche qu’il contient. Ou renverra true si l’un de ses enfants renvoie la valeur true. Ou il doit avoir au moins deux enfants.
ms.openlocfilehash: 9bc676da5bbaad64f11f6717fb487c2e9bcf2d89
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462478"
---
# <a name="or"></a>Ou

L’élément **ou** représente une expression de recherche qui effectue une **ou** logique sur l’expression de recherche qu’il contient. **Ou** renverra **true** si l’un de ses enfants renvoie la **valeur true**. **Ou** il doit avoir au moins deux enfants. 
  
```xml
<Or>
   <SearchExpression/>
   <SearchExpression/>
</Or>
```

 **OrType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[SearchExpression](searchexpression.md) <br/> | Représente la classe de base pour les expressions dans une restriction. <br/><br/>L’un des éléments suivants doit être substitué à l’élément **SearchExpression** : <br/> <br/>- [Existe](exists.md) <br/>- [Exclut](excludes.md) <br/>- [IsEqualTo](isequalto.md) <br/>- [IsNotEqualTo](isnotequalto.md) <br/>- [IsGreaterThan](isgreaterthan.md) <br/>- [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md) <br/>- [IsLessThan](islessthan.md) <br/>- [IsLessThanOrEqualTo](islessthanorequalto.md) <br/>- [Comporte](contains.md) <br/>- [Aucun](not.md) <br/>- [Les](and.md) <br/>- **Des** <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Restriction](restriction.md) <br/> |Représente la restriction ou la requête qui est utilisée pour filtrer des éléments ou des dossiers dans les opérations FindItem/FindFolder et Search Folder.  <br/> |
|[Not](not.md) <br/> |Représente une expression de recherche qui nie la valeur booléenne de l’expression de recherche qu’elle contient.  <br/> |
|[And](and.md) <br/> |Représente une expression de recherche qui vous permet d’effectuer une opération booléenne **et** une opération entre deux ou plusieurs expressions de recherche. Le résultat de l’opération **and** est **true** si toutes les expressions de recherche contenues dans l’élément **and** sont **true**.  <br/> |
|**Or** <br/> |Représente une expression de recherche qui effectue une opération **or** logique sur l’expression de recherche qu’elle contient. **Ou** renverra **true** si l’un de ses enfants renvoie la **valeur true**. **Ou** il doit avoir au moins deux enfants.  <br/> |
   
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

