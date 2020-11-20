---
title: Effectuer des recherches paginées à l’aide des services web Exchange (EWS) dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 64ed70e4-32eb-4c25-bfc4-43d1477296e5
description: Découvrez comment effectuer des recherches paginées dans votre API gérée EWS ou votre application EWS qui cible Exchange.
localization_priority: Priority
ms.openlocfilehash: fa36a2ce77150f29e5a62876138c9693a3b4ab1f
ms.sourcegitcommit: 37d4ecd4f469690ba1de87baad2f2f58c40c96ba
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49348821"
---
# <a name="perform-paged-searches-by-using-ews-in-exchange"></a>Effectuer des recherches paginées à l’aide des services web Exchange (EWS) dans Exchange

Découvrez comment effectuer des recherches paginées dans votre API gérée EWS ou votre application EWS qui cible Exchange.
  
La pagination est une fonctionnalité de EWS qui vous permet de contrôler la taille des résultats d’une recherche. Plutôt que de récupérer l’ensemble de résultats dans une seule réponse EWS, vous pouvez récupérer des ensembles plus petits dans plusieurs réponses EWS. Par exemple, prenons un utilisateur avec 10 000 e-mails dans sa boîte de réception. En théorie, vous pouvez récupérer les 10 000 e-mails en une seule réponse très volumineuse, mais vous voudrez peut-être diviser ces données en blocs plus gérables pour des raisons de bande passante ou de performances. La pagination vous donne les outils pour effectuer cette opération.
  
> [!NOTE]
> Bien que vous puissiez, en théorie, récupérer 10 000 éléments en une seule requête, cela est peu probable en réalité en raison de la limitation EWS. Si vous souhaitez en savoir plus, consultez l’article [Limitation EWS dans Exchange](ews-throttling-in-exchange.md). 
  
**Tableau 1. Paramètres de pagination dans l’API gérée EWS et EWS**

