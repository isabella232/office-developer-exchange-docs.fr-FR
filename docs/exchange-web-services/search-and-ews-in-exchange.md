---
title: Recherche et les services EWS d’Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 9fa5b836-857e-401d-9450-51e7dbc69104
description: Découvrez comment rechercher des éléments dans Exchange à l’aide de l’API managée EWS ou EWS.
ms.openlocfilehash: da24258ba94b842fa97fff92148620344c939f05
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755072"
---
# <a name="search-and-ews-in-exchange"></a>Recherche et les services EWS d’Exchange

Découvrez comment rechercher des éléments dans Exchange à l’aide de l’API managée EWS ou EWS.
  
Est cette familier ? Vous commencez enfin ce projet que vous avez mise des semaines, et vous avez besoin d’informations sur le projet que votre responsable vous a envoyé dans les semaines de la messagerie. Votre boîte de réception compte des centaines ou peut-être des milliers de messages. Que fais-tu ? Défiler votre courrier électronique analyse chaque objet et l’expéditeur jusqu'à ce que vous le trouvez ? Ou vous utilisez la fonctionnalité de recherche dans votre client de messagerie préféré pour rapidement ce dont vous avez besoin ?
  
La recherche est sans doute une fonctionnalité indispensable pour tout client de messagerie. Mais recherche peut être utilisée pour beaucoup plus de permettre aux utilisateurs de rechercher leur boîte aux lettres. Votre application a-t-elle besoin pour traiter les rendez-vous qui tombent dans les fenêtres de temps spécifique ? Vous devez peut-être créer des rapports sur tous les éléments de tâche avec un statut spécifique ou déplacer tous les contacts avec un nom de société spécifique vers un autre dossier. Recherche peut aider à toutes ces exigences.
  
## <a name="search-basics"></a>Concepts de base de recherche
<a name="bk_SearchBasics"> </a>

Les API managées EWS offrent deux méthodes permettant de spécifier une recherche de base. Vous pouvez utiliser un [filtre de recherche](how-to-use-search-filters-with-ews-in-exchange.md) ou une [chaîne de requête](how-to-perform-an-aqs-search-by-using-ews-in-exchange.md). La méthode à qu'utiliser dépend de l’intention de votre recherche.
  
**Le tableau 1. Scénarios pour les requêtes de recherche et des filtres de recherche**

|**Si vous souhaitez...**|**Utiliser un …**|**Remarques**|
|:-----|:-----|:-----|
|Limiter la recherche à une propriété spécifique ou un ensemble de propriétés  <br/> |Filtre de recherche  <br/> |Filtres de recherche fournissent le meilleur niveau de contrôle sur lequel les propriétés sont recherchées. Bien que les chaînes de requête puissent cibler un ensemble limité de propriétés à l’aide de la syntaxe de requête avancée (AQS), n’importe quelle propriété pouvant cibler des filtres de recherche.  <br/> |
|Créer des recherches à plusieurs critères  <br/> |Filtre de recherche  <br/> |Filtres de recherche, plusieurs critères de recherche peuvent être joints avec logique des opérateurs AND ou des opérateurs OR, permettant de recherches comme « l’objet contient « Notes réunion » et l’expéditeur est égale à « Sadie Daniels » ». Bien que les chaînes de requête peuvent également se joindre à plusieurs critères de recherche, ils sont limitées à l’ensemble des propriétés prises en charge par les chaînes de requête.  <br/> |
|Recherche des propriétés personnalisées  <br/> |Filtre de recherche  <br/> |Filtres de recherche peuvent cibler des propriétés personnalisées. Chaînes de requête ne recherche pas les propriétés personnalisées.  <br/> |
|Effectuer une recherche respectant la casse des propriétés de chaîne  <br/> |Filtre de recherche  <br/> |Les recherches de chaînes de requête ne respectent pas la casse.  <br/> |
|Contrôle le mode de relation contenant-contenu lors de la recherche des propriétés de type chaîne  <br/> |Filtre de recherche  <br/> |Les recherches de chaînes de requête sont toujours des recherches de sous-chaînes. Si vous avez besoin rechercher des préfixes spécifiques ou nécessitent des correspondances exactes, un filtre de recherche est le meilleur choix.  <br/> |
|Recherche de dossiers  <br/> |Filtre de recherche  <br/> |EWS ne prend pas en charge recherche des dossiers avec une chaîne de requête.  <br/> |
|Créer un dossier de recherche  <br/> |Filtre de recherche  <br/> |EWS ne prend pas en charge Création de dossiers de recherche avec une chaîne de requête.  <br/> |
|Recherche dans l’ensemble des propriétés couramment utilisées  <br/> |Chaîne de requête  <br/> |Recherchant des chaînes de requête qui ne contiennent pas AQS sur toutes les propriétés couramment utilisées. Par exemple, une valeur de chaîne de requête de « Mack n’a Chaves » renvoie tous les messages envoyés par Mack Chaves ainsi que tous les messages qui ont « Mack Chaves » dans le corps ou l’objet.  <br/> |
|Construire une recherche basée sur l’entrée utilisateur simple  <br/> |Chaîne de requête  <br/> |Une chaîne de requête est un bon choix pour permettre à un utilisateur final pour effectuer une recherche rapide en tapant dans une chaîne simple. Étant donné que la recherche d’une chaîne de requête inclut toutes les propriétés couramment utilisées, les résultats contiendra tous les éléments qui contiennent les termes de recherche de l’utilisateur.  <br/> |
   
