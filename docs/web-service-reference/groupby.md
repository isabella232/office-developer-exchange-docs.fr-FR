---
title: GroupBy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- GroupBy
api_type:
- schema
ms.assetid: 9728619b-4674-4b9d-9f6c-e75c6165966c
description: L’élément GroupBy spécifie un regroupement arbitraire pour les requêtes FindItem.
ms.openlocfilehash: 15e2d818ceae81f08ad0c52d9bdc881f7c3e2579
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539801"
---
# <a name="groupby"></a>GroupBy

**L’élément GroupBy** spécifie un regroupement arbitraire pour les requêtes FindItem. 
  
- [FindItem](finditem.md)
- [GroupBy](groupby.md)
  
```xml
<GroupBy Order="">
   <FieldURI/>
   <AggregateOn/>
</GroupBy>
```

```xml
<GroupBy Order="">
   <ExtendededFieldURI/>
   <AggregateOn/>
</GroupBy>
```

```xml
<GroupBy Order="">
   <IndexedFieldURI/>
   <AggregateOn/>
</GroupBy>
```

**GroupByType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**Order** <br/> | Détermine l’ordre des groupes dans le tableau d’éléments groupés qui est renvoyé dans la réponse. Cet attribut est de type SortDirectionType.  <br/> |
   
#### <a name="order-attribute-values"></a>Valeurs d’attribut de commande

|**Valeur**|**Description**|
|:-----|:-----|
|Croissant  <br/> |Les groupes sont triés dans l’ordre croissant.  <br/> |
|Décroissant  <br/> |Les groupes sont organisés dans l’ordre décroit.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[FieldURI](fielduri.md) <br/> |Identifie les propriétés fréquemment référencés par URI.  <br/> |
|[IndexedFieldURI](indexedfielduri.md) <br/> |Identifie les membres individuels d’un dictionnaire.  <br/> |
|[ExtendedFieldURI](extendedfielduri.md) <br/> |Identifie les propriétés MAPI étendues à obtenir, définir ou créer.  <br/> |
|[AggregateOn](aggregateon.md) <br/> |Représente le champ utilisé pour déterminer l’ordre des groupes dans une réponse.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[FindItem](finditem.md) <br/> |Définit une demande de recherche d’éléments dans une boîte aux lettres.  <br/><br/> Voici l’expression XPath de cet élément :  `/FindItem` <br/> |
   
## <a name="remarks"></a>Remarques

La réponse FindItem contient une collection de groupes. Chaque groupe contient tous les éléments dont les valeurs correspondent à la **propriété GroupBy.** La propriété qui détermine le regroupement est identifiée dans l’élément [FieldURI,](fielduri.md) [IndexedFieldURI](indexedfielduri.md)ou [ExtendedFieldURI.](extendedfielduri.md) 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération FindItem](finditem-operation.md)
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)
- [Recherche d’éléments](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

