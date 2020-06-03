---
title: FindItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindItem
api_type:
- schema
ms.assetid: f7624f5c-c390-4563-ab9a-08f1024fb914
description: L’élément FindItem définit une demande pour rechercher des éléments dans une boîte aux lettres.
ms.openlocfilehash: 3aeda1cffc03292734a91bc3fff3289d51c9b445
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460994"
---
# <a name="finditem"></a>FindItem

L’élément **FindItem** définit une demande pour rechercher des éléments dans une boîte aux lettres. 
  
```xml
<FindItem Traversal="">
   <ItemShape/>
   <IndexedPageItemView/>
   <GroupBy/>
   <Restriction/>
   <SortOrder/>
   <ParentFolderIds/>
   <QueryString/>
</FindItem>
```

```xml
<FindItem Traversal="">
   <ItemShape/>
   <IndexedPageItemView/>
   <DistinguishedGroupBy/>
   <Restriction/>
   <SortOrder/>
   <ParentFolderIds/>
   <QueryString/>
</FindItem>
```

```xml
<FindItem Traversal="">
   <ItemShape/>
   <ContactsView/>
   <GroupBy/>
   <Restriction/>
   <SortOrder/>
   <ParentFolderIds/>
   <QueryString/>
</FindItem>
```

```xml
<FindItem Traversal="">
   <ItemShape/>
   <ContactsView/> 
   <DistinguishedGroupBy/>
   <Restriction/>
   <SortOrder/>
   <ParentFolderIds/>
   <QueryString/>
</FindItem>
```

```xml
<FindItem Traversal="">
   <ItemShape/>
   <CalendarView/>
   <GroupBy/>
   <Restriction/>
   <SortOrder/>
   <ParentFolderIds/>
   <QueryString/>
</FindItem>
```

```xml
<FindItem Traversal="">
   <ItemShape/>
   <FractionalPageItemView/>
   <GroupBy/>
   <Restriction/>
   <SortOrder/>
   <ParentFolderIds/>
   <QueryString/>
</FindItem>
```

```xml
<FindItem Traversal="">
   <ItemShape/>
   <FractionalPageItemView/>
   <DistinguishedGroupBy/>
   <Restriction/>
   <SortOrder/>
   <ParentFolderIds/>
   <QueryString/>
</FindItem>
```


**FindItemType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**Traversée** <br/> |Détermine si la recherche trouve des éléments dans des dossiers ou dans les bennes de dossiers. Cet attribut est obligatoire.  <br/> |
   
#### <a name="traversal-attribute-values"></a>Valeurs d’attribut transversal

|**Valeur**|**Description**|
|:-----|:-----|
|Partielle  <br/> |Renvoie uniquement les identités des éléments du dossier.  <br/> |
|SoftDeleted  <br/> |Renvoie uniquement les identités des éléments situés dans la benne d’un dossier. Notez qu’une traversée supprimée de manière récupérable combinée à une restriction de recherche entraîne zéro élément retourné même s’il existe des éléments qui correspondent aux critères de recherche.  <br/> |
|Associé à  <br/> |Renvoie uniquement les identités des éléments associés dans le dossier.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[ItemShape](itemshape.md) <br/> |Identifie les propriétés d’élément et le contenu à inclure dans une réponse d' [opération FindItem](finditem-operation.md) .  <br/> |
|[IndexedPageItemView](indexedpageitemview.md) <br/> |Décrit comment les informations d’élément paginé sont renvoyées pour une demande **FindItem** . Cet élément est facultatif.  <br/> |
|[FractionalPageItemView](fractionalpageitemview.md) <br/> |Décrit l’emplacement où l’affichage paginé démarre et le nombre maximal d’éléments renvoyés dans une requête **FindItem** . Le décalage de l’affichage paginé à partir du début de l’ensemble des éléments trouvés est décrit par une fraction. Cet élément est facultatif.  <br/> |
|[CalendarView](calendarview.md) <br/> |Fournit des limites de durée de temps pour définir une recherche pour les éléments de calendrier. Cet élément est facultatif.  <br/> |
|[ContactsView](contactsview.md) <br/> |Définit une recherche pour les éléments de contact en fonction des noms d’affichage alphabétiques. Cet élément est facultatif.  <br/> |
|[GroupBy](groupby.md) <br/> |Spécifie des groupes arbitraires pour les requêtes **FindItem** . Cet élément est facultatif.  <br/> |
|[DistinguishedGroupBy](distinguishedgroupby.md) <br/> |Fournit des regroupements standard pour les requêtes **FindItem** . Cet élément est facultatif.  <br/> |
|[Restriction](restriction.md) <br/> |Définit la restriction ou la requête utilisée pour filtrer des éléments ou des dossiers **FindItem**dans /  les opérations FindItem**FindFolder** et Search Folder. Cet élément est facultatif.  <br/> |
|[SortOrder](sortorder.md) <br/> |Définit le mode de tri des éléments dans une requête FindItem. Cet élément est facultatif.  <br/> |
|[ParentFolderIds](parentfolderids.md) <br/> |Identifie les dossiers dans lesquels rechercher les opérations FindItem et FindFolder.  <br/> |
|[QueryString (QueryStringType)](querystring-querystringtype.md) <br/> |Contient une chaîne de requête de boîte aux lettres basée sur la syntaxe de requête avancée (AQS).  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="remarks"></a>Remarques

Un seul des éléments [IndexedPageItemView](indexedpageitemview.md), [FractionalPageItemView](fractionalpageitemview.md), [CalendarView](calendarview.md)ou [ContactsView](contactsview.md) peut être inclus dans une demande **FindItem** . Un seul des éléments [GroupBy](groupby.md) ou [DistinguishedGroupBy](distinguishedgroupby.md) peut être inclus dans une demande **FindItem** . 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération FindItem](finditem-operation.md)
- [Recherche d’éléments](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