### <a name="using-a-search-filter"></a>À l’aide d’un filtre de recherche

Filtres de recherche vous offrent un large éventail d’options de recherche et le plus haut niveau de contrôle sur la façon dont la recherche est effectuée. Vous pouvez utiliser les filtres de recherche pour effectuer des recherches de comparaison et d’égalité de base, mais vous pouvez également rechercher dans le contenu des propriétés de chaîne ou effectuer des comparaisons de masque de bits.
  
Par exemple, vous pouvez rechercher le contenu de l’objet d’éléments à l’aide de la classe [SearchFilter.ContainsSubstring](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.containssubstring%28v=exchg.80%29.aspx) dans l’API managée EWS. Dans cet exemple, un filtre de recherche est créé pour rechercher l’objet de la sous-chaîne « notes de réunion », indépendamment de la casse. 
  
```cs
SearchFilter.ContainsSubstring subjectFilter = new SearchFilter.ContainsSubstring(ItemSchema.Subject,
    "meeting notes", ContainmentMode.Substring, ComparisonMode.IgnoreCase);
```

Vous pouvez également rechercher par rapport à des propriétés personnalisées. Dans cet exemple, la propriété personnalisée **ItemIndex** est recherchée dans les valeurs supérieures à 3. 
  
```cs
Guid MyAppGuid = new Guid("{AA3DF801-4FC7-401F-BBC1-7C93D6498C2E}");
ExtendedPropertyDefinition customPropDefinition =
    new ExtendedPropertyDefinition(MyAppGuid, "ItemIndex", MapiPropertyType.Integer); 
SearchFilter.IsGreaterThan customPropFilter =
    new SearchFilter.IsGreaterThan(customPropDefinition, 3);
```

Vous pouvez également combiner plusieurs filtres de recherche pour créer des recherches plus complexes. Par exemple, vous pouvez combiner les deux filtres précédentes avec un et logique à l’aide de la classe [SearchFilter.SearchFilterCollection](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.searchfiltercollection%28v=exchg.80%29.aspx) . 
  
```cs
SearchFilter.SearchFilterCollection compoundFilter =
    new SearchFilter.SearchFilterCollection(LogicalOperator.And, subjectFilter, customPropFilter);
```

### <a name="using-a-query-string"></a>À l’aide d’une chaîne de requête

Chaînes de requête constituent une approche différente pour la recherche. Vous avez moins de contrôle sur les champs de recherche et comment la recherche est effectuée lorsque vous utilisez une recherche de chaîne de requête. Pas qui est une mauvaise chose ! Dans certains cas, vous pouvez souhaiter effectuer un cast un net plus large, pour ainsi dire.
  
Par exemple, vous pouvez rechercher « notes de réunion » à l’aide de la méthode d’API managées [ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/jj223808%28v=exchg.80%29.aspx) . 
  
```cs
FindItemsResults<Item> results = service.FindItems(folder, "meeting notes", view);
```

Si vous comparez les résultats de la recherche pour les résultats de l’exemple de recherche **SearchFilter.ContainsSubstring** précédemment, cette recherche contient plus de résultats. La recherche de filtre recherche retourne uniquement les éléments qui ont des « notes de réunion » dans l’objet, tandis que cette recherche renverra les éléments ayant des « notes de réunion » dans l’objet, le corps et autres champs. 
  
Examinons comment vous pouvez affiner la chaîne de requête pour obtenir les résultats que vous voyez du filtre de recherche plus proche. AQS, vous pouvez limiter votre recherche à l’objet.
  
```cs
FindItemsResults<Item> results = service.FindItems(folder, "subject:meeting notes", view);
```

