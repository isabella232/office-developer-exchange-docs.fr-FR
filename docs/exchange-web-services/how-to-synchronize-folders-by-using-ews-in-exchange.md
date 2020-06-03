---
title: Synchroniser des dossiers à l’aide d’EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: d3bbacd1-8e4b-4fd0-8d27-4cbbc045ec3f
description: Découvrez comment utiliser l’API managée EWS ou EWS pour obtenir une liste de dossiers ou une liste de dossiers qui ont été modifiés, afin de synchroniser votre client.
ms.openlocfilehash: e49fdaf2faf97c2369f2ad7dbb141c5ac3100884
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455862"
---
# <a name="synchronize-folders-by-using-ews-in-exchange"></a><span data-ttu-id="a9a8a-103">Synchroniser des dossiers à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="a9a8a-103">Synchronize folders by using EWS in Exchange</span></span>

<span data-ttu-id="a9a8a-104">Découvrez comment utiliser l’API managée EWS ou EWS pour obtenir une liste de dossiers ou une liste de dossiers qui ont été modifiés, afin de synchroniser votre client.</span><span class="sxs-lookup"><span data-stu-id="a9a8a-104">Find out how to use the EWS Managed API or EWS to get a list of folders, or a list of folders that have changed, in order to synchronize your client.</span></span>
  
<span data-ttu-id="a9a8a-105">EWS dans Exchange utilise la synchronisation des éléments et la synchronisation des dossiers pour synchroniser le contenu des boîtes aux lettres entre le client et le serveur.</span><span class="sxs-lookup"><span data-stu-id="a9a8a-105">EWS in Exchange uses item synchronization and folder synchronization to sync mailbox content between the client and server.</span></span> <span data-ttu-id="a9a8a-106">Synchronisation de dossiers obtient la liste initiale des dossiers d’un dossier racine, puis, au fil du temps, les modifications apportées à ces dossiers et les nouveaux dossiers.</span><span class="sxs-lookup"><span data-stu-id="a9a8a-106">Folder synchronization gets the initial list of folders from a root folder and then, over time, gets changes that were made to those folders and gets new folders as well.</span></span>
  
