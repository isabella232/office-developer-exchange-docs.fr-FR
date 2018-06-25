---
title: Effectuer des recherches groupées à l’aide de EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 55de92eb-8e8b-4156-8ad9-dd3828024242
description: Découvrez comment effectuer des recherches groupées dans votre application EWS cible Exchange ou d’API managées.
ms.openlocfilehash: 63a796e2c724351c15287a5596a9a063954f8b40
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754919"
---
# <a name="perform-grouped-searches-by-using-ews-in-exchange"></a>Effectuer des recherches groupées à l’aide de EWS dans Exchange

Découvrez comment effectuer des recherches groupées dans votre application EWS cible Exchange ou d’API managées.
  
Recherches groupées sont utiles en ce sens qu’ils vous permet de contrôler l’affichage des résultats de recherche sont organisés. Résultats de la recherche organisé peuvent rendre plus facile pour votre application traiter les résultats ou les afficher à un utilisateur final d’une manière facile à gérer.
  
Le fait de placer tous les éléments qui ont la même valeur d’un champ spécifique dans un groupe dans le jeu de résultats de regroupement works. Par exemple, vous pouvez regrouper les résultats de l’expéditeur, tous les éléments de la même personne seront inclus dans un groupe séparé, et les éléments au sein de chaque groupe sont triés selon l’ordre que vous spécifiez dans l’affichage. Les groupes eux-mêmes sont triés par une valeur d’agrégation basée sur un champ que vous choisissez.
  
**Le tableau 1. Méthodes d’API managées et opérations EWS pour organiser les résultats de la recherche**

