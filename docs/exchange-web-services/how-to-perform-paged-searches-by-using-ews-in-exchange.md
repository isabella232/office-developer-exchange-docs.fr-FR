---
title: Effectuer des recherches paginées à l’aide d’EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 64ed70e4-32eb-4c25-bfc4-43d1477296e5
description: Découvrez comment effectuer des recherches paginées dans votre API managée EWS ou votre application EWS qui cible Exchange.
localization_priority: Priority
ms.openlocfilehash: 2b608584918c936f62883b8b444d59c05c5952ff
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456833"
---
# <a name="perform-paged-searches-by-using-ews-in-exchange"></a>Effectuer des recherches paginées à l’aide d’EWS dans Exchange

Découvrez comment effectuer des recherches paginées dans votre API managée EWS ou votre application EWS qui cible Exchange.
  
La pagination est une fonctionnalité d’EWS qui vous permet de contrôler la taille des résultats d’une recherche. Au lieu de récupérer l’intégralité du jeu de résultats dans une réponse EWS, vous pouvez récupérer des jeux plus petits dans plusieurs réponses EWS. Par exemple, imaginons qu’un utilisateur dispose de 10 000 messages électroniques dans sa boîte de réception. De manière hypothétique, vous pouviez extraire tous les courriers électroniques de 10 000 en une seule très grande réponse, mais vous pouvez le diviser en morceaux plus faciles à gérer pour des raisons de performances ou de bande passante. La pagination vous offre les outils qui vous permettent d’effectuer cette opération.
  
> [!NOTE]
> Bien que vous puissiez généralement extraire 10 000 éléments dans une demande, en réalité, cela est improbable en raison de la limitation EWS. Pour en savoir plus, reportez-vous à la rubrique [limitation EWS dans Exchange](ews-throttling-in-exchange.md). 
  
**Tableau 1. Paramètres de pagination dans l’API managée EWS et EWS**

