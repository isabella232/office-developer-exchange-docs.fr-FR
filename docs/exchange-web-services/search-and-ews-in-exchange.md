---
title: Recherche et EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 9fa5b836-857e-401d-9450-51e7dbc69104
description: Découvrez comment rechercher des éléments dans Exchange à l’aide de l’API gérée EWS ou d’EWS.
ms.openlocfilehash: f78f4625880480e4f0d1ebb683c6e7c2c7fa83e0
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59524433"
---
# <a name="search-and-ews-in-exchange"></a>Recherche et EWS dans Exchange

Découvrez comment rechercher des éléments dans Exchange à l’aide de l’API gérée EWS ou d’EWS.

Est présent familier ? Vous démarrez enfin ce projet que vous avez mis en place depuis des semaines et vous avez besoin d’informations sur le projet que votre responsable vous a envoyé par courrier électronique il y a des semaines. Votre boîte de réception insère des centaines voire des milliers de messages. Que fais-tu? Faites-vous défiler votre courrier électronique pour analyser chaque objet et chaque expéditeur jusqu’à ce que vous le trouviez ? Ou utilisez-vous la fonctionnalité de recherche dans votre client de messagerie favori pour rapidement vous aider à trouver ce dont vous avez besoin ?

La recherche est sans doute une fonctionnalité obligatoire pour n’importe quel client de messagerie. Toutefois, la recherche ne s’utilise pas uniquement pour permettre aux utilisateurs d’effectuer des recherches dans leur boîte aux lettres. Votre application a-t-elle besoin de traiter les rendez-vous qui se trouveront dans des fenêtres de temps spécifiques ? Peut-être devez-vous signaler tous les éléments de tâche ayant un état spécifique ou déplacer tous les contacts avec un nom de société spécifique vers un autre dossier. La recherche peut vous aider avec toutes ces exigences.

## <a name="search-basics"></a>Informations de base sur la recherche
<a name="bk_SearchBasics"> </a>

L’API gérée EWS et EWS offrent deux méthodes de base pour spécifier une recherche. Vous pouvez utiliser un [filtre de recherche ou](how-to-use-search-filters-with-ews-in-exchange.md) une chaîne de [requête.](how-to-perform-an-aqs-search-by-using-ews-in-exchange.md) La méthode que vous utilisez dépend de l’objectif de votre recherche.

**Tableau 1. Scénarios pour les filtres de recherche et les requêtes de recherche**

|**Si vous souhaitez...**|**Utilisez un...**|**Remarques**|
|:-----|:-----|:-----|
|Limiter votre recherche à une propriété ou à un ensemble de propriétés spécifique  <br/> |Filtre de recherche  <br/> |Les filtres de recherche offrent le meilleur niveau de contrôle sur les propriétés à rechercher. Bien que les chaînes de requête peuvent cibler un ensemble limité de propriétés à l’aide de la syntaxe de requête avancée (AQS), les filtres de recherche peuvent cibler n’importe quelle propriété.  <br/> |
|Créer des recherches avec plusieurs critères  <br/> |Filtre de recherche  <br/> |Avec les filtres de recherche, plusieurs critères de recherche peuvent être joints avec des AND logiques ou des E/S, ce qui permet d’effectuer des recherches telles que « l’objet contient « Notes de réunion » ET l’expéditeur est égal à « Sadie Daniels ». Bien que les chaînes de requête peuvent également joindre plusieurs critères de recherche, elles sont limitées à l’ensemble de propriétés pris en charge par les chaînes de requête.  <br/> |
|Rechercher des propriétés personnalisées  <br/> |Filtre de recherche  <br/> |Les filtres de recherche peuvent cibler des propriétés personnalisées. Les chaînes de requête ne recherchent pas les propriétés personnalisées.  <br/> |
|Effectuer une recherche sensible à la cas des propriétés de chaîne  <br/> |Filtre de recherche  <br/> |Les recherches de chaîne de requête ne sont pas sensibles à la cas.  <br/> |
|Contrôler le mode de contenu lors de la recherche des propriétés de chaîne  <br/> |Filtre de recherche  <br/> |Les recherches de chaîne de requête sont toujours des recherches de sous-chaînes. Si vous devez rechercher des préfixes spécifiques ou exiger des correspondances exactes, un filtre de recherche est le meilleur choix.  <br/> |
|Rechercher des dossiers  <br/> |Filtre de recherche  <br/> |EWS ne prend pas en charge la recherche de dossiers avec une chaîne de requête.  <br/> |
|Créer un dossier de recherche  <br/> |Filtre de recherche  <br/> |EWS ne prend pas en charge la création de dossiers de recherche avec une chaîne de requête.  <br/> |
|Rechercher dans toutes les propriétés couramment utilisées  <br/> |Chaîne de requête  <br/> |Les chaînes de requête qui ne contiennent pas AQS recherchent toutes les propriétés couramment utilisées. Par exemple, une valeur de chaîne de requête de « Propriétés Duos » retournera tous les messages envoyés par LessysSys, ainsi que tous les messages dont le corps ou l’objet est « Étatssyen ».  <br/> |
|Créer une recherche basée sur une entrée utilisateur simple  <br/> |Chaîne de requête  <br/> |Une chaîne de requête est un excellent choix pour permettre à un utilisateur final d’effectuer une recherche rapide en tapant une chaîne simple. Étant donné qu’une recherche de chaîne de requête inclut toutes les propriétés couramment utilisées, les résultats contiennent tous les éléments qui contiennent les termes de recherche de l’utilisateur.  <br/> |

