---
title: Effectuer une recherche AQS à l’aide de EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: c136901a-313e-4adf-a223-1d090d16917a
description: Découvrez comment rechercher des chaînes de requête AQS dans des applications EWS API managées.
ms.openlocfilehash: dc859e24fa80cd5627477182979c9cc9527818d6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754939"
---
# <a name="perform-an-aqs-search-by-using-ews-in-exchange"></a>Effectuer une recherche AQS à l’aide de EWS dans Exchange

Découvrez comment rechercher des chaînes de requête AQS dans des applications EWS API managées.
  
Chaînes de requête constituent une alternative aux [filtres de recherche](how-to-use-search-filters-with-ews-in-exchange.md) pour l’expression de critères de recherche. Le principal avantage de chaînes de requête est que vous devez pas spécifier une propriété unique pour la recherche. Vous pouvez fournir simplement une valeur et la recherche s’appliquent à tous les champs couramment utilisées sur les éléments. Vous pouvez également affiner votre recherche à l’aide de la syntaxe de requête avancée (AQS) au lieu d’une valeur simple. Toutefois, les chaînes de requête ont les limitations suivantes que vous devez connaître avant de les ajouter à votre boîte à outils : 
  
- **Capacité limitée à rechercher des propriétés spécifiques.** Lorsque vous recherchez avec une valeur dans une chaîne de requête simple, la recherche est effectuée sur toutes les propriétés indexées. Vous pouvez affiner la recherche à des propriétés spécifiques, mais les propriétés disponibles pour une utilisation dans une chaîne AQS sont limitées. Si la propriété que vous souhaitez rechercher n’est pas une des propriétés qui sont disponibles pour AQS, envisagez d’utiliser un filtre de recherche. 
    
- **Propriétés personnalisées ne sont pas recherchées.** Les recherches de chaînes de requête sont effectuées par rapport à un index et des propriétés personnalisées ne sont pas incluses dans cet index. Si vous avez besoin rechercher des propriétés personnalisées, utilisez plutôt un filtre de recherche. 
    
- **Contrôle limité pour la chaîne de recherche.** Les recherches de chaînes de requête toujours ignorent la casse et sont toujours des recherches de sous-chaînes. Si vous souhaitez faire la casse, préfixe ou les recherches de concordance exacte, utilisent un filtre de recherche. 
    
- **Non disponible pour les dossiers ou les dossiers de recherche.** Les opérations EWS pour la recherche de dossiers ne prend pas en charge à l’aide d’une chaîne de requête. En outre, les dossiers de recherche ne prennent en charge les chaînes de requête. Dans les deux cas, un filtre de recherche est la seule option. 
    
## <a name="creating-a-query-string"></a>Création d’une chaîne de requête
<a name="bk_CreateQueryString"> </a>

Chaînes de requête dans les API managées EWS sont interprétées comme un sous-ensemble de la syntaxe AQS. Chaînes AQS sont composés des valeurs ou paires mot clé/valeur, séparées par un signe deux-points ( :)).
  
`keyword:value`

Lorsqu’une valeur est spécifiée sans un mot clé, la valeur sont recherchées dans toutes les propriétés indexées. Si un mot clé est associé à une valeur, le mot clé spécifie une propriété pour rechercher la valeur correspondante.
  
**Le tableau 1. Mots-clés AQS pris en charge**