|**Pour configurer ou récupérer…**|**Dans l’API gérée EWS, utilisez…**|**Dans EWS, utilisez…**|
|:-----|:-----|:-----|
|Le nombre maximum d’éléments ou de dossiers dans une réponse  <br/> |Le paramètre **pageSize** du [constructeur ItemView](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview.itemview%28v=exchg.80%29.aspx) ou du [constructeur FolderView](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderview.folderview%28v=exchg.80%29.aspx) <br/> Ou  <br/> La propriété [PagedView.PageSize](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pagedview.pagesize%28v=exchg.80%29.aspx)  <br/> |L’attribut **MaxEntriesReturned** de l’élément [IndexedPageItemView](https://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) ou de l’élément [IndexedPageFolderView](https://msdn.microsoft.com/library/c6dac232-244b-4db0-9a15-5e01b8aa7a7d%28Office.15%29.aspx)  <br/> |
|Le point de départ dans la liste des éléments ou des dossiers  <br/> |Le paramètre **offsetBasePoint** du constructeur **ItemView** ou du constructeur **FolderView**   <br/> Ou  <br/> La propriété [PagedView.OffsetBasePoint](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pagedview.offsetbasepoint%28v=exchg.80%29.aspx)  <br/> |L’attribut **BasePoint** de l’élément **IndexedPageItemView** ou de l’élément **IndexedPageFolderView**  <br/> |
|Le décalage par rapport au point de départ  <br/> |Le paramètre **offset** du constructeur **ItemView** ou du constructeur **FolderView**  <br/> Ou  <br/> La propriété [PagedView.Offset](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pagedview.offset%28v=exchg.80%29.aspx)  <br/> |L’attribut **Offset** sur l’élément **IndexedPageItemView** ou l’élément **IndexedPageFolderView**  <br/> |
|Le nombre total de résultats sur le serveur  <br/> |La propriété [FindItemsResults.TotalCount](https://msdn.microsoft.com/library/dd635348%28v=exchg.80%29.aspx) ou la propriété [FindFoldersResults.TotalCount](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.findfoldersresults.totalcount%28v=exchg.80%29.aspx)  <br/> |L’attribut **TotalItemsInView** sur l’élément [RootFolder (FindItemResponseMessage)](https://msdn.microsoft.com/library/187e009f-efaa-42a8-8962-329a645213ab%28Office.15%29.aspx) ou sur l’élément [RootFolder (FindFolderResponseMessage)](https://msdn.microsoft.com/library/5089c815-663f-46be-bc59-aed9ee20f94a%28Office.15%29.aspx)  <br/> |
|Le décalage du premier élément ou dossier non inclus dans la réponse actuelle  <br/> |La [propriété FindItemsResults.NextPageOffset](https://msdn.microsoft.com/library/ee693014%28v=exchg.80%29.aspx) ou la propriété [FindFoldersResults.NextPageOffset](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.findfoldersresults.nextpageoffset%28v=exchg.80%29.aspx)  <br/> |L’attribut **IndexedPagingOffset** sur l’élément **RootFolder**  <br/> |
|L’indicateur indiquant que la réponse inclut le dernier élément ou dossier de la liste  <br/> |La propriété [FindItemsResults.MoreAvailable](https://msdn.microsoft.com/library/dd635477%28v=exchg.80%29.aspx) ou la propriété [FindFoldersResults.MoreAvailable](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.findfoldersresults.moreavailable%28v=exchg.80%29.aspx)  <br/> |L’attribut **includesLastItemInRange** sur l’élément **RootFolder**  <br/> |
   
## <a name="how-paging-works"></a>Fonctionnement de la pagination
<a name="bk_HowPagingWorks"> </a>

Pour comprendre le fonctionnement de la pagination, imaginez les messages dans un dossier comme des panneaux d’affichage alignés côte à côte dans un champ à l’extérieur de votre maison. Vous pouvez voir certains de ces panneaux à travers une fenêtre magique. Vous avez la possibilité de modifier la taille de la fenêtre (pour voir plus ou moins de panneaux d’affichage à la fois) et de déplacer la fenêtre (pour contrôler les panneaux d’affichage que vous pouvez voir). Cette manipulation de la fenêtre est une pagination. 
  
Lorsque vous envoyez votre demande au serveur Exchange, vous spécifiez la taille de votre fenêtre en termes de nombre d’éléments à renvoyer. Vous définissez la position de la fenêtre en spécifiant un point de départ (soit le début de la ligne, soit la fin de la ligne) et un décalage par rapport à ce point de départ, exprimé en nombre d’éléments. Le début de la fenêtre correspond au nombre d’éléments spécifié par le décalage par rapport au point de départ.
  
Là où la pagination devient un peu plus intéressante, c’est dans la réponse du serveur et dans la manière dont votre application peut utiliser cette réponse pour façonner sa prochaine requête. Le serveur vous donne trois informations que vous pouvez utiliser pour déterminer comment configurer votre « fenêtre » pour votre prochaine requête : 
  
- Indique si les résultats de la réponse incluent le dernier élément de l’ensemble de résultats global sur le serveur.
    
- Le nombre total d’éléments dans le jeu de résultats sur le serveur.
    
- Quelle devrait être la valeur de décalage suivante, si vous souhaitez faire avancer votre fenêtre vers l’élément suivant du jeu de résultats qui n’est pas inclus dans la réponse actuelle.
    
Prenons un exemple simple. Imaginez une boîte de réception contenant 15 messages. Votre application envoie une demande initiale pour récupérer un maximum de 10 éléments, en commençant au début de la liste des messages (le décalage est donc nul). Le serveur répond avec les 10 premiers messages et indique que la réponse n’inclut pas le dernier élément, qu’il y a un total de 15 éléments et que le décalage suivant doit être de 10.
  
**Figure 1. Demande de 10 éléments avec un décalage de 0 à partir du début d’une liste de 15 éléments**

![Diagramme présentant les résultats d’une demande de 10 éléments avec un décalage 0 à partir du début d’une liste de 15 éléments.](media/Ex15_PagedSearch_FirstPage.png)
  
Votre application renvoie ensuite la même demande au serveur, le seul changement étant que le décalage est désormais de 10. Le serveur renvoie les cinq derniers éléments et indique que la réponse inclut le dernier élément, qu’il y a un total de 15 éléments et que le prochain décalage devrait être de 15 (même si vous avez atteint la fin de la liste et qu’il n’y aura pas de prochain décalage).
  
**Figure 2. Demande de 10 éléments avec un décalage de 10 à partir du début d’une liste de 15 éléments**

![Diagramme présentant les résultats d’une demande de 10 éléments avec un décalage de 10 à partir du début d’une liste de 15 éléments.](media/Ex15_PagedSearch_SecondPage.png)
  
## <a name="design-considerations-for-paging"></a>Aspects de conception à prendre en compte pour la pagination
<a name="bk_DesignConsiderations"> </a>

Profiter du meilleur de la pagination dans votre application nécessite une certaine réflexion. Par exemple, quelle est la taille de votre « fenêtre » ? Que faites-vous si les résultats sur le serveur changent pendant que vous déplacez votre « fenêtre » ?
  
### <a name="determine-the-size-of-your-window"></a>Déterminer la taille de votre fenêtre

Il n’y a pas de nombre maximum d’entrées à « taille unique » que toutes les applications doivent utiliser. Déterminer le nombre qui convient à votre application dépend de plusieurs facteurs différents. Cependant, il est utile de garder à l’esprit les instructions suivantes :
  
- Par défaut, Exchange limite le nombre maximal d’éléments pouvant être retournés dans une seule demande à 1 000.
    
- Si vous définissez le nombre maximum d’entrées sur un nombre plus élevé, vous devez envoyer moins de demandes pour obtenir tous les éléments, mais vous devrez attendre plus longtemps pour obtenir les réponses.
    
- Si vous définissez le nombre maximum d’entrées sur un nombre plus petit, les réponses sont plus rapides, mais vous devrez envoyer plus de demandes pour obtenir tous les éléments.
    
### <a name="handling-changes-to-the-result-set"></a>Gérer les modifications du jeu de résultats

Dans l’exemple simple présenté au début de cet article, le nombre d’éléments dans la boîte de réception de l’utilisateur est resté constant. Toutefois, dans la réalité, le nombre d’éléments dans une boîte de réception peut changer fréquemment. De nouveaux messages peuvent arriver et les éléments peuvent être supprimés ou déplacés à tout moment. En quoi cela affecte-t-il la pagination ? Nous allons modifier l’exemple de scénario précédent pour le découvrir.
  
Nous allons recommencer avec les 15 éléments de la boîte de réception de l’utilisateur et allons envoyer la même demande initiale. Comme dans l’exemple précédent, le serveur répond avec les 10 premiers messages et indique que la réponse n’inclut pas le dernier élément, qu’il y a un total de 15 éléments et que le décalage suivant doit être de 10, comme le montre la figure 1.
  
Mais, pendant que votre application traite ces 10 éléments, un nouveau message arrive dans la boîte de réception et est ajouté au jeu de résultats sur le serveur. Votre application renvoie la même demande au serveur (uniquement avec le décalage défini sur 10). Cette fois, le serveur récupère six éléments et indique qu’il y a un total de 16 éléments dans le jeu de résultats.
  
À ce stade, vous vous demandez peut-être en quoi cela est un problème. Après tout, vous avez récupéré 16 éléments sur les deux réponses, alors pourquoi s’en faire ? La réponse dépend du placement du nouvel élément dans la liste. Si la liste est triée de manière à ce que les éléments les plus anciens (par date ou heure de réception) soient les premiers, il n’y a pas lieu de s’inquiéter dans ce scénario. Le nouvel élément sera placé à la fin de la liste et sera inclus dans la deuxième réponse.
  
**Figure 3. Demande de 10 éléments avec un décalage de 10 à partir du début d’une liste de 16 éléments, le 16e élément de la liste étant nouveau**

![Diagramme présentant les résultats d’une demande de 10 éléments avec un décalage de 10 à partir du début d’une liste de 16 éléments quand le 16e élément a été ajouté à la fin de la liste.](media/Ex15_PagedSearch_SecondPage_NewItemEnd.png)
  
Si la liste est triée de manière à ce que les éléments les plus récents soient les premiers, c’est une autre histoire. Dans ce cas, le premier élément de la deuxième demande serait le dernier élément de la demande précédente en plus des cinq éléments restants des 15 éléments d’origine. Pour reprendre l’image de notre fenêtre magique imaginaire, vous avez déplacé la position de votre fenêtre de 10, mais les panneaux d’affichage eux-mêmes ont également été décalés de 1.
  
**Figure 4. Demande de 10 éléments avec un décalage de 10 depuis le début d’une liste de 16 éléments, le premier élément de la liste étant nouveau**

![Diagramme présentant les résultats d’une demande de 10 éléments avec un décalage de 10 à partir du début d’une liste de 16 éléments lorsque le 16e élément a été ajouté au début de la liste.](media/Ex15_PagedSearch_SecondPage_NewItemBeginning.png)
  
Une façon de détecter une modification des résultats sur le serveur consiste à utiliser le concept d’élément d’ancrage. Un élément d’ancrage est un élément supplémentaire dans votre réponse qui n’est pas traité avec le reste des résultats, mais est utilisé pour effectuer une comparaison avec les résultats suivants pour voir si les éléments eux-mêmes ont changé. En se basant à nouveau sur notre exemple simple, si votre application utilise une taille de « fenêtre » de 10, vous définissez en fait le nombre maximum d’éléments à retourner sur 11. Votre application traite les 10 premiers éléments de la réponse comme d’habitude. Pour le dernier élément, vous enregistrez l’identifiant de l’élément en tant qu’ancre, puis émettez la demande suivante avec un décalage de 10. Si les données n’ont pas changé, le premier élément de la deuxième réponse doit avoir un identifiant d’élément qui correspond à l’ancre. Si les identificateurs d’élément ne correspondent pas, vous savez que les données ont été supprimées ou insérées dans les parties de la liste que vous avez déjà « paginées ».
  
Même lorsque vous savez que les données ont changé, vous devez quand même décider comment réagir. Il n’y a pas non plus de réponse universelle à cette question. Vos actions dépendront de la nature de votre application et de l’importance de capturer tous les éléments. Vous pouvez l’ignorer complètement, redémarrer le processus depuis le début ou revenir en arrière et essayer de détecter où le changement s’est produit.
  
## <a name="example-perform-a-paged-search-by-using-the-ews-managed-api"></a>Exemple : effectuer une recherche paginée à l’aide de l’API gérée EWS
<a name="bk_PagedSearchEWSMA"> </a>

La pagination est prise en charge par les méthodes de l’API gérée EWS suivantes :
  
- [ExchangeService.FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx)
    
- [ExchangeService.FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)
    
- [Folder.FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx)
    
- [Folder.FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)
    
Si vous utilisez l’API gérée EWS, votre application configure la pagination avec la classe [ItemView](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview%28v=exchg.80%29.aspx) ou la classe [FolderView](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderview%28v=exchg.80%29.aspx) et reçoit les informations du serveur concernant la pagination de la classe [FindItemsResults](https://msdn.microsoft.com/library/dd635381%28v=exchg.80%29.aspx) ou de la classe [FindFoldersResults](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.findfoldersresults%28v=exchg.80%29.aspx). 
  
L’exemple suivant récupère tous les éléments d’un dossier à l’aide d’une recherche paginée qui renvoie cinq éléments dans chaque réponse. Il récupère également un élément supplémentaire pour servir d’ancre afin de détecter les modifications des résultats sur le serveur. 
  
Cet exemple suppose que l’objet **ExchangeService** a été initialisé avec des valeurs valides dans les propriétés [Identifiants](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) et [Url](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx). 
  
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
            if (moreItems && anchorId != null)
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
            int displayCount = 0;
            if ((results.MoreAvailable == false && results.Items.Count > pageSize) || (results.Items.Count < pageSize))
            {
                displayCount = results.Items.Count;
            }
            else
            {
                displayCount = pageSize;
            }
            
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

## <a name="example-perform-a-paged-search-by-using-ews"></a>Exemple : effectuer une recherche paginée à l’aide de EWS
<a name="bk_PagedSearchEWS"> </a>

La pagination est prise en charge par les opérations EWS suivantes :
  
- [FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)
    
- [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    
Si vous utilisez EWS, votre application configure la pagination avec l’élément [IndexedPageItemView](https://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) ou l’élément [IndexedPageFolderView](https://msdn.microsoft.com/library/c6dac232-244b-4db0-9a15-5e01b8aa7a7d%28Office.15%29.aspx) et reçoit les informations du serveur concernant la pagination de l’élément [RootFolder (FindItemResponseMessage)](https://msdn.microsoft.com/library/187e009f-efaa-42a8-8962-329a645213ab%28Office.15%29.aspx) ou de l’élément [RootFolder (FindFolderResponseMessage)](https://msdn.microsoft.com/library/5089c815-663f-46be-bc59-aed9ee20f94a%28Office.15%29.aspx). 
  
Dans cet exemple de demande, une demande **FindItem** est envoyée pour un maximum de six éléments, en commençant avec un décalage de zéro à partir du début de la liste des éléments dans la boîte de réception de l’utilisateur. 
  
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

Le serveur renvoie la réponse suivante, qui contient six éléments. La réponse indique également qu’il y a un total de huit éléments dans les résultats sur le serveur et que le dernier élément de la liste de résultats n’est pas présent dans cette réponse.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="775" MinorBuildNumber="35" Version="V2_4" 
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

Dans cet exemple, la même demande est envoyée, mais cette fois, l’attribut **Offset** passe à cinq, ce qui indique que le serveur doit renvoyer au plus six éléments à partir du décalage de cinq depuis le début. 
  
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

Le serveur envoie la réponse suivante, qui contient trois éléments. La réponse indique également que le nombre total d’éléments dans les résultats sur le serveur est toujours de huit et que le dernier élément de la liste de résultats est inclus dans cette réponse.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="775" MinorBuildNumber="35" Version="V2_4" 
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
    
- [Méthode ExchangeService.FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx)
    
- [Méthode ExchangeService.FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)
    
- [Méthode Folder.FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx)
    
- [Méthode Folder.FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)
    
- [Opération FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)
    
- [Opération FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    
- [Limitation EWS dans Exchange](ews-throttling-in-exchange.md)
    

