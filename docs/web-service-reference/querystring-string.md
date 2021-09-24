---
title: QueryString (String)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: f81b1b3d-9fe4-4ab3-b517-42e4207fa596
description: L’élément QueryString spécifie un ensemble de valeurs à retourner qui correspondent à la chaîne de requête dans une demande d’opération FindPeople. Une recherche sans QueryString spécifiée renvoie tous les éléments du dossier spécifié.
ms.openlocfilehash: 6dfd4b5552511e2551baf5ce645f82d4f74e5499
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523733"
---
# <a name="querystring-string"></a>QueryString (String)

**L’élément QueryString** spécifie un ensemble de valeurs à retourner qui correspondent à la chaîne de requête dans une [demande d’opération FindPeople.](findpeople-operation.md) Une recherche sans **QueryString spécifiée** renvoie tous les éléments du dossier spécifié. 
  
```XML
<QueryString/> 
```

 **chaîne**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[FindPeople](findpeople.md) <br/> |Contient les arguments d’une [recherche d’opération FindPeople.](findpeople-operation.md)  <br/> |
   
## <a name="text-value"></a>Valeur texte

La **valeur de texte QueryString** représente une requête de boîte aux lettres réalisée à l’aide d’un sous-ensemble de syntaxe de requête avancée [(AQS).](https://msdn.microsoft.com/library/aa965711%28VS.85%29.aspx) Pour plus d’informations sur la syntaxe de cet élément, voir [QueryString (QueryStringType).](querystring-querystringtype.md)
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d’Exchange Server 2013.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération FindPeople](findpeople-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

