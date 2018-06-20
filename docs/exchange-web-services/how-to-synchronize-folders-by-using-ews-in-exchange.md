---
title: Synchroniser les dossiers à l’aide de EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: d3bbacd1-8e4b-4fd0-8d27-4cbbc045ec3f
description: Découvrez comment utiliser les API managées EWS pour obtenir une liste de dossiers ou une liste de dossiers qui ont été modifiés, afin de synchroniser votre client.
ms.openlocfilehash: 4b0686134d642da34b2890a0e692e3d03e4a9fb1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19754950"
---
# <a name="synchronize-folders-by-using-ews-in-exchange"></a><span data-ttu-id="2bf3d-103">Synchroniser les dossiers à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="2bf3d-103">Synchronize folders by using EWS in Exchange</span></span>

<span data-ttu-id="2bf3d-104">Découvrez comment utiliser les API managées EWS pour obtenir une liste de dossiers ou une liste de dossiers qui ont été modifiés, afin de synchroniser votre client.</span><span class="sxs-lookup"><span data-stu-id="2bf3d-104">Find out how to use the EWS Managed API or EWS to get a list of folders, or a list of folders that have changed, in order to synchronize your client.</span></span>
  
<span data-ttu-id="2bf3d-105">EWS dans Exchange utilise l’option de synchronisation et la synchronisation du dossier au contenu de boîte aux lettres de synchronisation entre le client et le serveur.</span><span class="sxs-lookup"><span data-stu-id="2bf3d-105">EWS in Exchange uses item synchronization and folder synchronization to sync mailbox content between the client and server.</span></span> <span data-ttu-id="2bf3d-106">La synchronisation du dossier Obtient la liste initiale des dossiers à partir d’un dossier racine et obtient ensuite, au fil du temps, les modifications qui ont été apportées à ces dossiers et ainsi que de nouveaux dossiers.</span><span class="sxs-lookup"><span data-stu-id="2bf3d-106">Folder synchronization gets the initial list of folders from a root folder and then, over time, gets changes that were made to those folders and gets new folders as well.</span></span>
  