Il s’agit plus proche, mais les résultats sont toujours pas exactement les mêmes. Lorsque vous utilisez une chaîne de requête avec plusieurs mots, vous obtiendrez des correspondances même si les mots ne sont pas dans l’ordre que vous spécifiez, ou même si elles ne sont pas adjacentes. Avec la chaîne de requête « Remarques subject : réunion », vous serez obtenir des correspondances pour « notes de réunion », « notes de la réunion » et ainsi de suite. Pour affiner davantage, vous pouvez encapsuler les termes de recherche dans des guillemets doubles pour indiquer que vous ne souhaitez que cette phrase.
  
```cs
FindItemsResults<Item> results = service.FindItems(folder, "subject:\"meeting notes\"", view);
```

## <a name="requesting-specific-properties-in-search-results"></a>Demande des propriétés spécifiques dans les résultats de recherche
<a name="bk_RequestSpecific"> </a>

Par défaut, les résultats de recherche contient toutes les propriétés sur les éléments qui correspondent à la recherche. Dans certains cas, il peut s’agir de ce que vous voulez, mais dans la plupart des cas, votre application nécessite uniquement un ensemble discret de propriétés. Dans ce cas, vous devez limiter le jeu de propriétés qui sont renvoyées pour que les propriétés de votre application a besoin. Dans l’exemple suivant, la classe [l’annonceAfficher](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemview%28v=exchg.80%29.aspx) l’est utilisée pour limiter les propriétés retournées au sujet, date/heure de réception et les ID des éléments. 
  
```cs
ItemView view = new ItemView(10);
// Creating a new PropertySet with this constructor includes 
// ItemSchema.Id.
view.PropertySet = new PropertySet(ItemSchema.Subject, ItemSchema.DateTimeReceived);
```

## <a name="controlling-search-depth"></a>Contrôle la profondeur de recherche
<a name="bk_SearchDepth"> </a>

Définition du parcours sur l’affichage de contrôle la profondeur et la portée de la recherche. 
  
**Le tableau 2. Parcours de valeurs de recherche**

