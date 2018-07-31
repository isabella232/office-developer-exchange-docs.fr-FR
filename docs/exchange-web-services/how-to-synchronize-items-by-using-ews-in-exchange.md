---
title: Synchroniser des éléments à l’aide de EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 886e7d35-9096-480b-8a8c-a7db27da06c2
description: Découvrez comment utiliser les API managées EWS pour obtenir une liste de tous les éléments dans un dossier ou une liste des modifications qui se sont produites dans un dossier, afin de synchroniser votre client.
ms.openlocfilehash: 8763c053463e4787741ef992ddb99d29be4192fc
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353783"
---
# <a name="synchronize-items-by-using-ews-in-exchange"></a><span data-ttu-id="3b53a-103">Synchroniser des éléments à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="3b53a-103">Synchronize items by using EWS in Exchange</span></span>

<span data-ttu-id="3b53a-104">Découvrez comment utiliser les API managées EWS pour obtenir une liste de tous les éléments dans un dossier ou une liste des modifications qui se sont produites dans un dossier, afin de synchroniser votre client.</span><span class="sxs-lookup"><span data-stu-id="3b53a-104">Find out how to use the EWS Managed API or EWS to get a list of all items in a folder, or a list of changes that have occurred in a folder, in order to synchronize your client.</span></span>
  
<span data-ttu-id="3b53a-105">EWS dans Exchange utilise l’option de synchronisation et la synchronisation du dossier au contenu de boîte aux lettres de synchronisation entre le client et le serveur.</span><span class="sxs-lookup"><span data-stu-id="3b53a-105">EWS in Exchange uses item synchronization and folder synchronization to sync mailbox content between the client and server.</span></span> <span data-ttu-id="3b53a-106">Synchronisation de l’élément obtient la liste initiale des éléments dans un dossier et puis, au fil du temps, les modifications qui ont été apportées à ces éléments et obtient ainsi que de nouveaux éléments.</span><span class="sxs-lookup"><span data-stu-id="3b53a-106">Item synchronization gets the initial list of items in a folder and then, over time, gets changes that have been made to those items and gets new items as well.</span></span>
  