<span data-ttu-id="2bf3d-107">Si vous effectuez une synchronisation de dossiers à l’aide de l’API managées, vous premier [obtenir la liste initiale des dossiers dans le dossier racine](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncinitialewsma) à l’aide de la méthode [ExchangeService.SyncFolderHierarchy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderhierarchy%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="2bf3d-107">If you're performing folder synchronization by using the EWS Managed API, you first [get the initial list of folders in the root folder](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncinitialewsma) by using the [ExchangeService.SyncFolderHierarchy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderhierarchy%28v=exchg.80%29.aspx) method.</span></span> <span data-ttu-id="2bf3d-108">Ensuite, vous mettez à jour la valeur du paramètre _cSyncState_ lors des appels suivants pour obtenir la liste des dossiers de nouvelles et modifiées.</span><span class="sxs-lookup"><span data-stu-id="2bf3d-108">You then update the value of the  _cSyncState_ parameter during subsequent calls to get the list of new and changed folders.</span></span> 
  
<span data-ttu-id="2bf3d-109">Pour effectuer la synchronisation de dossiers à l’aide de EWS, vous demandez la [liste initiale des dossiers dans le dossier racine](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncewsrequest) à l’aide de l’opération [SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) , analyse de la réponse et ensuite à un moment donné à l’avenir [Obtenez les modifications dans les dossiers la racine](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncrespews)et analyse de la réponse.</span><span class="sxs-lookup"><span data-stu-id="2bf3d-109">To perform folder synchronization by using EWS, you request the [initial list of folders in the root folder](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncewsrequest) by using the [SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) operation, parse the response, and then at some point in the future [get the changes to the folders in the root](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncrespews), and parse the response.</span></span> <span data-ttu-id="2bf3d-110">Une fois que le client reçoit la liste de dossiers initiales ou modifiées, il [met à jour localement](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_nextsteps).</span><span class="sxs-lookup"><span data-stu-id="2bf3d-110">After the client receives the list of initial or changed folders, it [makes updates locally](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_nextsteps).</span></span> <span data-ttu-id="2bf3d-111">Comment et quand vous récupérez les modifications à l’avenir varie selon le [modèle de conception de la synchronisation](mailbox-synchronization-and-ews-in-exchange.md#bk_syncpatterns) à l’aide de votre application.</span><span class="sxs-lookup"><span data-stu-id="2bf3d-111">How and when you retrieve changes in the future depends on the [synchronization design pattern](mailbox-synchronization-and-ews-in-exchange.md#bk_syncpatterns) your application is using.</span></span> 
  
## <a name="get-the-list-of-all-folders-or-changed-folders-by-using-the-ews-managed-api"></a><span data-ttu-id="2bf3d-112">Obtenir la liste de tous les dossiers ou les dossiers modifiés à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="2bf3d-112">Get the list of all folders or changed folders by using the EWS Managed API</span></span>
<span data-ttu-id="2bf3d-113"><a name="bk_cesyncinitialewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="2bf3d-113"></span></span>

<span data-ttu-id="2bf3d-114">L’exemple de code suivant montre comment obtenir une liste initiale des dossiers dans un dossier racine, puis obtenir une liste des modifications apportées aux dossiers dans le dossier racine qui se sont produites depuis la dernière synchronisation.</span><span class="sxs-lookup"><span data-stu-id="2bf3d-114">The following code example shows how to get an initial list of folders in a root folder and then get a list of changes to folders in the root folder that have occurred since the previous synchronization.</span></span> <span data-ttu-id="2bf3d-115">Pendant l’appel initial à la méthode [ExchangeService.SyncFolderHierarchy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderhierarchy%28v=exchg.80%29.aspx) , définissez la valeur de _cSyncState_ sur null.</span><span class="sxs-lookup"><span data-stu-id="2bf3d-115">During the initial call to the [ExchangeService.SyncFolderHierarchy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderhierarchy%28v=exchg.80%29.aspx) method, set the  _cSyncState_ value to null.</span></span> <span data-ttu-id="2bf3d-116">Lorsque la méthode est terminée, enregistrez la valeur _cSyncState_ localement à utiliser dans l’appel de méthode suivant **SyncFolderHierarchy** .</span><span class="sxs-lookup"><span data-stu-id="2bf3d-116">When the method completes, save the  _cSyncState_ value locally to use in the next **SyncFolderHierarchy** method call.</span></span> <span data-ttu-id="2bf3d-117">Dans l’appel initial et ultérieures, les dossiers sont récupérés par lots de dix, à l’aide de la méthode **SyncFolderHierarchy** , les appels successifs jusqu'à ce qu’il ne reste aucune modification.</span><span class="sxs-lookup"><span data-stu-id="2bf3d-117">In both the initial call and the subsequent calls, the folders are retrieved in batches of ten, by using successive calls to the **SyncFolderHierarchy** method, until no more changes remain.</span></span> <span data-ttu-id="2bf3d-118">Cet exemple définit le paramètre _propertySet_ à IdOnly afin de réduire les appels vers la base de données Exchange, qui est une [meilleure pratique de synchronisation](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices).</span><span class="sxs-lookup"><span data-stu-id="2bf3d-118">This example sets the  _propertySet_ parameter to IdOnly to reduce calls to the Exchange database, which is a [synchronization best practice](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices).</span></span> <span data-ttu-id="2bf3d-119">Dans cet exemple, nous partons du principe que **le service** est une liaison d’objet **ExchangeService** valide et que _cSyncState_ représente l’état de synchronisation qui a été renvoyée par un appel précédent à **SyncFolderHierarchy**.</span><span class="sxs-lookup"><span data-stu-id="2bf3d-119">In this example, we assume that **service** is a valid **ExchangeService** object binding and that  _cSyncState_ represents the sync state that was returned by a prior call to **SyncFolderHierarchy**.</span></span> 
  
```cs
// Get a list of all folders in the mailbox by calling SyncFolderHierarchy.
// The folderId parameter must be set to the root folder to synchronize. 
// The propertySet parameter is set to IdOnly to reduce calls to the Exchange database
// because any additional properties result in additional calls to the Exchange database. 
// The syncState parameter is set to cSyncState, which should be null in the initial call, 
// and should be set to the sync state returned by the previous SyncFolderHierarchy call 
// in subsequent calls.
ChangeCollection<FolderChange> fcc = service.SyncFolderHierarchy(new FolderId(WellKnownFolderName.Root), PropertySet.IdOnly, cSyncState);
// If the count of changes is zero, there are no changes to synchronize.
if (fcc.Count == 0)
{
    Console.WriteLine("There are no folders to synchronize.");
}
// Otherwise, write all the changes included in the response 
// to the console. 
// For the initial synchronization, all the changes will be of type
// ChangeType.Create.
else
{
    foreach (FolderChange fc in fcc)
    {
        Console.WriteLine("ChangeType: " + fc.ChangeType.ToString());
        Console.WriteLine("FolderId: " + fc.FolderId);
        Console.WriteLine("===========");
    }
}
// Save the sync state for use in future SyncFolderItems requests.
// The sync state is used by the server to determine what changes to report
// to the client.
string fSyncState = fcc.SyncState;

```

<span data-ttu-id="2bf3d-120">Après avoir extraire la liste des dossiers nouveaux ou modifiés sur le serveur, [créer ou mettre à jour les dossiers sur le client](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_nextsteps).</span><span class="sxs-lookup"><span data-stu-id="2bf3d-120">After you retrieve the list of new or changed folders on the server, [create or update the folders on the client](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_nextsteps).</span></span>
  
## <a name="get-the-initial-list-of-folders-by-using-ews"></a><span data-ttu-id="2bf3d-121">Obtenir la liste initiale des dossiers à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="2bf3d-121">Get the initial list of folders by using EWS</span></span>
<span data-ttu-id="2bf3d-122"><a name="bk_cesyncewsrequest"> </a></span><span class="sxs-lookup"><span data-stu-id="2bf3d-122"></span></span>

<span data-ttu-id="2bf3d-123">L’exemple suivant montre une requête XML pour obtenir la hiérarchie de dossiers initiale à l’aide de l’opération [SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="2bf3d-123">The following example shows an XML request to get the initial folder hierarchy by using the [SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) operation.</span></span> <span data-ttu-id="2bf3d-124">Il s’agit de la demande XML que l’API managée EWS envoie quand également [récupérer la liste de dossiers initiales à l’aide de la méthode SyncFolderHierarchy](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncinitialewsma).</span><span class="sxs-lookup"><span data-stu-id="2bf3d-124">This is also the XML request that the EWS Managed API sends when [retrieving the list of initial folders by using the SyncFolderHierarchy method](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncinitialewsma).</span></span> <span data-ttu-id="2bf3d-125">L’élément [SyncState](http://msdn.microsoft.com/library/e5ebaae3-0f07-481d-ac67-d9687a3c7ac3%28Office.15%29.aspx) de l’opération [SyncFolderHierarchy](http://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx) n’est pas inclus, car il s’agit de la synchronisation initiale.</span><span class="sxs-lookup"><span data-stu-id="2bf3d-125">The [SyncState](http://msdn.microsoft.com/library/e5ebaae3-0f07-481d-ac67-d9687a3c7ac3%28Office.15%29.aspx) element of the [SyncFolderHierarchy](http://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx) operation is not included because this is the initial synchronization.</span></span> <span data-ttu-id="2bf3d-126">Cet exemple définit l’élément [BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) **IdOnly** afin de réduire les appels vers la base de données Exchange, qui est une [meilleure pratique de synchronisation](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices).</span><span class="sxs-lookup"><span data-stu-id="2bf3d-126">This example sets the [BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) element to **IdOnly** to reduce calls to the Exchange database, which is a [synchronization best practice](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices).</span></span>
  
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
    <m:SyncFolderHierarchy>
      <m:FolderShape>
        <t:BaseShape>IdOnly</t:BaseShape>
      </m:FolderShape>
      <m:SyncFolderId>
        <t:DistinguishedFolderId Id="root" />
      </m:SyncFolderId>
    </m:SyncFolderHierarchy>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="2bf3d-127">L’exemple suivant montre la réponse XML renvoyée par le serveur une fois le traitement de la requête d’opération [SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="2bf3d-127">The following example shows the XML response that is returned by the server after it processes the [SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) operation request.</span></span> <span data-ttu-id="2bf3d-128">La première réponse inclut [créer](http://msdn.microsoft.com/library/6b463d0a-70e9-40c5-ade4-c7d9a5f36bc1%28Office.15%29.aspx) des éléments pour tous les dossiers, car tous les dossiers sont considérés comme nouveau lors d’une synchronisation initiale.</span><span class="sxs-lookup"><span data-stu-id="2bf3d-128">The initial response includes [Create](http://msdn.microsoft.com/library/6b463d0a-70e9-40c5-ade4-c7d9a5f36bc1%28Office.15%29.aspx) elements for all folders because all folders are considered new during an initial synchronization.</span></span> <span data-ttu-id="2bf3d-129">Les valeurs de certains attributs et éléments ont été raccourcies pour des raisons de lisibilité, et certains blocs d’élément **créer** ont été supprimées par souci de concision.</span><span class="sxs-lookup"><span data-stu-id="2bf3d-129">The values of some attributes and elements have been shortened for readability, and some **Create** element blocks were removed for brevity.</span></span> 
  
```xml
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
    <m:SyncFolderHierarchyResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                                   xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:SyncFolderHierarchyResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:SyncState>H4sIAA==</m:SyncState>
          <m:IncludesLastFolderInRange>true</m:IncludesLastFolderInRange>
          <m:Changes>
            <t:Create>
              <t:Folder>
                <t:FolderId Id="AAMkADM="
                            ChangeKey="AQAAABYA"/>
              </t:Folder>
            </t:Create>
            <t:Create>
              <t:Folder>
                <t:FolderId Id="AAMkADMzM="
                            ChangeKey="AQAAABY"/>
              </t:Folder>
            </t:Create>
            <t:Create>
              <t:Folder>
                <t:FolderId Id="AAMkAD/AAA="
                            ChangeKey="AQAAABYA"/>
              </t:Folder>
            </t:Create>
            <t:Create>
              <t:Folder>
                <t:FolderId Id="AAMkADBh="
                            ChangeKey="AQAAABYA"/>
              </t:Folder>
            </t:Create>
            ...
          </m:Changes>
        </m:SyncFolderHierarchyResponseMessage>
      </m:ResponseMessages>
    </m:SyncFolderHierarchyResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="2bf3d-130">Après avoir extraire la liste des nouveaux dossiers sur le serveur, [créer les dossiers sur le client](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_nextsteps).</span><span class="sxs-lookup"><span data-stu-id="2bf3d-130">After you retrieve the list of new folders on the server, [create the folders on the client](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_nextsteps).</span></span>
  
## <a name="get-the-changes-since-the-last-sync-by-using-ews"></a><span data-ttu-id="2bf3d-131">Obtenir les modifications apportées depuis la dernière synchronisation à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="2bf3d-131">Get the changes since the last sync by using EWS</span></span>
<span data-ttu-id="2bf3d-132"><a name="bk_cesyncrespews"> </a></span><span class="sxs-lookup"><span data-stu-id="2bf3d-132"></span></span>

<span data-ttu-id="2bf3d-133">L’exemple suivant montre la demande XML pour obtenir la liste des modifications apportées aux dossiers dans le dossier racine à l’aide de l’opération [SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="2bf3d-133">The following example shows the XML request to get the list of changes to folders in the root folder by using the [SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) operation.</span></span> <span data-ttu-id="2bf3d-134">Il s’agit de la demande XML que l’API managée EWS envoie quand également [récupérer la liste des modifications dans le dossier racine](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncinitialewsma).</span><span class="sxs-lookup"><span data-stu-id="2bf3d-134">This is also the XML request that the EWS Managed API sends when [retrieving the list of changes to the root folder](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncinitialewsma).</span></span> <span data-ttu-id="2bf3d-135">Cet exemple définit la valeur de l’élément [SyncState](http://msdn.microsoft.com/library/e5ebaae3-0f07-481d-ac67-d9687a3c7ac3%28Office.15%29.aspx) à la valeur renvoyée dans la réponse précédente.</span><span class="sxs-lookup"><span data-stu-id="2bf3d-135">This example sets the [SyncState](http://msdn.microsoft.com/library/e5ebaae3-0f07-481d-ac67-d9687a3c7ac3%28Office.15%29.aspx) element value to the value returned in the previous response.</span></span> <span data-ttu-id="2bf3d-136">Et à des fins de démonstration, cet exemple définit l’élément [BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) **AllProperties** au lieu **IdOnly** pour afficher les propriétés supplémentaires renvoyées.</span><span class="sxs-lookup"><span data-stu-id="2bf3d-136">And for demonstration purposes, this example sets the [BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) element to **AllProperties** instead of **IdOnly** to show the additional properties returned.</span></span> <span data-ttu-id="2bf3d-137">Définissez l’élément [BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) **IdOnly** est une [meilleure pratique de synchronisation](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices).</span><span class="sxs-lookup"><span data-stu-id="2bf3d-137">Setting the [BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) element to **IdOnly** is a [synchronization best practice](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices).</span></span> <span data-ttu-id="2bf3d-138">La valeur de **SyncState** a été raccourcie pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="2bf3d-138">The value of **SyncState** has been shortened for readability.</span></span> 
  
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
    <m:SyncFolderHierarchy>
      <m:FolderShape>
        <t:BaseShape>AllProperties</t:BaseShape>
      </m:FolderShape>
      <m:SyncFolderId>
        <t:DistinguishedFolderId Id="root" />
      </m:SyncFolderId>
      <m:SyncState>H4sIAA==</m:SyncState>
    </m:SyncFolderHierarchy>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="2bf3d-139">L’exemple suivant montre la réponse XML renvoyée par le serveur une fois le traitement de la requête [d’opération SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) à partir du client.</span><span class="sxs-lookup"><span data-stu-id="2bf3d-139">The following example shows the XML response that is returned by the server after it processes the [SyncFolderHierarchy operation](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) request from the client.</span></span> <span data-ttu-id="2bf3d-140">Cette réponse indique qu’un dossier a été mis à jour, un dossier a été créé et un dossier a été supprimé depuis la synchronisation précédente.</span><span class="sxs-lookup"><span data-stu-id="2bf3d-140">This response indicates that one folder was updated, one folder was created, and one folder was deleted since the prior synchronization.</span></span> <span data-ttu-id="2bf3d-141">La valeur de l’élément de [SyncState](http://msdn.microsoft.com/library/e5ebaae3-0f07-481d-ac67-d9687a3c7ac3%28Office.15%29.aspx) , les attributs **Id** et les attributs **ChangeKey** ont été raccourcie pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="2bf3d-141">The value of the [SyncState](http://msdn.microsoft.com/library/e5ebaae3-0f07-481d-ac67-d9687a3c7ac3%28Office.15%29.aspx) element, **Id** attributes, and **ChangeKey** attributes have been shortened for readability.</span></span> 
  
<span data-ttu-id="2bf3d-142">N’oubliez pas que la demande inclus le **AllProperties**[BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="2bf3d-142">Remember that the request included the **AllProperties**[BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx).</span></span> <span data-ttu-id="2bf3d-143">Il s’agit uniquement à des fins de démonstration.</span><span class="sxs-lookup"><span data-stu-id="2bf3d-143">This is just for demonstration purposes.</span></span> <span data-ttu-id="2bf3d-144">Nous vous recommandons de définir l’élément **BaseShape** sur **IdOnly** en production.</span><span class="sxs-lookup"><span data-stu-id="2bf3d-144">We recommend that you set the **BaseShape** element to **IdOnly** in production.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
<h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="745" MinorBuildNumber="21" Version="V2_3" 
           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:SyncFolderHierarchyResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
            xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:SyncFolderHierarchyResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:SyncState>H4sIAAA</m:SyncState>
          <m:IncludesLastFolderInRange>true</m:IncludesLastFolderInRange>
          <m:Changes>
            <t:Update>
              <t:Folder>
                <t:FolderId Id="AAMkADM=" ChangeKey="AQAAABY" />
                <t:ParentFolderId Id="AQMkADMzADI1==" ChangeKey="AQAAAA==" />
                <t:FolderClass>IPF.Note</t:FolderClass>
                <t:DisplayName>Meeting Notes</t:DisplayName>
                <t:TotalCount>3</t:TotalCount>
                <t:ChildFolderCount>0</t:ChildFolderCount>
                <t:EffectiveRights>
                  <t:CreateAssociated>true</t:CreateAssociated>
                  <t:CreateContents>true</t:CreateContents>
                  <t:CreateHierarchy>true</t:CreateHierarchy>
                  <t:Delete>true</t:Delete>
                  <t:Modify>true</t:Modify>
                  <t:Read>true</t:Read>
                  <t:ViewPrivateItems>true</t:ViewPrivateItems>
                </t:EffectiveRights>
                <t:UnreadCount>0</t:UnreadCount>
              </t:Folder>
            </t:Update>
            <t:Create>
              <t:Folder>
                <t:FolderId Id="AAMkADMzM=" ChangeKey="AQAAABYAA" />
                <t:ParentFolderId Id="AQMkO67A==" ChangeKey="AQAAAA==" />
                <t:FolderClass>IPF.Note</t:FolderClass>
                <t:DisplayName>Schedules</t:DisplayName>
                <t:TotalCount>0</t:TotalCount>
                <t:ChildFolderCount>0</t:ChildFolderCount>
                <t:EffectiveRights>
                  <t:CreateAssociated>true</t:CreateAssociated>
                  <t:CreateContents>true</t:CreateContents>
                  <t:CreateHierarchy>true</t:CreateHierarchy>
                  <t:Delete>true</t:Delete>
                  <t:Modify>true</t:Modify>
                  <t:Read>true</t:Read>
                  <t:ViewPrivateItems>true</t:ViewPrivateItems>
                </t:EffectiveRights>
                <t:UnreadCount>0</t:UnreadCount>
              </t:Folder>
            </t:Create>
            <t:Delete>
              <t:FolderId Id="AAMkAD/AAA=" ChangeKey="AQAAAA==" />
            </t:Delete>
          </m:Changes>
        </m:SyncFolderHierarchyResponseMessage>
      </m:ResponseMessages>
    </m:SyncFolderHierarchyResponse>
  </s:Body>
</s:Envelope>

```

## <a name="update-the-client"></a><span data-ttu-id="2bf3d-145">Mise à jour du client</span><span class="sxs-lookup"><span data-stu-id="2bf3d-145">Update the client</span></span>
<span data-ttu-id="2bf3d-146"><a name="bk_nextsteps"> </a></span><span class="sxs-lookup"><span data-stu-id="2bf3d-146"></span></span>

<span data-ttu-id="2bf3d-147">Si vous utilisez l’API managée EWS, après avoir obtenir la liste des dossiers nouveaux ou modifiés, utilisez la méthode [Folder.Load](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.load%28v=exchg.80%29.aspx) pour obtenir les propriétés sur les éléments nouveaux ou modifiés, comparez les propriétés aux valeurs locales et mettre à jour ou créer les dossiers sur le client.</span><span class="sxs-lookup"><span data-stu-id="2bf3d-147">If you're using the EWS Managed API, after you get the list of new or changed folders, use the [Folder.Load](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.load%28v=exchg.80%29.aspx) method to get properties on the new or changed items, compare the properties to the local values, and update or create the folders on the client.</span></span> 
  
<span data-ttu-id="2bf3d-148">Si vous utilisez EWS, utilisez l' [opération GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) pour obtenir les propriétés sur les dossiers nouveaux ou modifiés et mettre à jour ou créer les dossiers sur le client.</span><span class="sxs-lookup"><span data-stu-id="2bf3d-148">If you're using EWS, use the [GetFolder operation](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) to get properties on the new or changed folders and update or create the folders on the client.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="2bf3d-149">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="2bf3d-149">See also</span></span>

- [<span data-ttu-id="2bf3d-150">Synchronisation de la boîte aux lettres et les services EWS d'Exchange</span><span class="sxs-lookup"><span data-stu-id="2bf3d-150">Mailbox synchronization and EWS in Exchange</span></span>](mailbox-synchronization-and-ews-in-exchange.md)   
- [<span data-ttu-id="2bf3d-151">Synchroniser des éléments à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="2bf3d-151">Synchronize items by using EWS in Exchange</span></span>](how-to-synchronize-items-by-using-ews-in-exchange.md)   
- [<span data-ttu-id="2bf3d-152">Gestion des erreurs liées à la synchronisation dans EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="2bf3d-152">Handling synchronization-related errors in EWS in Exchange</span></span>](handling-synchronization-related-errors-in-ews-in-exchange.md)
    