### <a name="using-a-search-filter"></a>Utilisation d’un filtre de recherche

Les filtres de recherche vous donnent un large éventail d’options de recherche et offrent le plus grand degré de contrôle sur la façon dont la recherche est effectuée. Vous pouvez utiliser des filtres de recherche pour effectuer des recherches d’égalité et de comparaison de base, mais vous pouvez également effectuer des recherches dans le contenu des propriétés de chaîne ou effectuer des comparaisons de masques de bits.

Par exemple, vous pouvez rechercher le contenu de l’objet des éléments à l’aide de la classe [SearchFilter.ContainsSubstring](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.containssubstring%28v=exchg.80%29.aspx) dans l’API gérée EWS. Dans cet exemple, un filtre de recherche est créé pour rechercher dans l’objet la sous-stration « notes de réunion », en ignorant la cas.

```cs
SearchFilter.ContainsSubstring subjectFilter = new SearchFilter.ContainsSubstring(ItemSchema.Subject,
    "meeting notes", ContainmentMode.Substring, ComparisonMode.IgnoreCase);
```

Vous pouvez également rechercher des propriétés personnalisées. Dans cet exemple, la propriété personnalisée **ItemIndex** recherche des valeurs supérieure à 3.

```cs
Guid MyAppGuid = new Guid("{AA3DF801-4FC7-401F-BBC1-7C93D6498C2E}");
ExtendedPropertyDefinition customPropDefinition =
    new ExtendedPropertyDefinition(MyAppGuid, "ItemIndex", MapiPropertyType.Integer);
SearchFilter.IsGreaterThan customPropFilter =
    new SearchFilter.IsGreaterThan(customPropDefinition, 3);
```

Vous pouvez également combiner plusieurs filtres de recherche pour créer des recherches plus complexes. Par exemple, vous pouvez combiner les deux filtres précédents avec un and logique à l’aide de la classe [SearchFilter.SearchFilterCollection.](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.searchfiltercollection%28v=exchg.80%29.aspx)

```cs
SearchFilter.SearchFilterCollection compoundFilter =
    new SearchFilter.SearchFilterCollection(LogicalOperator.And, subjectFilter, customPropFilter);
```

### <a name="using-a-query-string"></a>Utilisation d’une chaîne de requête

Les chaînes de requête offrent une approche différente de la recherche. Vous avez moins de contrôle sur les champs recherchés et la façon dont la recherche est effectuée lorsque vous utilisez une recherche de chaîne de requête. Cela n’est pas une mauvaise chose ! Dans certains cas, vous souhaitez peut-être caster un réseau plus large, pour ainsi dire.