|**Mot clé**|**Type de valeur**|**Exemple**|
|:-----|:-----|:-----|
|subject  <br/> |String  <br/> |objet : project  <br/> |
|body  <br/> |String  <br/> |illustrations de corps : ventes  <br/> |
|pièce jointe  <br/> |String  <br/> |pièce jointe : état  <br/> |
|et utilisez à la place  <br/> |String  <br/> |à : « Sadie danield »  <br/> |
|from  <br/> |String  <br/> |à partir de : espère que  <br/> |
|cc  <br/> |String  <br/> |cc : « Ronnie Sturgis »  <br/> |
|bcc  <br/> |String  <br/> |Bcc:Mack  <br/> |
|participants  <br/> |String  <br/> |participants : sadie  <br/> |
|catégorie  <br/> |String  <br/> |catégorie : projet  <br/> |
|importance  <br/> |String  <br/> |importance : haute  <br/> |
|type  <br/> |Type d’élément  <br/> |type : réunions  <br/> |
|envoyé  <br/> |Date  <br/> |envoyés : 10/12/2013  <br/> |
|reçus  <br/> |Date  <br/> |reçus : hier  <br/> |
|HasAttachment  <br/> |Bool�en  <br/> |Possède des pièces jointes : true  <br/> |
|est marqué  <br/> |Bool�en  <br/> |isflagged:true  <br/> |
|estlu  <br/> |Bool�en  <br/> |isread:False  <br/> |
|size  <br/> |Nombre  <br/> |taille :\>5000  <br/> |
   
Examinons comment fonctionnent les types de valeurs différents.
  
### <a name="using-a-string-value-type"></a>À l’aide d’une valeur de type chaîne

Types de valeur de chaîne sont par défaut exclu en tant que les recherches de sous-chaînes préfixe qui ne respectent pas la casse. Cela signifie que recherche d’objet : projet renverrait des sujets suivants : 
  
- Notes de la réunion de projet
    
- Avez-vous besoin des plans de projet ?
    
- Prévisions de ventes décembre
    
Vous pouvez modifier la recherche pour exiger que le mot entier plutôt que de correspondance de préfixes, en mettant la chaîne entre guillemets. Recherche de l’objet : « projet » élimine la valeur « Prévisions de ventes décembre » dans la liste des correspondances. Notez que la valeur est toujours pas la casse. 
  
Si vous utilisez plusieurs mots dans une chaîne de requête, une correspondance nécessite que les mots apparaissent dans les champs de recherches. Par exemple, recherche d’objet : projet renverrait des sujets suivants : 
  
- Plan de projet
    
- Avez-vous besoin des plans de projet ?
    
- Envoyez-moi le plan de projet
    
- Planification des jalons du projet
    
Si vous placez plusieurs mots entre guillemets, ils sont considérés comme une seule phrase. Recherche de l’objet : « projet » renverrait uniquement l’objet « Projet » de la liste précédente. 
  
### <a name="using-an-item-type-value-type"></a>À l’aide d’un type de valeur de type élément

Vous pouvez utiliser les valeurs de type d’élément suivantes avec le mot clé **type** pour limiter vos résultats de recherche à uniquement un type spécifique d’élément, tel que courrier ou les demandes de réunion : 
  
- contacts    
- documents    
- email    
- télécopies    
- messagerie instantanée (correspond aux messages instantanés)    
- feuilles    
- réunions (correspond au rendez-vous et demandes de réunion)    
- notes    
- posts    
- rssfeeds    
- tasks    
- messagerie vocale
    
### <a name="using-a-date-value-type"></a>À l’aide d’un type de valeur de date

Vous pouvez rechercher des types de valeur de date dans un certain nombre de différentes manières. Est la plus simple pour rechercher une date spécifique. Recherche avec reçus : 12/11/2013 retournera tous les éléments reçus sur le 11 décembre 2013. Toutefois, vous pouvez également être moins spécifique. Recherche avec reçus : 12/11 retournera tous les éléments reçus sur le 11 décembre de l’année en cours. 
  
Une autre option consiste à utiliser les noms de mois. Vous pouvez rechercher avec reçus : le 11 décembre 2013 ou 11 décembre pour obtenir les mêmes résultats reçues : 12/11/2013 et reçus : 12/11, respectivement. Vous pouvez également rechercher avec reçus : décembre pour obtenir tous les éléments reçus dans le mois de décembre, l’année en cours. 
  
