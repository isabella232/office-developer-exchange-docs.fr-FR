---
title: Recherche et EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 9fa5b836-857e-401d-9450-51e7dbc69104
description: Découvrez comment rechercher des éléments dans Exchange à l’aide de l’API managée EWS ou d’EWS.
ms.openlocfilehash: d35cc74ab2fa79530ac09256e315a780023d833b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463835"
---
# <a name="search-and-ews-in-exchange"></a>Recherche et EWS dans Exchange

Découvrez comment rechercher des éléments dans Exchange à l’aide de l’API managée EWS ou d’EWS.

Est présent familier ? Vous commencez enfin le projet que vous avez mis en place pendant des semaines, et vous avez besoin d’informations sur le projet que votre responsable vous a envoyé par courrier électronique il y a semaines. Votre boîte de réception contient des centaines voire des milliers de messages. Que fais-tu? Faites-vous défiler votre courrier électronique pour analyser chaque objet et expéditeur jusqu’à ce que vous les trouviez ? Ou utilisez-vous la fonctionnalité de recherche de votre client de messagerie préféré pour passer rapidement à zéro sur ce dont vous avez besoin ?

La recherche est probablement une fonctionnalité obligatoire pour n’importe quel client de messagerie. Toutefois, la recherche peut être utilisée pour beaucoup plus qu’autoriser les utilisateurs à effectuer des recherches dans leur boîte aux lettres. Votre application doit-elle traiter des rendez-vous qui se situent dans des fenêtres temporelles spécifiques ? Vous avez peut-être besoin de signaler toutes les tâches ayant un statut spécifique ou de déplacer tous les contacts ayant un nom de société spécifique vers un autre dossier. La recherche peut vous aider à répondre à toutes ces exigences.

## <a name="search-basics"></a>Notions de base de la recherche
<a name="bk_SearchBasics"> </a>

L’API managée EWS et EWS proposent deux méthodes de base pour la spécification d’une recherche. Vous pouvez utiliser un [filtre de recherche](how-to-use-search-filters-with-ews-in-exchange.md) ou une [chaîne de requête](how-to-perform-an-aqs-search-by-using-ews-in-exchange.md). La méthode que vous utilisez dépend de l’intention de votre recherche.

**Tableau 1. Scénarios pour les filtres de recherche et les requêtes de recherche**

|**Si vous souhaitez...**|**Utiliser un...**|**Notes**|
|:-----|:-----|:-----|
|Limiter votre recherche à une propriété spécifique ou à un ensemble de propriétés  <br/> |Filtre de recherche  <br/> |Les filtres de recherche fournissent le meilleur niveau de contrôle sur les propriétés recherchées. Bien que les chaînes de requête puissent cibler un ensemble limité de propriétés à l’aide de la syntaxe de requête avancée (AQS), les filtres de recherche peuvent cibler n’importe quelle propriété.  <br/> |
|Créer des recherches avec plusieurs critères  <br/> |Filtre de recherche  <br/> |Avec les filtres de recherche, plusieurs critères de recherche peuvent être associés à des opérateurs and logiques ou à des ORs, permettant des recherches comme « l’objet contient «notes de réunion » et l’expéditeur est égal à « Sadie Daniels ». Bien que les chaînes de requête puissent également rejoindre plusieurs critères de recherche, elles sont limitées à l’ensemble des propriétés prises en charge par les chaînes de requête.  <br/> |
|Rechercher des propriétés personnalisées  <br/> |Filtre de recherche  <br/> |Les filtres de recherche peuvent cibler des propriétés personnalisées. Les chaînes de requête ne recherchent pas les propriétés personnalisées.  <br/> |
|Effectuer une recherche de propriétés de chaîne respectant la casse  <br/> |Filtre de recherche  <br/> |Les recherches de chaîne de requête ne respectent pas la casse.  <br/> |
|Contrôler le mode d’imbrication lors de la recherche de propriétés de chaîne  <br/> |Filtre de recherche  <br/> |Les recherches de chaîne de requête sont toujours des recherches de sous-chaînes. Si vous devez rechercher des préfixes spécifiques ou exiger des correspondances exactes, un filtre de recherche est le meilleur choix.  <br/> |
|Rechercher des dossiers  <br/> |Filtre de recherche  <br/> |EWS ne prend pas en charge la recherche de dossiers avec une chaîne de requête.  <br/> |
|Créer un dossier de recherche  <br/> |Filtre de recherche  <br/> |EWS ne prend pas en charge la création de dossiers de recherche avec une chaîne de requête.  <br/> |
|Recherche dans toutes les propriétés couramment utilisées  <br/> |Chaîne de requête  <br/> |Les chaînes de requête qui ne contiennent pas de AQS effectuent une recherche dans toutes les propriétés couramment utilisées. Par exemple, la valeur de chaîne de requête « Mack Chaves » renvoie tous les messages envoyés par Mack Chaves, ainsi que tous les messages dont le corps ou l’objet contient « Mack Chaves ».  <br/> |
|Créer une recherche basée sur une entrée utilisateur simple  <br/> |Chaîne de requête  <br/> |Une chaîne de requête est un bon choix pour permettre à un utilisateur final d’effectuer une recherche rapide en tapant une chaîne simple. Étant donné qu’une recherche de chaîne de requête inclut toutes les propriétés couramment utilisées, les résultats contiendront tous les éléments qui contiennent les termes de recherche de l’utilisateur.  <br/> |

