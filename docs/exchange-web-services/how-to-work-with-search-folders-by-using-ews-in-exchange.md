---
title: Utilisation de dossiers de recherche à l’aide de EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: abe703c5-6d85-46d9-bf20-230c34782a9f
description: Découvrez comment créer, obtenir, mettre à jour et supprimer des dossiers de recherche à l’aide de l’API managée EWS ou EWS dans Exchange.
ms.openlocfilehash: e38ff50fcdb5e42cea3f4b2e25345375f84ae6eb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19754989"
---
# <a name="work-with-search-folders-by-using-ews-in-exchange"></a><span data-ttu-id="02308-103">Utilisation de dossiers de recherche à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="02308-103">Work with search folders by using EWS in Exchange</span></span>

<span data-ttu-id="02308-104">Découvrez comment créer, obtenir, mettre à jour et supprimer des dossiers de recherche à l’aide de l’API managée EWS ou EWS dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="02308-104">Find out how to create, get, update, and delete search folders by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="02308-105">Un dossier de recherche représente une recherche permanente « toujours active » dans la boîte aux lettres d’un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="02308-105">A search folder represents a persistent "always-on" search in a user's mailbox.</span></span> <span data-ttu-id="02308-106">Un dossier de recherche se présente et se comporte comme un dossier de boîte aux lettres standard.</span><span class="sxs-lookup"><span data-stu-id="02308-106">A search folder looks and acts like a regular mailbox folder.</span></span> <span data-ttu-id="02308-107">Toutefois, au lieu de contenant des éléments, il contient une copie « virtuelle » d’éléments à partir de tous les dossiers dans son étendue de recherche qui correspondent aux critères de recherche définis sur le dossier.</span><span class="sxs-lookup"><span data-stu-id="02308-107">However, instead of containing items, it contains a "virtual" copy of items from any folders in its search scope that match the search criteria set on the folder.</span></span> <span data-ttu-id="02308-108">Les applications et les utilisateurs finaux peuvent utiliser les dossiers de recherche.</span><span class="sxs-lookup"><span data-stu-id="02308-108">Both applications and end-users can use search folders.</span></span> <span data-ttu-id="02308-109">Votre application a-t-elle besoin pour effectuer la même recherche continuellement ?</span><span class="sxs-lookup"><span data-stu-id="02308-109">Does your application need to perform the same search over and over?</span></span> <span data-ttu-id="02308-110">Dossiers de recherche constituent un excellent outil pour cette tâche.</span><span class="sxs-lookup"><span data-stu-id="02308-110">Search folders are a great tool for this task.</span></span> <span data-ttu-id="02308-111">Ou peut-être que vous souhaitez simplement donner aux utilisateurs la possibilité d’accéder et de gérer les dossiers de recherche dans votre client.</span><span class="sxs-lookup"><span data-stu-id="02308-111">Or maybe you just want to give your users the ability to access and manage search folders in your client.</span></span> <span data-ttu-id="02308-112">Quelle que soit votre scénario, les API managées EWS permettent à votre application interagir avec les dossiers de recherche.</span><span class="sxs-lookup"><span data-stu-id="02308-112">Whatever your scenario, the EWS Managed API and EWS enable your application to fully interact with search folders.</span></span>
  
<span data-ttu-id="02308-113">**Le tableau 1. Méthodes d’API managées et opérations EWS pour travailler avec des dossiers de recherche**</span><span class="sxs-lookup"><span data-stu-id="02308-113">**Table 1. EWS Managed API methods and EWS operations for working with search folders**</span></span>