Les noms des jours de la semaine est également une option. Recherche avec reçus : Mardi retournera tous les éléments reçus mardi de la semaine en cours. 
  
Types de valeur de date prennent également en charge un ensemble de mots clés pour les recherches par rapport à l’heure actuelle. Les mots clés suivants sont pris en charge :
  
- aujourd’hui  
- tomorrow
- yesterday
- this week    
- La semaine dernière    
- mois suivant    
- dernier mois    
- année à venir
    
Types de valeur de date peuvent également être comparées aux opérateurs relationnels comme supérieur ou inférieur à, ou une plage avec l’opérateur de plage **.**. Par exemple, reçu :\>30/11/2013, envoyés :\>= hier, et received:12/1/2013..today sont toutes les chaînes de requête valide. 
  
### <a name="using-a-boolean-value-type"></a>À l’aide d’un type de valeur de type Boolean

Types de valeur de type Boolean peuvent être « true » ou « false ». Les valeurs ne respectent pas la casse, donc isread:false produira les mêmes résultats qu’isread:FALSE.
  
### <a name="using-a-number-value-type"></a>À l’aide d’un type de valeur numérique

Types de valeur numériques peuvent être recherchées correspondances exactes, mais ils peuvent également être recherchés à l’aide des opérateurs relationnels comme supérieur ou inférieur à. Par exemple, taille : 10000 retourne uniquement les éléments qui ont une taille d’exactement 10 000 octets, mais la taille :\>= 10000 renvoie les éléments qui ont une taille supérieure ou égale à 10 000 octets. Vous pouvez également spécifier une plage à l’aide de l’opérateur de plage ( **.**). Par exemple, taille : 7000..8000 renvoie les éléments qui ont une taille comprise entre 7000 et 8000. 
  
### <a name="using-logical-operators"></a>Utilisation d’opérateurs logiques

Chaînes de requête prend en charge les opérateurs logiques suivants.
  
**Le tableau 2. Prise en charge des opérateurs logiques**

|**Opérateur**|**Exemples**|
|:-----|:-----|
|AND  <br/> |projet et à partir de : « Sadie Daniels »  <br/> objet :(project AND plan)  <br/> |
|OU  <br/> |objet : réunion ou à partir de : « Expédition brut »  <br/> à partir de : (« Sadie danield » ou « J’espère que brut »)  <br/> |
|NOT  <br/> |Non : « Ronnie Sturgis »  <br/> reçus : pas aujourd'hui  <br/> |
   
Notez que vous pouvez utiliser ces opérateurs pour joindre plusieurs critères ou pour joindre plusieurs valeurs dans une paire mot clé/valeur unique. Cependant, pour prendre part à plusieurs valeurs dans une paire mot clé/valeur unique, vous devez utiliser entre parenthèses pour délimiter les valeurs multiples. Pour comprendre pourquoi, envisagez de recherche à l’aide de : « Sadie Daniels » ou « Expédition brut ». Cette recherche est interprétée comme les critères suivants :
  
- L’élément provient Sadie danield, ou
    
- L’élément a l’expression « Expédition brut » dans une de ses propriétés indexées.
    
En revanche, à partir de : (« Sadie Daniels » ou « Expédition brut ») est interprétée comme : 
  
- L’élément provient Sadie danield, ou
    
- L’élément provient d’expédition brut
    
L’opérateur par défaut lorsque plusieurs critères sont spécifiés, mais aucun opérateur logique n’est inclus est and. Par exemple, a des pièces jointes : true subject : projet équivaut à a : pièce jointe : true et subject : project.
  
## <a name="example-find-items-by-using-a-query-string-and-the-ews-managed-api"></a>Exemple : Rechercher des éléments à l’aide d’une chaîne de requête et de l’API managée EWS
<a name="bk_ExampleEWSMA"> </a>

