---
title: Effectuer une recherche AQS à l’aide d’EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: c136901a-313e-4adf-a223-1d090d16917a
description: Découvrez comment effectuer des recherches à l’aide de chaînes de requête et de AQS dans votre application EWS ou API managée EWS.
localization_priority: Priority
ms.openlocfilehash: 9f611a8d90c6baf0f307897735c6366c82bb63c8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455715"
---
# <a name="perform-an-aqs-search-by-using-ews-in-exchange"></a>Effectuer une recherche AQS à l’aide d’EWS dans Exchange

Découvrez comment effectuer des recherches à l’aide de chaînes de requête et de AQS dans votre application EWS ou API managée EWS.
  
Les chaînes de requête fournissent une alternative aux [filtres de recherche](how-to-use-search-filters-with-ews-in-exchange.md) pour exprimer des critères de recherche. Le plus grand avantage de l’utilisation des chaînes de requête est que vous n’êtes pas obligé de spécifier une seule propriété à rechercher. Vous pouvez simplement indiquer une valeur, et la recherche s’appliquera à tous les champs couramment utilisés sur les éléments. Vous pouvez également affiner votre recherche à l’aide de la syntaxe de requête avancée (AQS) au lieu d’une valeur simple. Toutefois, les chaînes de requête présentent les limitations suivantes que vous devez connaître avant de les ajouter à votre boîte à outils : 
  
- **La possibilité de rechercher des propriétés spécifiques est limitée.** Lorsque vous effectuez une recherche avec une valeur simple dans une chaîne de requête, la recherche est effectuée sur toutes les propriétés indexées. Vous pouvez affiner votre recherche à des propriétés spécifiques, mais les propriétés pouvant être utilisées dans une chaîne AQS sont limitées. Si la propriété que vous souhaitez rechercher n’est pas l’une des propriétés disponibles pour AQS, envisagez d’utiliser un filtre de recherche. 
    
- **Les propriétés personnalisées ne sont pas recherchées.** Les recherches de chaîne de requête sont effectuées sur un index, et les propriétés personnalisées ne sont pas incluses dans cet index. Si vous devez rechercher des propriétés personnalisées, utilisez plutôt un filtre de recherche. 
    
- **Contrôle limité pour les recherches de chaînes.** Les recherches de chaîne de requête ignorent toujours la casse, et sont toujours des recherches de sous-chaînes. Si vous souhaitez effectuer des recherches en tenant compte de la casse, du préfixe ou de la correspondance exacte, utilisez un filtre de recherche. 
    
- **Non disponible pour les dossiers ou les dossiers de recherche.** Les opérations EWS pour la recherche de dossiers ne prennent pas en charge l’utilisation d’une chaîne de requête. En outre, les dossiers de recherche ne prennent pas en charge les chaînes de requête. Dans les deux cas, un filtre de recherche est votre seule option. 
    
## <a name="creating-a-query-string"></a>Création d’une chaîne de requête
<a name="bk_CreateQueryString"> </a>

Les chaînes de requête dans l’API managée EWS et EWS sont interprétées comme un sous-ensemble de la syntaxe AQS. Les chaînes AQS sont composées de valeurs ou de paires mot clé/valeur, séparées par un signe deux-points ( :).
  
`keyword:value`

Lorsqu’une valeur est spécifiée sans mot clé, toutes les propriétés indexées sont recherchées pour la valeur. Si un mot clé est associé à une valeur, le mot clé spécifie une propriété à rechercher pour la valeur correspondante.
  
**Tableau 1. Mots clés AQS pris en charge**

|**Mot clé**|**Type de valeur**|**Exemple**|
|:-----|:-----|:-----|
|subject  <br/> |Chaîne  <br/> |Subject : Project  <br/> |
|corps  <br/> |Chaîne  <br/> |corps : chiffres de ventes  <br/> |
|pièce jointe  <br/> |Chaîne  <br/> |pièce jointe : rapport  <br/> |
|au  <br/> |Chaîne  <br/> |à : « Sadie Daniels »  <br/> |
|from  <br/> |Chaîne  <br/> |de : espérons  <br/> |
|cc  <br/> |Chaîne  <br/> |CC : "Ronnie Sturgis"  <br/> |
|bcc  <br/> |Chaîne  <br/> |CCI : Mack  <br/> |
|participants  <br/> |Chaîne  <br/> |participants : Sadie  <br/> |
|category  <br/> |String  <br/> |Catégorie : projet  <br/> |
|importance  <br/> |String  <br/> |importance:high  <br/> |
|type  <br/> |Type d’élément  <br/> |type : réunions  <br/> |
|envoyé  <br/> |Date  <br/> |envoyés : 12/10/2013  <br/> |
|reçu  <br/> |Date  <br/> |reçu : hier  <br/> |
|HasAttachment  <br/> |Valeur booléenne  <br/> |Avec pièce jointe : true  <br/> |
|isflagged  <br/> |Valeur booléenne  <br/> |isflagged : true  <br/> |
|IsRead  <br/> |Valeur booléenne  <br/> |IsRead : false  <br/> |
|size  <br/> |Nombre  <br/> |taille : \> 5000  <br/> |
   
