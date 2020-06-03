---
title: Utiliser des dossiers de recherche à l’aide d’EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: abe703c5-6d85-46d9-bf20-230c34782a9f
description: Découvrez comment créer, obtenir, mettre à jour et supprimer des dossiers de recherche à l’aide de l’API managée EWS ou d’EWS dans Exchange.
ms.openlocfilehash: 880c14bc99c4f6c674d4f7566036c4b8f5f19e55
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456366"
---
# <a name="work-with-search-folders-by-using-ews-in-exchange"></a><span data-ttu-id="4b956-103">Utiliser des dossiers de recherche à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="4b956-103">Work with search folders by using EWS in Exchange</span></span>

<span data-ttu-id="4b956-104">Découvrez comment créer, obtenir, mettre à jour et supprimer des dossiers de recherche à l’aide de l’API managée EWS ou d’EWS dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="4b956-104">Find out how to create, get, update, and delete search folders by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="4b956-105">Un dossier de recherche représente une recherche permanente « toujours active » dans la boîte aux lettres d’un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="4b956-105">A search folder represents a persistent "always-on" search in a user's mailbox.</span></span> <span data-ttu-id="4b956-106">Un dossier de recherche se présente et agit comme un dossier de boîte aux lettres ordinaire.</span><span class="sxs-lookup"><span data-stu-id="4b956-106">A search folder looks and acts like a regular mailbox folder.</span></span> <span data-ttu-id="4b956-107">Toutefois, au lieu de contenir des éléments, il contient une copie « virtuelle » des éléments des dossiers de son étendue de recherche qui correspondent aux critères de recherche définis sur le dossier.</span><span class="sxs-lookup"><span data-stu-id="4b956-107">However, instead of containing items, it contains a "virtual" copy of items from any folders in its search scope that match the search criteria set on the folder.</span></span> <span data-ttu-id="4b956-108">Les applications et les utilisateurs finaux peuvent utiliser des dossiers de recherche.</span><span class="sxs-lookup"><span data-stu-id="4b956-108">Both applications and end-users can use search folders.</span></span> <span data-ttu-id="4b956-109">Votre application doit-elle effectuer la même recherche sur et en plus ?</span><span class="sxs-lookup"><span data-stu-id="4b956-109">Does your application need to perform the same search over and over?</span></span> <span data-ttu-id="4b956-110">Les dossiers de recherche constituent un excellent outil pour cette tâche.</span><span class="sxs-lookup"><span data-stu-id="4b956-110">Search folders are a great tool for this task.</span></span> <span data-ttu-id="4b956-111">Ou vous voulez peut-être simplement donner à vos utilisateurs la possibilité d’accéder à des dossiers de recherche et de les gérer dans votre client.</span><span class="sxs-lookup"><span data-stu-id="4b956-111">Or maybe you just want to give your users the ability to access and manage search folders in your client.</span></span> <span data-ttu-id="4b956-112">Quel que soit votre scénario, l’API managée EWS et EWS permettent à votre application d’interagir pleinement avec les dossiers de recherche.</span><span class="sxs-lookup"><span data-stu-id="4b956-112">Whatever your scenario, the EWS Managed API and EWS enable your application to fully interact with search folders.</span></span>

> [!NOTE] 
> <span data-ttu-id="4b956-113">Cet article s’applique uniquement lors de l’utilisation d’Outlook en mode en ligne.</span><span class="sxs-lookup"><span data-stu-id="4b956-113">This article applies only when using Outlook in online mode.</span></span> <span data-ttu-id="4b956-114">Les dossiers de recherche ne sont pas synchronisés ; par conséquent, les dossiers de recherche créés en mode en ligne ne s’afficheront pas en mode mis en cache.</span><span class="sxs-lookup"><span data-stu-id="4b956-114">Search folders do not sync; therefore, search folders created in online mode will not appear in cached mode.</span></span>
  
<span data-ttu-id="4b956-115">**Tableau 1. Méthodes de l’API managée EWS et opérations EWS pour l’utilisation de dossiers de recherche**</span><span class="sxs-lookup"><span data-stu-id="4b956-115">**Table 1. EWS Managed API methods and EWS operations for working with search folders**</span></span>