Dans cet exemple, une méthode appelée **SearchWithQueryString** est définie. Il prend un objet [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , un objet [WellKnownFolderName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) et un objet de **type string** qui représente la chaîne de requête en tant que paramètres. Cet exemple suppose que l’objet **ExchangeService** a été initialisée avec des valeurs valides dans les propriétés [d’Url](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) et les [informations d’identification](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) . 
  
```cs
using Microsoft.Exchange.WebServices.Data;
static void SearchWithQueryString(ExchangeService service, WellKnownFolderName folder, string queryString)
{
    // Limit the result set to 10 items.
    ItemView view = new ItemView(10);
    view.PropertySet = new PropertySet(ItemSchema.Subject,
                                       ItemSchema.DateTimeReceived,
                                       ItemSchema.Size,
                                       ItemSchema.Importance,
                                       EmailMessageSchema.IsRead);
    // Item searches do not support Deep traversal.
    view.Traversal = ItemTraversal.Shallow;
    // Sorting
    view.OrderBy.Add(ItemSchema.DateTimeReceived, SortDirection.Descending);
    try
    {
        // Execute the search based on the query string.
        // Example: "subject:project plan"
        FindItemsResults<Item> results = service.FindItems(folder, queryString, view);
        foreach (Item item in results.Items)
        {
            Console.WriteLine("Subject: {0}", item.Subject);
            Console.WriteLine("Received: {0}", item.DateTimeReceived.ToString());
            Console.WriteLine("Size: {0}", item.Size.ToString());
            Console.WriteLine("Importance: {0}", item.Importance.ToString());
            if (item is EmailMessage)
            {
                EmailMessage message = item as EmailMessage;
                Console.WriteLine("Read: {0}", message.IsRead.ToString());
            }
        }
    }
    catch (Exception ex)
    {
        Console.WriteLine("Exception while enumerating results: {0}", ex.Message);
    }
}
```

Vous pouvez utiliser cette méthode pour rechercher tous les éléments contenant l’expression « projet » dans l’objet, comme illustré dans cet exemple.
  
```cs
string queryString = "subject:\"project plan\"";
SearchWithQueryString(service, WellKnownFolderName.Inbox, queryString);
```

## <a name="example-find-items-by-using-a-query-string-and-ews"></a>Exemple : Rechercher des éléments à l’aide d’une chaîne de requête et les EWS
<a name="bk_ExampleEWS"> </a>

Dans cet exemple, une demande SOAP [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) recherche tous les éléments dans la boîte de réception avec l’expression « projet » dans l’objet. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
  <soap:Body>
    <m:FindItem Traversal="Shallow">
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
          <t:FieldURI FieldURI="item:DateTimeReceived" />
          <t:FieldURI FieldURI="item:Size" />
          <t:FieldURI FieldURI="item:Importance" />
          <t:FieldURI FieldURI="message:IsRead" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="10" Offset="0" BasePoint="Beginning" />
      <m:SortOrder>
        <t:FieldOrder Order="Descending">
          <t:FieldURI FieldURI="item:DateTimeReceived" />
        </t:FieldOrder>
      </m:SortOrder>
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox" />
      </m:ParentFolderIds>
      <m:QueryString>subject:"project plan"</m:QueryString>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

L’exemple suivant montre la réponse du serveur avec les résultats de recherche.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="712" MinorBuildNumber="22" Version="V2_3" 
        xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="1" TotalItemsInView="1" IncludesLastItemInRange="true">
            <t:Items>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>project plan</t:Subject>
                <t:DateTimeReceived>2013-12-11T15:42:02Z</t:DateTimeReceived>
                <t:Size>7406</t:Size>
                <t:Importance>Normal</t:Importance>
                <t:IsRead>false</t:IsRead>
              </t:Message>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>
```

## <a name="see-also"></a>Voir aussi

- [Recherche et EWS dans Exchange](search-and-ews-in-exchange.md)    
- [Utiliser des filtres de recherche avec EWS dans Exchange](how-to-use-search-filters-with-ews-in-exchange.md)    
- [ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)    
- [Opération FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    