Examinons le fonctionnement des différents types de valeur.
  
### <a name="using-a-string-value-type"></a>Utilisation d’un type de valeur de chaîne

Par défaut, les types de valeur de chaîne sont recherchés dans des recherches de sous-chaînes de préfixe qui ne respectent pas la casse. Cela signifie que la recherche d’objet : Project correspond à l’un des objets suivants : 
  
- Notes de réunion Project
    
- Avez-vous des plans de projet ?
    
- Projections de ventes de décembre
    
Vous pouvez modifier la recherche pour exiger le mot entier plutôt que les préfixes correspondants en encadrant la chaîne entre guillemets. Recherche d’un objet : « projet » supprime la valeur « projections de ventes de décembre » de la liste des correspondances. Notez que la valeur n’est toujours pas sensible à la casse. 
  
Si vous utilisez plusieurs mots dans une chaîne de requête, une correspondance exige que les deux mots apparaissent dans les champs recherchés. Par exemple, la recherche d’un objet : plan de projet correspond à l’un des objets suivants : 
  
- Plan de projet
    
- Avez-vous des plans de projet ?
    
- Veuillez m’envoyer le plan de notre projet.
    
- Planification des jalons du projet
    
Si vous placez plusieurs mots entre guillemets, ils sont considérés comme une seule phrase. Recherche d’un objet : « plan de projet » ne correspondait qu’au « plan de projet » de la liste précédente. 
  
### <a name="using-an-item-type-value-type"></a>Utilisation d’un type de valeur de type d’élément

Vous pouvez utiliser les valeurs de types d’éléments suivantes avec le mot clé **Kind** pour limiter les résultats de la recherche à un type d’élément spécifique, tel que les demandes de messagerie ou de réunion : 
  
- contacts    
- docs    
- email    
- faxes    
- messagerie instantanée (correspond aux messages instantanés)    
- journals    
- réunions (correspond aux rendez-vous et aux demandes de réunion)    
- notes    
- posts    
- rssfeeds    
- tasks    
- voicemail
    
### <a name="using-a-date-value-type"></a>Utilisation d’un type de valeur de date

Vous pouvez rechercher des types de valeur de date de plusieurs façons différentes. La plus simple consiste à rechercher une date spécifique. Recherche avec reçus : 12/11/2013 renverra tous les éléments reçus le 11 décembre 2013. Toutefois, vous pouvez également être moins spécifique. Recherche avec reçus : 12/11 renverra tous les éléments reçus le 11 décembre de l’année en cours. 
  
Une autre option consiste à utiliser les noms de mois. Vous pouvez rechercher avec reçu le 11 décembre 2013 ou le 11 décembre pour obtenir les mêmes résultats que ceux reçus : 12/11/2013 et reçus : 12/11, respectivement. Vous pouvez également effectuer une recherche avec received : décembre pour obtenir tous les éléments reçus dans le mois de décembre, dans l’année en cours. 
  
L’utilisation des noms des jours de la semaine est également une option. Recherche avec reçu : mardi renverra tous les éléments reçus le mardi de la semaine en cours. 
  
Les types de valeur date prennent également en charge un ensemble de mots clés pour les recherches relatives à l’heure actuelle. Les mots clés suivants sont pris en charge :
  
- aujourd’hui  
- demain
- yesterday
- this week    
- La semaine dernière    
- mois suivant    
- mois précédent    
- année à venir
    
Les types de valeur date peuvent également être comparés à des opérateurs relationnels comme supérieur ou inférieur à ou spécifiés en tant que plage avec l’opérateur de plage **..**. Par exemple, received : \> 11/30/2013, sent : \> = hier, et Received : 12/1/2013.. Today sont toutes des chaînes de requête valides. 
  