|**Pour configurer ou récupérer le...**|**Dans l’API managée EWS, utilisez...**|**Dans EWS, utilisez...**|
|:-----|:-----|:-----|
|Nombre maximal d’éléments ou de dossiers dans une réponse  <br/> |Le paramètre **pageSize** vers le [constructeur objetitemview](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview.itemview%28v=exchg.80%29.aspx) ou le [constructeur folderview](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderview.folderview%28v=exchg.80%29.aspx) <br/> Ou  <br/> Propriété [PagedView. PageSize](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pagedview.pagesize%28v=exchg.80%29.aspx)  <br/> |Attribut **MaxEntriesReturned** de l’élément [IndexedPageItemView](https://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) ou de l’élément [IndexedPageFolderView](https://msdn.microsoft.com/library/c6dac232-244b-4db0-9a15-5e01b8aa7a7d%28Office.15%29.aspx)  <br/> |
|Point de départ dans la liste d’éléments ou de dossiers  <br/> |Le paramètre **offsetBasePoint** pour le constructeur **objetitemview** ou le constructeur **folderview**  <br/> Ou  <br/> Propriété [PagedView. OffsetBasePoint](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pagedview.offsetbasepoint%28v=exchg.80%29.aspx)  <br/> |Attribut **BasePoint** de l’élément **IndexedPageItemView** ou de l’élément **IndexedPageFolderView**  <br/> |
|Décalage depuis le point de départ  <br/> |Le paramètre **offset** pour le constructeur **objetitemview** ou le constructeur **folderview**  <br/> Ou  <br/> Propriété [PagedView. Offset](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pagedview.offset%28v=exchg.80%29.aspx)  <br/> |L’attribut **offset** sur l’élément **IndexedPageItemView** ou l’élément **IndexedPageFolderView**  <br/> |
|Nombre total de résultats sur le serveur  <br/> |La propriété [FindItemsResults. TotalCount](https://msdn.microsoft.com/library/dd635348%28v=exchg.80%29.aspx) ou la propriété [FindFoldersResults. TotalCount](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.findfoldersresults.totalcount%28v=exchg.80%29.aspx)  <br/> |L’attribut **TotalItemsInView** sur l’élément [RootFolder (FindItemResponseMessage)](https://msdn.microsoft.com/library/187e009f-efaa-42a8-8962-329a645213ab%28Office.15%29.aspx) ou l’élément [RootFolder (FindFolderResponseMessage)](https://msdn.microsoft.com/library/5089c815-663f-46be-bc59-aed9ee20f94a%28Office.15%29.aspx)  <br/> |
|Décalage du premier élément ou du dossier non inclus dans la réponse actuelle  <br/> |La propriété [FindItemsResults. NextPageOffset](https://msdn.microsoft.com/library/ee693014%28v=exchg.80%29.aspx) ou la propriété [FindFoldersResults. NextPageOffset](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.findfoldersresults.nextpageoffset%28v=exchg.80%29.aspx)  <br/> |Attribut **IndexedPagingOffset** de l’élément **RootFolder**  <br/> |
|Indicateur indiquant que la réponse inclut le dernier élément ou dossier de la liste  <br/> |La propriété [FindItemsResults. MoreAvailable](https://msdn.microsoft.com/library/dd635477%28v=exchg.80%29.aspx) ou la propriété [FindFoldersResults. MoreAvailable](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.findfoldersresults.moreavailable%28v=exchg.80%29.aspx)  <br/> |Attribut **IncludesLastItemInRange** de l’élément **RootFolder**  <br/> |
   
## <a name="how-paging-works"></a>Fonctionnement de la pagination
<a name="bk_HowPagingWorks"> </a>

Pour comprendre le fonctionnement de la pagination, il est utile de visualiser les messages d’un dossier sous forme de panneaux alignés côte à côte dans un champ extérieur à votre maison. Vous pouvez voir certains de ces panneaux dans une fenêtre magique. Vous avez la possibilité de modifier la taille de la fenêtre (pour afficher plus ou moins de panneaux d’affichage en même temps) et de déplacer la fenêtre (afin de contrôler les panneaux des panneaux que vous pouvez voir). Cette manipulation de la fenêtre est la pagination. 
  
Lorsque vous envoyez votre demande au serveur Exchange, vous spécifiez la taille de votre fenêtre en termes de nombre d’éléments à renvoyer. Vous définissez la position de la fenêtre en spécifiant un point de départ (au début de la ligne ou à la fin de la ligne) et un décalage par rapport à ce point de départ, exprimé par un certain nombre d’éléments. Le début de la fenêtre est le nombre d’éléments spécifié par le décalage à partir du point de départ.
  
Lorsque la pagination obtient un peu plus attrayant se trouve dans la réponse du serveur et comment votre application peut utiliser cette réponse pour adapter sa requête suivante. Le serveur vous fournit trois informations que vous pouvez utiliser pour déterminer la procédure à suivre pour configurer votre « fenêtre » pour votre prochaine requête : 
  
- Indique si les résultats dans la réponse incluent le dernier élément dans l’ensemble de résultats global sur le serveur.
    
- Nombre total d’éléments dans le jeu de résultats sur le serveur.
    
- La valeur de décalage suivante, si vous souhaitez faire avancer votre fenêtre à l’élément suivant dans le jeu de résultats qui n’est pas inclus dans la réponse actuelle.
    
Examinons un exemple simple. Imaginez une boîte de réception comportant 15 messages. Votre application envoie une demande initiale pour extraire un maximum de 10 éléments, en commençant au début de la liste des messages (de sorte que le décalage est égal à zéro). Le serveur répond avec les 10 premiers messages et indique que la réponse n’inclut pas le dernier élément, qu’il y a au total 15 éléments, et que le prochain décalage doit être de 10.
  
**Figure 1. Demande de 10 éléments au décalage 0 à partir du début d’une liste de 15 éléments**

![Diagramme présentant les résultats d’une demande de 10 éléments au décalage de 0 à partir du début d’une liste de 15 éléments.](media/Ex15_PagedSearch_FirstPage.png)
  
Votre application renvoie ensuite la même demande au serveur, avec la seule modification dont le décalage est désormais égal à 10. Le serveur renvoie les cinq derniers éléments, et indique que la réponse inclut le dernier élément, qu’il y a au total 15 éléments, et que le prochain décalage doit être 15 (bien entendu, vous avez atteint la fin, de sorte qu’il n’y aura pas de décalage suivant.)
  
**Figure 2. Demande de 10 éléments au décalage de 10 à partir du début d’une liste de 15 éléments**

![Diagramme présentant les résultats d’une demande de 10 éléments au décalage de 10 à partir du début d’une liste de 15 éléments.](media/Ex15_PagedSearch_SecondPage.png)
  
## <a name="design-considerations-for-paging"></a>Considérations relatives à la conception pour la pagination
<a name="bk_DesignConsiderations"> </a>

Pour tirer le meilleur parti de la pagination dans votre application, vous devez tenir compte de la nécessité. Par exemple, quelle est la taille de votre « fenêtre » ? Que faire si les résultats sur le serveur changent pendant que vous déplacez votre « fenêtre » ?
  
### <a name="determine-the-size-of-your-window"></a>Déterminer la taille de votre fenêtre

Il n’existe pas de nombre maximal d’entrées « à taille unique » que toutes les applications doivent utiliser. La détermination du nombre correct pour votre application dépend de plusieurs facteurs. Toutefois, il est utile de garder à l’esprit les instructions suivantes :
  
- Par défaut, Exchange limite le nombre maximal d’éléments qui peuvent être renvoyés dans une demande unique à 1000.
    
- Le fait de définir le nombre maximal d’entrées sur un nombre plus élevé entraîne l’envoi de moins de demandes pour obtenir tous les éléments, au coût de l’attente de réponses plus longues.
    
- Le fait de définir le nombre maximal d’entrées sur un nombre inférieur entraîne des temps de réponse plus rapides, au prix de l’envoi de demandes supplémentaires pour obtenir tous les éléments.
    
### <a name="handling-changes-to-the-result-set"></a>Gestion des modifications apportées au jeu de résultats

Dans l’exemple simple plus haut dans cet article, le nombre d’éléments dans la boîte de réception de l’utilisateur restait constant. Toutefois, en réalité, le nombre d’éléments dans une boîte de réception peut changer fréquemment. Les nouveaux messages peuvent arriver et les éléments peuvent être supprimés ou déplacés à tout moment. En quoi cela affecte-t-il la pagination ? Nous allons modifier l’exemple de scénario précédent pour le savoir.
  
Nous allons redémarrer avec les 15 éléments dans la boîte de réception de l’utilisateur, puis envoyer la même demande initiale. Comme précédemment, le serveur répond avec les 10 premiers messages et indique que la réponse n’inclut pas le dernier élément, qu’il y a un total de 15 éléments, et que le décalage suivant doit être de 10, comme illustré dans la figure 1.
  
Maintenant, pendant que votre application traite ces 10 éléments, un nouveau message arrive dans la boîte de réception et est ajouté au jeu de résultats sur le serveur. Votre application renvoie la même demande au serveur (uniquement avec le décalage défini sur 10). Cette fois, le serveur renvoie six éléments et indique qu’il y a au total 16 éléments dans le jeu de résultats.
  
À ce stade, vous vous demandez s’il s’agit d’un problème même. Après tout, vous avez 16 éléments sur les deux réponses, alors pourquoi tout ça ? La réponse dépend de l’emplacement du nouvel élément dans la liste. Si la liste est triée de façon à ce que les éléments les plus anciens (par date/heure de réception) soient les premiers, il n’y a aucune cause de préoccupation dans ce scénario. Le nouvel élément sera placé à la fin de la liste et sera inclus dans la deuxième réponse.
  
**Figure 3. Demande de 10 éléments au décalage de 10 à partir du début d’une liste de 16 éléments, avec le 16ème élément de la liste en cours de nouvelle**

![Diagramme présentant les résultats d’une demande de 10 éléments au décalage de 10 à partir du début d’une liste de 16 éléments quand le 16e élément a été ajouté à la fin de la liste.](media/Ex15_PagedSearch_SecondPage_NewItemEnd.png)
  
Si la liste est triée de sorte que les éléments les plus récents soient les premiers, il s’agit d’un autre article. Dans ce cas, le premier élément de la deuxième requête est le dernier élément de la requête précédente plus les cinq éléments restants du 15 initial. Pour le placer en tant que fenêtre magique imaginaire, vous avez déplacé la position de votre fenêtre de 10, mais les panneaux ont eux-mêmes également été décalés de 1.
  
**Figure 4. Demande de 10 éléments au décalage de 10 à partir du début d’une liste de 16 éléments, avec le premier élément de la liste en cours de nouvelle**

![Diagramme présentant les résultats d’une demande de 10 éléments au décalage de 10 à partir du début d’une liste de 16 éléments lorsque le 16e élément a été ajouté au début de la liste.](media/Ex15_PagedSearch_SecondPage_NewItemBeginning.png)
  
Pour détecter une modification apportée aux résultats sur le serveur, vous pouvez utiliser le concept d’un élément d’ancrage. Un élément d’ancrage est un élément supplémentaire de votre réponse qui n’est pas traité avec le reste des résultats, mais qui est utilisé pour comparer avec les résultats suivants pour voir si les éléments eux-mêmes ont été déplacés. Si votre application utilise une taille de 10, vous pouvez définir le nombre maximal d’éléments à 11, si votre application utilise une taille de « fenêtre ». Votre application traite les 10 premiers éléments de la réponse comme d’habitude. Pour le dernier élément, enregistrez l’identificateur de l’élément en tant qu’ancre, puis émettez la requête suivante avec un décalage de 10. Si les données n’ont pas été modifiées, le premier élément de la deuxième réponse doit avoir un identificateur d’élément correspondant à l’ancre. Si les identificateurs d’élément ne correspondent pas, cela signifie que les données ont été supprimées ou insérées dans les parties de la liste que vous avez déjà « paginée ».
  
Même si vous êtes conscient que les données ont été modifiées, vous devez toujours décider comment réagir. Il n’y a pas de réponse à une seule taille pour cette question. Vos actions dépendent de la nature de votre application et de l’importance de la capture de tous les éléments. Vous pouvez l’ignorer, redémarrez le processus depuis le début ou l’arrière et essayez de détecter où la modification s’est produite.
  
## <a name="example-perform-a-paged-search-by-using-the-ews-managed-api"></a>Exemple : effectuer une recherche paginée à l’aide de l’API managée EWS
<a name="bk_PagedSearchEWSMA"> </a>

La pagination est prise en charge par les méthodes d’API managée EWS suivantes :
  
- [ExchangeService. FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx)
    
- [ExchangeService. FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)
    
- [Folder. FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx)
    
- [Folder. FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)
    
Si vous utilisez l’API managée EWS, votre application configure la pagination à l’aide de la classe [objetitemview](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview%28v=exchg.80%29.aspx) ou [folderview](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderview%28v=exchg.80%29.aspx) et reçoit des informations du serveur concernant la pagination à partir de la classe [FindItemsResults](https://msdn.microsoft.com/library/dd635381%28v=exchg.80%29.aspx) ou [FindFoldersResults](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.findfoldersresults%28v=exchg.80%29.aspx) . 
  
L’exemple suivant récupère tous les éléments d’un dossier à l’aide d’une recherche paginée qui renvoie cinq éléments dans chaque réponse. Il extrait également un élément supplémentaire qui servira d’ancre pour détecter les modifications apportées aux résultats sur le serveur. 
  
Cet exemple part du principe que l’objet **ExchangeService** a été initialisé avec des valeurs valides dans les [informations d’identification](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) et les propriétés de l' [URL](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) . 
  
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

## <a name="example-perform-a-paged-search-by-using-ews"></a>Exemple : effectuer une recherche paginée à l’aide d’EWS
<a name="bk_PagedSearchEWS"> </a>

La pagination est prise en charge par les opérations EWS suivantes :
  
- [FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)
    
- [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    
Si vous utilisez EWS, votre application configure la pagination avec l’élément [IndexedPageItemView](https://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) ou l’élément [IndexedPageFolderView](https://msdn.microsoft.com/library/c6dac232-244b-4db0-9a15-5e01b8aa7a7d%28Office.15%29.aspx) et reçoit des informations du serveur concernant la pagination à partir de l’élément [RootFolder (FindItemResponseMessage)](https://msdn.microsoft.com/library/187e009f-efaa-42a8-8962-329a645213ab%28Office.15%29.aspx) ou de l’élément [RootFolder (FindFolderResponseMessage)](https://msdn.microsoft.com/library/5089c815-663f-46be-bc59-aed9ee20f94a%28Office.15%29.aspx) . 
  
Dans cet exemple de requête, une requête **FindItem** est envoyée pour un maximum de six éléments, en commençant à un offset de zéro à partir du début de la liste des éléments dans la boîte de réception de l’utilisateur. 
  
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

Le serveur renvoie la réponse suivante, qui contient six éléments. La réponse indique également qu’il y a au total huit éléments dans les résultats sur le serveur, et que le dernier élément de la liste des résultats n’est pas présent dans cette réponse.
  
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

Dans cet exemple, la même demande est envoyée, mais cette fois, l’attribut **offset** est remplacé par cinq, ce qui indique que le serveur doit renvoyer au plus six éléments en commençant au décalage cinq depuis le début. 
  
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

Le serveur envoie la réponse suivante, qui contient trois éléments. La réponse indique également que le nombre total d’éléments dans les résultats sur le serveur est toujours huit et que le dernier élément de la liste de résultats est inclus dans cette réponse.
  
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
    
- [Méthode ExchangeService. FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx)
    
- [Méthode ExchangeService. FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)
    
- [Méthode Folder. FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx)
    
- [Méthode Folder. FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)
    
- [Opération FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)
    
- [Opération FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    
- [Limitation EWS dans Exchange](ews-throttling-in-exchange.md)
    