|<span data-ttu-id="02308-114">**Si vous souhaitez...**</span><span class="sxs-lookup"><span data-stu-id="02308-114">**If you want to…**</span></span>|<span data-ttu-id="02308-115">**Dans l’API managée EWS, utilisez...**</span><span class="sxs-lookup"><span data-stu-id="02308-115">**In the EWS Managed API, use…**</span></span>|<span data-ttu-id="02308-116">**Dans les services EWS, utilisez...**</span><span class="sxs-lookup"><span data-stu-id="02308-116">**In EWS, use…**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="02308-117">Créer un dossier de recherche</span><span class="sxs-lookup"><span data-stu-id="02308-117">Create a search folder</span></span>  <br/> |[<span data-ttu-id="02308-118">SearchFolder.Save</span><span class="sxs-lookup"><span data-stu-id="02308-118">SearchFolder.Save</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfolder.save%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="02308-119">Opération CreateFolder</span><span class="sxs-lookup"><span data-stu-id="02308-119">CreateFolder operation</span></span>](http://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="02308-120">Obtenir un dossier de recherche</span><span class="sxs-lookup"><span data-stu-id="02308-120">Get a search folder</span></span>  <br/> |[<span data-ttu-id="02308-121">SearchFolder.Bind</span><span class="sxs-lookup"><span data-stu-id="02308-121">SearchFolder.Bind</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfolder.bind%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="02308-122">Opération GetFolder</span><span class="sxs-lookup"><span data-stu-id="02308-122">GetFolder operation</span></span>](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="02308-123">Mettre à jour un dossier de recherche</span><span class="sxs-lookup"><span data-stu-id="02308-123">Update a search folder</span></span>  <br/> |[<span data-ttu-id="02308-124">SearchFolder.Update</span><span class="sxs-lookup"><span data-stu-id="02308-124">SearchFolder.Update</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="02308-125">Opération UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="02308-125">UpdateFolder operation</span></span>](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="02308-126">Supprimer un dossier de recherche</span><span class="sxs-lookup"><span data-stu-id="02308-126">Delete a search folder</span></span>  <br/> |[<span data-ttu-id="02308-127">SearchFolder.Delete</span><span class="sxs-lookup"><span data-stu-id="02308-127">SearchFolder.Delete</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="02308-128">Opération DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="02308-128">DeleteFolder operation</span></span>](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |
   
## <a name="core-concepts-to-know-for-working-with-search-folders"></a><span data-ttu-id="02308-129">Principaux concepts à connaître pour l’utilisation de dossiers de recherche</span><span class="sxs-lookup"><span data-stu-id="02308-129">Core concepts to know for working with search folders</span></span>
<span data-ttu-id="02308-130"><a name="bk_CoreConcepts"> </a></span><span class="sxs-lookup"><span data-stu-id="02308-130"></span></span>

<span data-ttu-id="02308-131">Avant de commencer à utiliser les dossiers de recherche, vous souhaiterez vous familiariser avec la façon dont des filtres de recherche.</span><span class="sxs-lookup"><span data-stu-id="02308-131">Before you start working with search folders, you'll want to be familiar with how search filters work.</span></span> <span data-ttu-id="02308-132">Dossiers de recherche s’appuient sur les filtres pour exprimer leurs critères de recherche.</span><span class="sxs-lookup"><span data-stu-id="02308-132">Search folders rely on search filters to express their criteria.</span></span> <span data-ttu-id="02308-133">Filtres de recherche pour les dossiers de recherche sont construits de la même façon que [les filtres de recherche pour les opérations de recherche](how-to-use-search-filters-with-ews-in-exchange.md) sont construits.</span><span class="sxs-lookup"><span data-stu-id="02308-133">Search filters for search folders are constructed in the same way that [search filters for search operations](how-to-use-search-filters-with-ews-in-exchange.md) are constructed.</span></span> 
  
## <a name="create-a-search-folder-by-using-the-ews-managed-api"></a><span data-ttu-id="02308-134">Créer un dossier de recherche à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="02308-134">Create a search folder by using the EWS Managed API</span></span>
<span data-ttu-id="02308-135"><a name="bk_CreateEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="02308-135"></span></span>

<span data-ttu-id="02308-136">En fait, vous créez un dossier de recherche à l’aide de l’API managée EWS de la même manière que vous créez un dossier.</span><span class="sxs-lookup"><span data-stu-id="02308-136">Basically, you create a search folder using the EWS Managed API in the same way that you create a regular folder.</span></span> <span data-ttu-id="02308-137">Toutefois, au lieu d’utiliser la [classe d’un dossier](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx), vous utilisez la [classe SearchFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx)et définissez la [propriété SearchParameters](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfolder.searchparameters%28v=exchg.80%29.aspx) pour configurer les critères de recherche.</span><span class="sxs-lookup"><span data-stu-id="02308-137">However, instead of using the [Folder class](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx), you use the [SearchFolder class](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx), and set the [SearchParameters property](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfolder.searchparameters%28v=exchg.80%29.aspx) to configure the search criteria.</span></span> 
  
<span data-ttu-id="02308-138">Dans l’exemple suivant, un dossier de recherche est créé pour rechercher tous les messages dans la boîte de réception et ses sous-dossiers qui ont été envoyés par le responsable de l’utilisateur, sadie@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="02308-138">In the following example, a search folder is created to find all messages in the Inbox and its subfolders that were sent by the user's manager, sadie@contoso.com.</span></span> <span data-ttu-id="02308-139">Le dossier est créé en tant qu’enfant du dossier dossiers de recherche de boîte aux lettres de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="02308-139">The folder is created as a child of the Search Folders folder in the user's mailbox.</span></span>
  
> [!NOTE]
> <span data-ttu-id="02308-140">Vous pouvez créer un dossier de recherche en tant qu’enfant de n’importe quel dossier de boîte aux lettres de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="02308-140">You can create a search folder as a child of any folder in the user's mailbox.</span></span> <span data-ttu-id="02308-141">Toutefois, si vous souhaitez que le nouveau dossier s’affiche sous dossiers de recherche dans Outlook, créer sous le dossier connu de dossiers de recherche, à l’aide de la valeur **SearchFolders** de l' [énumération WellKnownFolderName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="02308-141">However, if you want the newly created folder to show up under Search Folders in Outlook, create it under the Search Folders well-known folder, using the **SearchFolders** value of the [WellKnownFolderName enumeration](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx).</span></span> 
  
<span data-ttu-id="02308-142">Cet exemple suppose que l’objet **ExchangeService** a été initialisée avec des valeurs valides dans les propriétés [d’Url](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) et les [informations d’identification](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="02308-142">This example assumes that the **ExchangeService** object has been initialized with valid values in the [Credentials](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) and [Url](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) properties.</span></span> 
  
```cs
using Microsoft.Exchange.WebServices.Data;
static void CreateSearchFolder(ExchangeService service)
{
    // Create the folder.
    SearchFolder searchFolder = new SearchFolder(service);
    searchFolder.DisplayName = "From Manager";
    // Create a search filter to express the criteria
    // for the folder.
    EmailAddress manager = new EmailAddress("sadie@contoso.com");
    SearchFilter.IsEqualTo fromManagerFilter =
        new SearchFilter.IsEqualTo(EmailMessageSchema.Sender, manager);
    // Set the search filter.
    searchFolder.SearchParameters.SearchFilter = fromManagerFilter;
    // Set the folder to search.
    searchFolder.SearchParameters.RootFolderIds.Add(WellKnownFolderName.Inbox);
    // Set the search traversal. Deep will search all subfolders.
    searchFolder.SearchParameters.Traversal = SearchFolderTraversal.Deep;
    // Call Save to make the EWS call to create the folder.
    searchFolder.Save(WellKnownFolderName.SearchFolders);
}
```

## <a name="create-a-search-folder-by-using-ews"></a><span data-ttu-id="02308-143">Créer un dossier de recherche à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="02308-143">Create a search folder by using EWS</span></span>
<span data-ttu-id="02308-144"><a name="bk_CreateEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="02308-144"></span></span>

<span data-ttu-id="02308-145">Si vous utilisez EWS, utilisez l' [opération CreateFolder](http://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) avec un élément [SearchFolder](http://msdn.microsoft.com/library/1a7d408b-2e98-4391-8834-085ed6d5757c%28Office.15%29.aspx) pour créer un dossier de recherche.</span><span class="sxs-lookup"><span data-stu-id="02308-145">If you are using EWS, use the [CreateFolder operation](http://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) with a [SearchFolder](http://msdn.microsoft.com/library/1a7d408b-2e98-4391-8834-085ed6d5757c%28Office.15%29.aspx) element to create a search folder.</span></span> <span data-ttu-id="02308-146">Dans l’exemple de requête suivant, un dossier de recherche est créé pour rechercher tous les messages dans la boîte de réception et ses sous-dossiers qui ont été envoyés par le responsable de l’utilisateur, sadie@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="02308-146">In the following request example, a search folder is created to find all messages in the Inbox and its subfolders that were sent by the user's manager, sadie@contoso.com.</span></span> <span data-ttu-id="02308-147">Le dossier est créé dans le dossier de dossiers de recherche dans la boîte aux lettres de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="02308-147">The folder is created in the Search Folders folder in the user's mailbox.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="02308-148">Vous pouvez créer un dossier de recherche en tant qu’enfant de n’importe quel dossier de boîte aux lettres de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="02308-148">You can create a search folder as a child of any folder in the user's mailbox.</span></span> <span data-ttu-id="02308-149">Toutefois, si vous souhaitez que le nouveau dossier s’affiche sous dossiers de recherche dans Outlook, créer sous le dossier connu de dossiers de recherche, à l’aide de la valeur **searchfolders** dans l’attribut **Id** de l’élément [DistinguishedFolderId](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="02308-149">However, if you want the newly created folder to show up under Search Folders in Outlook, create it under the Search Folders well-known folder, using the **searchfolders** value in the **Id** attribute of the [DistinguishedFolderId](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) element.</span></span> 
  
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
    <m:CreateFolder>
      <m:ParentFolderId>
        <t:DistinguishedFolderId Id="searchfolders" />
      </m:ParentFolderId>
      <m:Folders>
        <t:SearchFolder>
          <t:DisplayName>From Manager</t:DisplayName>
          <t:SearchParameters Traversal="Deep">
            <t:Restriction>
              <t:IsEqualTo>
                <t:FieldURI FieldURI="message:Sender" />
                <t:FieldURIOrConstant>
                  <t:Constant Value="sadie@contoso.com" />
                </t:FieldURIOrConstant>
              </t:IsEqualTo>
            </t:Restriction>
            <t:BaseFolderIds>
              <t:DistinguishedFolderId Id="inbox" />
            </t:BaseFolderIds>
          </t:SearchParameters>
        </t:SearchFolder>
      </m:Folders>
    </m:CreateFolder>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="02308-150">Le serveur répond avec un message [CreateFolderResponse](http://msdn.microsoft.com/library/158adecc-491a-47d9-af73-acc2cd3f8566%28Office.15%29.aspx) qui contient une valeur [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, qui indique une réussite.</span><span class="sxs-lookup"><span data-stu-id="02308-150">The server responds with a [CreateFolderResponse](http://msdn.microsoft.com/library/158adecc-491a-47d9-af73-acc2cd3f8566%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates success.</span></span>
  
## <a name="get-a-search-folder-by-using-the-ews-managed-api"></a><span data-ttu-id="02308-151">Obtenir un dossier de recherche à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="02308-151">Get a search folder by using the EWS Managed API</span></span>
<span data-ttu-id="02308-152"><a name="bk_RetrieveEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="02308-152"></span></span>

<span data-ttu-id="02308-153">Utilisez la méthode d’API managées [ExchangeService.FindFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx) pour trouver les dossiers de recherche.</span><span class="sxs-lookup"><span data-stu-id="02308-153">Use the [ExchangeService.FindFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx) EWS Managed API method to find search folders.</span></span> <span data-ttu-id="02308-154">Toutefois, notez que vous ne pouvez pas limiter vos résultats pour n’inclure que les dossiers de recherche ; Vous souhaiterez qui Gardez à l’esprit lorsque vous traitez les résultats.</span><span class="sxs-lookup"><span data-stu-id="02308-154">Note, however, that you can't limit your results to only include search folders; you'll want to keep that in mind when you process the results.</span></span> <span data-ttu-id="02308-155">Utilisez la méthode [SearchFolder.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfolder.bind%28v=exchg.80%29.aspx) pour obtenir les dossiers de recherche.</span><span class="sxs-lookup"><span data-stu-id="02308-155">Use the [SearchFolder.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfolder.bind%28v=exchg.80%29.aspx) method to get search folders.</span></span> 
  
<span data-ttu-id="02308-156">L’exemple suivant recherche les 10 premiers dossiers dans le dossier de dossiers de recherche.</span><span class="sxs-lookup"><span data-stu-id="02308-156">The following example finds the first 10 folders in the Search Folders folder.</span></span> <span data-ttu-id="02308-157">Il vérifie pour déterminer si chacun d’eux est un dossier de recherche, et si Oui, il obtient le dossier de recherche et affiche le nombre de dossiers cible retenus.</span><span class="sxs-lookup"><span data-stu-id="02308-157">It checks to determine whether each one is a search folder, and if so, it gets the search folder and displays how many target folders it searches.</span></span>
  
```cs
using Microsoft.Exchange.WebServices.Data;
static void GetSearchFolders(ExchangeService service)
{
    FolderView folderView = new FolderView(10);
    folderView.PropertySet = new PropertySet(FolderSchema.DisplayName);
    try
    {
        FindFoldersResults findResults = service.FindFolders(WellKnownFolderName.SearchFolders, folderView);
        foreach (Folder folder in findResults.Folders)
        {
            // You can't request only search folders in 
            // a FindFolders request, so other search folders might also be present.
            if (folder is SearchFolder)
            {
                Console.WriteLine("{0} is a search folder.", folder.DisplayName);
                // In order to access the SearchParameters property,
                // you have to bind to the folder. SearchParameters are not
                // returned in FindFolders results.
                SearchFolder searchFolder = SearchFolder.Bind(service, folder.Id);
                Console.WriteLine("Number of folders searched: {0}.",
                    searchFolder.SearchParameters.RootFolderIds.Count);
            }
            else
            {
                Console.WriteLine("{0} is NOT a search folder.", folder.DisplayName);
            }
        }
    }
    catch (Exception ex)
    {
        Console.WriteLine("Exception while enumerating results: {0}", ex.Message);
    }
}
```

## <a name="get-a-search-folder-by-using-ews"></a><span data-ttu-id="02308-158">Obtenir un dossier de recherche à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="02308-158">Get a search folder by using EWS</span></span>
<span data-ttu-id="02308-159"><a name="bk_RetrieveEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="02308-159"></span></span>

<span data-ttu-id="02308-160">Si vous utilisez EWS, utilisez l' [opération FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) pour rechercher les dossiers de recherche et l' [opération GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) pour obtenir les dossiers de recherche.</span><span class="sxs-lookup"><span data-stu-id="02308-160">If you're using EWS, use the [FindFolder operation](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) to find search folders, and the [GetFolder operation](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) to get search folders.</span></span> <span data-ttu-id="02308-161">Une réponse positive de **GetFolder** pour un dossier de recherche contient un élément [SearchFolder](http://msdn.microsoft.com/library/1a7d408b-2e98-4391-8834-085ed6d5757c%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="02308-161">A successful **GetFolder** response for a search folder will contain a [SearchFolder](http://msdn.microsoft.com/library/1a7d408b-2e98-4391-8834-085ed6d5757c%28Office.15%29.aspx) element.</span></span> <span data-ttu-id="02308-162">L’exemple de requête suivante recherche les 10 premiers dossiers dans le dossier de dossiers de recherche.</span><span class="sxs-lookup"><span data-stu-id="02308-162">The following request example finds the first 10 folders in the Search Folders folder.</span></span> 
  
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
    <m:FindFolder Traversal="Shallow">
      <m:FolderShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="folder:DisplayName" />
        </t:AdditionalProperties>
      </m:FolderShape>
      <m:IndexedPageFolderView MaxEntriesReturned="10" Offset="0" BasePoint="Beginning" />
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="searchfolders" />
      </m:ParentFolderIds>
    </m:FindFolder>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="02308-163">Le serveur renvoie la réponse suivante, qui indique un dossier de recherche.</span><span class="sxs-lookup"><span data-stu-id="02308-163">The server returns the following response, which shows one search folder.</span></span>
  
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
    <m:FindFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="3" TotalItemsInView="3" IncludesLastItemInRange="true">
            <t:Folders>
              <t:SearchFolder>
                <t:FolderId Id="AAMkAGM2..." ChangeKey="CAAAABYA..." />
                <t:DisplayName>From Manager</t:DisplayName>
              </t:SearchFolder>
            </t:Folders>
          </m:RootFolder>
        </m:FindFolderResponseMessage>
      </m:ResponseMessages>
    </m:FindFolderResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="02308-164">Une demande de l’exemple suivant utilise la valeur de l’élément [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) à partir de la réponse précédente dans une requête d’opération **GetFolder** pour obtenir le dossier de recherche.</span><span class="sxs-lookup"><span data-stu-id="02308-164">The following example of a request uses the value of the [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) element from the previous response in a **GetFolder** operation request to get the search folder.</span></span> 
  
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
    <m:GetFolder>
      <m:FolderShape>
        <t:BaseShape>AllProperties</t:BaseShape>
      </m:FolderShape>
      <m:FolderIds>
        <t:FolderId Id="AAMkAGM2..." ChangeKey="CAAAABYA..." />
      </m:FolderIds>
    </m:GetFolder>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="02308-165">Le serveur renvoie la réponse suivante avec toutes les propriétés de première classe pour le dossier de recherche.</span><span class="sxs-lookup"><span data-stu-id="02308-165">The server returns the following response with all the first-class properties for the search folder.</span></span>
  
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
    <m:GetFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:SearchFolder>
              <t:FolderId Id="AAMkAGM2..." ChangeKey="CAAAABYA..." />
              <t:ParentFolderId Id="AQMkAGM2..." ChangeKey="AQAAAA==" />
              <t:FolderClass>IPF.Note</t:FolderClass>
              <t:DisplayName>From Manager</t:DisplayName>
              <t:TotalCount>8</t:TotalCount>
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
              <t:SearchParameters Traversal="Deep">
                <t:Restriction>
                  <t:IsEqualTo>
                    <t:FieldURI FieldURI="message:Sender" />
                    <t:FieldURIOrConstant>
                      <t:Constant Value="/o=First Organization/ou=Exchange Administrative Group (FYDIBOHF23SPDLT)/cn=Recipients/cn=8d84a3f4cbb34d48838a3aecf99795c0-Sadie" />
                    </t:FieldURIOrConstant>
                  </t:IsEqualTo>
                </t:Restriction>
                <t:BaseFolderIds>
                  <t:FolderId Id="AQMkAGM2..." ChangeKey="AQAAAA==" />
                </t:BaseFolderIds>
              </t:SearchParameters>
            </t:SearchFolder>
          </m:Folders>
        </m:GetFolderResponseMessage>
      </m:ResponseMessages>
    </m:GetFolderResponse>
  </s:Body>
</s:Envelope>
```

## <a name="update-a-search-folder-by-using-the-ews-managed-api"></a><span data-ttu-id="02308-166">Mettre à jour un dossier de recherche à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="02308-166">Update a search folder by using the EWS Managed API</span></span>
<span data-ttu-id="02308-167"><a name="bk_UpdateEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="02308-167"></span></span>

<span data-ttu-id="02308-168">Utilisez la méthode d’API managées [Folder.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) sur un objet **SearchFolder** pour mettre à jour un dossier de recherche.</span><span class="sxs-lookup"><span data-stu-id="02308-168">Use the [Folder.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) EWS Managed API method on a **SearchFolder** object to update a search folder.</span></span> <span data-ttu-id="02308-169">L’exemple suivant met à jour les critères de recherche dans un dossier de recherche avec le nom complet « À partir du gestionnaire ».</span><span class="sxs-lookup"><span data-stu-id="02308-169">The following example updates the search criteria on a search folder with the display name "From Manager".</span></span> 
  
```cs
using Microsoft.Exchange.WebServices.Data;
static void UpdateSearchFolder(ExchangeService service)
{
    FolderView folderView = new FolderView(10);
    folderView.PropertySet = new PropertySet(FolderSchema.DisplayName);
    try
    {
        FindFoldersResults findResults = service.FindFolders(WellKnownFolderName.SearchFolders, folderView);
        foreach (Folder folder in findResults.Folders)
        {
            // You cannot request only search folders in 
            // a FindFolders request, so other search folders might also be present.
            if (folder is SearchFolder &amp;&amp; folder.DisplayName.Equals("From Manager"))
            {
                Console.WriteLine("\"{0}\" folder found.", folder.DisplayName);
                SearchFolder searchFolder = folder as SearchFolder;
                EmailAddress newManager = new EmailAddress("hope@contoso.com");
                SearchFilter.IsEqualTo newManagerFilter =
                    new SearchFilter.IsEqualTo(EmailMessageSchema.Sender, newManager);
                searchFolder.SearchParameters.SearchFilter = newManagerFilter;
                searchFolder.SearchParameters.RootFolderIds.Add(WellKnownFolderName.Inbox);
                searchFolder.SearchParameters.Traversal = SearchFolderTraversal.Deep;
                searchFolder.Update();
                Console.WriteLine("\"{0}\" folder updated.", folder.DisplayName);
            }
        }
    }
    catch (Exception ex)
    {
        Console.WriteLine("Exception while enumerating results: {0}", ex.Message);
    }
}
```

## <a name="update-a-search-folder-by-using-ews"></a><span data-ttu-id="02308-170">Mettre à jour un dossier de recherche à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="02308-170">Update a search folder by using EWS</span></span>
<span data-ttu-id="02308-171"><a name="bk_UpdateEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="02308-171"></span></span>

<span data-ttu-id="02308-172">Si vous utilisez EWS, utilisez l' [opération UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) avec un élément [SearchFolder](http://msdn.microsoft.com/library/1a7d408b-2e98-4391-8834-085ed6d5757c%28Office.15%29.aspx) pour mettre à jour un dossier de recherche.</span><span class="sxs-lookup"><span data-stu-id="02308-172">If you're using EWS, use the [UpdateFolder operation](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) with a [SearchFolder](http://msdn.microsoft.com/library/1a7d408b-2e98-4391-8834-085ed6d5757c%28Office.15%29.aspx) element to update a search folder.</span></span> <span data-ttu-id="02308-173">L’exemple de requête suivant met à jour les critères de recherche dans le dossier de recherche « À partir du gestionnaire ».</span><span class="sxs-lookup"><span data-stu-id="02308-173">The following request example updates the search criteria on the "From Manager" search folder.</span></span> 
  
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
    <m:UpdateFolder>
      <m:FolderChanges>
        <t:FolderChange>
          <t:FolderId Id="AAMkAGM2..." ChangeKey="CAAAABYA..." />
          <t:Updates>
            <t:SetFolderField>
              <t:FieldURI FieldURI="folder:SearchParameters" />
              <t:SearchFolder>
                <t:SearchParameters Traversal="Deep">
                  <t:Restriction>
                    <t:IsEqualTo>
                      <t:FieldURI FieldURI="message:Sender" />
                      <t:FieldURIOrConstant>
                        <t:Constant Value="hope@contoso.com" />
                      </t:FieldURIOrConstant>
                    </t:IsEqualTo>
                  </t:Restriction>
                  <t:BaseFolderIds>
                    <t:DistinguishedFolderId Id="inbox" />
                  </t:BaseFolderIds>
                </t:SearchParameters>
              </t:SearchFolder>
            </t:SetFolderField>
          </t:Updates>
        </t:FolderChange>
      </m:FolderChanges>
    </m:UpdateFolder>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="02308-174">Le serveur répond avec un message [UpdateFolderResponse](http://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx) qui contient une valeur [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, qui indique une réussite.</span><span class="sxs-lookup"><span data-stu-id="02308-174">The server responds with an [UpdateFolderResponse](http://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates success.</span></span>
  
## <a name="delete-a-search-folder-by-using-the-ews-managed-api"></a><span data-ttu-id="02308-175">Supprimer un dossier de recherche à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="02308-175">Delete a search folder by using the EWS Managed API</span></span>
<span data-ttu-id="02308-176"><a name="bk_DeleteEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="02308-176"></span></span>

<span data-ttu-id="02308-177">Pour supprimer un dossier de recherche, utilisez la méthode d’API managées [Folder.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) sur un objet **SearchFolder** .</span><span class="sxs-lookup"><span data-stu-id="02308-177">Use the [Folder.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) EWS Managed API method on a **SearchFolder** object to delete a search folder.</span></span> <span data-ttu-id="02308-178">L’exemple suivant supprime un dossier de recherche avec le nom complet « À partir du gestionnaire ».</span><span class="sxs-lookup"><span data-stu-id="02308-178">The following example deletes a search folder with the display name "From Manager".</span></span> <span data-ttu-id="02308-179">Le dossier de recherche supprimé est déplacé vers le dossier éléments supprimés.</span><span class="sxs-lookup"><span data-stu-id="02308-179">The deleted search folder is moved to the Deleted Items folder.</span></span> 
  
```cs
using Microsoft.Exchange.WebServices.Data;
static void DeleteSearchFolder(ExchangeService service)
{
    FolderView folderView = new FolderView(10);
    folderView.PropertySet = new PropertySet(FolderSchema.DisplayName);
    try
    {
        FindFoldersResults findResults = service.FindFolders(WellKnownFolderName.SearchFolders, folderView);
        foreach (Folder folder in findResults.Folders)
        {
            // You cannot request only search folders in 
            // a FindFolders request, so other folders might also be present.
            if (folder is SearchFolder &amp;&amp; folder.DisplayName.Equals("From Manager"))
            {
                Console.WriteLine("\"{0}\" folder found.", folder.DisplayName);
                folder.Delete(DeleteMode.MoveToDeletedItems);
                Console.WriteLine("\"{0}\" folder deleted.", folder.DisplayName);
            }
        }
    }
    catch (Exception ex)
    {
        Console.WriteLine("Exception while enumerating results: {0}", ex.Message);
    }
}
```

## <a name="delete-a-search-folder-by-using-ews"></a><span data-ttu-id="02308-180">Supprimer un dossier de recherche à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="02308-180">Delete a search folder by using EWS</span></span>
<span data-ttu-id="02308-181"><a name="bk_DeleteEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="02308-181"></span></span>

<span data-ttu-id="02308-182">Si vous utilisez EWS, utilisez l' [opération DeleteFolder](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) pour supprimer un dossier de recherche.</span><span class="sxs-lookup"><span data-stu-id="02308-182">If you're using EWS, use the [DeleteFolder operation](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) to delete a search folder.</span></span> <span data-ttu-id="02308-183">L’exemple suivant supprime un dossier de recherche et le déplace vers le dossier éléments supprimés.</span><span class="sxs-lookup"><span data-stu-id="02308-183">The following example deletes a search folder and moves it to the Deleted Items folder.</span></span> 
  
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
    <m:DeleteFolder DeleteType="MoveToDeletedItems">
      <m:FolderIds>
        <t:FolderId Id="AAMkAGM2..." ChangeKey="CAAAABYA..." />
      </m:FolderIds>
    </m:DeleteFolder>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="02308-184">Le serveur répond avec un message [DeleteFolderResponse](http://msdn.microsoft.com/library/27578bda-ef0a-4a33-bccc-2c1bc1735424%28Office.15%29.aspx) qui contient une valeur [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, qui indique une réussite.</span><span class="sxs-lookup"><span data-stu-id="02308-184">The server responds with a [DeleteFolderResponse](http://msdn.microsoft.com/library/27578bda-ef0a-4a33-bccc-2c1bc1735424%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates success.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="02308-185">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="02308-185">See also</span></span>


- [<span data-ttu-id="02308-186">Recherche et EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="02308-186">Search and EWS in Exchange</span></span>](search-and-ews-in-exchange.md)
    
- [<span data-ttu-id="02308-187">Utiliser des filtres de recherche avec EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="02308-187">Use search filters with EWS in Exchange</span></span>](how-to-use-search-filters-with-ews-in-exchange.md)
    
- [<span data-ttu-id="02308-188">Classe SearchFolder</span><span class="sxs-lookup"><span data-stu-id="02308-188">SearchFolder class</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="02308-189">Opération CreateFolder</span><span class="sxs-lookup"><span data-stu-id="02308-189">CreateFolder operation</span></span>](http://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx)
    
- [<span data-ttu-id="02308-190">Opération FindFolder</span><span class="sxs-lookup"><span data-stu-id="02308-190">FindFolder operation</span></span>](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)
    
- [<span data-ttu-id="02308-191">Opération GetFolder</span><span class="sxs-lookup"><span data-stu-id="02308-191">GetFolder operation</span></span>](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx)
    
- [<span data-ttu-id="02308-192">Opération UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="02308-192">UpdateFolder operation</span></span>](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx)
    
- [<span data-ttu-id="02308-193">Opération DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="02308-193">DeleteFolder operation</span></span>](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx)
    

