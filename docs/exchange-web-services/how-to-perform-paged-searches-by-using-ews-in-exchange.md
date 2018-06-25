---
title: Effectuer des recherches paginées à l’aide de EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 64ed70e4-32eb-4c25-bfc4-43d1477296e5
description: Découvrez comment effectuer des recherches paginées dans votre application EWS cible Exchange ou d’API managées.
ms.openlocfilehash: 3f82f46d0582b0b7ff8be63de8a7054b5f3cacab
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754922"
---
# <a name="perform-paged-searches-by-using-ews-in-exchange"></a>Effectuer des recherches paginées à l’aide de EWS dans Exchange

Découvrez comment effectuer des recherches paginées dans votre application EWS cible Exchange ou d’API managées.
  
Pagination est une fonctionnalité dans EWS qui vous permet de contrôler la taille des résultats d’une recherche. Au lieu d’extraire le jeu dans une réponse EWS de résultats, vous pouvez récupérer plus petits ensembles dans plusieurs réponses EWS. Par exemple, imaginons un utilisateur disposant de 10 000 messages électroniques dans leur boîte de réception. En théorie, vous pouvez récupérer tous les messages électroniques 10 000 dans une réponse de très grande taille, mais vous voudrez peut-être que diviser en segments plus facile à gérer pour des raisons de performances ou de la bande passante. Pagination vous offre les outils à cette fin.
  
> [!NOTE]
> Alors que vous pouvez récupérer théorie de 10 000 éléments dans une requête, en réalité, il s’agit probablement pas en raison de la limitation EWS. Pour plus d’informations, voir [limitation EWS dans Exchange](ews-throttling-in-exchange.md). 
  
**Le tableau 1. Paramètres de pagination dans les API managées EWS**