<span data-ttu-id="3b53a-107">Notez qu’avant que vous pouvez synchroniser des éléments sur un client, vous devez d’abord [la hiérarchie de dossiers de synchronisation](how-to-synchronize-folders-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="3b53a-107">Note that before you can sync items to a client, you first have to [sync the folder hierarchy](how-to-synchronize-folders-by-using-ews-in-exchange.md).</span></span> <span data-ttu-id="3b53a-108">Une fois le dossier hiérarchie est en place sur le client, si vous effectuez une synchronisation de l’élément à l’aide de l’API managées, vous premier [obtenir la liste initiale des éléments dans la boîte de réception](#bk_cesyncongoingewsma) à l’aide de la méthode [ExchangeService.SyncFolderItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderitems%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="3b53a-108">After the folder hierarchy is in place on the client, if you're performing item synchronization by using the EWS Managed API, you first [get the initial list of items in the Inbox](#bk_cesyncongoingewsma) by using the [ExchangeService.SyncFolderItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderitems%28v=exchg.80%29.aspx) method.</span></span> <span data-ttu-id="3b53a-109">Ensuite, vous mettez à jour la valeur du paramètre _cSyncState_ lors des appels suivants pour obtenir la liste des éléments modifiés dans la boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="3b53a-109">You then update the value of the  _cSyncState_ parameter during subsequent calls to get the list of changed items in the Inbox.</span></span> 
  
<span data-ttu-id="3b53a-110">Pour effectuer une synchronisation de l’élément à l’aide de EWS, après la [synchronisation de la hiérarchie de dossiers](how-to-synchronize-folders-by-using-ews-in-exchange.md), vous demander la [liste initiale des éléments dans la boîte de réception](#bk_ewsexamplea) à l’aide de l' [opération SyncFolderItems](http://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx), analyse de la réponse, puis à un moment donné à l’avenir [ obtenir les modifications aux éléments dans la boîte aux lettres](#bk_ewsexamplec)et analyse de la réponse.</span><span class="sxs-lookup"><span data-stu-id="3b53a-110">To perform item synchronization by using EWS, after you [sync the folder hierarchy](how-to-synchronize-folders-by-using-ews-in-exchange.md), you request the [initial list of items in the Inbox](#bk_ewsexamplea) by using the [SyncFolderItems operation](http://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx), parse the response, and then at some point in the future [get the changes to the items in the mailbox](#bk_ewsexamplec), and parse the response.</span></span> <span data-ttu-id="3b53a-111">Une fois que le client reçoit la liste des éléments initiales ou modifiées, il [met à jour localement](#bk_nextsteps).</span><span class="sxs-lookup"><span data-stu-id="3b53a-111">After the client receives the list of initial or changed items, it [makes updates locally](#bk_nextsteps).</span></span> <span data-ttu-id="3b53a-112">Comment et quand vous récupérez les modifications à l’avenir varie selon le [modèle de conception de la synchronisation](mailbox-synchronization-and-ews-in-exchange.md#bk_syncpatterns) à l’aide de votre application.</span><span class="sxs-lookup"><span data-stu-id="3b53a-112">How and when you retrieve changes in the future depends on the [synchronization design pattern](mailbox-synchronization-and-ews-in-exchange.md#bk_syncpatterns) your application is using.</span></span> 
  
## <a name="get-the-list-of-all-items-or-changed-items-by-using-the-ews-managed-api"></a><span data-ttu-id="3b53a-113">Obtenir la liste de tous les éléments ou les éléments modifiés à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="3b53a-113">Get the list of all items or changed items by using the EWS Managed API</span></span>
<span data-ttu-id="3b53a-114"><a name="bk_cesyncongoingewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="3b53a-114"></span></span>

<span data-ttu-id="3b53a-115">L’exemple de code suivant montre comment obtenir une liste initiale de tous les éléments dans le dossier boîte de réception, puis obtenir une liste des modifications apportées aux éléments dans le dossier boîte de réception qui se sont produites depuis la dernière synchronisation.</span><span class="sxs-lookup"><span data-stu-id="3b53a-115">The following code example shows how to get an initial list of all items in the Inbox folder and then get a list of changes to items in the Inbox folder that have occurred since the previous synchronization.</span></span> <span data-ttu-id="3b53a-116">Pendant l’appel initial à la méthode [SyncFolderItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderitems%28v=exchg.80%29.aspx) , définissez la valeur de _cSyncState_ sur null.</span><span class="sxs-lookup"><span data-stu-id="3b53a-116">During the initial call to the [SyncFolderItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderitems%28v=exchg.80%29.aspx) method, set the  _cSyncState_ value to null.</span></span> <span data-ttu-id="3b53a-117">Lorsque la méthode est terminée, enregistrez la valeur _cSyncState_ localement à utiliser dans l’appel de méthode suivant **SyncFolderItems** .</span><span class="sxs-lookup"><span data-stu-id="3b53a-117">When the method completes, save the  _cSyncState_ value locally to use in the next **SyncFolderItems** method call.</span></span> <span data-ttu-id="3b53a-118">Dans l’appel initial et ultérieures, les éléments sont récupérés par lots de dix, à l’aide de la méthode **SyncFolderItems** , les appels successifs jusqu'à ce qu’il ne reste aucune modification.</span><span class="sxs-lookup"><span data-stu-id="3b53a-118">In both the initial call and the subsequent calls, the items are retrieved in batches of ten, by using successive calls to the **SyncFolderItems** method, until no more changes remain.</span></span> 
  
<span data-ttu-id="3b53a-119">Cet exemple définit le paramètre _propertySet_ à IdOnly afin de réduire les appels vers la base de données Exchange, qui est une [meilleure pratique de synchronisation](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices).</span><span class="sxs-lookup"><span data-stu-id="3b53a-119">This example sets the  _propertySet_ parameter to IdOnly to reduce calls to the Exchange database, which is a [synchronization best practice](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices).</span></span> <span data-ttu-id="3b53a-120">Dans cet exemple, nous partons du principe que **le service** est une liaison d’objet **ExchangeService** valide et que _cSyncState_ représente l’état de synchronisation qui a été renvoyée par un appel précédent à **SyncFolderItems**.</span><span class="sxs-lookup"><span data-stu-id="3b53a-120">In this example, we assume that **service** is a valid **ExchangeService** object binding and that  _cSyncState_ represents the sync state that was returned by a prior call to **SyncFolderItems**.</span></span> 
  
```cs
// Track whether there are more items available for download on the server.
bool moreChangesAvailable = false;
do
{
    // Get a list of all items in the Inbox by calling SyncFolderHierarchy repeatedly until no more changes are available.
    // The folderId parameter must be set to the root folder to synchronize,
    // and must be same folder ID as used in previous synchronization calls. 
    // The propertySet parameter is set to IdOnly to reduce calls to the Exchange database,
    // because any additional properties result in additional calls to the Exchange database. 
    // The ignoredItemIds parameter is set to null, so that no items are ignored.
    // The maxChangesReturned parameter is set to return a maximum of 10 items (512 is the maximum).
    // The syncScope parameter is set to Normal items, so that associated items will not be returned.
    // The syncState parameter is set to cSyncState, which should be null in the initial call, 
    // and should be set to the sync state returned by the 
    // previous SyncFolderItems call in subsequent calls.
    ChangeCollection<ItemChange> icc = service.SyncFolderItems(new FolderId(WellKnownFolderName.Inbox), PropertySet.IdOnly, null, 10, SyncFolderItemsScope.NormalItems, cSyncState);
    // If the count of changes is zero, there are no changes to synchronize.
    if (icc.Count == 0)
    {
        Console.WriteLine("There are no item changes to synchronize.");
    }
    // Otherwise, write all the changes included in the response 
    // to the console. 
    else
    {
        foreach (ItemChange ic in icc)
        {
            Console.WriteLine("ChangeType: " + ic.ChangeType.ToString());
            Console.WriteLine("ItemId: " + ic.ItemId);
            Console.WriteLine("===========");
        }
    }
    // Save the sync state for use in future SyncFolderContent requests.
    // The sync state is used by the server to determine what changes to report
    // to the client.
    string sSyncState = icc.SyncState;
   // Determine whether more changes are available on the server.
   moreChangesAvailable = icc.MoreChangesAvailable;
}
while (moreChangesAvailable);

```

La méthode **SyncFolderItems** est similaire à la méthode [FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) en ce sens qu’il ne peut pas renvoyer des propriétés telles que le [corps](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.body%28v=exchg.80%29.aspx) ou les [pièces jointes](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.attachments%28v=exchg.80%29.aspx). <span data-ttu-id="3b53a-122">Si vous avez besoin des propriétés qui ne peuvent pas être renvoyées par la méthode **SyncFolderItems** , spécifiez la propriété [IdOnly](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.propertyset.idonly%28v=exchg.80%29.aspx) lorsque vous appelez **SyncFolderItems**, puis utilisez la méthode [ExchangeService.LoadPropertiesForItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.loadpropertiesforitems%28v=exchg.80%29.aspx) pour obtenir le les propriétés que vous avez besoin pour les éléments qui ont été retournés par la méthode **SyncFolderItems** .</span><span class="sxs-lookup"><span data-stu-id="3b53a-122">If you need properties that cannot be returned by the **SyncFolderItems** method, specify the [IdOnly](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.propertyset.idonly%28v=exchg.80%29.aspx) property set when you call **SyncFolderItems**, and then use the [ExchangeService.LoadPropertiesForItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.loadpropertiesforitems%28v=exchg.80%29.aspx) method to get the properties you require for the items that were returned by the **SyncFolderItems** method.</span></span> 
  
<span data-ttu-id="3b53a-123">Après avoir extraire la liste des éléments nouveaux ou modifiés sur le serveur, [créer ou mettre à jour les éléments sur le client](#bk_nextsteps).</span><span class="sxs-lookup"><span data-stu-id="3b53a-123">After you retrieve the list of new or changed items on the server, [create or update the items on the client](#bk_nextsteps).</span></span>
  
## <a name="get-the-initial-list-of-items-by-using-ews"></a><span data-ttu-id="3b53a-124">Obtenir la liste initiale des éléments à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="3b53a-124">Get the initial list of items by using EWS</span></span>
<span data-ttu-id="3b53a-125"><a name="bk_ewsexamplea"> </a></span><span class="sxs-lookup"><span data-stu-id="3b53a-125"></span></span>

<span data-ttu-id="3b53a-126">L’exemple suivant montre la demande XML pour obtenir la liste initiale des éléments dans la boîte de réception à l’aide de l' [opération SyncFolderItems](http://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="3b53a-126">The following example shows the XML request to get the initial list of items in the Inbox by using the [SyncFolderItems operation](http://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx).</span></span> <span data-ttu-id="3b53a-127">Il s’agit de la demande XML que l’API managée EWS envoie quand également [récupérer la liste des éléments à l’aide de la méthode SyncFolderItems](#bk_cesyncongoingewsma).</span><span class="sxs-lookup"><span data-stu-id="3b53a-127">This is also the XML request that the EWS Managed API sends when [retrieving the list of items by using the SyncFolderItems method](#bk_cesyncongoingewsma).</span></span> <span data-ttu-id="3b53a-128">L’élément [SyncState](http://msdn.microsoft.com/library/e5ebaae3-0f07-481d-ac67-d9687a3c7ac3%28Office.15%29.aspx) de l’opération **SyncFolderItems** n’est pas inclus, car il s’agit de la synchronisation initiale.</span><span class="sxs-lookup"><span data-stu-id="3b53a-128">The [SyncState](http://msdn.microsoft.com/library/e5ebaae3-0f07-481d-ac67-d9687a3c7ac3%28Office.15%29.aspx) element of the **SyncFolderItems** operation is not included because this is the initial synchronization.</span></span> <span data-ttu-id="3b53a-129">Cet exemple définit l’élément [BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) **IdOnly** afin de réduire les appels vers la base de données Exchange, qui est une [meilleure pratique de synchronisation](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices).</span><span class="sxs-lookup"><span data-stu-id="3b53a-129">This example sets the [BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) element to **IdOnly** to reduce calls to the Exchange database, which is a [synchronization best practice](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices).</span></span>
  
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
    <m:SyncFolderItems>
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
      </m:ItemShape>
      <m:SyncFolderId>
        <t:DistinguishedFolderId Id="inbox" />
      </m:SyncFolderId>
      <m:MaxChangesReturned>10</m:MaxChangesReturned>
      <m:SyncScope>NormalItems</m:SyncScope>
    </m:SyncFolderItems>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="3b53a-130"><a name="bk_responsesyncfolderitems"> </a></span><span class="sxs-lookup"><span data-stu-id="3b53a-130"></span></span>

<span data-ttu-id="3b53a-131">L’exemple suivant montre la réponse XML renvoyée par le serveur une fois le traitement de la requête d’opération **SyncFolderItems** à partir du client.</span><span class="sxs-lookup"><span data-stu-id="3b53a-131">The following example shows the XML response that is returned by the server after it processes the **SyncFolderItems** operation request from the client.</span></span> <span data-ttu-id="3b53a-132">La première réponse inclut des éléments de [créer](http://msdn.microsoft.com/library/cb5e64a2-66a5-4447-921e-7c13efb8f6bf%28Office.15%29.aspx) des cinq éléments, car tous les éléments sont considérés comme nouveau lors d’une synchronisation initiale.</span><span class="sxs-lookup"><span data-stu-id="3b53a-132">The initial response includes [Create](http://msdn.microsoft.com/library/cb5e64a2-66a5-4447-921e-7c13efb8f6bf%28Office.15%29.aspx) elements for five items because all items are considered new during an initial synchronization.</span></span> <span data-ttu-id="3b53a-133">Les valeurs de certains attributs et éléments ont été raccourcies pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="3b53a-133">The values of some attributes and elements have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="785"
                         MinorBuildNumber="6"
                         Version="V2_6"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:SyncFolderItemsResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:SyncFolderItemsResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:SyncState>H4sIAAA==</m:SyncState>
          <m:IncludesLastItemInRange>true</m:IncludesLastItemInRange>
          <m:Changes>
            <t:Create>
              <t:Message>
                <t:ItemId Id="q04QAAAA=="
                          ChangeKey="CQAAABYAAABhFfgM7MNwSYx0VZ0GoBMJAAAATVdC"/>
              </t:Message>
            </t:Create>
            <t:Create>
              <t:Message>
                <t:ItemId Id="q07AAAAA=="
                          ChangeKey="CQAAABYAAABhFfgM7MNwSYx0VZ0GoBMJAAAATVdB"/>
              </t:Message>
            </t:Create>
            <t:Create>
              <t:Message>
                <t:ItemId Id="q1AwAAAA=="
                          ChangeKey="CQAAABYAAABhFfgM7MNwSYx0VZ0GoBMJAAAATVdA"/>
              </t:Message>
            </t:Create>
            <t:Create>
              <t:Message>
                <t:ItemId Id="AAMkADBh=="
                          ChangeKey="CQAAABYAAABhFfgM7MNwSYx0VZ0GoBMJAAAATVc5"/>
              </t:Message>
            </t:Create>
            <t:Create>
              <t:Message>
                <t:ItemId Id="AAMkADBh=="
                          ChangeKey="CQAAABYAAABhFfgM7MNwSYx0VZ0GoBMJAAAATVc4"/>
              </t:Message>
            </t:Create>
          </m:Changes>
        </m:SyncFolderItemsResponseMessage>
      </m:ResponseMessages>
    </m:SyncFolderItemsResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="3b53a-134">Après avoir extraire la liste des nouveaux éléments sur le serveur, [créer les éléments sur le client](#bk_nextsteps).</span><span class="sxs-lookup"><span data-stu-id="3b53a-134">After you retrieve the list of new items on the server, [create the items on the client](#bk_nextsteps).</span></span>
  
## <a name="get-the-changes-since-the-last-sync-by-using-ews"></a><span data-ttu-id="3b53a-135">Obtenir les modifications apportées depuis la dernière synchronisation à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="3b53a-135">Get the changes since the last sync by using EWS</span></span>
<span data-ttu-id="3b53a-136"><a name="bk_ewsexamplec"> </a></span><span class="sxs-lookup"><span data-stu-id="3b53a-136"></span></span>

<span data-ttu-id="3b53a-137">L’exemple suivant montre la demande XML pour obtenir la liste des modifications apportées aux éléments dans la boîte de réception à l’aide de l’opération [SyncFolderItems](http://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="3b53a-137">The following example shows the XML request to get the list of changes to items in the Inbox by using the [SyncFolderItems](http://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx) operation.</span></span> <span data-ttu-id="3b53a-138">Il s’agit de la demande XML que l’API managée EWS envoie quand également [récupérer la liste des modifications apportées à la boîte de réception](#bk_cesyncongoingewsma).</span><span class="sxs-lookup"><span data-stu-id="3b53a-138">This is also the XML request that the EWS Managed API sends when [retrieving the list of changes to the Inbox](#bk_cesyncongoingewsma).</span></span> <span data-ttu-id="3b53a-139">Cet exemple définit la valeur de l’élément [SyncState](http://msdn.microsoft.com/library/e5ebaae3-0f07-481d-ac67-d9687a3c7ac3%28Office.15%29.aspx) à la valeur renvoyée dans la [réponse précédente](#bk_responsesyncfolderitems).</span><span class="sxs-lookup"><span data-stu-id="3b53a-139">This example sets the [SyncState](http://msdn.microsoft.com/library/e5ebaae3-0f07-481d-ac67-d9687a3c7ac3%28Office.15%29.aspx) element value to the value returned in the [previous response](#bk_responsesyncfolderitems).</span></span> <span data-ttu-id="3b53a-140">Et à des fins de démonstration, cet exemple définit l’élément [BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) **AllProperties** au lieu **IdOnly** pour afficher les propriétés supplémentaires renvoyées.</span><span class="sxs-lookup"><span data-stu-id="3b53a-140">And for demonstration purposes, this example sets the [BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) element to **AllProperties** instead of **IdOnly** to show the additional properties returned.</span></span> <span data-ttu-id="3b53a-141">Définissez l’élément [BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) **IdOnly** est une [meilleure pratique de synchronisation](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices).</span><span class="sxs-lookup"><span data-stu-id="3b53a-141">Setting the [BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) element to **IdOnly** is a [synchronization best practice](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices).</span></span> <span data-ttu-id="3b53a-142">La valeur de **SyncState** a été raccourcie pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="3b53a-142">The value of **SyncState** has been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
      <t:RequestServerVersion Version="Exchange2010_SP2" />
  </soap:Header>
  <soap:Body>
    <m:SyncFolderItems>
      <m:ItemShape>
        <t:BaseShape>AllProperties</t:BaseShape>
      </m:ItemShape>
      <m:SyncFolderId>
        <t:DistinguishedFolderId Id="inbox" />
      </m:SyncFolderId>
      <m:SyncState>H4sIAAA==</m:SyncState>
      <m:MaxChangesReturned>10</m:MaxChangesReturned>
      <m:SyncScope>NormalItems</m:SyncScope>
    </m:SyncFolderItems>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="3b53a-143">L’exemple suivant montre la réponse XML renvoyée par le serveur une fois le traitement de la requête d’opération **SyncFolderItems** à partir du client.</span><span class="sxs-lookup"><span data-stu-id="3b53a-143">The following example shows the XML response that is returned by the server after it processes the **SyncFolderItems** operation request from the client.</span></span> <span data-ttu-id="3b53a-144">Cette réponse indique qu’un élément a été mis à jour, deux éléments ont été créés, l’indicateur de lecture d’un élément a été modifié et un élément a été supprimé depuis la synchronisation précédente.</span><span class="sxs-lookup"><span data-stu-id="3b53a-144">This response indicates that one item was updated, two items were created, the read flag of one item was changed, and one item was deleted since the prior synchronization.</span></span> <span data-ttu-id="3b53a-145">Les valeurs de certains attributs et éléments ont été raccourcies pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="3b53a-145">The values of some attributes and elements have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="731" MinorBuildNumber="10" Version="V2_3"
                 xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                 xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                 xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:SyncFolderItemsResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:SyncFolderItemsResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:SyncState>H4sIAAAAAAAEAO29B2AcSZY==</m:SyncState>
          <m:IncludesLastItemInRange>true</m:IncludesLastItemInRange>
          <m:Changes>
            <t:Update>
                <t:Message>
                  <t:ItemId Id="q04QAAAA==" ChangeKey="CQAAABYAAADZGACZQpSgSpyNkexYe2b7AAAAird/" />
                  <t:ParentFolderId Id=" AgENAAAA" ChangeKey="AQAAAA==" />
                  <t:ItemClass>IPM.Note</t:ItemClass>
                  <t:Subject>RE: Company Soccer Team</t:Subject>
                  <t:Sensitivity>Normal</t:Sensitivity>
                  <t:DateTimeReceived>2013-08-29T15:22:10Z</t:DateTimeReceived>
                  <t:Size>23110</t:Size>
                  <t:Importance>Normal</t:Importance>
                  <t:InReplyTo>&amp;lt;8e084ea1a5b64f97b95fa8a863a5869d@CH1SR01MB001.namsdf01.sdf.contoso.com&amp;gt;</t:InReplyTo>
                  <t:IsSubmitted>false</t:IsSubmitted>
                  <t:IsDraft>false</t:IsDraft>
                  <t:IsFromMe>false</t:IsFromMe>
                  <t:IsResend>false</t:IsResend>
                  <t:IsUnmodified>false</t:IsUnmodified>
                  <t:DateTimeSent>2013-08-29T15:22:10Z</t:DateTimeSent>
                  <t:DateTimeCreated>2013-08-28T04:07:38Z</t:DateTimeCreated>
                  <t:DisplayCc />
                  <t:DisplayTo>All Employees</t:DisplayTo>
                  <t:HasAttachments>false</t:HasAttachments>
                  <t:Culture>en-US</t:Culture>
                  <t:EffectiveRights>
                    <t:CreateAssociated>false</t:CreateAssociated>
                    <t:CreateContents>false</t:CreateContents>
                    <t:CreateHierarchy>false</t:CreateHierarchy>
                    <t:Delete>true</t:Delete>
                    <t:Modify>true</t:Modify>
                    <t:Read>true</t:Read>
                    <t:ViewPrivateItems>true</t:ViewPrivateItems>
                  </t:EffectiveRights>
                  <t:LastModifiedName>Mara  Whitley</t:LastModifiedName>
                  <t:LastModifiedTime>2013-08-28T16:53:35Z</t:LastModifiedTime>
                  <t:IsAssociated>false</t:IsAssociated>
                  <t:WebClientReadFormQueryString>?ae=Item&amp;amp;a=Open&amp;amp;t=IPM.Note&amp;amp;id=&amp;amp;exvsurl=1</t:WebClientReadFormQueryString>
                  <t:ConversationId Id="AAQkADkzNjJjODUzLWZhMDMtNDVkMS05ZDdjLWVmMDlkYjQ1Zjc4MwAQACAi+NTh0F5Eg5YDwpJsXPE=" />
                  <t:Sender>
                    <t:Mailbox>
                      <t:Name>Alfred  Welker </t:Name>
                      <t:EmailAddress>Alfred.Welker@contoso.com</t:EmailAddress>
                      <t:RoutingType>SMTP</t:RoutingType>
                      <t:MailboxType>Mailbox</t:MailboxType>
                    </t:Mailbox>
                  </t:Sender>
                  <t:IsReadReceiptRequested>false</t:IsReadReceiptRequested>
                  <t:ConversationIndex>AQHM5V/ZICL41OHQXkSDlgPCkmxc8ZYxA3I4gAAP5UeAANHpbIAAEE+0gAABYhSAACGYTIAAA2+vgAAE81qAkhv0Eg==</t:ConversationIndex>
                  <t:ConversationTopic>Company Soccer Team</t:ConversationTopic>
                  <t:From>
                    <t:Mailbox>
                      <t:Name>Alfred  Welker </t:Name>
                      <t:EmailAddress>Alfred.Welker@contoso.com</t:EmailAddress>
                      <t:RoutingType>SMTP</t:RoutingType>
                      <t:MailboxType>Mailbox</t:MailboxType>
                    </t:Mailbox>
                  </t:From>
                  <t:InternetMessageId>&amp;lt;e5919a09c8fc4d64b6ffd3542e194fc3@BY2SR01MB609.contoso.com&amp;gt;</t:InternetMessageId>
                  <t:IsRead>true</t:IsRead>
                  <t:References>namsdf01.sdf.contoso.com&amp;gt;</t:References>
                </t:Message>
            </t:Update>
            <t:Create>
              <t:Message>
                <t:ItemId Id="AQMkAD+" />
                <t:ParentFolderId Id="AQMkA==" ChangeKey="AQAAAA==" />
                <t:ItemClass>IPM.Note</t:ItemClass>
                  <t:Subject>RE: Review Proposal for Contoso</t:Subject>
                  <t:Sensitivity>Normal</t:Sensitivity>
                  <t:DateTimeReceived>2013-08-29T16:20:10Z</t:DateTimeReceived>
                  <t:Size>32515</t:Size>
                  <t:Importance>Normal</t:Importance>
                  <t:InReplyTo>&amp;lt;e52a4de6b98d484887e141da094a2ce6@SN2SR01MB006.contoso.com&amp;gt;</t:InReplyTo>
                  <t:IsSubmitted>false</t:IsSubmitted>
                  <t:IsDraft>false</t:IsDraft>
                  <t:IsFromMe>false</t:IsFromMe>
                  <t:IsResend>false</t:IsResend>
                  <t:IsUnmodified>false</t:IsUnmodified>
                  <t:DateTimeSent>2013-08-29T16:20:10Z</t:DateTimeSent>
                  <t:DateTimeCreated>2013-08-28T04:07:33Z</t:DateTimeCreated>
                  <t:DisplayCc />
                  <t:DisplayTo>Legal Team; Executives</t:DisplayTo>
                  <t:HasAttachments>false</t:HasAttachments>
                  <t:Culture>en-US</t:Culture>
                  <t:EffectiveRights>
                    <t:CreateAssociated>false</t:CreateAssociated>
                    <t:CreateContents>false</t:CreateContents>
                    <t:CreateHierarchy>false</t:CreateHierarchy>
                    <t:Delete>true</t:Delete>
                    <t:Modify>true</t:Modify>
                    <t:Read>true</t:Read>
                    <t:ViewPrivateItems>true</t:ViewPrivateItems>
                  </t:EffectiveRights>
                  <t:LastModifiedName>Mara  Whitley</t:LastModifiedName>
                  <t:LastModifiedTime>2013-08-28T04:07:35Z</t:LastModifiedTime>
                  <t:IsAssociated>false</t:IsAssociated>
                  <t:WebClientReadFormQueryString>?ae=Item&amp;amp;a=Open&amp;amp;t=IPM.Note&amp;amp;id=&amp;amp;exvsurl=1</t:WebClientReadFormQueryString>
                  <t:ConversationId Id="AAQkADkzNjJjODUzLWZhMDMtNDVkMS05ZDdjLWVmMDlkYjQ1Zjc4MwAQAIsBEZp25UpElByLLUQFH6Q=" />
                  <t:Sender>
                    <t:Mailbox>
                      <t:Name>Hope Gross</t:Name>
                      <t:EmailAddress>Hope.Gross@contoso.com</t:EmailAddress>
                      <t:RoutingType>SMTP</t:RoutingType>
                      <t:MailboxType>Mailbox</t:MailboxType>
                    </t:Mailbox>
                  </t:Sender>
                  <t:IsReadReceiptRequested>false</t:IsReadReceiptRequested>
                  <t:ConversationIndex>AQHM5WBRiwERmnblSkSUHIstRAUfpJYw9fbSgAAAdm2AAAB6koAAAHTDgAADl6+AAAbxCYAABm5PgAACSA+AANx034AAEKGQgAAAfsiAAB7m3IAABG+ngAABPZyAAASUzoAAA2DNgAAAfKE=</t:ConversationIndex>
                  <t:ConversationTopic>Review Proposal for Contoso</t:ConversationTopic>
                  <t:From>
                    <t:Mailbox>
                      <t:Name>Hope Gross</t:Name>
                      <t:EmailAddress>Hope.Gross@contoso.com</t:EmailAddress>
                      <t:RoutingType>SMTP</t:RoutingType>
                      <t:MailboxType>Mailbox</t:MailboxType>
                    </t:Mailbox>
                  </t:From>
                  <t:InternetMessageId>&amp;lt;bcdb185495834370a874a1e7ebedbb96@SN2SR01MB005.namsdf01.sdf.contoso.com&amp;gt;</t:InternetMessageId>
                  <t:IsRead>true</t:IsRead>
                  <t:References>&amp;lt;2d4d7d…</t:References>
                </t:Message>
              </t:Create>
              <t:Create>
                <t:Message>
                  <t:ItemId Id="Q04AAAAA==" ChangeKey="AAAirbnd" />
                  <t:ParentFolderId Id="AgENAAAA" ChangeKey="AQAAAA==" />
                  <t:ItemClass>IPM.Note</t:ItemClass>
                  <t:Subject>RE: Review Proposal for Contoso</t:Subject>
                  <t:Sensitivity>Normal</t:Sensitivity>
                  <t:DateTimeReceived>2013-08-29T15:30:10Z</t:DateTimeReceived>
                  <t:Size>29518</t:Size>
                  <t:Importance>Normal</t:Importance>
                  <t:InReplyTo>&amp;lt;f0db3ead01db4fe087d98022149aa16f@SN2SR01MB001.namsdf01.sdf.contoso.com&amp;gt;</t:InReplyTo>
                  <t:IsSubmitted>false</t:IsSubmitted>
                  <t:IsDraft>false</t:IsDraft>
                  <t:IsFromMe>false</t:IsFromMe>
                  <t:IsResend>false</t:IsResend>
                  <t:IsUnmodified>false</t:IsUnmodified>
                  <t:DateTimeSent>2013-08-29T15:30:10Z</t:DateTimeSent>
                  <t:DateTimeCreated>2013-08-28T04:07:36Z</t:DateTimeCreated>
                  <t:DisplayCc />
                  <t:DisplayTo>Legal Team; Executives</t:DisplayTo>
                  <t:HasAttachments>false</t:HasAttachments>
                  <t:Culture>en-US</t:Culture>
                  <t:EffectiveRights>
                    <t:CreateAssociated>false</t:CreateAssociated>
                    <t:CreateContents>false</t:CreateContents>
                    <t:CreateHierarchy>false</t:CreateHierarchy>
                    <t:Delete>true</t:Delete>
                    <t:Modify>true</t:Modify>
                    <t:Read>true</t:Read>
                    <t:ViewPrivateItems>true</t:ViewPrivateItems>
                  </t:EffectiveRights>
                  <t:LastModifiedName>Mara Whitley</t:LastModifiedName>
                  <t:LastModifiedTime>2013-08-28T04:07:38Z</t:LastModifiedTime>
                  <t:IsAssociated>false</t:IsAssociated>
                  <t:WebClientReadFormQueryString>?ae=Item&amp;amp;a=Open&amp;amp;t=IPM.Note&amp;amp;id=&amp;amp;exvsurl=1</t:WebClientReadFormQueryString>
                  <t:ConversationId Id="AAQkADkzNjJjODUzLWZhMDMtNDVkMS05ZDdjLWVmMDlkYjQ1Zjc4MwAQAIsBEZp25UpElByLLUQFH6Q=" />
                  <t:Sender>
                    <t:Mailbox>
                      <t:Name>Mack Chaves</t:Name>
                      <t:EmailAddress>Mack.Chaves@contoso.com</t:EmailAddress>
                      <t:RoutingType>SMTP</t:RoutingType>
                      <t:MailboxType>Mailbox</t:MailboxType>
                    </t:Mailbox>
                  </t:Sender>
                  <t:IsReadReceiptRequested>false</t:IsReadReceiptRequested>
                  <t:ConversationIndex>AQHM5WBRiwERmnblSkSUHIstRAUfpJYw9fbSgAAAdm2AAAB6koAAAHTDgAADl6+AAAbxCYAABm5PgAACSA+AANx034AAEKGQgAAAfsiAAB7m3IAABG+ngAABPZyAAASUzoAAA2DN</t:ConversationIndex>
                  <t:ConversationTopic>Review Proposal for Contoso</t:ConversationTopic>
                  <t:From>
                    <t:Mailbox>
                      <t:Name>Mack Chaves</t:Name>
                      <t:EmailAddress>Mack.Chaves@contoso.com</t:EmailAddress>
                      <t:RoutingType>SMTP</t:RoutingType>
                      <t:MailboxType>Mailbox</t:MailboxType>
                    </t:Mailbox>
                  </t:From>
                  <t:InternetMessageId>&amp;lt;e52a4de6b98d484887e141da094a2ce6@SN2SR01MB006.namsdf01.sdf.contoso.com&amp;gt;</t:InternetMessageId>
                  <t:IsRead>true</t:IsRead>
                  <t:References>namsdf01.sdf.contoso.com&amp;gt;</t:References>
                </t:Message>
              </t:Create>
              <t:ReadFlagChange>
                <t:ItemId Id=" q07AAAAA==" ChangeKey="CQAAAA==" />
                <t:IsRead>true</t:IsRead>
              </t:ReadFlagChange>
              <t:Delete>
                <t:ItemId Id=" q1AwAAAA==" ChangeKey="CQAAAA==" />
              </t:Delete>
          </m:Changes>
        </m:SyncFolderItemsResponseMessage>
      </m:ResponseMessages>
    </m:SyncFolderItemsResponse>
  </s:Body>
</s:Envelope>
```

L’opération **SyncFolderItems** est similaire à la méthode [FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) en ce sens qu’il ne peut pas renvoyer des éléments tels que les éléments du [corps](http://msdn.microsoft.com/library/7851ea9b-9f87-4adc-a26f-7a27df4a9bca%28Office.15%29.aspx) ou [pièces jointes](http://msdn.microsoft.com/library/b470e614-34bb-44f0-8790-7ddbdcbbd29d%28Office.15%29.aspx) . <span data-ttu-id="3b53a-147">Si vous avez besoin des propriétés qui ne peuvent pas être renvoyées à l’opération **SyncFolderItems** , définissez la valeur de l’élément [BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) pour IdOnly lorsque vous appelez **SyncFolderItems**, puis utilisez l' [opération GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) pour obtenir les propriétés vous demander pour les éléments qui ont été retournées par l’opération **SyncFolderItems** .</span><span class="sxs-lookup"><span data-stu-id="3b53a-147">If you need properties that cannot be returned by the **SyncFolderItems** operation, set the value of the [BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) element to IdOnly when you call **SyncFolderItems**, and then use the [GetItem operation](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) to get the properties you require for the items that were returned by the **SyncFolderItems** operation.</span></span> 
  
<span data-ttu-id="3b53a-148">Après avoir extraire la liste des éléments modifiés sur le serveur, [mettre à jour les éléments sur le client](#bk_nextsteps).</span><span class="sxs-lookup"><span data-stu-id="3b53a-148">After you retrieve the list of changed items on the server, [update the items on the client](#bk_nextsteps).</span></span>
  
## <a name="update-the-client"></a><span data-ttu-id="3b53a-149">Mise à jour du client</span><span class="sxs-lookup"><span data-stu-id="3b53a-149">Update the client</span></span>
<span data-ttu-id="3b53a-150"><a name="bk_nextsteps"> </a></span><span class="sxs-lookup"><span data-stu-id="3b53a-150"></span></span>

<span data-ttu-id="3b53a-151">Si vous utilisez l’API managée EWS, une fois que vous obtenez la liste des éléments nouveaux ou modifiés, utilisez la méthode [LoadPropertiesForItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.loadpropertiesforitems%28v=exchg.80%29.aspx) pour obtenir les propriétés sur les éléments nouveaux ou modifiés, comparez les propriétés aux valeurs locales et mettre à jour les éléments sur le client.</span><span class="sxs-lookup"><span data-stu-id="3b53a-151">If you're using the EWS Managed API, after you get the list of new or changed items, use the [LoadPropertiesForItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.loadpropertiesforitems%28v=exchg.80%29.aspx) method to get properties on the new or changed items, compare the properties to the local values, and update the items on the client.</span></span> 
  
<span data-ttu-id="3b53a-152">Si vous utilisez EWS, utilisez l' [opération GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) pour obtenir les propriétés sur les éléments nouveaux ou modifiés et mettre à jour les éléments sur le client.</span><span class="sxs-lookup"><span data-stu-id="3b53a-152">If you're using EWS, use the [GetItem operation](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) to get properties on the new or changed items and update the items on the client.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="3b53a-153">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="3b53a-153">See also</span></span>


- [<span data-ttu-id="3b53a-154">Synchronisation de la boîte aux lettres et les services EWS d'Exchange</span><span class="sxs-lookup"><span data-stu-id="3b53a-154">Mailbox synchronization and EWS in Exchange</span></span>](mailbox-synchronization-and-ews-in-exchange.md)
    
- [<span data-ttu-id="3b53a-155">Synchroniser les dossiers à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="3b53a-155">Synchronize folders by using EWS in Exchange</span></span>](how-to-synchronize-folders-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="3b53a-156">Gestion des erreurs liées à la synchronisation dans EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="3b53a-156">Handling synchronization-related errors in EWS in Exchange</span></span>](handling-synchronization-related-errors-in-ews-in-exchange.md)
    
- [<span data-ttu-id="3b53a-157">Abonnements à des notifications, événements de boîte aux lettres et EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="3b53a-157">Notification subscriptions, mailbox events, and EWS in Exchange</span></span>](notification-subscriptions-mailbox-events-and-ews-in-exchange.md)
    

