---
title: Effectuer des recherches groupées à l’aide d’EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 55de92eb-8e8b-4156-8ad9-dd3828024242
description: Découvrez comment effectuer des recherches groupées dans votre API managée EWS ou votre application EWS qui cible Exchange.
ms.openlocfilehash: 65c6f75ea6b8ab848a263349dcceceead52fa210
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527919"
---
# <a name="perform-grouped-searches-by-using-ews-in-exchange"></a>Effectuer des recherches groupées à l’aide d’EWS dans Exchange

Découvrez comment effectuer des recherches groupées dans votre API managée EWS ou votre application EWS qui cible Exchange.
  
Les recherches groupées sont utiles dans la mesure où elles vous permettent de contrôler la façon dont les résultats de la recherche sont organisés. Les résultats de la recherche organisés permettent à votre application de traiter plus facilement les résultats ou de les afficher à un utilisateur final de manière gérable.
  
Le regroupement consiste à placer tous les éléments dans le jeu de résultats qui ont la même valeur d’un champ spécifique dans un groupe. Par exemple, vous pouvez regrouper vos résultats par expéditeur et tous les éléments de la même personne se trouveront dans un groupe distinct, et les éléments de chaque groupe seront triés en fonction de l’ordre que vous spécifiez dans l’affichage. Les groupes eux-mêmes sont triés en fonction d’un champ que vous choisissez.
  
**Tableau 1. Méthodes de l’API managée EWS et opérations EWS pour organiser les résultats de la recherche**

