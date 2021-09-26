---
title: Non
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Not
api_type:
- schema
ms.assetid: 1aa16318-7e90-4b19-bce8-dd1a20a66223
description: L’élément Not représente une expression de recherche qui annule la valeur booléle de l’expression de recherche qu’il contient.
ms.openlocfilehash: a62a964043d85033ceffc5ca380468e0aeebdfc3
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541958"
---
# <a name="not"></a>Non

**L’élément Not** représente une expression de recherche qui annule la valeur booléle de l’expression de recherche qu’il contient. 
  
```xml
<Not>
   <SearchExpression/>
</Not>
```

 **NotType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[SearchExpression](searchexpression.md) <br/> | Représente la classe de base pour les expressions au sein d’une restriction. <br/><br/>L’un des éléments suivants doit être remplacé par **l’élément SearchExpression** : <br/> <br/>- [Existe](exists.md) <br/>- [Excludes](excludes.md) <br/>- [IsEqualTo](isequalto.md) <br/>- [IsNotEqualTo](isnotequalto.md) <br/>- [IsGreaterThan](isgreaterthan.md) <br/>- [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md) <br/>- [IsLessThan](islessthan.md) <br/>- [IsLessThanOrEqualTo](islessthanorequalto.md) <br/>- [Contient](contains.md) <br/>- **Not** <br/>- [And](and.md) <br/>- [Ou](or.md) <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Restriction](restriction.md) <br/> |Représente la restriction ou la requête utilisée pour filtrer des éléments ou des dossiers dans les opérations FindItem/FindFolder et des dossiers de recherche.  <br/> |
|**Not** <br/> |Représente une expression de recherche qui annule la valeur booléle de l’expression de recherche qu’elle contient.  <br/> |
|[And](and.md) <br/> |Représente une expression de recherche qui vous permet d’effectuer une opération **BOOlean AND** entre deux ou plusieurs expressions de recherche. Le résultat de **l’opération AND** est **true** si toutes les expressions de recherche contenues dans l’élément **And** sont **vraies.**  <br/> |
|[Or](or.md) <br/> |Représente une expression de recherche qui effectue une opération **LOGIQUE OR** sur l’expression de recherche qu’elle contient. **Ou** retournera **true si** l’un de ses enfants retourne **true**. **Ou** doit avoir au moins deux enfants.  <br/> |
   
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