### <a name="using-a-search-filter"></a>Utilisation d’un filtre de recherche

Les filtres de recherche vous offrent un large éventail d’options de recherche et le plus grand degré de contrôle sur le mode d’exécution de la recherche. Vous pouvez utiliser des filtres de recherche pour effectuer des recherches d’égalité et de comparaison, mais vous pouvez également effectuer des recherches dans le contenu des propriétés de chaîne ou effectuer des comparaisons de masque de masques.

Par exemple, vous pouvez rechercher le contenu de l’objet d’éléments à l’aide de la classe [unsearchfilter. ContainsSubstring](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.containssubstring%28v=exchg.80%29.aspx) dans l’API managée EWS. Dans cet exemple, un filtre de recherche est créé pour Rechercher l’objet de la sous-chaîne « notes de réunion », sans tenir compte de la casse.

```cs
SearchFilter.ContainsSubstring subjectFilter = new SearchFilter.ContainsSubstring(ItemSchema.Subject,
    "meeting notes", ContainmentMode.Substring, ComparisonMode.IgnoreCase);
```

Vous pouvez également rechercher des propriétés personnalisées. Dans cet exemple, la propriété personnalisée **itemIndex** fait l’objet d’une recherche de valeurs supérieures à 3.

```cs
Guid MyAppGuid = new Guid("{AA3DF801-4FC7-401F-BBC1-7C93D6498C2E}");
ExtendedPropertyDefinition customPropDefinition =
    new ExtendedPropertyDefinition(MyAppGuid, "ItemIndex", MapiPropertyType.Integer);
SearchFilter.IsGreaterThan customPropFilter =
    new SearchFilter.IsGreaterThan(customPropDefinition, 3);
```

Vous pouvez également combiner plusieurs filtres de recherche pour créer des recherches plus complexes. Par exemple, vous pouvez combiner les deux filtres précédents avec un AND logique à l’aide de la classe [unsearchfilter. élément searchfiltercollectionpour](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.searchfiltercollection%28v=exchg.80%29.aspx) .

```cs
SearchFilter.SearchFilterCollection compoundFilter =
    new SearchFilter.SearchFilterCollection(LogicalOperator.And, subjectFilter, customPropFilter);
```

### <a name="using-a-query-string"></a>Utilisation d’une chaîne de requête

Les chaînes de requête fournissent une approche différente de la recherche. Vous avez moins de contrôle sur les champs qui sont recherchés et sur la façon dont la recherche est effectuée lorsque vous utilisez une recherche de chaîne de requête. Il ne s’agit pas d’une mauvaise chose ! Dans certains cas, vous souhaiterez peut-être utiliser un grand plus grand filet pour parler.