|**Si vous souhaitez...**|**Dans l’API managée EWS, utilisez...**|**Dans les services EWS, utilisez...**|
|:-----|:-----|:-----|
|Regrouper les éléments ayant la même valeur dans une propriété spécifique dans les résultats  <br/> |[Grouping.GroupOn](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.grouping.groupon%28v=exchg.80%29.aspx) <br/> |Élément [FieldURI](http://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) en tant qu’enfant de l’élément [Group](http://msdn.microsoft.com/library/9728619b-4674-4b9d-9f6c-e75c6165966c%28Office.15%29.aspx)  <br/> |
|Trier les éléments dans chaque groupe par la valeur dans une propriété spécifique  <br/> |[ItemView.OrderBy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemview.orderby%28v=exchg.80%29.aspx) <br/> |[SortOrder](http://msdn.microsoft.com/library/c2413f0b-8c03-46ae-9990-13338b3c53a6%28Office.15%29.aspx) , élément  <br/> |
|Trier les groupes  <br/> |[Grouping.AggregateOn](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.grouping.aggregateon%28v=exchg.80%29.aspx) <br/><br/> [Grouping.AggregateType](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.grouping.aggregatetype%28v=exchg.80%29.aspx) <br/><br/> [Grouping.SortDirection](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.grouping.sortdirection%28v=exchg.80%29.aspx) <br/> |Élément **FieldURI** en tant qu’enfant de l’élément [AggregateOn](http://msdn.microsoft.com/library/9b0a03f2-3282-46e1-b1a0-cbb9a0fbe9bb%28Office.15%29.aspx)<br/><br/> Attribut **d’agrégat** dans l’élément **AggregateOn**<br/><br/>Attribut de **commande** sur le **GroupBy,** élément  <br/> |
   
Prenons étape par étape.
  
## <a name="group-results-by-a-specific-property"></a>Regrouper des résultats par une propriété spécifique
<a name="bk_GroupResults"> </a>

La première étape à l’aide de regroupement consiste à sélectionner une propriété ou d’attribut sur les éléments de la banque d’informations Exchange, par lequel regrouper. L’API managée EWS expose en tant que propriétés de la classe sur les classes correspondantes, tandis que EWS les expose comme des éléments XML. Vous pouvez choisir de n’importe quelle propriété, y compris les propriétés personnalisées ou étendues, mais il est utile de comprendre comment les éléments sont regroupés en fonction de la valeur de la propriété que vous choisissez. 

Tous les éléments qui ont la même valeur dans la propriété que vous choisissez de regrouper sur vont être regroupés. Cela peut sembler évident, mais il s’agit d’un détail important. Prendre en compte que se passe-t-il si vous regroupez selon une propriété de date/heure, tels [Item.DateTimeReceived](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.datetimereceived%28v=exchg.80%29.aspx) dans l’API managée EWS ou l’élément [DateTimeReceived](http://msdn.microsoft.com/library/8f489bd4-2434-4d0a-91fe-1b5ba7eb5765%28Office.15%29.aspx) dans EWS. L’objectif est peut-être pour regrouper les résultats, avec chaque groupe contenant les éléments du même jour. Toutefois, regroupement ressemble à la valeur entière, qui inclut l’heure. 

Le résultat final est que les éléments sont regroupés afin que les éléments reçus en même temps, jusqu'à la seconde, se trouvent dans leurs propres groupes. Les résultats sont triés probablement dans un grand nombre de groupes avec un petit nombre d’éléments dans chaque groupe. 
  
Pour obtenir un jeu avec un plus petit nombre de groupes et un plus grand nombre d’éléments dans chaque groupe de résultats, choisissez une propriété qui est susceptible d’avoir un plus petit nombre de valeurs, telles que [EmailMessage.From](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.from%28v=exchg.80%29.aspx) ou [Item.Categories](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.categories%28v=exchg.80%29.aspx) dans l’API managée EWS, ou [à partir](http://msdn.microsoft.com/library/5a52d644-3677-4049-874c-12bd5c3080dc%28Office.15%29.aspx) de ou [catégories](http://msdn.microsoft.com/library/d84d4927-b524-4e62-bf3d-1f12fec8c21a%28Office.15%29.aspx) dans EWS. La figure suivante illustre une liste de messages électroniques qui apparaissent dans une boîte de réception. 
  
**La figure 1. Messages dans une boîte de réception**

![Exemple de liste de messages dans la boîte de réception d’un utilisateur.](media/Ex15_GroupedSearch_MsgList.png)
  
Si vous regroupez les éléments dans la Figure 1 par la propriété **EmailMessage.From** , le résultat sera deux groupes, un pour les messages envoyés par expédition brut et l’autre pour les messages envoyés par Sadie Daniels. 
  
**La figure 2. Messages séparés par des groupes en fonction de la propriété From**

![Image affichant des messages triés dans deux listes par la propriété From.](media/Ex15_GroupedSearch_SeparateGroups.png)
  
## <a name="sort-the-items-within-groups"></a>Trier les éléments dans des groupes
<a name="bk_SortItems"> </a>

Vous pouvez contrôler comment les éléments sont triés dans chaque groupe à l’aide de la propriété [ItemView.OrderBy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemview.orderby%28v=exchg.80%29.aspx) dans l’API managée EWS, ou l’élément [SortOrder](http://msdn.microsoft.com/library/c2413f0b-8c03-46ae-9990-13338b3c53a6%28Office.15%29.aspx) dans EWS. La même commande s’applique à chaque groupe. Par exemple, si vous triez les éléments de la Figure 1 par la propriété **Item.DateTimeReceived** , dans l’ordre décroissant, l’objet récemment reçu d’expédition brut apparaît en premier dans le groupe brut d’expédition et l’objet récemment reçu à partir de Sadie Daniels sera tout d’abord dans le groupe Sadie Daniels. Plus de commodité, les groupes dans la Figure 2 sont déjà triés de cette manière. 
  
## <a name="sort-the-groups"></a>Trier les groupes
<a name="bk_SortGroups"> </a>

Maintenant que vous disposez de vos groupes réglés, la dernière étape du tri les groupes eux-mêmes. Étant donné que les groupes eux-mêmes ont des valeurs spécifiques, le processus de regroupement doit affecter une valeur de tri à chaque groupe. Cela s’effectue par l’agrégation des valeurs d’une propriété spécifique au sein de chaque groupe, spécifiée par la propriété [Grouping.AggregateOn](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.grouping.aggregateon%28v=exchg.80%29.aspx) dans l’API managée EWS, ou de l’élément [FieldURI](http://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) en tant qu’enfant de l’élément [AggregateOn](http://msdn.microsoft.com/library/9b0a03f2-3282-46e1-b1a0-cbb9a0fbe9bb%28Office.15%29.aspx) dans EWS. La propriété [Grouping.AggregateType](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.grouping.aggregatetype%28v=exchg.80%29.aspx) dans l’API managée EWS (ou l’attribut **agrégation** sur l’élément **AggregateOn** dans EWS) spécifie la valeur à partir des éléments dans chaque groupe est affectée à la valeur de tri pour le groupe, soit le valeur la plus grande ou la plus petite valeur. Enfin, l’ordre de tri (par croissant ou décroissant) est spécifiée par la propriété [Grouping.SortDirection](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.grouping.sortdirection%28v=exchg.80%29.aspx) dans l’API managée EWS, ou l’attribut de **commande** sur l’élément [GroupBy](http://msdn.microsoft.com/library/9728619b-4674-4b9d-9f6c-e75c6165966c%28Office.15%29.aspx) dans EWS. 
  
Par exemple, si les groupes de la Figure 2 sont triés par l’agrégation de la propriété **Item.DateTimeReceived** , à l’aide de la plus petite valeur et le tri par ordre décroissant, les éléments sont retournés dans l’ordre indiqué Figure 3. 
  
**La figure 3. Résultats de recherche groupées et les groupes triés par la propriété DateTimeReceived**

![Image montrant une liste triée de messages, regroupés par la propriété From, avec les groupes triés en fonction de la date/heure de réception la plus récente.](media/Ex15_GroupedSearch_Results.png)
  
Les sections suivantes vous montrent comment vous pourrez extraire de regroupement et de tri ensemble dans le code.
  
## <a name="example-perform-a-grouped-search-by-using-the-ews-managed-api"></a>Exemple : Effectuer une recherche groupée à l’aide de l’API managée EWS
<a name="bk_GroupSearchEWSMA"> </a>

Les méthodes API managées suivantes peuvent utiliser le regroupement :
  
- [ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)
    
- [Folder.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)
    
L’exemple suivant utilise la méthode **ExchangeService.FindItems** ; Toutefois, les mêmes règles et concepts s’appliquent à la méthode **Folder.FindItems** . Dans cet exemple, une méthode appelée **GroupItemsByFrom** est définie. Il prend un objet [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) et un objet [WellKnownFolderName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) en tant que paramètres. Il demande les 50 premiers éléments dans le dossier, regroupés par la propriété **EmailMessage.From** , triée par la propriété **Item.DateTimeReceived** dans l’ordre décroissant. Les groupes eux-mêmes sont triés par la plus petite valeur de propriété **Item.DateTimeReceived** sur leurs éléments, dans l’ordre décroissant. 
  
Cet exemple suppose que l’objet **ExchangeService** a été initialisée avec des valeurs valides dans les propriétés [d’Url](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) et les [informations d’identification](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) . 
  
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

## <a name="example-perform-a-grouped-search-by-using-ews"></a>Exemple : Effectuer une recherche groupée à l’aide de EWS
<a name="bk_GroupSearchEWS"> </a>

L’exemple de requête suivante montre une demande [d’opération FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) pour les 50 premiers éléments dans le dossier, regroupée par l’élément **à partir de** , trié par l’élément **DateTimeReceived** dans l’ordre décroissant. Les groupes eux-mêmes sont triés par la plus petite valeur d’élément **DateTimeReceived** sur leurs éléments, dans l’ordre décroissant. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="712" MinorBuildNumber="22" Version="V2_3" 
        xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

Versions d’Exchange depuis la version majeure 15 et se terminant par build 15.0.775.38 **groupe** d’éléments à retourner (de type **GroupedItemsType**) à la place des éléments [GroupedItems](http://msdn.microsoft.com/library/53170df4-4272-4b37-b23f-cd8e2d4a7396%28Office.15%29.aspx) dans la réponse SOAP. Si vous utilisez l’API managée EWS, alors la collection [GroupedFindItemsResults.ItemGroups](http://msdn.microsoft.com/en-us/library/office/dd633961%28v=exchg.80%29.aspx) contenir les objets 0. Si vous utilisez EWS, éléments de **groupe** doivent être traités en tant qu’éléments **GroupedItems** . 
  
Versions d’Exchange depuis la version majeure 15 renvoient des éléments supplémentaires de **groupe** ou **GroupedItems** avec l’attribut **xsi : nil** a la valeur **true** dans la réponse SOAP. Si vous utilisez l’API managée EWS, ces éléments supplémentaires entraîne une [ServiceXmlDeserializationException](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.servicexmldeserializationexception%28v=exchg.80%29.aspx) levée. Si vous utilisez EWS, ces éléments supplémentaires doivent être ignorés. 
  
## <a name="see-also"></a>Voir aussi

- [Recherche et EWS dans Exchange](search-and-ews-in-exchange.md)    
- [ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)    
- [Folder.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)   
- [Classe de regroupement](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.grouping%28v=exchg.80%29.aspx)    
- [Opération FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    