### <a name="using-a-boolean-value-type"></a>Utilisation d’un type de valeur booléenne

Les types de valeurs booléennes peuvent être « true » ou « false ». Les valeurs ne respectent pas la casse, par conséquent IsRead : false produira les mêmes résultats que IsRead : FALSe.
  
### <a name="using-a-number-value-type"></a>Utilisation d’un type de valeur numérique

Les types de valeurs numériques peuvent être recherchés comme correspondances exactes, mais ils peuvent également faire l’objet d’une recherche à l’aide d’opérateurs relationnels comme supérieur ou inférieur à. Par exemple, Size : 10000 renvoie uniquement les éléments dont la taille est égale à 10000 octets, mais Size : \> = 10000 renverra des éléments dont la taille est supérieure ou égale à 10000 octets. Vous pouvez également spécifier une plage à l’aide de l’opérateur de plage ( **..**). Par exemple, Size : 7000.. 8000 renverra des éléments dont la taille est comprise entre 7000 et 8000. 
  
### <a name="using-logical-operators"></a>Utilisation d’opérateurs logiques

Les chaînes de requête prennent en charge les opérateurs logiques suivants.
  
**Tableau 2. Opérateurs logiques pris en charge**

|**Opérateur**|**Exemples**|
|:-----|:-----|
|AND  <br/> |Project et from : "Sadie Daniels"  <br/> objet : (Project et plan)  <br/> |
|OR  <br/> |Subject : réunion ou de : « espoir brut »  <br/> from :("Sadie Daniels" ou "espoir brut")  <br/> |
|NOT  <br/> |NE provenant pas de : « Ronnie Sturgis »  <br/> reçu : pas aujourd’hui  <br/> |
   
Notez que vous pouvez utiliser ces opérateurs pour joindre plusieurs critères ou joindre plusieurs valeurs au sein d’une seule paire mot clé/valeur. Toutefois, lorsque vous associez plusieurs valeurs dans une paire mot clé/valeur unique, vous devez utiliser des parenthèses pour encadrer les valeurs multiples. Pour comprendre pourquoi, envisagez d’effectuer une recherche à partir de : « Sadie Daniels » ou « espérons brut ». Cette recherche est en fait interprétée comme suit :
  
- L’élément provient de Sadie Daniels ou
    
- L’élément a l’expression « espoir brut » dans l’une de ses propriétés indexées.
    
En revanche, à partir de :(« Sadie Daniels » ou « espoir brut ») est interprétée comme : 
  
- L’élément provient de Sadie Daniels ou
    
- L’article est d’espoir brut
    
Opérateur par défaut lorsque plusieurs critères sont spécifiés, mais qu’aucun opérateur logique n’est inclus, et. Par exemple, comporte Attachment : true Subject : le projet équivaut à : Attachment : true et Subject : Project.
  
## <a name="example-find-items-by-using-a-query-string-and-the-ews-managed-api"></a>Exemple : Rechercher des éléments à l’aide d’une chaîne de requête et de l’API managée EWS
<a name="bk_ExampleEWSMA"> </a>

Dans cet exemple, une méthode appelée **SearchWithQueryString** est définie. Il prend un objet [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , un objet [WellKnownFolderName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) et un objet **String** qui représente la chaîne de requête en tant que paramètres. Cet exemple part du principe que l’objet **ExchangeService** a été initialisé avec des valeurs valides dans les [informations d’identification](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) et les propriétés de l' [URL](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) . 
  
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

Vous pouvez utiliser cette méthode pour rechercher tous les éléments avec l’expression « plan de projet » dans l’objet, comme illustré dans cet exemple.
  
```cs
string queryString = "subject:\"project plan\"";
SearchWithQueryString(service, WellKnownFolderName.Inbox, queryString);
```

## <a name="example-find-items-by-using-a-query-string-and-ews"></a>Exemple : Rechercher des éléments à l’aide d’une chaîne de requête et EWS
<a name="bk_ExampleEWS"> </a>

Dans cet exemple, une requête [FINDITEM](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) SOAP recherche tous les éléments de la boîte de réception avec l’expression « plan Project » dans l’objet. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

L’exemple suivant montre la réponse du serveur avec les résultats de la recherche.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="712" MinorBuildNumber="22" Version="V2_3" 
        xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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
- [ExchangeService. FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)    
- [Opération FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    