|**Si vous souhaitez...**|**Dans l’API managée EWS, utilisez...**|**Dans EWS, utilisez...**|
|:-----|:-----|:-----|
|Organiser les éléments avec la même valeur dans une propriété spécifique de vos résultats dans des groupes  <br/> |[GROUPING. Groupon](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.grouping.groupon%28v=exchg.80%29.aspx) <br/> |Élément [FieldURI](https://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) en tant qu’enfant de l’élément [GroupBy](https://msdn.microsoft.com/library/9728619b-4674-4b9d-9f6c-e75c6165966c%28Office.15%29.aspx)  <br/> |
|Trier les éléments de chaque groupe par valeur dans une propriété spécifique  <br/> |[Objetitemview. OrderBy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview.orderby%28v=exchg.80%29.aspx) <br/> |[OrdreTri](https://msdn.microsoft.com/library/c2413f0b-8c03-46ae-9990-13338b3c53a6%28Office.15%29.aspx) , élément  <br/> |
|Trier les groupes  <br/> |[GROUPING. AggregateOn](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.grouping.aggregateon%28v=exchg.80%29.aspx) <br/><br/> [GROUPING. AggregateType](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.grouping.aggregatetype%28v=exchg.80%29.aspx) <br/><br/> [GROUPING. SortDirection](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.grouping.sortdirection%28v=exchg.80%29.aspx) <br/> |Élément **FieldURI** en tant qu’enfant de l’élément [AggregateOn](https://msdn.microsoft.com/library/9b0a03f2-3282-46e1-b1a0-cbb9a0fbe9bb%28Office.15%29.aspx)<br/><br/> Attribut **Aggregate** sur l’élément **AggregateOn**<br/><br/>Attribut **Order** sur l’élément **GroupBy**  <br/> |
   
Nous allons procéder étape par étape.
  
## <a name="group-results-by-a-specific-property"></a>Regrouper les résultats par une propriété spécifique
<a name="bk_GroupResults"> </a>

La première étape de l’utilisation du regroupement consiste à sélectionner une propriété, ou un attribut sur les éléments de la Banque d’aide Exchange, sur lequel effectuer le regroupement. L’API managée EWS expose ces propriétés en tant que propriétés de classe sur les classes correspondantes, tandis que EWS les expose en tant qu’éléments XML. Vous pouvez choisir n’importe quelle propriété, y compris des propriétés personnalisées ou étendues, mais il est utile de comprendre comment les éléments sont regroupés en fonction de la valeur de la propriété que vous choisissez. 

Tous les éléments qui ont la même valeur dans la propriété que vous choisissez de regrouper seront regroupés. Cela peut sembler évident, mais il s’agit d’un détail important. Examinez ce qui se passe si vous regroupez par une propriété de date/heure, telle que [Item. DateTimeReceived](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.datetimereceived%28v=exchg.80%29.aspx) dans l’API managée EWS ou l’élément [DateTimeReceived](https://msdn.microsoft.com/library/8f489bd4-2434-4d0a-91fe-1b5ba7eb5765%28Office.15%29.aspx) dans EWS. L’objectif peut être d’organiser les résultats en groupes, chaque groupe contenant des éléments du même jour. Toutefois, le regroupement examine l’ensemble de la valeur, ce qui inclut l’heure. 

Le résultat final est que les éléments seront groupés de sorte que les éléments reçus en même temps, jusqu’au second, soient dans leurs propres groupes. Les résultats seront probablement triés dans un grand nombre de groupes avec un petit nombre d’éléments dans chaque groupe. 
  
Pour obtenir un jeu de résultats avec un plus petit nombre de groupes et un plus grand nombre d’éléments dans chaque groupe, choisissez une propriété susceptible de contenir un plus petit nombre de valeurs, telles que [EmailMessage. from](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.from%28v=exchg.80%29.aspx) ou [Item. Categories](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.categories%28v=exchg.80%29.aspx) dans l’API managée EWS, ou [à partir de ou de](https://msdn.microsoft.com/library/5a52d644-3677-4049-874c-12bd5c3080dc%28Office.15%29.aspx) [catégories](https://msdn.microsoft.com/library/d84d4927-b524-4e62-bf3d-1f12fec8c21a%28Office.15%29.aspx) dans EWS. La figure suivante montre une liste des courriers électroniques qui apparaissent dans une boîte de réception. 
  
**Figure 1. Messages dans une boîte de réception**

![Exemple de liste de messages dans la boîte de réception d’un utilisateur.](media/Ex15_GroupedSearch_MsgList.png)
  
Si vous regroupez les éléments de la figure 1 par la propriété **EmailMessage. from** , le résultat sera deux groupes, un pour les messages envoyés par l’espoir brut et un pour les messages envoyés par Sadie Daniels. 
  
**Figure 2. Messages séparés en groupes en fonction de la propriété from**

![Image affichant des messages triés dans deux listes par la propriété From.](media/Ex15_GroupedSearch_SeparateGroups.png)
  
## <a name="sort-the-items-within-groups"></a>Trier les éléments dans des groupes
<a name="bk_SortItems"> </a>

Vous pouvez contrôler la façon dont les éléments sont triés dans chaque groupe à l’aide de la propriété [objetitemview. OrderBy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview.orderby%28v=exchg.80%29.aspx) de l’API managée EWS, ou de l’élément [SortOrder](https://msdn.microsoft.com/library/c2413f0b-8c03-46ae-9990-13338b3c53a6%28Office.15%29.aspx) dans EWS. Le même ordre s’applique à chaque groupe. Par exemple, si vous triez les éléments de la figure 1 à l’aide de la propriété **Item. DateTimeReceived** , dans l’ordre décroissant, le dernier élément reçu d’espoir brut sera le premier dans le groupe brut de l’espoir, et le dernier élément reçu de Sadie Daniels sera d’abord dans le groupe Sadie Daniels. De manière commode, les groupes de la figure 2 sont déjà triés de cette façon. 
  
## <a name="sort-the-groups"></a>Trier les groupes
<a name="bk_SortGroups"> </a>

À présent que vous avez réglé vos groupes, la dernière étape consiste à trier les groupes eux-mêmes. Étant donné que les groupes eux-mêmes n’ont pas de valeurs spécifiques, le processus de regroupement doit affecter une valeur de tri à chaque groupe. Cette opération est réalisée par agrégation des valeurs d’une propriété spécifique au sein de chaque groupe, spécifiée par la propriété [Grouping. AggregateOn](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.grouping.aggregateon%28v=exchg.80%29.aspx) dans l’API managée EWS ou l’élément [FieldURI](https://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) en tant qu’enfant de l’élément [AggregateOn](https://msdn.microsoft.com/library/9b0a03f2-3282-46e1-b1a0-cbb9a0fbe9bb%28Office.15%29.aspx) dans EWS. La propriété [Grouping. AggregateType](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.grouping.aggregatetype%28v=exchg.80%29.aspx) de l’API managée EWS (ou l’attribut **Aggregate** sur l’élément **AggregateOn** dans EWS) spécifie quelle valeur des éléments de chaque groupe est affectée à la valeur de tri du groupe, soit la plus grande valeur, soit la plus petite. Enfin, l’ordre de tri (décroissant ou croissant) est spécifié par la propriété [Grouping. SortDirection](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.grouping.sortdirection%28v=exchg.80%29.aspx) de l’API managée EWS ou l’attribut **Order** de l’élément [GroupBy](https://msdn.microsoft.com/library/9728619b-4674-4b9d-9f6c-e75c6165966c%28Office.15%29.aspx) dans EWS. 
  
Par exemple, si les groupes de la figure 2 sont triés par agrégation sur la propriété **Item. DateTimeReceived** , en utilisant la plus petite valeur et un tri par ordre décroissant, les éléments sont renvoyés dans l’ordre indiqué dans la figure 3. 
  
**Figure 3. Résultats de recherche groupés avec les groupes triés par la propriété DateTimeReceived**

![Image montrant une liste triée de messages, regroupés par la propriété From, avec les groupes triés en fonction de la date/heure de réception la plus récente.](media/Ex15_GroupedSearch_Results.png)
  
Les sections suivantes montrent comment vous pouvez extraire ensemble le regroupement et le tri dans le code.
  
## <a name="example-perform-a-grouped-search-by-using-the-ews-managed-api"></a>Exemple : effectuer une recherche groupée à l’aide de l’API managée EWS
<a name="bk_GroupSearchEWSMA"> </a>

Les méthodes d’API managée EWS suivantes peuvent utiliser le regroupement :
  
- [ExchangeService. FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)
    
- [Folder. FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)
    
L’exemple suivant utilise la méthode **ExchangeService. FindItems** ; Toutefois, les mêmes règles et concepts s’appliquent à la méthode **Folder. FindItems** . Dans cet exemple, une méthode appelée **GroupItemsByFrom** est définie. Il utilise un objet [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) et un objet [WellKnownFolderName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) comme paramètres. Il demande les premiers 50 éléments du dossier, groupés par la propriété **EmailMessage. from** , triée par la propriété **Item. DateTimeReceived** dans l’ordre décroissant. Les groupes sont triés par valeur de propriété **Item. DateTimeReceived** sur leurs éléments, par ordre décroissant. 
  
Cet exemple part du principe que l’objet **ExchangeService** a été initialisé avec des valeurs valides dans les [informations d’identification](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) et les propriétés de l' [URL](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) . 
  
```cs
static void GroupItemsByFrom(ExchangeService service, WellKnownFolderName folder)
{
    // Limit the result set to 50 items.
    ItemView view = new ItemView(50);
    view.PropertySet = new PropertySet(ItemSchema.Subject,
                                       ItemSchema.DateTimeReceived,
                                       EmailMessageSchema.From,
                                       ItemSchema.Categories);
    // Item searches do not support Deep traversal.
    view.Traversal = ItemTraversal.Shallow;
    // Specify the sorting done within the groups.
    view.OrderBy.Add(ItemSchema.DateTimeReceived, SortDirection.Descending);
    // Configure grouping.
    Grouping groupByFrom = new Grouping();
    groupByFrom.GroupOn = EmailMessageSchema.From;
    groupByFrom.AggregateOn = ItemSchema.DateTimeReceived;
    groupByFrom.AggregateType = AggregateType.Minimum;
    groupByFrom.SortDirection = SortDirection.Descending;
    try
    {
        GroupedFindItemsResults<Item> results = service.FindItems(folder,
            view, groupByFrom);
        foreach (ItemGroup<Item> group in results.ItemGroups)
        {
            Console.WriteLine("Group: {0}", group.GroupIndex);
            foreach (Item item in group.Items)
            {
                if (item is EmailMessage)
                {
                    EmailMessage message = item as EmailMessage;
                    Console.WriteLine("From: {0}", message.From);
                    Console.WriteLine("Subject: {0}", message.Subject);
                    Console.WriteLine("Id: {0}\n", message.Id.ToString());
                }
            }
        }
    }
    catch (Exception ex)
    {
        Console.WriteLine("Exception while enumerating results: {0}", ex.Message);
    }
}
```

## <a name="example-perform-a-grouped-search-by-using-ews"></a>Exemple : effectuer une recherche groupée à l’aide d’EWS
<a name="bk_GroupSearchEWS"> </a>

L’exemple de requête suivant montre une demande d' [opération FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) pour les premiers éléments 50 dans le dossier, regroupés par l’élément **from** , trié par l’élément **DateTimeReceived** dans l’ordre décroissant. Les groupes sont triés en fonction de la plus petite valeur de l’élément **DateTimeReceived** sur leurs éléments, dans l’ordre décroissant. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Eastern Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:FindItem Traversal="Shallow">
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
          <t:FieldURI FieldURI="item:DateTimeReceived" />
          <t:FieldURI FieldURI="message:From" />
          <t:FieldURI FieldURI="item:Categories" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="50" Offset="0" BasePoint="Beginning" />
      <m:GroupBy Order="Descending">
        <t:FieldURI FieldURI="message:From" />
        <t:AggregateOn Aggregate="Minimum">
          <t:FieldURI FieldURI="item:DateTimeReceived" />
        </t:AggregateOn>
      </m:GroupBy>
      <m:SortOrder>
        <t:FieldOrder Order="Descending">
          <t:FieldURI FieldURI="item:DateTimeReceived" />
        </t:FieldOrder>
      </m:SortOrder>
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox" />
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

Le serveur renvoie la réponse suivante.
  
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
    <m:FindItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="10" TotalItemsInView="8" IncludesLastItemInRange="true">
            <t:Groups>
              <t:GroupedItems>
                <t:GroupIndex>0</t:GroupIndex>
                <t:Items>
                  <t:Message>
                    <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                    <t:Subject>Planning resources</t:Subject>
                    <t:DateTimeReceived>2013-12-10T17:41:05Z</t:DateTimeReceived>
                    <t:From>
                      <t:Mailbox>
                        <t:Name>Sadie Daniels</t:Name>
                        <t:EmailAddress>/O=FIRST ORGANIZATION/OU=EXCHANGE ADMINISTRATIVE GROUP (FYDIBOHF23SPDLT)/CN=RECIPIENTS/CN=8D84A3F4CBB34D48838A3AECF99795C0-SADIE</t:EmailAddress>
                        <t:RoutingType>EX</t:RoutingType>
                      </t:Mailbox>
                    </t:From>
                  </t:Message>
                  <t:Message>
                    <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                    <t:Subject>Timeline</t:Subject>
                    <t:DateTimeReceived>2013-12-10T17:40:37Z</t:DateTimeReceived>
                    <t:Categories>
                      <t:String>Project</t:String>
                    </t:Categories>
                    <t:From>
                      <t:Mailbox>
                        <t:Name>Sadie Daniels</t:Name>
                        <t:EmailAddress>/O=FIRST ORGANIZATION/OU=EXCHANGE ADMINISTRATIVE GROUP (FYDIBOHF23SPDLT)/CN=RECIPIENTS/CN=8D84A3F4CBB34D48838A3AECF99795C0-SADIE</t:EmailAddress>
                        <t:RoutingType>EX</t:RoutingType>
                      </t:Mailbox>
                    </t:From>
                  </t:Message>
                  <t:Message>
                    <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                    <t:Subject>For your perusal</t:Subject>
                    <t:DateTimeReceived>2013-11-20T21:51:16Z</t:DateTimeReceived>
                    <t:From>
                      <t:Mailbox>
                        <t:Name>Sadie Daniels</t:Name>
                        <t:EmailAddress>/O=FIRST ORGANIZATION/OU=EXCHANGE ADMINISTRATIVE GROUP (FYDIBOHF23SPDLT)/CN=RECIPIENTS/CN=8D84A3F4CBB34D48838A3AECF99795C0-SADIE</t:EmailAddress>
                        <t:RoutingType>EX</t:RoutingType>
                      </t:Mailbox>
                    </t:From>
                  </t:Message>
                  <t:Message>
                    <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                    <t:Subject>meeting notes</t:Subject>
                    <t:DateTimeReceived>2013-11-20T21:18:51Z</t:DateTimeReceived>
                    <t:Categories>
                      <t:String>Blue category</t:String>
                    </t:Categories>
                    <t:From>
                      <t:Mailbox>
                        <t:Name>Sadie Daniels</t:Name>
                        <t:EmailAddress>/O=FIRST ORGANIZATION/OU=EXCHANGE ADMINISTRATIVE GROUP (FYDIBOHF23SPDLT)/CN=RECIPIENTS/CN=8D84A3F4CBB34D48838A3AECF99795C0-SADIE</t:EmailAddress>
                        <t:RoutingType>EX</t:RoutingType>
                      </t:Mailbox>
                    </t:From>
                  </t:Message>
                  <t:Message>
                    <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                    <t:Subject>Meeting notes</t:Subject>
                    <t:DateTimeReceived>2013-11-20T21:18:51Z</t:DateTimeReceived>
                    <t:From>
                      <t:Mailbox>
                        <t:Name>Sadie Daniels</t:Name>
                        <t:EmailAddress>/O=FIRST ORGANIZATION/OU=EXCHANGE ADMINISTRATIVE GROUP (FYDIBOHF23SPDLT)/CN=RECIPIENTS/CN=8D84A3F4CBB34D48838A3AECF99795C0-SADIE</t:EmailAddress>
                        <t:RoutingType>EX</t:RoutingType>
                      </t:Mailbox>
                    </t:From>
                  </t:Message>
                </t:Items>
              </t:GroupedItems>
              <t:GroupedItems>
                <t:GroupIndex>1</t:GroupIndex>
                <t:Items>
                  <t:Message>
                    <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                    <t:Subject>Query</t:Subject>
                    <t:DateTimeReceived>2013-12-10T17:43:15Z</t:DateTimeReceived>
                    <t:From>
                      <t:Mailbox>
                        <t:Name>Hope Gross</t:Name>
                        <t:EmailAddress>/O=FIRST ORGANIZATION/OU=EXCHANGE ADMINISTRATIVE GROUP (FYDIBOHF23SPDLT)/CN=RECIPIENTS/CN=9B55E4100C064D9D8C5F72FF36802ED3-HOPE</t:EmailAddress>
                        <t:RoutingType>EX</t:RoutingType>
                      </t:Mailbox>
                    </t:From>
                  </t:Message>
                  <t:Message>
                    <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                    <t:Subject>Update</t:Subject>
                    <t:DateTimeReceived>2013-12-10T17:42:33Z</t:DateTimeReceived>
                    <t:Categories>
                      <t:String>Project</t:String>
                      <t:String>Blue category</t:String>
                    </t:Categories>
                    <t:From>
                      <t:Mailbox>
                        <t:Name>Hope Gross</t:Name>
                        <t:EmailAddress>/O=FIRST ORGANIZATION/OU=EXCHANGE ADMINISTRATIVE GROUP (FYDIBOHF23SPDLT)/CN=RECIPIENTS/CN=9B55E4100C064D9D8C5F72FF36802ED3-HOPE</t:EmailAddress>
                        <t:RoutingType>EX</t:RoutingType>
                      </t:Mailbox>
                    </t:From>
                  </t:Message>
                  <t:Message>
                    <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                    <t:Subject>This cat is hilarious!</t:Subject>
                    <t:DateTimeReceived>2013-10-15T20:22:12Z</t:DateTimeReceived>
                    <t:From>
                      <t:Mailbox>
                        <t:Name>Hope Gross</t:Name>
                        <t:EmailAddress>/O=FIRST ORGANIZATION/OU=EXCHANGE ADMINISTRATIVE GROUP (FYDIBOHF23SPDLT)/CN=RECIPIENTS/CN=9B55E4100C064D9D8C5F72FF36802ED3-HOPE</t:EmailAddress>
                        <t:RoutingType>EX</t:RoutingType>
                      </t:Mailbox>
                    </t:From>
                  </t:Message>
                </t:Items>
              </t:GroupedItems>
            </t:Groups>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>
```

## <a name="version-differences"></a>Différences entre les versions
<a name="bk_VersionDiffs"> </a>

Les versions d’Exchange commençant par la version principale 15 et se terminant par Build 15.0.775.38 renvoient les éléments de **groupe** (de type **GroupedItemsType**) à la place des éléments [GroupedItems](https://msdn.microsoft.com/library/53170df4-4272-4b37-b23f-cd8e2d4a7396%28Office.15%29.aspx) dans la réponse SOAP. Si vous utilisez l’API managée EWS, la collection [GroupedFindItemsResults. ItemGroups](https://msdn.microsoft.com/library/office/dd633961%28v=exchg.80%29.aspx) doit contenir 0 objet. Si vous utilisez EWS, les éléments de **groupe** doivent être traités comme des éléments **GroupedItems** . 
  
Les versions d’Exchange commençant par la version principale 15 renvoient des éléments **Group** ou **GroupedItems** avec l’attribut **xsi : Nil** défini sur **true** dans la réponse SOAP. Si vous utilisez l’API managée EWS, ces éléments supplémentaires entraînent la levée d’une [ServiceXmlDeserializationException](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.servicexmldeserializationexception%28v=exchg.80%29.aspx) . Si vous utilisez EWS, ces éléments supplémentaires doivent être ignorés. 
  
## <a name="see-also"></a>Voir aussi

- [Recherche et EWS dans Exchange](search-and-ews-in-exchange.md)    
- [ExchangeService. FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)    
- [Folder. FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)   
- [Classe GROUPING](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.grouping%28v=exchg.80%29.aspx)    
- [Opération FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    