Par exemple, vous pouvez rechercher « notes de réunion » à l’aide de la méthode de l’API managée EWS [ExchangeService. FindItems](https://msdn.microsoft.com/library/jj223808%28v=exchg.80%29.aspx) .

```cs
FindItemsResults<Item> results = service.FindItems(folder, "meeting notes", view);
```

Si vous comparez les résultats de cette recherche aux résultats de l’exemple de recherche **unsearchfilter. ContainsSubstring** précédemment, cette recherche contiendra plus de résultats. La recherche de filtre de recherche ne renvoie que les éléments qui ont « notes de réunion » dans l’objet, tandis que cette recherche renvoie les éléments qui ont « notes de réunion » dans l’objet, le corps et les autres champs.

Voyons comment vous pouvez affiner la chaîne de requête pour vous rapprocher des résultats que vous voyez du filtre de recherche. À l’aide de AQS, vous pouvez limiter votre recherche à l’objet.

```cs
FindItemsResults<Item> results = service.FindItems(folder, "subject:meeting notes", view);
```

Cette approche est plus proche, mais les résultats ne sont toujours pas les mêmes. Lorsque vous utilisez une chaîne de requête avec plusieurs mots, vous obtiendrez des correspondances même si les mots ne sont pas dans l’ordre que vous spécifiez ou même s’ils ne sont pas adjacents. Avec la chaîne de requête « Subject : Meeting notes », vous obtiendrez des correspondances pour les « notes de réunion », « notes de la réunion », etc. Pour affiner davantage, vous pouvez encapsuler les termes de recherche entre guillemets pour indiquer que vous souhaitez uniquement cette expression.

```cs
FindItemsResults<Item> results = service.FindItems(folder, "subject:\"meeting notes\"", view);
```

## <a name="requesting-specific-properties-in-search-results"></a>Demande de propriétés spécifiques dans les résultats de la recherche
<a name="bk_RequestSpecific"> </a>

Par défaut, les résultats de la recherche contiendront toutes les propriétés des éléments qui correspondent à la recherche. Dans certains cas, il peut s’agir de ce que vous souhaitez, mais dans la plupart des cas, votre application requiert uniquement un ensemble discret de propriétés. Dans ce cas, vous devez limiter l’ensemble des propriétés qui sont renvoyées uniquement aux propriétés dont votre application a besoin. Dans l’exemple suivant, la classe [objetitemview](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview%28v=exchg.80%29.aspx) est utilisée pour limiter les propriétés renvoyées à l’objet, date/heure de réception et ID des éléments.

```cs
ItemView view = new ItemView(10);
// Creating a new PropertySet with this constructor includes
// ItemSchema.Id.
view.PropertySet = new PropertySet(ItemSchema.Subject, ItemSchema.DateTimeReceived);
```

## <a name="controlling-search-depth"></a>Contrôle de la profondeur de recherche
<a name="bk_SearchDepth"> </a>

La définition de la traversée sur la vue contrôle la profondeur et l’étendue de la recherche.

**Tableau 2. Valeurs de parcours de recherche**

|**Valeur transversale**|**S'applique à**|**Description**|
|:-----|:-----|:-----|
|Partielle  <br/> |Éléments et dossiers  <br/> |Les recherches superficielles sont limitées aux enfants directs du dossier recherché.  <br/> |
|Développée  <br/> |Éléments (uniquement avec les dossiers de recherche) et dossiers  <br/> |Les recherches approfondies effectuent une recherche de manière récursive dans le dossier recherché et ses sous-dossiers.  <br/> |
|Associé à  <br/> |Éléments  <br/> |Les recherches associées incluent uniquement les éléments associés à partir du dossier recherché. Les éléments associés sont des éléments masqués dans le dossier.  <br/> |
|SoftDeleted  <br/> |Éléments et dossiers  <br/> |Ce type de parcours est déconseillé. Les recherches SoftDeleted incluent uniquement les éléments qui se trouvent dans la benne. La benne a été remplacée par le [dossier éléments récupérables](https://docs.microsoft.com/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder) dans Exchange Online, Exchange Online dans le cadre d’Office 365 et les versions d’Exchange à partir d’Exchange 2010.  <br/> |

## <a name="managing-search-results"></a>Gestion des résultats de recherche
<a name="bk_ManageSearchResults"> </a>

L’API managée EWS et EWS vous permettent également de modifier la façon dont les résultats de la recherche sont renvoyés. Vous pouvez utiliser les affichages pour spécifier les propriétés à inclure dans les résultats, trier les résultats et pager vos résultats pour obtenir uniquement un nombre défini de résultats par réponse. Vous pouvez également regrouper les résultats par valeurs de champ spécifiques et contrôler la profondeur d’une recherche en spécifiant un type de parcours. Enfin, vous pouvez utiliser les dossiers de recherche pour créer des recherches permanentes qui sont mises à jour dynamiquement à l’arrivée de nouveaux éléments.

### <a name="sorting"></a>Tri

Vous pouvez faire en sorte que le serveur renvoie des résultats triés, ce qui permet d’afficher ou de traiter plus facilement les éléments dans l’ordre. Dans cet exemple, les résultats sont triés par date/heure de réception, avec les éléments les plus récents en premier.

```cs
view.OrderBy.Add(ItemSchema.DateTimeReceived, SortDirection.Descending);
```

### <a name="paging"></a>Pagination

Lorsque vous envoyez une demande de recherche à l’aide de l’API managée EWS ou EWS, vous spécifiez une taille d’affichage, qui contrôle le nombre maximal d’éléments renvoyés. Toutefois, le nombre d’éléments sur le serveur qui correspondent à votre recherche peut être supérieur à la taille de l’affichage. Dans ce cas, le serveur indique que d’autres éléments sont disponibles. Vous pouvez [utiliser la pagination pour répéter votre recherche](how-to-perform-paged-searches-by-using-ews-in-exchange.md) et obtenir l’ensemble de résultats suivant.

Par exemple, vous pouvez envoyer une demande de recherche avec une taille d’affichage de 10. Il peut y avoir 15 éléments sur le serveur qui correspondent à votre recherche, mais vous obtiendrez uniquement les 10 premiers, ainsi qu’un indicateur ( [FindItemsResults \<TItem\> . Propriété MoreAvailable](https://msdn.microsoft.com/library/dd635477%28v=exchg.80%29.aspx) si vous utilisez l’API managée EWS), il existe d’autres résultats sur le serveur. Vous pouvez ensuite envoyer la même recherche avec un décalage de 10 pour demander les 10 éléments suivants qui correspondent à votre recherche. Le serveur renverra les cinq éléments restants.

**Figure 1. Exemple de recherche paginée**

![Illustration présentant une recherche paginée. Une première requête est envoyée pour 10 éléments. Une seconde requête est envoyée pour les 10 éléments suivants.](media/Ex15_Search_PagedSearch.png)

### <a name="grouping"></a>Regroupement

 Exchange vous permet de regrouper les résultats de la recherche selon un champ spécifique. Cela peut vous aider à diviser les résultats de la recherche en ensembles plus faciles à gérer. Par exemple, vous pouvez rechercher « notes de réunion » et regrouper les résultats par expéditeur. Comme illustré dans la figure suivante, les éléments renvoyés seront séparés en groupes, avec tous les éléments correspondant aux critères du même expéditeur dans un groupe, tous les éléments correspondants d’un autre expéditeur dans un autre groupe, et ainsi de suite.

**Figure 2. Résultats de la recherche groupés par expéditeur**

![Illustration présentant les résultats de recherche regroupés par expéditeur.](media/Ex15_Search_GroupedResults.png)

## <a name="search-folders"></a>Dossiers de recherche
<a name="bk_SearchFolders"> </a>

Avec une recherche régulière, la recherche est exécutée, les résultats sont renvoyés à votre application pour traitement et la recherche cesse d’exister. Les dossiers de recherche permettent de rendre un processus de recherche permanent. Il s’agit d’une option intéressante pour les recherches que vous souhaitez exécuter plusieurs fois. Au lieu d’exécuter la même recherche à plusieurs reprises, ce qui entraîne l’évaluation de la recherche à partir de zéro à chaque fois, un dossier de recherche effectue une recherche toujours, ce qui permet au serveur de mettre à jour le jeu de résultats existant lorsque des éléments sont ajoutés ou supprimés de l’étendue de recherche. Les dossiers de recherche agissent comme des dossiers ordinaires, dans la mesure où ils apparaissent sous la forme de dossiers contenant des éléments. La différence réside dans le fait que les seuls éléments contenus dans le dossier sont ceux qui correspondent aux critères de recherche associés au dossier. Une fois qu’un dossier de recherche est créé, votre application peut obtenir les résultats de la recherche à jour, en vérifiant simplement le contenu du dossier.

La création d’un dossier de recherche est simple lorsque vous maîtrisez la création de filtres de recherche. Dans l’exemple suivant, un dossier de recherche est créé pour afficher tous les messages électroniques dont l’objet contient « notes de réunion ».

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

- [Effectuer une recherche AQS à l’aide d’EWS dans Exchange](how-to-perform-an-aqs-search-by-using-ews-in-exchange.md)

- [Effectuer des recherches paginées à l’aide d’EWS dans Exchange](how-to-perform-paged-searches-by-using-ews-in-exchange.md)

- [Effectuer des recherches groupées à l’aide d’EWS dans Exchange](how-to-perform-grouped-searches-by-using-ews-in-exchange.md)

- [Utiliser des dossiers de recherche à l’aide d’EWS dans Exchange](how-to-work-with-search-folders-by-using-ews-in-exchange.md)

## <a name="see-also"></a>Voir aussi


- [Développer des clients de service web pour Exchange](develop-web-service-clients-for-exchange.md)

- [Dossier éléments récupérables](https://docs.microsoft.com/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder)

- [ExchangeService. FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)

- [Paramètres de stratégie de limitation qui affectent les opérations de recherche EWS](ews-throttling-in-exchange.md#throttling-policy-parameters-that-affect-ews-search-operations)