Par exemple, vous pouvez rechercher des « notes de réunion » à l’aide de la méthode d’API gérée EWS [ExchangeService.FindItems.](https://msdn.microsoft.com/library/jj223808%28v=exchg.80%29.aspx)

```cs
FindItemsResults<Item> results = service.FindItems(folder, "meeting notes", view);
```

Si vous comparez les résultats de cette recherche aux résultats de l’exemple de recherche **SearchFilter.ContainsSubstring** précédemment, cette recherche contiendra davantage de résultats. La recherche de filtre de recherche ne retourne que les éléments qui ont des « notes de réunion » dans l’objet, tandis que cette recherche retourne les éléments qui ont des « notes de réunion » dans l’objet, le corps et d’autres champs.

Examinons la façon dont vous pouvez affiner la chaîne de requête pour vous rapprocher des résultats que vous voyez à partir du filtre de recherche. À l’aide d’AQS, vous pouvez limiter votre recherche à l’objet.

```cs
FindItemsResults<Item> results = service.FindItems(folder, "subject:meeting notes", view);
```

Cela est plus proche, mais les résultats ne sont toujours pas tout à fait identiques. Lorsque vous utilisez une chaîne de requête avec plusieurs mots, vous obtenez des correspondances même si les mots ne sont pas dans l’ordre que vous spécifiez, ou même s’ils ne sont pas adjacents les uns aux autres. Avec la chaîne de requête « subject:meeting notes », vous obtenez des correspondances pour « notes de réunion », « notes de la réunion », etc. Pour affiner davantage, vous pouvez encapsuler les termes de recherche entre guillemets doubles pour indiquer que vous souhaitez uniquement cette expression.

```cs
FindItemsResults<Item> results = service.FindItems(folder, "subject:\"meeting notes\"", view);
```

## <a name="requesting-specific-properties-in-search-results"></a>Demande de propriétés spécifiques dans les résultats de recherche
<a name="bk_RequestSpecific"> </a>

Par défaut, les résultats de la recherche contiennent toutes les propriétés des éléments qui correspondent à la recherche. Dans certains cas, il peut s’agit de ce que vous souhaitez, mais dans la plupart des cas, votre application requiert uniquement un ensemble discret de propriétés. Dans ce cas, vous devez limiter l’ensemble des propriétés renvoyées uniquement aux propriétés dont votre application a besoin. Dans l’exemple suivant, la classe [ItemView](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview%28v=exchg.80%29.aspx) est utilisée pour limiter les propriétés renvoyées à l’objet, à la date/l’heure de réception et à l’ID des éléments.

```cs
ItemView view = new ItemView(10);
// Creating a new PropertySet with this constructor includes
// ItemSchema.Id.
view.PropertySet = new PropertySet(ItemSchema.Subject, ItemSchema.DateTimeReceived);
```

## <a name="controlling-search-depth"></a>Contrôle de la profondeur de recherche
<a name="bk_SearchDepth"> </a>

La définition de la traversée sur l’affichage contrôle la profondeur et l’étendue de la recherche.

**Tableau 2. Valeurs de traversée de recherche**

|**Valeur traversale**|**S'applique à**|**Description**|
|:-----|:-----|:-----|
|Superficiel  <br/> |Éléments et dossiers  <br/> |Les recherches superficiels sont limitées aux enfants directs du dossier recherché.  <br/> |
|Deep  <br/> |Éléments (uniquement avec dossiers de recherche) et dossiers  <br/> |Les recherches approfondies recherchent de manière récursive le dossier recherché et les sous-dossiers.  <br/> |
|Associé  <br/> |Éléments  <br/> |Les recherches associées incluent uniquement les éléments associés du dossier recherché. Les éléments associés sont des éléments masqués dans le dossier.  <br/> |
|SoftDeleted  <br/> |Éléments et dossiers  <br/> |Ce type de traversée est déprécié. Les recherches SoftDeleted incluent uniquement les éléments qui se trouve dans la benne. La benne a été remplacée par le dossier Éléments [récupérables](https://docs.microsoft.com/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder) dans Exchange Online, Exchange Online dans le cadre de Office 365 et les versions de Exchange à partir de Exchange 2010.  <br/> |

## <a name="managing-search-results"></a>Gestion des résultats de recherche
<a name="bk_ManageSearchResults"> </a>

L’API gérée EWS et EWS vous permettent également de modifier la façon dont vos résultats de recherche sont renvoyés. Vous pouvez utiliser les affichages pour spécifier les propriétés incluses dans les résultats, trier les résultats et pager vos résultats pour obtenir uniquement un nombre de résultats par réponse. Vous pouvez également grouper les résultats par valeurs de champ spécifiques et contrôler la profondeur d’une recherche en spécifiant un type de traversée. Enfin, vous pouvez utiliser des dossiers de recherche pour créer des recherches persistantes qui sont mises à jour dynamiquement à mesure que de nouveaux éléments arrivent.

### <a name="sorting"></a>Tri

Vous pouvez obtenir que le serveur retourne les résultats triés, ce qui peut faciliter l’affichage ou le traitement des éléments dans l’ordre. Dans cet exemple, les résultats sont triés selon la date et l’heure de réception, les éléments les plus récents étant en premier.

```cs
view.OrderBy.Add(ItemSchema.DateTimeReceived, SortDirection.Descending);
```

### <a name="paging"></a>Pagination

Lorsque vous envoyez une demande de recherche à l’aide de l’API gérée EWS ou d’EWS, vous spécifiez une taille d’affichage qui contrôle le nombre maximal d’éléments renvoyés. Toutefois, le nombre d’éléments sur le serveur qui correspondent à votre recherche peut être supérieur à la taille de l’affichage. Dans ce cas, le serveur indique que d’autres éléments sont disponibles. Vous pouvez [utiliser la pagination pour répéter votre recherche](how-to-perform-paged-searches-by-using-ews-in-exchange.md) et obtenir l’ensemble de résultats suivant.

Par exemple, vous pouvez envoyer une demande de recherche avec une taille d’affichage de 10. Il peut y avoir 15 éléments sur le serveur qui correspondent à votre recherche, mais vous ne recevez que les 10 premiers, ainsi qu’un indicateur [(FindItemsResults \<TItem\> . Propriété MoreAvailable](https://msdn.microsoft.com/library/dd635477%28v=exchg.80%29.aspx) si vous utilisez l’API gérée EWS) qui a davantage de résultats sur le serveur. Vous pouvez ensuite envoyer la même recherche avec un décalage de 10 pour demander les 10 éléments suivants qui correspondent à votre recherche. Le serveur retourne les cinq éléments restants.

**Figure 1. Exemple de recherche pagyée**

![Illustration présentant une recherche paginée. Une première requête est envoyée pour 10 éléments. Une seconde requête est envoyée pour les 10 éléments suivants.](media/Ex15_Search_PagedSearch.png)

### <a name="grouping"></a>Regroupement

 Exchange vous permet de grouper les résultats de recherche par champ spécifique. Cela peut aider à décomposer les résultats de recherche en ensembles plus faciles à gérer. Par exemple, vous pouvez rechercher des « notes de réunion » et grouper les résultats par expéditeur. Comme illustré dans la figure suivante, les éléments renvoyés seront séparés en groupes, avec tous les éléments qui correspondent aux critères du même expéditeur dans un groupe, tous les éléments correspondants d’un autre expéditeur dans un autre groupe, etc.

**Figure 2. Résultats de la recherche regroupés par expéditeur**

![Illustration présentant les résultats de recherche regroupés par expéditeur.](media/Ex15_Search_GroupedResults.png)

## <a name="search-folders"></a>Dossiers de recherche
<a name="bk_SearchFolders"> </a>

Avec une recherche régulière, la recherche est exécutée, les résultats sont renvoyés à votre application pour traitement et la recherche cesse d’exister. Les dossiers de recherche permettent de rendre une recherche persistante. Il s’agit d’une option idéale pour les recherches que vous souhaitez exécuter plusieurs fois. Au lieu d’exécuter la même recherche à plusieurs reprises, ce qui a pour effet que le serveur évalue la recherche à partir de zéro à chaque fois, un dossier de recherche effectue une recherche toujours en cours, ce qui permet au serveur de mettre à jour le jeu de résultats existant à mesure que des éléments sont ajoutés ou supprimés de l’étendue de recherche. Les dossiers de recherche agissent comme des dossiers ordinaires, dans la mesure où ils apparaissent en tant que dossiers contenant des éléments. La différence est que les seuls éléments contenus dans le dossier sont ceux qui correspondent aux critères de recherche associés au dossier. Une fois qu’un dossier de recherche est créé, votre application peut obtenir les résultats à jour de la recherche en vérifiant simplement le contenu du dossier.

La création d’un dossier de recherche est simple lorsque vous maîtrisez la création de filtres de recherche. Dans l’exemple suivant, un dossier de recherche est créé pour afficher tous les messages électroniques dont l’objet contient des « notes de réunion ».

```cs
static void CreateSearchFolder(ExchangeService service)
{
    SearchFilter.ContainsSubstring subjectFilter = new SearchFilter.ContainsSubstring(ItemSchema.Subject,
        "meeting notes", ContainmentMode.Substring, ComparisonMode.IgnoreCase);
    SearchFolder searchFolder = new SearchFolder(service);
    searchFolder.DisplayName = "Meeting Notes";
    searchFolder.SearchParameters.RootFolderIds.Add(WellKnownFolderName.Inbox);
    searchFolder.SearchParameters.Traversal = SearchFolderTraversal.Deep;
    searchFolder.SearchParameters.SearchFilter = subjectFilter;
    searchFolder.Save(WellKnownFolderName.SearchFolders);
}
```

## <a name="in-this-section"></a>Dans cette section
<a name="bk_InThisSection"> </a>

- [Utiliser des filtres de recherche avec EWS dans Exchange](how-to-use-search-filters-with-ews-in-exchange.md)

- [Effectuer une recherche AQS à l’aide d’EWS Exchange](how-to-perform-an-aqs-search-by-using-ews-in-exchange.md)

- [Effectuer des recherches paginées à l’aide des services web Exchange (EWS) dans Exchange](how-to-perform-paged-searches-by-using-ews-in-exchange.md)

- [Effectuer des recherches groupées à l’aide d’EWS Exchange](how-to-perform-grouped-searches-by-using-ews-in-exchange.md)

- [Utiliser des dossiers de recherche à l’aide d’EWS dans Exchange](how-to-work-with-search-folders-by-using-ews-in-exchange.md)

## <a name="see-also"></a>Voir aussi


- [Développer des clients de service web pour Exchange](develop-web-service-clients-for-exchange.md)

- [Dossier Éléments récupérables](https://docs.microsoft.com/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder)

- [ExchangeService.FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)

- [Paramètres de stratégie de limitation qui affectent les opérations de recherche EWS](ews-throttling-in-exchange.md#throttling-policy-parameters-that-affect-ews-search-operations)
