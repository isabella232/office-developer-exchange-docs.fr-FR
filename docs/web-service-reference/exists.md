---
title: Exists
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Exists
api_type:
- schema
ms.assetid: 55d568bd-8dbc-4d50-b9d7-54b74a54d4b5
description: L’élément Exists représente une expression de recherche qui renvoie la valeur true si la propriété fournie existe sur un élément.
ms.openlocfilehash: 992283d42f2060b7408f40289198bdbd22e71ec6
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541405"
---
# <a name="exists"></a>Exists

**L’élément Exists** représente une expression de recherche qui renvoie la valeur **true** si la propriété fournie existe sur un élément. 
  
```xml
<Exists>
   <Path/>
</Exists>
```

 **ExistsType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[FieldURI](fielduri.md) <br/> |Identifie les propriétés fréquemment référencés par URI.  <br/> |
|[IndexedFieldURI](indexedfielduri.md) <br/> |Identifie les membres individuels d’un dictionnaire.  <br/> |
|[ExtendedFieldURI](extendedfielduri.md) <br/> |Identifie les propriétés MAPI.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Restriction](restriction.md) <br/> |Représente la restriction ou la requête utilisée pour filtrer des éléments ou des dossiers dans les opérations FindItem/FindFolder et des dossiers de recherche.  <br/> |
|[Not](not.md) <br/> |Représente une expression de recherche qui annule la valeur booléle de l’expression de recherche qu’elle contient.  <br/> |
|[And](and.md) <br/> |Représente une expression de recherche qui vous permet d’effectuer une opération Boolean And entre deux ou plusieurs expressions de recherche. Le résultat de l’opération And est **true** si toutes les expressions de recherche contenues dans la et sont **vraies**.  <br/> |
|[Or](or.md) <br/> |Représente une expression de recherche qui effectue un OR logique sur l’expression de recherche qu’elle contient. [Ou](or.md) retournera **true si** l’un de ses enfants retourne **true**.  <br/> |
   
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