|**Valeur Traversal**|**S'applique à**|**Description**|
|:-----|:-----|:-----|
|Peu profond  <br/> |Éléments et les dossiers  <br/> |Recherches superficielles sont limitées à diriger les enfants du dossier en cours de recherche.  <br/> |
|Profond  <br/> |Éléments (uniquement avec les dossiers de recherche) et les dossiers  <br/> |Le dossier en cours de recherche et les sous-dossiers de recherche récursive recherche approfondie.  <br/> |
|Associé  <br/> |Éléments  <br/> |Recherches associées incluent uniquement les éléments associés à partir du dossier en cours de recherche. Éléments associés sont des éléments masqués dans le dossier.  <br/> |
|SoftDeleted  <br/> |Éléments et les dossiers  <br/> |Ce type de parcours est déconseillé. Recherches SoftDeleted incluent uniquement les éléments qui se trouvent dans la benne. La benne a été remplacée par le [dossier éléments récupérables](http://technet.microsoft.com/en-us/library/ee364755%28v=exchg.150%29.aspx(Office.15).aspx) dans Exchange Online, Exchange Online dans le cadre d’Office 365 et les versions d’Exchange commençant par Exchange 2010.  <br/> |
   
## <a name="managing-search-results"></a>Gestion des résultats de la recherche
<a name="bk_ManageSearchResults"> </a>

Les API managées EWS permettent également vous permet de modifier la façon dont vos résultats de recherche sont renvoyés. Vous pouvez utiliser des affichages pour spécifier les propriétés qui sont incluses dans les résultats, trier les résultats et vos résultats pour réafficher uniquement un nombre défini de résultats par une réponse de page. Vous pouvez également regrouper les résultats par contrôle la profondeur d’une recherche et les valeurs de champ spécifique en spécifiant un type de parcours. Enfin, vous pouvez utiliser les dossiers de recherche pour créer des recherches permanentes sont mis à jour dynamiquement comme nouveaux éléments.
  
### <a name="sorting"></a>Tri

Vous pouvez obtenir le serveur renvoie des résultats triés, il peuvent être plus facile d’afficher ou de traiter les éléments dans l’ordre. Dans cet exemple, les résultats sont triés par date et heure de réception, avec les éléments les plus récents étant le premier.
  
```cs
view.OrderBy.Add(ItemSchema.DateTimeReceived, SortDirection.Descending);
```

### <a name="paging"></a>Pagination

Lorsque vous envoyez une demande de recherche à l’aide de l’API managée EWS ou EWS, vous spécifiez une taille d’affichage, qui contrôle le nombre maximal d’éléments renvoyés. Toutefois, le nombre d’éléments sur le serveur qui correspondent à votre recherche peut être supérieur à la taille d’affichage. Dans ce cas, le serveur indique que plusieurs éléments sont disponibles. Vous pouvez [utiliser la pagination pour répéter la recherche](how-to-perform-paged-searches-by-using-ews-in-exchange.md) et obtenir le jeu de résultats suivant. 
  
Par exemple, vous pouvez envoyer une demande de recherche avec une taille d’affichage de 10. Il peut y avoir 15 éléments sur le serveur qui correspondent à votre recherche, mais vous seulement recevrez des 10 premiers, ainsi qu’un indicateur (la [FindItemsResults\<TItem\>. MoreAvailable](http://msdn.microsoft.com/en-us/library/dd635477%28v=exchg.80%29.aspx) propriété si vous utilisez l’API managée EWS) qu’il n’y a plus de résultats sur le serveur. Vous pouvez envoyer la même recherche avec un décalage de 10 pour demander les 10 éléments qui correspondent à votre recherche. Le serveur renvoie les cinq éléments restants. 
  
**La figure 1. Exemple de recherche paginée**

![Illustration présentant une recherche paginée. Une première requête est envoyée pour 10 éléments. Une seconde requête est envoyée pour les 10 éléments suivants.](media/Ex15_Search_PagedSearch.png)
  
### <a name="grouping"></a>Regroupement

 Exchange vous permet de regrouper des résultats de recherche par un champ spécifique. Cela permet de dissocier les résultats de la recherche dans des ensembles plus facile à gérer. Par exemple, vous pourrez rechercher des « notes réunion » et regrouper les résultats par l’expéditeur. Comme indiqué dans la figure suivante, les éléments renvoyés sont classées par groupes, avec tous les éléments qui correspondent aux critères de l’expéditeur dans un même groupe, tous les éléments correspondants à partir d’un autre expéditeur dans un autre groupe et ainsi de suite. 
  
**La figure 2. Résultats de la recherche regroupés par expéditeur**

![Illustration présentant les résultats de recherche regroupés par expéditeur.](media/Ex15_Search_GroupedResults.png)
  
## <a name="search-folders"></a>Dossiers de recherche
<a name="bk_SearchFolders"> </a>

Avec une recherche standard, la recherche est exécutée, les résultats sont renvoyés à votre application pour le traitement et la recherche n’existe plus. Dossiers de recherche vous permettent d’effectuer une recherche permanente. Il s’agit d’une option intéressante pour les recherches que vous savez que vous souhaitez exécuter à plusieurs reprises. Au lieu de l’exécution de la même recherche à plusieurs reprises, un dossier de recherche à l’origine évaluer la recherche à partir de zéro, chaque fois que le serveur d’effectue une recherche toujours sur, ce qui permet au serveur de mettre à jour le résultat existant définir comme éléments sont ajoutés à ou supprimés de l’étendue de recherche. Act de dossiers de recherche comme les dossiers standard, en ce sens qu’ils apparaissent sous forme de dossiers qui ont des éléments. La différence est que les seuls éléments contenus dans le dossier sont ceux qui correspondent aux critères de recherche qui sont associés au dossier. Après la création d’un dossier de recherche, votre application peut obtenir des résultats de la recherche en vérifiant le contenu du dossier.
  
Création d’un dossier de recherche est simple lorsque vous maîtrisez la création des filtres de recherche. Dans l’exemple suivant, un dossier de recherche est créé pour afficher tous les messages dont l’objet contient « notes de réunion ».
  
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
    
- [Effectuer une recherche AQS à l’aide de EWS dans Exchange](how-to-perform-an-aqs-search-by-using-ews-in-exchange.md)
    
- [Effectuer des recherches paginées à l’aide de EWS dans Exchange](how-to-perform-paged-searches-by-using-ews-in-exchange.md)
    
- [Effectuer des recherches groupées à l’aide de EWS dans Exchange](how-to-perform-grouped-searches-by-using-ews-in-exchange.md)
    
- [Utilisation de dossiers de recherche à l’aide de EWS dans Exchange](how-to-work-with-search-folders-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a>Voir aussi


- [Développer des clients de service web pour Exchange](develop-web-service-clients-for-exchange.md)
    
- [Dossier éléments récupérables](http://technet.microsoft.com/en-us/library/ee364755%28v=exchg.150%29.aspx(Office.15).aspx)
    
- [ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)
    
- [Paramètres de stratégie de limitation EWS d’affecter les opérations de recherche](ews-throttling-in-exchange.md#bk_ThrottlingSearch)
    

