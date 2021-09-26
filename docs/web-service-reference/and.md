---
title: And
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- And
api_type:
- schema
ms.assetid: 790246c2-37ad-49a8-91b9-6186d743b011
description: L’élément And représente une expression de recherche qui vous permet d’effectuer une opération Boolean AND entre deux ou plusieurs expressions de recherche. Le résultat de l’opération AND est true si toutes les expressions de recherche contenues dans l’élément And sont vraies.
ms.openlocfilehash: b6cf8ffbb19ea3aff917493e6ae4e324025c6ac9
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541531"
---
# <a name="and"></a>And

**L’élément And** représente une expression de recherche qui vous permet d’effectuer une opération **Boolean AND** entre deux ou plusieurs expressions de recherche. Le résultat de **l’opération AND** est **true** si toutes les expressions de recherche contenues dans l’élément **And** sont **vraies.**
  
```xml
<And>
   <SearchExpression/>
   <SearchExpression/>
</And>
```

 **AndType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[SearchExpression](searchexpression.md) <br/> | Représente la classe de base pour les expressions au sein d’une restriction. Il doit y avoir au moins deux expressions de recherche dans une opération And.<br/><br/>  L’un des éléments suivants doit être remplacé par **l’élément SearchExpression** :<ul><li> [Exists](exists.md)</li><li>[Excludes](excludes.md)</li><li>[IsEqualTo](isequalto.md)</li><li>[IsNotEqualTo](isnotequalto.md)</li><li>[IsGreaterThan](isgreaterthan.md)</li><li>[IsGreaterThanOrEqualTo](isgreaterthanorequalto.md)</li><li>[IsLessThan](islessthan.md)</li><li>[IsLessThanOrEqualTo](islessthanorequalto.md)</li><li>[Contains](contains.md)</li><li>[Not](not.md)</li><li>**And**</li><li>[Or](or.md) </li></ul> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Restriction](restriction.md) <br/> |Représente la restriction ou la requête utilisée pour filtrer des éléments ou des dossiers dans les opérations FindItem/FindFolder et des dossiers de recherche.  <br/> |
|[Not](not.md) <br/> |Représente une expression de recherche qui annule la valeur booléle de l’expression de recherche qu’elle contient.  <br/> |
|**And** <br/> |Représente une expression de recherche qui vous permet d’effectuer une opération **BOOlean AND** entre deux ou plusieurs expressions de recherche. Le résultat de **l’opération AND** est **true** si toutes les expressions de recherche contenues dans l’élément **And** sont **vraies.**  <br/> |
|[Or](or.md) <br/> |Représente une expression de recherche qui effectue une opération **LOGIQUE OR** sur l’expression de recherche qu’elle contient. **Ou** retournera **true si** l’un de ses enfants retourne **true**. **Ou** doit avoir au moins deux enfants.  <br/> |
   
## <a name="remarks"></a>Remarques

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