<span data-ttu-id="a9a8a-107">Si vous effectuez une synchronisation des dossiers à l’aide de l’API managée EWS, vous obtenez d’abord [la liste initiale des dossiers dans le dossier racine](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncinitialewsma) à l’aide de la méthode [ExchangeService. opérationsyncfolderhierarchy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderhierarchy%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="a9a8a-107">If you're performing folder synchronization by using the EWS Managed API, you first [get the initial list of folders in the root folder](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncinitialewsma) by using the [ExchangeService.SyncFolderHierarchy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderhierarchy%28v=exchg.80%29.aspx) method.</span></span> <span data-ttu-id="a9a8a-108">Ensuite, vous mettez à jour la valeur du paramètre _cSyncState_ pendant les appels suivants pour obtenir la liste des dossiers nouveaux et modifiés.</span><span class="sxs-lookup"><span data-stu-id="a9a8a-108">You then update the value of the  _cSyncState_ parameter during subsequent calls to get the list of new and changed folders.</span></span> 
  
<span data-ttu-id="a9a8a-109">Pour effectuer une synchronisation des dossiers à l’aide d’EWS, vous devez demander la [liste initiale des dossiers dans le dossier racine](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncewsrequest) à l’aide de l’opération [opérationsyncfolderhierarchy](https://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) , analyser la réponse, puis à un moment donné [obtenir les modifications apportées aux dossiers dans la racine](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncrespews), puis analyser la réponse.</span><span class="sxs-lookup"><span data-stu-id="a9a8a-109">To perform folder synchronization by using EWS, you request the [initial list of folders in the root folder](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncewsrequest) by using the [SyncFolderHierarchy](https://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) operation, parse the response, and then at some point in the future [get the changes to the folders in the root](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncrespews), and parse the response.</span></span> <span data-ttu-id="a9a8a-110">Une fois que le client a reçu la liste des dossiers initiaux ou modifiés, il [effectue les mises à jour localement](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_nextsteps).</span><span class="sxs-lookup"><span data-stu-id="a9a8a-110">After the client receives the list of initial or changed folders, it [makes updates locally](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_nextsteps).</span></span> <span data-ttu-id="a9a8a-111">Le mode de récupération des modifications à venir dépend du modèle de [conception de synchronisation](mailbox-synchronization-and-ews-in-exchange.md#bk_syncpatterns) utilisé par votre application.</span><span class="sxs-lookup"><span data-stu-id="a9a8a-111">How and when you retrieve changes in the future depends on the [synchronization design pattern](mailbox-synchronization-and-ews-in-exchange.md#bk_syncpatterns) your application is using.</span></span> 
  
## <a name="get-the-list-of-all-folders-or-changed-folders-by-using-the-ews-managed-api"></a><span data-ttu-id="a9a8a-112">Obtenir la liste de tous les dossiers ou dossiers modifiés à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="a9a8a-112">Get the list of all folders or changed folders by using the EWS Managed API</span></span>
<span data-ttu-id="a9a8a-113"><a name="bk_cesyncinitialewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="a9a8a-113"><a name="bk_cesyncinitialewsma"> </a></span></span>

<span data-ttu-id="a9a8a-114">L’exemple de code suivant montre comment obtenir une liste initiale de dossiers dans un dossier racine, puis obtenir la liste des modifications apportées aux dossiers dans le dossier racine qui se sont produites depuis la synchronisation précédente.</span><span class="sxs-lookup"><span data-stu-id="a9a8a-114">The following code example shows how to get an initial list of folders in a root folder and then get a list of changes to folders in the root folder that have occurred since the previous synchronization.</span></span> <span data-ttu-id="a9a8a-115">Lors de l’appel initial à la méthode [ExchangeService. opérationsyncfolderhierarchy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderhierarchy%28v=exchg.80%29.aspx) , définissez la valeur _cSyncState_ sur null.</span><span class="sxs-lookup"><span data-stu-id="a9a8a-115">During the initial call to the [ExchangeService.SyncFolderHierarchy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderhierarchy%28v=exchg.80%29.aspx) method, set the  _cSyncState_ value to null.</span></span> <span data-ttu-id="a9a8a-116">Une fois la méthode terminée, enregistrez la valeur _cSyncState_ localement pour l’utiliser dans le prochain appel de la méthode **opérationsyncfolderhierarchy** .</span><span class="sxs-lookup"><span data-stu-id="a9a8a-116">When the method completes, save the  _cSyncState_ value locally to use in the next **SyncFolderHierarchy** method call.</span></span> <span data-ttu-id="a9a8a-117">Dans l’appel initial et les appels ultérieurs, les dossiers sont récupérés par lots de dix, à l’aide d’appels successifs à la méthode **opérationsyncfolderhierarchy** , jusqu’à ce qu’il ne reste plus aucune modification.</span><span class="sxs-lookup"><span data-stu-id="a9a8a-117">In both the initial call and the subsequent calls, the folders are retrieved in batches of ten, by using successive calls to the **SyncFolderHierarchy** method, until no more changes remain.</span></span> <span data-ttu-id="a9a8a-118">Cet exemple définit le paramètre _PropertySet_ sur IdOnly pour réduire les appels à la base de données Exchange, ce qui est une [meilleure pratique de synchronisation](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices).</span><span class="sxs-lookup"><span data-stu-id="a9a8a-118">This example sets the  _propertySet_ parameter to IdOnly to reduce calls to the Exchange database, which is a [synchronization best practice](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices).</span></span> <span data-ttu-id="a9a8a-119">Dans cet exemple, nous partons du principe que le **service** est une liaison d’objet **ExchangeService** valide et que _cSyncState_ représente l’état de synchronisation renvoyé par un appel antérieur à **opérationsyncfolderhierarchy**.</span><span class="sxs-lookup"><span data-stu-id="a9a8a-119">In this example, we assume that **service** is a valid **ExchangeService** object binding and that  _cSyncState_ represents the sync state that was returned by a prior call to **SyncFolderHierarchy**.</span></span> 
  
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

<span data-ttu-id="a9a8a-120">Une fois que vous avez récupéré la liste des dossiers nouveaux ou modifiés sur le serveur, [créez ou mettez à jour les dossiers sur le client](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_nextsteps).</span><span class="sxs-lookup"><span data-stu-id="a9a8a-120">After you retrieve the list of new or changed folders on the server, [create or update the folders on the client](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_nextsteps).</span></span>
  
## <a name="get-the-initial-list-of-folders-by-using-ews"></a><span data-ttu-id="a9a8a-121">Obtenir la liste initiale des dossiers à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="a9a8a-121">Get the initial list of folders by using EWS</span></span>
<span data-ttu-id="a9a8a-122"><a name="bk_cesyncewsrequest"> </a></span><span class="sxs-lookup"><span data-stu-id="a9a8a-122"><a name="bk_cesyncewsrequest"> </a></span></span>

<span data-ttu-id="a9a8a-123">L’exemple suivant montre une requête XML pour obtenir la hiérarchie de dossiers initiale à l’aide de l’opération [opérationsyncfolderhierarchy](https://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="a9a8a-123">The following example shows an XML request to get the initial folder hierarchy by using the [SyncFolderHierarchy](https://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) operation.</span></span> <span data-ttu-id="a9a8a-124">Il s’agit également de la demande XML que l’API managée EWS envoie lors [de la récupération de la liste des dossiers initiaux à l’aide de la méthode opérationsyncfolderhierarchy](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncinitialewsma).</span><span class="sxs-lookup"><span data-stu-id="a9a8a-124">This is also the XML request that the EWS Managed API sends when [retrieving the list of initial folders by using the SyncFolderHierarchy method](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncinitialewsma).</span></span> <span data-ttu-id="a9a8a-125">L’élément [SyncState](https://msdn.microsoft.com/library/e5ebaae3-0f07-481d-ac67-d9687a3c7ac3%28Office.15%29.aspx) de l’opération [opérationsyncfolderhierarchy](https://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx) n’est pas inclus car il s’agit de la synchronisation initiale.</span><span class="sxs-lookup"><span data-stu-id="a9a8a-125">The [SyncState](https://msdn.microsoft.com/library/e5ebaae3-0f07-481d-ac67-d9687a3c7ac3%28Office.15%29.aspx) element of the [SyncFolderHierarchy](https://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx) operation is not included because this is the initial synchronization.</span></span> <span data-ttu-id="a9a8a-126">Cet exemple définit l’élément [BaseShape](https://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) sur **IdOnly** pour réduire les appels à la base de données Exchange, ce qui est une [meilleure pratique de synchronisation](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices).</span><span class="sxs-lookup"><span data-stu-id="a9a8a-126">This example sets the [BaseShape](https://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) element to **IdOnly** to reduce calls to the Exchange database, which is a [synchronization best practice](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices).</span></span>
  
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

<span data-ttu-id="a9a8a-127">L’exemple suivant montre la réponse XML renvoyée par le serveur après qu’il a traité la demande d’opération [opérationsyncfolderhierarchy](https://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="a9a8a-127">The following example shows the XML response that is returned by the server after it processes the [SyncFolderHierarchy](https://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) operation request.</span></span> <span data-ttu-id="a9a8a-128">La réponse initiale inclut la [création](https://msdn.microsoft.com/library/6b463d0a-70e9-40c5-ade4-c7d9a5f36bc1%28Office.15%29.aspx) d’éléments pour tous les dossiers, car tous les dossiers sont considérés comme nouveaux lors d’une synchronisation initiale.</span><span class="sxs-lookup"><span data-stu-id="a9a8a-128">The initial response includes [Create](https://msdn.microsoft.com/library/6b463d0a-70e9-40c5-ade4-c7d9a5f36bc1%28Office.15%29.aspx) elements for all folders because all folders are considered new during an initial synchronization.</span></span> <span data-ttu-id="a9a8a-129">Les valeurs de certains attributs et éléments ont été raccourcies pour des raisons de lisibilité, et certains blocs d’élément **Create** ont été supprimés pour des raisons de brièveté.</span><span class="sxs-lookup"><span data-stu-id="a9a8a-129">The values of some attributes and elements have been shortened for readability, and some **Create** element blocks were removed for brevity.</span></span> 
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="785"
                         MinorBuildNumber="6"
                         Version="V2_6"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:SyncFolderHierarchyResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                                   xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="a9a8a-130">Une fois que vous avez récupéré la liste des nouveaux dossiers sur le serveur, [créez les dossiers sur le client](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_nextsteps).</span><span class="sxs-lookup"><span data-stu-id="a9a8a-130">After you retrieve the list of new folders on the server, [create the folders on the client](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_nextsteps).</span></span>
  
## <a name="get-the-changes-since-the-last-sync-by-using-ews"></a><span data-ttu-id="a9a8a-131">Obtenir les modifications depuis la dernière synchronisation à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="a9a8a-131">Get the changes since the last sync by using EWS</span></span>
<span data-ttu-id="a9a8a-132"><a name="bk_cesyncrespews"> </a></span><span class="sxs-lookup"><span data-stu-id="a9a8a-132"><a name="bk_cesyncrespews"> </a></span></span>

<span data-ttu-id="a9a8a-133">L’exemple suivant montre la requête XML pour obtenir la liste des modifications apportées aux dossiers dans le dossier racine à l’aide de l’opération [opérationsyncfolderhierarchy](https://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="a9a8a-133">The following example shows the XML request to get the list of changes to folders in the root folder by using the [SyncFolderHierarchy](https://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) operation.</span></span> <span data-ttu-id="a9a8a-134">Il s’agit également de la demande XML que l’API managée EWS envoie lors [de la récupération de la liste des modifications apportées au dossier racine](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncinitialewsma).</span><span class="sxs-lookup"><span data-stu-id="a9a8a-134">This is also the XML request that the EWS Managed API sends when [retrieving the list of changes to the root folder](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncinitialewsma).</span></span> <span data-ttu-id="a9a8a-135">Cet exemple définit la valeur de l’élément [SyncState](https://msdn.microsoft.com/library/e5ebaae3-0f07-481d-ac67-d9687a3c7ac3%28Office.15%29.aspx) sur la valeur renvoyée dans la réponse précédente.</span><span class="sxs-lookup"><span data-stu-id="a9a8a-135">This example sets the [SyncState](https://msdn.microsoft.com/library/e5ebaae3-0f07-481d-ac67-d9687a3c7ac3%28Office.15%29.aspx) element value to the value returned in the previous response.</span></span> <span data-ttu-id="a9a8a-136">À des fins de démonstration, cet exemple montre comment définir l’élément [BaseShape](https://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) à **AllProperties** au lieu de **IdOnly** pour afficher les propriétés supplémentaires renvoyées.</span><span class="sxs-lookup"><span data-stu-id="a9a8a-136">And for demonstration purposes, this example sets the [BaseShape](https://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) element to **AllProperties** instead of **IdOnly** to show the additional properties returned.</span></span> <span data-ttu-id="a9a8a-137">La définition de l’élément [BaseShape](https://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) sur **IdOnly** est une [meilleure pratique de synchronisation](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices).</span><span class="sxs-lookup"><span data-stu-id="a9a8a-137">Setting the [BaseShape](https://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) element to **IdOnly** is a [synchronization best practice](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices).</span></span> <span data-ttu-id="a9a8a-138">La valeur de **SyncState** a été raccourcie pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="a9a8a-138">The value of **SyncState** has been shortened for readability.</span></span> 
  
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

<span data-ttu-id="a9a8a-139">L’exemple suivant montre la réponse XML renvoyée par le serveur après qu’il a traité la demande d' [opération opérationsyncfolderhierarchy](https://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) du client.</span><span class="sxs-lookup"><span data-stu-id="a9a8a-139">The following example shows the XML response that is returned by the server after it processes the [SyncFolderHierarchy operation](https://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) request from the client.</span></span> <span data-ttu-id="a9a8a-140">Cette réponse indique qu’un dossier a été mis à jour, qu’un dossier a été créé et qu’un dossier a été supprimé depuis la synchronisation précédente.</span><span class="sxs-lookup"><span data-stu-id="a9a8a-140">This response indicates that one folder was updated, one folder was created, and one folder was deleted since the prior synchronization.</span></span> <span data-ttu-id="a9a8a-141">La valeur des attributs [SyncState](https://msdn.microsoft.com/library/e5ebaae3-0f07-481d-ac67-d9687a3c7ac3%28Office.15%29.aspx) , **ID** et **ChangeKey** a été raccourcie pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="a9a8a-141">The value of the [SyncState](https://msdn.microsoft.com/library/e5ebaae3-0f07-481d-ac67-d9687a3c7ac3%28Office.15%29.aspx) element, **Id** attributes, and **ChangeKey** attributes have been shortened for readability.</span></span> 
  
<span data-ttu-id="a9a8a-142">N’oubliez pas que la demande incluait le **AllProperties**[BaseShape](https://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="a9a8a-142">Remember that the request included the **AllProperties**[BaseShape](https://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx).</span></span> <span data-ttu-id="a9a8a-143">Ceci est uniquement à des fins de démonstration.</span><span class="sxs-lookup"><span data-stu-id="a9a8a-143">This is just for demonstration purposes.</span></span> <span data-ttu-id="a9a8a-144">Nous vous recommandons de définir l’élément **BaseShape** sur **IdOnly** en production.</span><span class="sxs-lookup"><span data-stu-id="a9a8a-144">We recommend that you set the **BaseShape** element to **IdOnly** in production.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
<h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="745" MinorBuildNumber="21" Version="V2_3" 
           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:SyncFolderHierarchyResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
            xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="update-the-client"></a><span data-ttu-id="a9a8a-145">Mettre à jour le client</span><span class="sxs-lookup"><span data-stu-id="a9a8a-145">Update the client</span></span>
<span data-ttu-id="a9a8a-146"><a name="bk_nextsteps"> </a></span><span class="sxs-lookup"><span data-stu-id="a9a8a-146"><a name="bk_nextsteps"> </a></span></span>

<span data-ttu-id="a9a8a-147">Si vous utilisez l’API managée EWS, une fois que vous avez obtenu la liste des dossiers nouveaux ou modifiés, utilisez la méthode [Folder. Load](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.load%28v=exchg.80%29.aspx) pour obtenir des propriétés sur les éléments nouveaux ou modifiés, comparez les propriétés aux valeurs locales, et mettez à jour ou créez les dossiers sur le client.</span><span class="sxs-lookup"><span data-stu-id="a9a8a-147">If you're using the EWS Managed API, after you get the list of new or changed folders, use the [Folder.Load](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.load%28v=exchg.80%29.aspx) method to get properties on the new or changed items, compare the properties to the local values, and update or create the folders on the client.</span></span> 
  
<span data-ttu-id="a9a8a-148">Si vous utilisez EWS, utilisez l' [opération GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) pour obtenir les propriétés des dossiers nouveaux ou modifiés, et mettre à jour ou créer les dossiers sur le client.</span><span class="sxs-lookup"><span data-stu-id="a9a8a-148">If you're using EWS, use the [GetFolder operation](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) to get properties on the new or changed folders and update or create the folders on the client.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="a9a8a-149">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a9a8a-149">See also</span></span>

- [<span data-ttu-id="a9a8a-150">Synchronisation de la boîte aux lettres et les services EWS d'Exchange</span><span class="sxs-lookup"><span data-stu-id="a9a8a-150">Mailbox synchronization and EWS in Exchange</span></span>](mailbox-synchronization-and-ews-in-exchange.md)   
- [<span data-ttu-id="a9a8a-151">Synchroniser des éléments à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="a9a8a-151">Synchronize items by using EWS in Exchange</span></span>](how-to-synchronize-items-by-using-ews-in-exchange.md)   
- [<span data-ttu-id="a9a8a-152">Gestion des erreurs liées à la synchronisation dans EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="a9a8a-152">Handling synchronization-related errors in EWS in Exchange</span></span>](handling-synchronization-related-errors-in-ews-in-exchange.md)
    

