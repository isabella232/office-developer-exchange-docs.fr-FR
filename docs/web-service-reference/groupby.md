---
title: GroupBy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GroupBy
api_type:
- schema
ms.assetid: 9728619b-4674-4b9d-9f6c-e75c6165966c
description: L’élément GroupBy spécifie un regroupement pour les requêtes FindItem arbitraire.
ms.openlocfilehash: d85c0fddec244c99dfbea1f85da331fc5319536d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827753"
---
# <a name="groupby"></a>GroupBy

L’élément **GroupBy** spécifie un regroupement pour les requêtes FindItem arbitraire. 
  
- [FindItem](finditem.md)
- [GroupBy](groupby.md)
  
```xml
<GroupBy Order="">
   <FieldURI/>
   <AggregateOn/>
</GroupBy>
```

 **GroupByType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**Order** <br/> | Détermine l’ordre des groupes dans le tableau élément groupé qui est renvoyé dans la réponse. Cet attribut est de type SortDirectionType.  <br/> |
   
#### <a name="order-attribute-values"></a>Valeurs d’attribut ordre

|**Valeur**|**Description**|
|:-----|:-----|
|Croissant  <br/> |Les groupes sont triés par ordre croissant.  <br/> |
|Décroissant  <br/> |Les groupes sont triés par ordre décroissant.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[FieldURI](fielduri.md) <br/> |Identifie les propriétés fréquemment référencées par un URI.  <br/> |
|[IndexedFieldURI](indexedfielduri.md) <br/> |Identifie les membres individuels d’un dictionnaire.  <br/> |
|[ExtendedFieldURI](extendedfielduri.md) <br/> |Identifie les propriétés MAPI étendues pour obtenir, définir ou créer.  <br/> |
|[AggregateOn](aggregateon.md) <br/> |Représente le champ qui est utilisé pour déterminer l’ordre des groupes dans une réponse.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[FindItem](finditem.md) <br/> |Définit une requête pour rechercher des éléments dans une boîte aux lettres.  <br/><br/> Vous trouverez ci-dessous l’expression XPath pour cet élément :`/FindItem` <br/> |
   
## <a name="remarks"></a>Remarques

La réponse FindItem contient une collection de groupes. Chaque groupe contiendra tous les éléments ayant des valeurs de la propriété **GroupBy** correspondantes. La propriété qui détermine le groupement est identifiée dans l’élément [FieldURI](fielduri.md), [IndexedFieldURI](indexedfielduri.md)ou [ExtendedFieldURI](extendedfielduri.md) . 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération FindItem](finditem-operation.md)
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)
- [Recherche d’éléments](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