|<span data-ttu-id="4b956-116">Si vous souhaitez...</span><span class="sxs-lookup"><span data-stu-id="4b956-116">If you want to…</span></span>|<span data-ttu-id="4b956-117">Dans l’API managée EWS, utilisez...</span><span class="sxs-lookup"><span data-stu-id="4b956-117">In the EWS Managed API, use…</span></span>|<span data-ttu-id="4b956-118">Dans EWS, utilisez...</span><span class="sxs-lookup"><span data-stu-id="4b956-118">In EWS, use…</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="4b956-119">Créer un dossier de recherche</span><span class="sxs-lookup"><span data-stu-id="4b956-119">Create a search folder</span></span>  <br/> |[<span data-ttu-id="4b956-120">SearchFolder. Save</span><span class="sxs-lookup"><span data-stu-id="4b956-120">SearchFolder.Save</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfolder.save%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="4b956-121">Opération CreateFolder</span><span class="sxs-lookup"><span data-stu-id="4b956-121">CreateFolder operation</span></span>](https://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="4b956-122">Obtenir un dossier de recherche</span><span class="sxs-lookup"><span data-stu-id="4b956-122">Get a search folder</span></span>  <br/> |[<span data-ttu-id="4b956-123">SearchFolder. bind</span><span class="sxs-lookup"><span data-stu-id="4b956-123">SearchFolder.Bind</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfolder.bind%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="4b956-124">Opération GetFolder</span><span class="sxs-lookup"><span data-stu-id="4b956-124">GetFolder operation</span></span>](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="4b956-125">Mettre à jour un dossier de recherche</span><span class="sxs-lookup"><span data-stu-id="4b956-125">Update a search folder</span></span>  <br/> |[<span data-ttu-id="4b956-126">SearchFolder. Update</span><span class="sxs-lookup"><span data-stu-id="4b956-126">SearchFolder.Update</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="4b956-127">Opération UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="4b956-127">UpdateFolder operation</span></span>](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="4b956-128">Supprimer un dossier de recherche</span><span class="sxs-lookup"><span data-stu-id="4b956-128">Delete a search folder</span></span>  <br/> |[<span data-ttu-id="4b956-129">SearchFolder. Delete</span><span class="sxs-lookup"><span data-stu-id="4b956-129">SearchFolder.Delete</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="4b956-130">Opération DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="4b956-130">DeleteFolder operation</span></span>](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |
   
## <a name="core-concepts-to-know-for-working-with-search-folders"></a><span data-ttu-id="4b956-131">Concepts de base à prendre en compte pour utiliser les dossiers de recherche</span><span class="sxs-lookup"><span data-stu-id="4b956-131">Core concepts to know for working with search folders</span></span>
<span data-ttu-id="4b956-132"><a name="bk_CoreConcepts"> </a></span><span class="sxs-lookup"><span data-stu-id="4b956-132"><a name="bk_CoreConcepts"> </a></span></span>

<span data-ttu-id="4b956-133">Avant de commencer à travailler avec des dossiers de recherche, vous devez être familiarisé avec le fonctionnement des filtres de recherche.</span><span class="sxs-lookup"><span data-stu-id="4b956-133">Before you start working with search folders, you'll want to be familiar with how search filters work.</span></span> <span data-ttu-id="4b956-134">Les dossiers de recherche s’appuient sur des filtres de recherche pour exprimer leurs critères.</span><span class="sxs-lookup"><span data-stu-id="4b956-134">Search folders rely on search filters to express their criteria.</span></span> <span data-ttu-id="4b956-135">Les filtres de recherche pour les dossiers de recherche sont construits de la même manière que les [filtres de recherche pour les opérations de recherche](how-to-use-search-filters-with-ews-in-exchange.md) .</span><span class="sxs-lookup"><span data-stu-id="4b956-135">Search filters for search folders are constructed in the same way that [search filters for search operations](how-to-use-search-filters-with-ews-in-exchange.md) are constructed.</span></span> 
  
## <a name="create-a-search-folder-by-using-the-ews-managed-api"></a><span data-ttu-id="4b956-136">Créer un dossier de recherche à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="4b956-136">Create a search folder by using the EWS Managed API</span></span>
<span data-ttu-id="4b956-137"><a name="bk_CreateEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="4b956-137"><a name="bk_CreateEWSMA"> </a></span></span>

<span data-ttu-id="4b956-138">Fondamentalement, vous créez un dossier de recherche à l’aide de l’API managée EWS de la même façon que vous créez un dossier normal.</span><span class="sxs-lookup"><span data-stu-id="4b956-138">Basically, you create a search folder using the EWS Managed API in the same way that you create a regular folder.</span></span> <span data-ttu-id="4b956-139">Toutefois, au lieu d’utiliser la [classe Folder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx), vous utilisez la [classe SearchFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx)et vous définissez la [propriété SearchParameters](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfolder.searchparameters%28v=exchg.80%29.aspx) pour configurer les critères de recherche.</span><span class="sxs-lookup"><span data-stu-id="4b956-139">However, instead of using the [Folder class](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx), you use the [SearchFolder class](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx), and set the [SearchParameters property](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfolder.searchparameters%28v=exchg.80%29.aspx) to configure the search criteria.</span></span> 
  
<span data-ttu-id="4b956-140">Dans l’exemple suivant, un dossier de recherche est créé pour rechercher tous les messages dans la boîte de réception et ses sous-dossiers qui ont été envoyés par le responsable de l’utilisateur, sadie@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="4b956-140">In the following example, a search folder is created to find all messages in the Inbox and its subfolders that were sent by the user's manager, sadie@contoso.com.</span></span> <span data-ttu-id="4b956-141">Le dossier est créé en tant qu’enfant du dossier dossiers de recherche dans la boîte aux lettres de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="4b956-141">The folder is created as a child of the Search Folders folder in the user's mailbox.</span></span>
  
> [!NOTE]
> <span data-ttu-id="4b956-142">Vous pouvez créer un dossier de recherche en tant qu’enfant d’un dossier dans la boîte aux lettres de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="4b956-142">You can create a search folder as a child of any folder in the user's mailbox.</span></span> <span data-ttu-id="4b956-143">Toutefois, si vous souhaitez que le dossier nouvellement créé s’affiche sous dossiers de recherche dans Outlook, créez-le sous le dossier connu des dossiers de recherche, à l’aide de la valeur **SearchFolders** de l' [énumération WellKnownFolderName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="4b956-143">However, if you want the newly created folder to show up under Search Folders in Outlook, create it under the Search Folders well-known folder, using the **SearchFolders** value of the [WellKnownFolderName enumeration](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx).</span></span> 
  
<span data-ttu-id="4b956-144">Cet exemple part du principe que l’objet **ExchangeService** a été initialisé avec des valeurs valides dans les [informations d’identification](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) et les propriétés de l' [URL](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="4b956-144">This example assumes that the **ExchangeService** object has been initialized with valid values in the [Credentials](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) and [Url](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) properties.</span></span> 
  
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

## <a name="create-a-search-folder-by-using-ews"></a><span data-ttu-id="4b956-145">Créer un dossier de recherche à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="4b956-145">Create a search folder by using EWS</span></span>
<span data-ttu-id="4b956-146"><a name="bk_CreateEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="4b956-146"><a name="bk_CreateEWS"> </a></span></span>

<span data-ttu-id="4b956-147">Si vous utilisez EWS, utilisez l' [opération CreateFolder](https://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) avec un élément [SearchFolder](https://msdn.microsoft.com/library/1a7d408b-2e98-4391-8834-085ed6d5757c%28Office.15%29.aspx) pour créer un dossier de recherche.</span><span class="sxs-lookup"><span data-stu-id="4b956-147">If you are using EWS, use the [CreateFolder operation](https://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) with a [SearchFolder](https://msdn.microsoft.com/library/1a7d408b-2e98-4391-8834-085ed6d5757c%28Office.15%29.aspx) element to create a search folder.</span></span> <span data-ttu-id="4b956-148">Dans l’exemple de requête suivant, un dossier de recherche est créé pour rechercher tous les messages dans la boîte de réception et ses sous-dossiers qui ont été envoyés par le responsable de l’utilisateur, sadie@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="4b956-148">In the following request example, a search folder is created to find all messages in the Inbox and its subfolders that were sent by the user's manager, sadie@contoso.com.</span></span> <span data-ttu-id="4b956-149">Le dossier est créé dans le dossier dossiers de recherche de la boîte aux lettres de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="4b956-149">The folder is created in the Search Folders folder in the user's mailbox.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="4b956-150">Vous pouvez créer un dossier de recherche en tant qu’enfant d’un dossier dans la boîte aux lettres de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="4b956-150">You can create a search folder as a child of any folder in the user's mailbox.</span></span> <span data-ttu-id="4b956-151">Toutefois, si vous souhaitez que le dossier nouvellement créé s’affiche sous dossiers de recherche dans Outlook, créez-le sous le dossier connu des dossiers de recherche, à l’aide de la valeur **SearchFolders** dans l’attribut **ID** de l’élément [DistinguishedFolderId](https://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="4b956-151">However, if you want the newly created folder to show up under Search Folders in Outlook, create it under the Search Folders well-known folder, using the **searchfolders** value in the **Id** attribute of the [DistinguishedFolderId](https://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) element.</span></span> 
  
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

<span data-ttu-id="4b956-152">Le serveur répond avec un message [CreateFolderResponse](https://msdn.microsoft.com/library/158adecc-491a-47d9-af73-acc2cd3f8566%28Office.15%29.aspx) qui inclut une valeur [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NOERROR**, ce qui indique la réussite.</span><span class="sxs-lookup"><span data-stu-id="4b956-152">The server responds with a [CreateFolderResponse](https://msdn.microsoft.com/library/158adecc-491a-47d9-af73-acc2cd3f8566%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates success.</span></span>
  
## <a name="get-a-search-folder-by-using-the-ews-managed-api"></a><span data-ttu-id="4b956-153">Obtenir un dossier de recherche à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="4b956-153">Get a search folder by using the EWS Managed API</span></span>
<span data-ttu-id="4b956-154"><a name="bk_RetrieveEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="4b956-154"><a name="bk_RetrieveEWSMA"> </a></span></span>

<span data-ttu-id="4b956-155">Utilisez la méthode de l’API managée EWS [ExchangeService. FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx) pour rechercher des dossiers de recherche.</span><span class="sxs-lookup"><span data-stu-id="4b956-155">Use the [ExchangeService.FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx) EWS Managed API method to find search folders.</span></span> <span data-ttu-id="4b956-156">Notez toutefois que vous ne pouvez pas limiter vos résultats à inclure uniquement les dossiers de recherche ; n’oubliez pas que vous devez garder ces résultats à l’esprit lorsque vous traitez les résultats.</span><span class="sxs-lookup"><span data-stu-id="4b956-156">Note, however, that you can't limit your results to only include search folders; you'll want to keep that in mind when you process the results.</span></span> <span data-ttu-id="4b956-157">Utilisez la méthode [SearchFolder. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfolder.bind%28v=exchg.80%29.aspx) pour obtenir des dossiers de recherche.</span><span class="sxs-lookup"><span data-stu-id="4b956-157">Use the [SearchFolder.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfolder.bind%28v=exchg.80%29.aspx) method to get search folders.</span></span> 
  
<span data-ttu-id="4b956-158">L’exemple suivant recherche les 10 premiers dossiers dans le dossier de dossiers de recherche.</span><span class="sxs-lookup"><span data-stu-id="4b956-158">The following example finds the first 10 folders in the Search Folders folder.</span></span> <span data-ttu-id="4b956-159">Il vérifie s’il s’agit d’un dossier de recherche et, si c’est le cas, il obtient le dossier de recherche et affiche le nombre de dossiers cibles qu’il recherche.</span><span class="sxs-lookup"><span data-stu-id="4b956-159">It checks to determine whether each one is a search folder, and if so, it gets the search folder and displays how many target folders it searches.</span></span>
  
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

## <a name="get-a-search-folder-by-using-ews"></a><span data-ttu-id="4b956-160">Obtenir un dossier de recherche à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="4b956-160">Get a search folder by using EWS</span></span>
<span data-ttu-id="4b956-161"><a name="bk_RetrieveEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="4b956-161"><a name="bk_RetrieveEWS"> </a></span></span>

<span data-ttu-id="4b956-162">Si vous utilisez EWS, utilisez l' [opération FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) pour rechercher des dossiers de recherche et l' [opération GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) pour obtenir des dossiers de recherche.</span><span class="sxs-lookup"><span data-stu-id="4b956-162">If you're using EWS, use the [FindFolder operation](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) to find search folders, and the [GetFolder operation](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) to get search folders.</span></span> <span data-ttu-id="4b956-163">Une réponse **GetFolder** réussie pour un dossier de recherche contient un élément [SearchFolder](https://msdn.microsoft.com/library/1a7d408b-2e98-4391-8834-085ed6d5757c%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="4b956-163">A successful **GetFolder** response for a search folder will contain a [SearchFolder](https://msdn.microsoft.com/library/1a7d408b-2e98-4391-8834-085ed6d5757c%28Office.15%29.aspx) element.</span></span> <span data-ttu-id="4b956-164">L’exemple de requête suivant recherche les 10 premiers dossiers dans le dossier de dossiers de recherche.</span><span class="sxs-lookup"><span data-stu-id="4b956-164">The following request example finds the first 10 folders in the Search Folders folder.</span></span> 
  
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

<span data-ttu-id="4b956-165">Le serveur renvoie la réponse suivante, qui affiche un dossier de recherche.</span><span class="sxs-lookup"><span data-stu-id="4b956-165">The server returns the following response, which shows one search folder.</span></span>
  
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
    <m:FindFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="4b956-166">L’exemple de requête suivant utilise la valeur de l’élément [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) de la réponse précédente dans une demande d’opération **GetFolder** pour obtenir le dossier de recherche.</span><span class="sxs-lookup"><span data-stu-id="4b956-166">The following example of a request uses the value of the [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) element from the previous response in a **GetFolder** operation request to get the search folder.</span></span> 
  
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

<span data-ttu-id="4b956-167">Le serveur renvoie la réponse suivante avec toutes les propriétés de première classe du dossier de recherche.</span><span class="sxs-lookup"><span data-stu-id="4b956-167">The server returns the following response with all the first-class properties for the search folder.</span></span>
  
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
    <m:GetFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="update-a-search-folder-by-using-the-ews-managed-api"></a><span data-ttu-id="4b956-168">Mettre à jour un dossier de recherche à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="4b956-168">Update a search folder by using the EWS Managed API</span></span>
<span data-ttu-id="4b956-169"><a name="bk_UpdateEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="4b956-169"><a name="bk_UpdateEWSMA"> </a></span></span>

<span data-ttu-id="4b956-170">Utilisez le [dossier. mettre à](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) jour la méthode d’API managée EWS sur un objet **SearchFolder** pour mettre à jour un dossier de recherche.</span><span class="sxs-lookup"><span data-stu-id="4b956-170">Use the [Folder.Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) EWS Managed API method on a **SearchFolder** object to update a search folder.</span></span> <span data-ttu-id="4b956-171">L’exemple suivant met à jour les critères de recherche sur un dossier de recherche dont le nom complet est « à partir du gestionnaire ».</span><span class="sxs-lookup"><span data-stu-id="4b956-171">The following example updates the search criteria on a search folder with the display name "From Manager".</span></span> 
  
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

## <a name="update-a-search-folder-by-using-ews"></a><span data-ttu-id="4b956-172">Mettre à jour un dossier de recherche à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="4b956-172">Update a search folder by using EWS</span></span>
<span data-ttu-id="4b956-173"><a name="bk_UpdateEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="4b956-173"><a name="bk_UpdateEWS"> </a></span></span>

<span data-ttu-id="4b956-174">Si vous utilisez EWS, utilisez l' [opération UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) avec un élément [SearchFolder](https://msdn.microsoft.com/library/1a7d408b-2e98-4391-8834-085ed6d5757c%28Office.15%29.aspx) pour mettre à jour un dossier de recherche.</span><span class="sxs-lookup"><span data-stu-id="4b956-174">If you're using EWS, use the [UpdateFolder operation](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) with a [SearchFolder](https://msdn.microsoft.com/library/1a7d408b-2e98-4391-8834-085ed6d5757c%28Office.15%29.aspx) element to update a search folder.</span></span> <span data-ttu-id="4b956-175">L’exemple de requête suivant met à jour les critères de recherche dans le dossier de recherche « à partir du gestionnaire ».</span><span class="sxs-lookup"><span data-stu-id="4b956-175">The following request example updates the search criteria on the "From Manager" search folder.</span></span> 
  
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

<span data-ttu-id="4b956-176">Le serveur répond avec un message [UpdateFolderResponse](https://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx) qui inclut une valeur [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NOERROR**, ce qui indique la réussite.</span><span class="sxs-lookup"><span data-stu-id="4b956-176">The server responds with an [UpdateFolderResponse](https://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates success.</span></span>
  
## <a name="delete-a-search-folder-by-using-the-ews-managed-api"></a><span data-ttu-id="4b956-177">Supprimer un dossier de recherche à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="4b956-177">Delete a search folder by using the EWS Managed API</span></span>
<span data-ttu-id="4b956-178"><a name="bk_DeleteEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="4b956-178"><a name="bk_DeleteEWSMA"> </a></span></span>

<span data-ttu-id="4b956-179">Utilisez le [dossier. Supprimez](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) la méthode de l’API managée EWS sur un objet **SearchFolder** pour supprimer un dossier de recherche.</span><span class="sxs-lookup"><span data-stu-id="4b956-179">Use the [Folder.Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) EWS Managed API method on a **SearchFolder** object to delete a search folder.</span></span> <span data-ttu-id="4b956-180">L’exemple suivant montre comment supprimer un dossier de recherche dont le nom d’affichage est « from Manager ».</span><span class="sxs-lookup"><span data-stu-id="4b956-180">The following example deletes a search folder with the display name "From Manager".</span></span> <span data-ttu-id="4b956-181">Le dossier de recherche supprimé est déplacé vers le dossier éléments supprimés.</span><span class="sxs-lookup"><span data-stu-id="4b956-181">The deleted search folder is moved to the Deleted Items folder.</span></span> 
  
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

## <a name="delete-a-search-folder-by-using-ews"></a><span data-ttu-id="4b956-182">Supprimer un dossier de recherche à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="4b956-182">Delete a search folder by using EWS</span></span>
<span data-ttu-id="4b956-183"><a name="bk_DeleteEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="4b956-183"><a name="bk_DeleteEWS"> </a></span></span>

<span data-ttu-id="4b956-184">Si vous utilisez EWS, utilisez l' [opération DeleteFolder](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) pour supprimer un dossier de recherche.</span><span class="sxs-lookup"><span data-stu-id="4b956-184">If you're using EWS, use the [DeleteFolder operation](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) to delete a search folder.</span></span> <span data-ttu-id="4b956-185">L’exemple suivant supprime un dossier de recherche et le déplace vers le dossier éléments supprimés.</span><span class="sxs-lookup"><span data-stu-id="4b956-185">The following example deletes a search folder and moves it to the Deleted Items folder.</span></span> 
  
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
    <m:DeleteFolder DeleteType="MoveToDeletedItems">
      <m:FolderIds>
        <t:FolderId Id="AAMkAGM2..." ChangeKey="CAAAABYA..." />
      </m:FolderIds>
    </m:DeleteFolder>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="4b956-186">Le serveur répond avec un message [DeleteFolderResponse](https://msdn.microsoft.com/library/27578bda-ef0a-4a33-bccc-2c1bc1735424%28Office.15%29.aspx) qui inclut une valeur [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NOERROR**, ce qui indique la réussite.</span><span class="sxs-lookup"><span data-stu-id="4b956-186">The server responds with a [DeleteFolderResponse](https://msdn.microsoft.com/library/27578bda-ef0a-4a33-bccc-2c1bc1735424%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates success.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="4b956-187">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4b956-187">See also</span></span>

- [<span data-ttu-id="4b956-188">Recherche et EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="4b956-188">Search and EWS in Exchange</span></span>](search-and-ews-in-exchange.md)   
- [<span data-ttu-id="4b956-189">Utiliser des filtres de recherche avec EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="4b956-189">Use search filters with EWS in Exchange</span></span>](how-to-use-search-filters-with-ews-in-exchange.md)    
- [<span data-ttu-id="4b956-190">Classe SearchFolder</span><span class="sxs-lookup"><span data-stu-id="4b956-190">SearchFolder class</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx)    
- [<span data-ttu-id="4b956-191">Opération CreateFolder</span><span class="sxs-lookup"><span data-stu-id="4b956-191">CreateFolder operation</span></span>](https://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx)    
- [<span data-ttu-id="4b956-192">Opération FindFolder</span><span class="sxs-lookup"><span data-stu-id="4b956-192">FindFolder operation</span></span>](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)   
- [<span data-ttu-id="4b956-193">Opération GetFolder</span><span class="sxs-lookup"><span data-stu-id="4b956-193">GetFolder operation</span></span>](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx)    
- [<span data-ttu-id="4b956-194">Opération UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="4b956-194">UpdateFolder operation</span></span>](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx)    
- [<span data-ttu-id="4b956-195">Opération DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="4b956-195">DeleteFolder operation</span></span>](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx)
    

