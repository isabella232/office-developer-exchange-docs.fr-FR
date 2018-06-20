---
title: QueryString (chaîne)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f81b1b3d-9fe4-4ab3-b517-42e4207fa596
description: L’élément QueryString spécifie un ensemble de valeurs à renvoyer qui correspondent à la chaîne de requête dans une requête d’opération FindPeople. Une recherche avec aucune chaîne de requête spécifiée retourne tous les éléments à partir du dossier spécifié.
ms.openlocfilehash: 9c5c733adcec1496e36986fd720b56b0a0274593
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828935"
---
# <a name="querystring-string"></a>QueryString (chaîne)

L’élément **QueryString** spécifie un ensemble de valeurs à renvoyer qui correspondent à la chaîne de requête dans une requête [d’opération FindPeople](findpeople-operation.md) . Une recherche avec aucune **chaîne de requête** spécifiée retourne tous les éléments à partir du dossier spécifié. 
  
```XML
<QueryString/> 
```

 **string**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[FindPeople](findpeople.md) <br/> |Contient les arguments pour une recherche de [l’opération FindPeople](findpeople-operation.md) .  <br/> |
   
## <a name="text-value"></a>Valeur de texte

La valeur de texte **QueryString** représente une requête de boîte aux lettres effectuée à l’aide d’un sous-ensemble de [La syntaxe de requête avancée (AQS)](http://msdn.microsoft.com/en-us/library/aa965711%28VS.85%29.aspx). Pour plus d’informations sur la syntaxe de cet élément, voir [QueryString (QueryStringType)](querystring-querystringtype.md).
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération FindPeople](findpeople-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

