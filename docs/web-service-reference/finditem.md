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
description: L’élément FindItem définit une requête pour rechercher des éléments dans une boîte aux lettres.
ms.openlocfilehash: 9831b034be7deb0cf6e756bb585bdbe34b370afd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756403"
---
# <a name="finditem"></a>FindItem

L’élément **FindItem** définit une requête pour rechercher des éléments dans une boîte aux lettres. 
  
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

 **FindItemType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**Traversée du contenu** <br/> |Définit si la recherche trouve des éléments dans les dossiers ou dumpsters des dossiers. Cet attribut est requis.  <br/> |
   
#### <a name="traversal-attribute-values"></a>Valeurs d’attribut Traversal

|**Valeur**|**Description**|
|:-----|:-----|
|Peu profond  <br/> |Renvoie uniquement les identités des éléments dans le dossier.  <br/> |
|SoftDeleted  <br/> |Renvoie uniquement les identités des éléments qui se trouvent dans un dossier de benne. Notez que zéro renvoyés entraînera un parcours récupérable combiné à une restriction de recherche même s’il existe des éléments qui correspondent aux critères de recherche.  <br/> |
|Associé  <br/> |Renvoie uniquement les identités des éléments associés dans le dossier.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[ItemShape](itemshape.md) <br/> |Identifie les propriétés de l’élément et le contenu à inclure dans une réponse de [l’opération FindItem](finditem-operation.md) .  <br/> |
|[IndexedPageItemView](indexedpageitemview.md) <br/> |Décrit comment paginé informations sont retournées pour une demande **FindItem** . Cet élément est facultatif.  <br/> |
|[FractionalPageItemView](fractionalpageitemview.md) <br/> |Décrit où l’affichage paginé démarre et le nombre maximal d’éléments renvoyés dans une requête **FindItem** . Le décalage d’affichage paginé depuis le début de l’ensemble des éléments trouvés est décrit par une fraction. Cet élément est facultatif.  <br/> |
|[CalendarView](calendarview.md) <br/> |Fournit des temps couvrent des limites pour définir une recherche des éléments de calendrier. Cet élément est facultatif.  <br/> |
|[ContactsView](contactsview.md) <br/> |Définit une recherche des éléments de contact basées sur des noms d’affichage alphabétiques. Cet élément est facultatif.  <br/> |
|[GroupBy](groupby.md) <br/> |Spécifie les regroupements arbitraires pour les requêtes **FindItem** . Cet élément est facultatif.  <br/> |
|[DistinguishedGroupBy](distinguishedgroupby.md) <br/> |Fournit des regroupements standards pour les requêtes **FindItem** . Cet élément est facultatif.  <br/> |
|[Restriction](restriction.md) <br/> |Définit la restriction ou la requête qui est utilisé pour filtrer des éléments ou des dossiers dans **FindItem**/ opérations de dossier**FindFolder** et la recherche. Cet élément est facultatif.  <br/> |
|[SortOrder](sortorder.md) <br/> |Définit comment les éléments sont triés dans une requête FindItem. Cet élément est facultatif.  <br/> |
|[ParentFolderIds](parentfolderids.md) <br/> |Identifie les dossiers pour rechercher les opérations FindItem et FindFolder.  <br/> |
|[QueryString (QueryStringType)](querystring-querystringtype.md) <br/> |Contient une chaîne de requête de boîte aux lettres basée sur la syntaxe de requête avancée (AQS).  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="remarks"></a>Remarques

Seul le [IndexedPageItemView](indexedpageitemview.md), [FractionalPageItemView](fractionalpageitemview.md), [CalendarView](calendarview.md)ou éléments [ContactsView](contactsview.md) peut être inclus dans une demande **FindItem** . Une seule des éléments [GroupBy](groupby.md) ou [DistinguishedGroupBy](distinguishedgroupby.md) peut être incluse dans une demande **FindItem** . 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération FindItem](finditem-operation.md)


[Recherche d’éléments](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