|**Pour configurer ou récupérer le...**|**Dans l’API managée EWS, utilisez...**|**Dans les services EWS, utilisez...**|
|:-----|:-----|:-----|
|Nombre maximal d’éléments ou des dossiers dans une réponse  <br/> |Le paramètre **pageSize** au [constructeur l’annonceAfficher](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemview.itemview%28v=exchg.80%29.aspx) l’ou le [constructeur FolderView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderview.folderview%28v=exchg.80%29.aspx) <br/> Or  <br/> La propriété [PagedView.PageSize](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.pagedview.pagesize%28v=exchg.80%29.aspx)  <br/> |L’attribut **MaxEntriesReturned** sur l’élément [IndexedPageItemView](http://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) ou l’élément [IndexedPageFolderView](http://msdn.microsoft.com/library/c6dac232-244b-4db0-9a15-5e01b8aa7a7d%28Office.15%29.aspx)  <br/> |
|Point de départ de la liste des éléments ou des dossiers  <br/> |Le paramètre **offsetBasePoint** au constructeur **l’annonceAfficher** l’ou le constructeur **FolderView**  <br/> Or  <br/> La propriété [PagedView.OffsetBasePoint](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.pagedview.offsetbasepoint%28v=exchg.80%29.aspx)  <br/> |L’attribut de **point de base** sur l’élément **IndexedPageItemView** ou l’élément **IndexedPageFolderView**  <br/> |
|Décalé du point de départ  <br/> |Le paramètre **offset** au constructeur **l’annonceAfficher** l’ou le constructeur **FolderView**  <br/> Or  <br/> La propriété [PagedView.Offset](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.pagedview.offset%28v=exchg.80%29.aspx)  <br/> |L’attribut **Offset** sur l’élément **IndexedPageItemView** ou l’élément **IndexedPageFolderView**  <br/> |
|Nombre total de résultats sur le serveur  <br/> |La propriété [FindItemsResults.TotalCount](http://msdn.microsoft.com/en-us/library/dd635348%28v=exchg.80%29.aspx) ou la propriété [FindFoldersResults.TotalCount](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.findfoldersresults.totalcount%28v=exchg.80%29.aspx)  <br/> |L’attribut **TotalItemsInView** sur l’élément [RootFolder (FindItemResponseMessage)](http://msdn.microsoft.com/library/187e009f-efaa-42a8-8962-329a645213ab%28Office.15%29.aspx) ou l’élément [RootFolder (FindFolderResponseMessage)](http://msdn.microsoft.com/library/5089c815-663f-46be-bc59-aed9ee20f94a%28Office.15%29.aspx)  <br/> |
|Décalage du premier élément ou un dossier non inclus dans la réponse en cours  <br/> |La propriété [FindItemsResults.NextPageOffset](http://msdn.microsoft.com/en-us/library/ee693014%28v=exchg.80%29.aspx) ou la propriété [FindFoldersResults.NextPageOffset](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.findfoldersresults.nextpageoffset%28v=exchg.80%29.aspx)  <br/> |L’attribut **IndexedPagingOffset** sur l’élément **RootFolder**  <br/> |
|Indicateur que réponse inclut le dernier élément ou le dossier dans la liste  <br/> |La propriété [FindItemsResults.MoreAvailable](http://msdn.microsoft.com/en-us/library/dd635477%28v=exchg.80%29.aspx) ou la propriété [FindFoldersResults.MoreAvailable](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.findfoldersresults.moreavailable%28v=exchg.80%29.aspx)  <br/> |L’attribut **IncludesLastItemInRange** sur l’élément **RootFolder**  <br/> |
   
## <a name="how-paging-works"></a>Fonctionne de la pagination
<a name="bk_HowPagingWorks"> </a>

Pour comprendre le fonctionne de la pagination, il est utile de visualiser les messages dans un dossier en tant que panneaux placés côte à côte dans un champ à l’extérieur de votre domicile. Vous pouvez voir certains de ces panneaux d’affichage dans une fenêtre magique. Vous avez la possibilité de modifier la taille de la fenêtre (pour voir plus ou moins de panneaux à la fois) et pour déplacer la fenêtre (pour contrôler les panneaux d’affichage que vous pouvez voir). Cette manipulation de la fenêtre est la pagination. 
  
Lorsque vous envoyez votre demande au serveur Exchange, vous spécifiez la taille de votre fenêtre en termes de nombre d’éléments à renvoyer. Vous définissez la position de la fenêtre en spécifiant un point de départ (le début de la ligne) ou la fin de la ligne et un décalage à partir de ce point de départ, exprimé en un nombre d’éléments. Le début de la fenêtre est le nombre d’éléments spécifié par le décalage du point de départ.
  
Où pagination Obtient un peu plus intéressante est dans la réponse du serveur, et comment votre application peut utiliser la réponse à la requête suivante de la forme. Le serveur fournit trois éléments d’information que vous pouvez utiliser pour déterminer comment configurer votre « fenêtre » pour votre requête suivante : 
  
- Si les résultats dans la réponse incluent le dernier élément dans le résultat global est défini sur le serveur.
    
- Nombre total d’éléments dans le jeu de résultats sur le serveur.
    
- Ce que la valeur de décalage suivante doit être, si vous souhaitez passer la fenêtre à l’élément suivant dans le jeu de résultats qui n’est pas inclus dans la réponse en cours.
    
Voici un exemple simple. Imaginez une boîte de réception avec 15 messages. Votre application envoie une demande initiale pour récupérer un maximum de 10 éléments, en commençant au début de la liste des messages (de sorte que le décalage est égale à zéro). Le serveur répond avec les 10 premiers messages et indique que la réponse n’inclut pas le dernier élément, qu’il n’y a un total de 15 éléments, et que le prochain offset doit être 10.
  
**La figure 1. Demande de 10 éléments au décalage de 0 à partir du début d’une liste de 15 éléments**

![Diagramme présentant les résultats d’une demande de 10 éléments au décalage de 0 à partir du début d’une liste de 15 éléments.](media/Ex15_PagedSearch_FirstPage.png)
  
Votre application puis renvoie la demande au serveur, avec le seul changement de même que le décalage est maintenant 10. Le serveur renvoie les cinq derniers éléments et indique que la réponse n’inclut pas le dernier élément, qu’il n’y a un total de 15 éléments, et que le prochain offset doit être 15 (bien évidemment, vous avez atteint la fin, il y un décalage suivant.)
  
**La figure 2. Demande de 10 éléments au décalage de 10 à partir du début d’une liste de 15 éléments**

![Diagramme présentant les résultats d’une demande de 10 éléments au décalage de 10 à partir du début d’une liste de 15 éléments.](media/Ex15_PagedSearch_SecondPage.png)
  
## <a name="design-considerations-for-paging"></a>Considérations de conception pour la pagination
<a name="bk_DesignConsiderations"> </a>

Tirer le meilleur parti pagination dans votre application nécessite en compte certains aspects. Par exemple, la taille en faire votre « fenêtre » ? Que faire si les résultats sur le serveur modifiez alors que vous déplacez votre « fenêtre » ?
  
### <a name="determine-the-size-of-your-window"></a>Déterminer la taille de votre fenêtre

Il n’existe aucune « unique » nombre maximal d’entrées que toutes les applications doivent utiliser. Détermination du nombre est un bon choix pour votre application dépend de plusieurs facteurs. Toutefois, il est utile à garder à l’esprit les instructions suivantes :
  
- Par défaut, Exchange limite le nombre maximal d’éléments pouvant être renvoyés dans une demande unique et 1000.
    
- Si le nombre maximal d’entrées à une plus grande entraîne numéro que vous ayez à envoyer des demandes de moins pour obtenir tous les éléments, au détriment de devoir attendre plus de réponses.
    
- Définir le nombre maximal d’entrées pour un plus petit nombre des résultats dans le temps de réponse plus rapides, au détriment de devoir envoyer plusieurs demandes pour obtenir tous les éléments.
    
### <a name="handling-changes-to-the-result-set"></a>Gestion des modifications apportées au jeu de résultats

Dans l’exemple simple plus haut dans cet article, le nombre d’éléments dans la boîte de réception de l’utilisateur est resté constant. Toutefois, en réalité, le nombre d’éléments dans une boîte de réception permettre changer fréquemment. Nouveaux messages peuvent arriver et les éléments peuvent être supprimés ou déplacés à tout moment. Mais comment cette pagination impact ? Nous allons modifier l’exemple de scénario permettant de savoir antérieur.
  
Nous allons commencer à nouveau les 15 éléments dans la boîte de réception et envoyer la demande initiale de même. Comme avant, le serveur répond avec les 10 premiers messages et indique que la réponse n’inclut pas le dernier élément, qu’il n’y a un total de 15 éléments, et que le prochain offset doit être 10, comme le montre la Figure 1.
  
À présent, alors que votre application traite les 10 éléments, un nouveau message arrive dans la boîte de réception et est ajouté pour le jeu de résultats sur le serveur. Votre application renvoie la même requête sur le serveur (uniquement avec le décalage est défini sur 10). Cette fois le serveur obtient en six éléments et indique qu’il n’y a un total de 16 éléments dans le jeu de résultats.
  
À ce stade vous vous demandez peut-être si c’est même un problème. Après tout, vous avez 16 éléments renvoyé sur les deux réponses, alors, pourquoi tous les tracas ? La réponse dépend où le nouvel élément est placé dans la liste. Si la liste est triée afin que les éléments les plus anciens (par date/heure de réception) sont d’abord, il n’existe aucun motif de préoccupation dans ce scénario. Le nouvel élément sera passé à la fin de la liste et doivent être inclus dans la seconde réponse.
  
**La figure 3. Demande de 10 éléments au décalage de 10 à partir du début d’une liste de 16 éléments, avec le 16e élément dans la liste en cours de nouveau**

![Diagramme présentant les résultats d’une demande de 10 éléments au décalage de 10 à partir du début d’une liste de 16 éléments quand le 16e élément a été ajouté à la fin de la liste.](media/Ex15_PagedSearch_SecondPage_NewItemEnd.png)
  
Si la liste est triée afin que les éléments les plus récents sont d’abord, il est un autre article. Dans ce cas, le premier élément de la deuxième demande serait le dernier élément de la requête précédente ainsi que les éléments restants cinq le 15 d’origine. Pour mettre en termes de notre fenêtre magique imaginaire, vous déplacés de votre fenêtre par 10, mais les panneaux eux-mêmes sont également déplacés par 1.
  
**La figure 4. Demande de 10 éléments au décalage de 10 à partir du début d’une liste de 16 éléments, avec le premier élément dans la liste en cours de nouveau**

![Diagramme présentant les résultats d’une demande de 10 éléments au décalage de 10 à partir du début d’une liste de 16 éléments lorsque le 16e élément a été ajouté au début de la liste.](media/Ex15_PagedSearch_SecondPage_NewItemBeginning.png)
  
Permet de détecter une modification dans les résultats sur le serveur consiste à utiliser le concept d’un élément d’ancrage. Un élément d’ancrage est un élément supplémentaire dans votre réponse qui n’est pas traitée avec le reste des résultats, mais sert à comparer avec les résultats suivantes pour voir si les éléments ont déplacé. Création de nouveau dans notre exemple, si votre application utilise une taille de « fenêtre » de 10, réellement définir le nombre maximal d’éléments à renvoyer à 11. Votre application traite les 10 premiers éléments dans la réponse comme d’habitude. Pour le dernier élément, enregistrez l’identificateur de l’élément comme point d’ancrage, puis publier la requête suivante avec un décalage de 10. Si les données n’a pas changé, le premier élément de la deuxième réponse doit avoir un identificateur d’élément qui correspond à l’ancrage. Si les identificateurs d’élément ne correspondent pas, vous savez que les données a été supprimées ou insérées dans les composants de la liste que vous avez déjà « paginée » sur.
  
Même lorsque vous savez que les données ont changé, vous devez toujours décider comment réagir. Il n’existe pas soit une réponse unique pour cette question. Vos actions dépend de la nature de votre application et elle est essentielle pour capturer tous les éléments. Vous pourrez ignorer complètement, redémarrez le processus à partir du début, ou sauvegarder le suivi et essayer de détecter où la modification a eu lieu.
  
## <a name="example-perform-a-paged-search-by-using-the-ews-managed-api"></a>Exemple : Effectuer une recherche paginée à l’aide de l’API managée EWS
<a name="bk_PagedSearchEWSMA"> </a>

Pagination est pris en charge par les méthodes API managées suivantes :
  
- [ExchangeService.FindFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx)
    
- [ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)
    
- [Folder.FindFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx)
    
- [Folder.FindFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)
    
Si vous utilisez l’API managée EWS, votre application configure pagination avec la classe [l’annonceAfficher](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemview%28v=exchg.80%29.aspx) l’ou [FolderView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderview%28v=exchg.80%29.aspx) et reçoit des informations à partir du serveur en ce qui concerne la pagination de la [FindItemsResults](http://msdn.microsoft.com/en-us/library/dd635381%28v=exchg.80%29.aspx) ou de [FindFoldersResults](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.findfoldersresults%28v=exchg.80%29.aspx) classe. 
  
L’exemple suivant récupère tous les éléments dans un dossier à l’aide d’une recherche paginée qui renvoie les cinq éléments dans chaque réponse. Elle récupère également un élément supplémentaire qui agira comme un point d’ancrage pour détecter les modifications apportées aux résultats sur le serveur. 
  
Cet exemple suppose que l’objet **ExchangeService** a été initialisée avec des valeurs valides dans les propriétés [d’Url](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) et les [informations d’identification](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) . 
  
```cs
using Microsoft.Exchange.WebServices.Data;
static void PageSearchItems(ExchangeService service, WellKnownFolderName folder)
{
    int pageSize = 5;
    int offset = 0;
    // Request one more item than your actual pageSize.
    // This will be used to detect a change to the result
    // set while paging.
    ItemView view = new ItemView(pageSize + 1, offset);
    view.PropertySet = new PropertySet(ItemSchema.Subject);
    view.OrderBy.Add(ItemSchema.DateTimeReceived, SortDirection.Descending);
    view.Traversal = ItemTraversal.Shallow;
    bool moreItems = true;
    ItemId anchorId = null;
    while (moreItems)
    {
        try
        {
            FindItemsResults<Item> results = service.FindItems(folder, view);
            moreItems = results.MoreAvailable;
            if (moreItems &amp;&amp; anchorId != null)
            {
                // Check the first result to make sure it matches
                // the last result (anchor) from the previous page.
                // If it doesn't, that means that something was added
                // or deleted since you started the search.
                if (results.Items.First<Item>().Id != anchorId)
                {
                    Console.WriteLine("The collection has changed while paging. Some results may be missed.");
                }
            }
            if (moreItems)
                view.Offset += pageSize;
            anchorId = results.Items.Last<Item>().Id;
            // Because you're including an additional item on the end of your results
            // as an anchor, you don't want to display it.
            // Set the number to loop as the smaller value between
            // the number of items in the collection and the page size.
            int displayCount = results.Items.Count > pageSize ? pageSize : results.Items.Count;
            for (int i = 0; i < displayCount; i++)
            {
                Item item = results.Items[i];
                Console.WriteLine("Subject: {0}", item.Subject);
                Console.WriteLine("Id: {0}\n", item.Id.ToString());
            }
        }
        catch (Exception ex)
        {
            Console.WriteLine("Exception while paging results: {0}", ex.Message);
        }
    }
}
```

## <a name="example-perform-a-paged-search-by-using-ews"></a>Exemple : Effectuer une recherche paginée à l’aide de EWS
<a name="bk_PagedSearchEWS"> </a>

Pagination est pris en charge par les opérations EWS suivantes :
  
- [FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)
    
- [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    
Si vous utilisez EWS, votre application configure pagination avec l’élément [IndexedPageItemView](http://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) ou l’élément [IndexedPageFolderView](http://msdn.microsoft.com/library/c6dac232-244b-4db0-9a15-5e01b8aa7a7d%28Office.15%29.aspx) et reçoit des informations à partir du serveur en ce qui concerne la pagination de la [(RootFolder FindItemResponseMessage)](http://msdn.microsoft.com/library/187e009f-efaa-42a8-8962-329a645213ab%28Office.15%29.aspx) élément ou l’élément [RootFolder (FindFolderResponseMessage)](http://msdn.microsoft.com/library/5089c815-663f-46be-bc59-aed9ee20f94a%28Office.15%29.aspx) . 
  
Dans cet exemple de requête, une demande **FindItem** est envoyée pour un maximum de six éléments, en commençant à un offset de zéro depuis le début de la liste des éléments dans la boîte de réception de l’utilisateur. 
  
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
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="6" Offset="0" BasePoint="Beginning" />
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox" />
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

Le serveur renvoie la réponse suivante, qui contient des éléments de six. La réponse indique également qu’il n’y a un total de huit articles dans les résultats sur le serveur, et que le dernier élément dans la liste des résultats n’est pas présent dans cette réponse.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="775" MinorBuildNumber="35" Version="V2_4" 
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
          <m:RootFolder IndexedPagingOffset="6" TotalItemsInView="8" IncludesLastItemInRange="false">
            <t:Items>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>Query</t:Subject>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>Update</t:Subject>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>Planning resources</t:Subject>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>Timeline</t:Subject>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>For your perusal</t:Subject>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>meeting notes</t:Subject>
              </t:Message>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>
```

Dans cet exemple, la même demande est envoyée, mais cette fois, l’attribut de **décalage** est modifiée à cinq, ce qui indique que le serveur doit renvoyer au maximum six éléments en commençant au décalage de cinq à partir du début. 
  
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
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="6" Offset="5" BasePoint="Beginning" />
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox" />
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

Le serveur envoie la réponse suivante, qui contient trois éléments. La réponse indique également que le nombre total d’éléments dans les résultats sur le serveur est toujours huit et que le dernier élément dans les résultats de la liste est incluse dans cette réponse.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="775" MinorBuildNumber="35" Version="V2_4" 
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
          <m:RootFolder IndexedPagingOffset="8" TotalItemsInView="8" IncludesLastItemInRange="true">
            <t:Items>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>meeting notes</t:Subject>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>Meeting notes</t:Subject>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>This cat is hilarious!</t:Subject>
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
    
- [Méthode ExchangeService.FindFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx)
    
- [Méthode ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)
    
- [Méthode Folder.FindFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx)
    
- [Méthode Folder.FindFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)
    
- [Opération FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)
    
- [Opération FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    
- [Limitation EWS dans Exchange](ews-throttling-in-exchange.md)
    

