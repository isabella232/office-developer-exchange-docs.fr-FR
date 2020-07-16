---
title: Utiliser des dossiers à l’aide d’EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 4b3eb746-74c4-42a0-aa2c-742c147f1871
description: Découvrez comment créer, obtenir, mettre à jour et supprimer des dossiers à l’aide de l’API managée EWS ou d’EWS dans Exchange.
localization_priority: Priority
ms.openlocfilehash: a184d8da4d6949f01f47afc6a9fb7ed30729fd3b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456380"
---
# <a name="work-with-folders-by-using-ews-in-exchange"></a><span data-ttu-id="ab7eb-103">Utiliser des dossiers à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ab7eb-103">Work with folders by using EWS in Exchange</span></span>

<span data-ttu-id="ab7eb-104">Découvrez comment créer, obtenir, mettre à jour et supprimer des dossiers à l’aide de l’API managée EWS ou d’EWS dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="ab7eb-104">Learn how to create, get, update, and delete folders by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="ab7eb-105">EWS dans Exchange utilise des dossiers pour structurer et organiser les boîtes aux lettres.</span><span class="sxs-lookup"><span data-stu-id="ab7eb-105">EWS in Exchange uses folders to structure and organize mailboxes.</span></span> <span data-ttu-id="ab7eb-106">Vous pouvez créer de nouveaux dossiers, obtenir, mettre à jour et supprimer des dossiers à l’aide de l’API managée EWS ou d’EWS.</span><span class="sxs-lookup"><span data-stu-id="ab7eb-106">You can create new, get, update, and delete folders by using the EWS Managed API or EWS.</span></span> <span data-ttu-id="ab7eb-107">Chacune des méthodes ou opérations indiquées dans le tableau suivant est exécutée sur un objet [Folder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx) , un type [Folder](https://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) ou l' [une des classes ou types de dossier dérivés](folders-and-items-in-ews-in-exchange.md#bk_folders).</span><span class="sxs-lookup"><span data-stu-id="ab7eb-107">Each of the methods or operations listed in the following table is performed on a [Folder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx) object, a [Folder](https://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) type, or [one of the derived folder classes or types](folders-and-items-in-ews-in-exchange.md#bk_folders).</span></span>
  
<span data-ttu-id="ab7eb-108">**Tableau 1. Méthodes et opérations de création, d’obtention, de mise à jour et de suppression de dossiers**</span><span class="sxs-lookup"><span data-stu-id="ab7eb-108">**Table 1. Methods and operations for creating, getting, updating and deleting folders**</span></span>

|<span data-ttu-id="ab7eb-109">**Afin de...**</span><span class="sxs-lookup"><span data-stu-id="ab7eb-109">**In order to…**</span></span>|<span data-ttu-id="ab7eb-110">**Méthode d'API managée EWS**</span><span class="sxs-lookup"><span data-stu-id="ab7eb-110">**EWS Managed API method**</span></span>|<span data-ttu-id="ab7eb-111">**Opération EWS**</span><span class="sxs-lookup"><span data-stu-id="ab7eb-111">**EWS operation**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="ab7eb-112">Créer un dossier</span><span class="sxs-lookup"><span data-stu-id="ab7eb-112">Create a folder</span></span>  <br/> |[<span data-ttu-id="ab7eb-113">Folder. Save</span><span class="sxs-lookup"><span data-stu-id="ab7eb-113">Folder.Save</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.save%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="ab7eb-114">CreateFolder</span><span class="sxs-lookup"><span data-stu-id="ab7eb-114">CreateFolder</span></span>](https://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="ab7eb-115">Créer une hiérarchie de dossiers</span><span class="sxs-lookup"><span data-stu-id="ab7eb-115">Create a folder hierarchy</span></span>  <br/> |<span data-ttu-id="ab7eb-116">Non disponible</span><span class="sxs-lookup"><span data-stu-id="ab7eb-116">Not available</span></span>  <br/> |[<span data-ttu-id="ab7eb-117">CreateFolderPath</span><span class="sxs-lookup"><span data-stu-id="ab7eb-117">CreateFolderPath</span></span>](https://msdn.microsoft.com/library/5a10aa5e-3f25-4ec3-a0b9-284c30918a1f%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="ab7eb-118">Obtenir un dossier</span><span class="sxs-lookup"><span data-stu-id="ab7eb-118">Get a folder</span></span>  <br/> |[<span data-ttu-id="ab7eb-119">Folder. bind</span><span class="sxs-lookup"><span data-stu-id="ab7eb-119">Folder.Bind</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="ab7eb-120">GetFolder</span><span class="sxs-lookup"><span data-stu-id="ab7eb-120">GetFolder</span></span>](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="ab7eb-121">Obtenir une hiérarchie de dossiers</span><span class="sxs-lookup"><span data-stu-id="ab7eb-121">Get a folder hierarchy</span></span>  <br/> |[<span data-ttu-id="ab7eb-122">Folder. FindFolders</span><span class="sxs-lookup"><span data-stu-id="ab7eb-122">Folder.FindFolders</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="ab7eb-123">FindFolder</span><span class="sxs-lookup"><span data-stu-id="ab7eb-123">FindFolder</span></span>](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="ab7eb-124">Mettre à jour un dossier</span><span class="sxs-lookup"><span data-stu-id="ab7eb-124">Update a folder</span></span>  <br/> |[<span data-ttu-id="ab7eb-125">Folder. Update</span><span class="sxs-lookup"><span data-stu-id="ab7eb-125">Folder.Update</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="ab7eb-126">UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="ab7eb-126">UpdateFolder</span></span>](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="ab7eb-127">Supprimer un dossier</span><span class="sxs-lookup"><span data-stu-id="ab7eb-127">Delete a folder</span></span>  <br/> |[<span data-ttu-id="ab7eb-128">Folder. Delete</span><span class="sxs-lookup"><span data-stu-id="ab7eb-128">Folder.Delete</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="ab7eb-129">DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="ab7eb-129">DeleteFolder</span></span>](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |

<span data-ttu-id="ab7eb-130"><a name="bk_createfolderewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="ab7eb-130"><a name="bk_createfolderewsma"> </a></span></span>

## <a name="create-a-folder-by-using-the-ews-managed-api"></a><span data-ttu-id="ab7eb-131">Créer un dossier à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="ab7eb-131">Create a folder by using the EWS Managed API</span></span>

<span data-ttu-id="ab7eb-132">L’exemple de code suivant montre comment utiliser la classe [Folder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx) pour créer un nouveau dossier générique avec un [DisplayName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.displayname%28v=exchg.80%29.aspx) de « Custom Folder » et une valeur de propriété [FolderClass](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.folderclass%28v=exchg.80%29.aspx) de IPF. Note.</span><span class="sxs-lookup"><span data-stu-id="ab7eb-132">The following code example shows how to use the [Folder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx) class to create a new generic folder with a [DisplayName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.displayname%28v=exchg.80%29.aspx) of "Custom Folder" and a [FolderClass](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.folderclass%28v=exchg.80%29.aspx) property value of IPF.Note.</span></span> <span data-ttu-id="ab7eb-133">La méthode [Folder. Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.save%28v=exchg.80%29.aspx) enregistre le dossier en tant que dossier enfant du dossier boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="ab7eb-133">The [Folder.Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.save%28v=exchg.80%29.aspx) method saves the folder as a child folder of the Inbox folder.</span></span> 
  
<span data-ttu-id="ab7eb-134">Ces exemples supposent que le **service** est un objet [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur a été authentifié auprès d’un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="ab7eb-134">These examples assume that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
// Create a custom folder.
Folder folder = new Folder(service);
folder.DisplayName = "Custom Folder";
folder.FolderClass = "IPF.Note";
// Save the folder as a child folder of the Inbox.
folder.Save(WellKnownFolderName.Inbox);
```

<span data-ttu-id="ab7eb-135">Pour créer un autre type de dossier, tel qu’un [CalendarFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.calendarfolder%28v=exchg.80%29.aspx), [ContactsFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contactsfolder%28v=exchg.80%29.aspx), [SearchFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx)ou [TasksFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.tasksfolder%28v=exchg.80%29.aspx), créez une instance de la classe spécifique (au lieu de la classe de **dossier** générique) et ne définissez pas la propriété **FolderClass** .</span><span class="sxs-lookup"><span data-stu-id="ab7eb-135">To create a different type of folder, such as a [CalendarFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.calendarfolder%28v=exchg.80%29.aspx), [ContactsFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contactsfolder%28v=exchg.80%29.aspx), [SearchFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx), or [TasksFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.tasksfolder%28v=exchg.80%29.aspx), create a new instance of the specific class (instead of the generic **Folder** class) and do not set the **FolderClass** property.</span></span> <span data-ttu-id="ab7eb-136">Par exemple, l’exemple de code suivant montre comment créer un nouveau [TasksFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.tasksfolder%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="ab7eb-136">For example, the following code example shows how to create a new [TasksFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.tasksfolder%28v=exchg.80%29.aspx).</span></span>
  
```cs
// Create a custom Tasks folder.
TasksFolder folder = new TasksFolder(service);
folder.DisplayName = "Custom Tasks";
// Save the folder as a child folder in the Inbox folder.
// This method call results in a CreateFolder call to EWS.
folder.Save(WellKnownFolderName.Inbox);
```

<span data-ttu-id="ab7eb-137">Si vous essayez de créer une instance d’une classe spécifique et que vous définissez également la propriété **FolderClass** , l’erreur [ErrorNoFolderClassOverride](https://msdn.microsoft.com/library/exchangewebservices.responsecodetype%28v=exchg.80%29.aspx) est générée.</span><span class="sxs-lookup"><span data-stu-id="ab7eb-137">If you try to create an instance of a specific class and also set the **FolderClass** property, the [ErrorNoFolderClassOverride](https://msdn.microsoft.com/library/exchangewebservices.responsecodetype%28v=exchg.80%29.aspx) error is thrown.</span></span> 
  
<span data-ttu-id="ab7eb-138">Notez que vous ne pouvez pas créer par lots la création de plusieurs dossiers dans un seul appel de méthode à l’aide de l’API managée EWS.</span><span class="sxs-lookup"><span data-stu-id="ab7eb-138">Note that you cannot batch the creation of multiple folders in a single method call by using the EWS Managed API.</span></span>
  
## <a name="create-a-folder-by-using-ews"></a><span data-ttu-id="ab7eb-139">Créer un dossier à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="ab7eb-139">Create a folder by using EWS</span></span>
<span data-ttu-id="ab7eb-140"><a name="bk_createfolderews"> </a></span><span class="sxs-lookup"><span data-stu-id="ab7eb-140"><a name="bk_createfolderews"> </a></span></span>

<span data-ttu-id="ab7eb-141">Vous pouvez créer un seul dossier ou plusieurs dossiers à l’aide d’EWS.</span><span class="sxs-lookup"><span data-stu-id="ab7eb-141">You can create a single folder or multiple of folders by using EWS.</span></span>
  
<span data-ttu-id="ab7eb-142">Pour créer un dossier unique, envoyez un message de demande d’opération [CreateFolder](https://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="ab7eb-142">To create a single folder, send a [CreateFolder](https://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) operation request message.</span></span> <span data-ttu-id="ab7eb-143">La demande d’opération **CreateFolder** indique que le dossier parent est la boîte de réception, que [DisplayName](https://msdn.microsoft.com/library/e7efbbe1-6629-4d11-bed1-ed899e3f9d77%28Office.15%29.aspx) est « dossier personnalisé » et que la valeur de l’élément [FolderClass](https://msdn.microsoft.com/library/0041d135-2869-4612-89a5-d1aa86aa1093%28Office.15%29.aspx) est IPF. Note.</span><span class="sxs-lookup"><span data-stu-id="ab7eb-143">The **CreateFolder** operation request indicates that the parent folder is the Inbox, the [DisplayName](https://msdn.microsoft.com/library/e7efbbe1-6629-4d11-bed1-ed899e3f9d77%28Office.15%29.aspx) is "Custom Folder", and the [FolderClass](https://msdn.microsoft.com/library/0041d135-2869-4612-89a5-d1aa86aa1093%28Office.15%29.aspx) element value is IPF.Note.</span></span> 
  
<span data-ttu-id="ab7eb-144">Il s’agit également de la demande XML que l’API managée EWS envoie lorsque vous créez un nouveau dossier et appelez la méthode [Folder. Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.save%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="ab7eb-144">This is also the XML request that the EWS Managed API sends when you create a new folder and call the [Folder.Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.save%28v=exchg.80%29.aspx) method.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:CreateFolder>
      <m:ParentFolderId>
        <t:DistinguishedFolderId Id="inbox" />
      </m:ParentFolderId>
      <m:Folders>
        <t:Folder>
          <t:FolderClass>IPF.Note</t:FolderClass>
          <t:DisplayName>Custom Folder</t:DisplayName>
        </t:Folder>
      </m:Folders>
    </m:CreateFolder>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="ab7eb-145">Le serveur répond à la demande **CreateFolder** avec un message [CreateFolderResponse](https://msdn.microsoft.com/library/158adecc-491a-47d9-af73-acc2cd3f8566%28Office.15%29.aspx) qui inclut une valeur [ResponseCode](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) de **NOERROR**, ce qui indique que le dossier a été créé avec succès et le [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) du message nouvellement créé.</span><span class="sxs-lookup"><span data-stu-id="ab7eb-145">The server responds to the **CreateFolder** request with a [CreateFolderResponse](https://msdn.microsoft.com/library/158adecc-491a-47d9-af73-acc2cd3f8566%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the folder was created successfully, and the [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) of the newly created message.</span></span> 
  
<span data-ttu-id="ab7eb-146">Pour créer plusieurs dossiers, incluez plusieurs éléments de [dossier](https://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) dans le message de demande d’opération **CreateFolder** .</span><span class="sxs-lookup"><span data-stu-id="ab7eb-146">To create multiple folders, include multiple [Folder](https://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) elements in the **CreateFolder** operation request message.</span></span> <span data-ttu-id="ab7eb-147">Tous les nouveaux dossiers doivent se trouver dans le même dossier parent.</span><span class="sxs-lookup"><span data-stu-id="ab7eb-147">All the new folders must be in the same parent folder.</span></span> 
  
## <a name="create-a-folder-hierarchy-by-using-ews"></a><span data-ttu-id="ab7eb-148">Créer une hiérarchie de dossiers à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="ab7eb-148">Create a folder hierarchy by using EWS</span></span>
<span data-ttu-id="ab7eb-149"><a name="bk_createfolderhierarchy"> </a></span><span class="sxs-lookup"><span data-stu-id="ab7eb-149"><a name="bk_createfolderhierarchy"> </a></span></span>

<span data-ttu-id="ab7eb-150">Vous pouvez créer une hiérarchie de dossiers dans un seul appel à l’aide de l’opération EWS [CreateFolderPath](https://msdn.microsoft.com/library/5a10aa5e-3f25-4ec3-a0b9-284c30918a1f%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="ab7eb-150">You can create a folder hierarchy in a single call by using the EWS [CreateFolderPath](https://msdn.microsoft.com/library/5a10aa5e-3f25-4ec3-a0b9-284c30918a1f%28Office.15%29.aspx) operation.</span></span> <span data-ttu-id="ab7eb-151">Les mêmes fonctionnalités ne sont pas disponibles dans l’API managée EWS.</span><span class="sxs-lookup"><span data-stu-id="ab7eb-151">The same functionality is not available in the EWS Managed API.</span></span> <span data-ttu-id="ab7eb-152">Au lieu de cela, si vous utilisez l’API managée EWS, vous pouvez créer des dossiers un par un, comme illustré dans [créer un dossier à l’aide d’EWS](#bk_createfolderews).</span><span class="sxs-lookup"><span data-stu-id="ab7eb-152">Instead, if you are using the EWS Managed API, you can create folders one by one, as shown in [Create a folder by using EWS](#bk_createfolderews).</span></span>
  
> [!NOTE]
> <span data-ttu-id="ab7eb-153">L’API managée EWS n’implémente pas cette fonctionnalité.</span><span class="sxs-lookup"><span data-stu-id="ab7eb-153">The EWS Managed API does not implement this functionality.</span></span> 
  
## <a name="get-a-folder-by-using-the-ews-managed-api"></a><span data-ttu-id="ab7eb-154">Obtenir un dossier à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="ab7eb-154">Get a folder by using the EWS Managed API</span></span>
<span data-ttu-id="ab7eb-155"><a name="bk_getfolderewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="ab7eb-155"><a name="bk_getfolderewsma"> </a></span></span>

<span data-ttu-id="ab7eb-156">L’exemple de code suivant montre comment utiliser la méthode [Folder. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) pour obtenir le dossier boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="ab7eb-156">The following code example shows how to use the [Folder.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) method to get the Inbox folder.</span></span> <span data-ttu-id="ab7eb-157">Il est recommandé de limiter les propriétés renvoyées à celles requises pour votre application.</span><span class="sxs-lookup"><span data-stu-id="ab7eb-157">As a best practice, limit the properties returned to only those required for your application.</span></span> <span data-ttu-id="ab7eb-158">Cet exemple limite les propriétés de retour à inclure uniquement la propriété [ID](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx) en créant un objet [PropertySet](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) et en appliquant la valeur [IdOnly](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.basepropertyset%28v=exchg.80%29.aspx) à la propriété [BasePropertySet](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.propertyset.basepropertyset%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="ab7eb-158">This example limits the return properties to only include the [Id](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx) property by creating a [PropertySet](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) object and applying the [IdOnly](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.basepropertyset%28v=exchg.80%29.aspx) value to the [BasePropertySet](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.propertyset.basepropertyset%28v=exchg.80%29.aspx) property.</span></span> 
  
<span data-ttu-id="ab7eb-159">Cet exemple suppose que le **service** est un objet[ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur a bien été authentifié pour un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="ab7eb-159">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
// As a best practice, limit the properties returned to only those that are required.
// In this scenario, you only need the FolderId.
PropertySet propSet = new PropertySet(BasePropertySet.IdOnly);
// Bind to an existing folder and get only the properties specified in the PropertySet.
// This method call results in a GetFolder call to EWS.
Folder rootfolder = Folder.Bind(service, WellKnownFolderName.Inbox, propSet);
```

<span data-ttu-id="ab7eb-160">Si vous devez renvoyer des propriétés supplémentaires, ajoutez des propriétés à partir de la classe [FolderSchema](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderschema%28v=exchg.80%29.aspx) à la classe **PropertySet**ou utilisez l’une des méthodes de [liaison](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) surchargées qui renvoie toutes les propriétés de première classe.</span><span class="sxs-lookup"><span data-stu-id="ab7eb-160">If you need to return additional properties, add properties from the [FolderSchema](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderschema%28v=exchg.80%29.aspx) class to the **PropertySet**, or use one of the overloaded [Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) methods that returns all first class properties.</span></span> 
  
<span data-ttu-id="ab7eb-161">Notez que vous ne pouvez pas obtenir plusieurs dossiers à la fois à l’aide de l’API managée EWS.</span><span class="sxs-lookup"><span data-stu-id="ab7eb-161">Note that you cannot get multiple folders at one time by using the EWS Managed API.</span></span> <span data-ttu-id="ab7eb-162">Vous devez appeler la méthode **Bind** sur chaque dossier séparément.</span><span class="sxs-lookup"><span data-stu-id="ab7eb-162">You have to call the **Bind** method on each folder separately.</span></span> 
  
## <a name="get-a-folder-by-using-ews"></a><span data-ttu-id="ab7eb-163">Obtenir un dossier à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="ab7eb-163">Get a folder by using EWS</span></span>
<span data-ttu-id="ab7eb-164"><a name="bk_getfolderews"> </a></span><span class="sxs-lookup"><span data-stu-id="ab7eb-164"><a name="bk_getfolderews"> </a></span></span>

<span data-ttu-id="ab7eb-165">Vous pouvez obtenir un dossier ou plusieurs dossiers à l’aide d’EWS.</span><span class="sxs-lookup"><span data-stu-id="ab7eb-165">You can get a single folder or multiple folders by using EWS.</span></span>
  
<span data-ttu-id="ab7eb-166">Pour obtenir un seul dossier, envoyez un message de demande d’opération [GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) au serveur.</span><span class="sxs-lookup"><span data-stu-id="ab7eb-166">To get a single folder, send a [GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) operation request message to the server.</span></span> <span data-ttu-id="ab7eb-167">Dans l’exemple suivant, le [BaseShape](https://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) est défini sur **IdOnly**, de sorte que seul le [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) du dossier spécifié est retourné.</span><span class="sxs-lookup"><span data-stu-id="ab7eb-167">In the following example, the [BaseShape](https://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) is set to **IdOnly**, so only the [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) of the specified folder is returned.</span></span> <span data-ttu-id="ab7eb-168">L’élément [FolderIds](https://msdn.microsoft.com/library/3ff9d15a-7220-4785-ae6b-583a7eb82005%28Office.15%29.aspx) indique que le dossier à récupérer est le dossier boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="ab7eb-168">The [FolderIds](https://msdn.microsoft.com/library/3ff9d15a-7220-4785-ae6b-583a7eb82005%28Office.15%29.aspx) element indicates that the folder to retrieve is the Inbox folder.</span></span> 
  
<span data-ttu-id="ab7eb-169">Il s’agit également de la demande XML que l’API managée EWS envoie lorsque vous liez un dossier à l’aide de la méthode [Folder. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="ab7eb-169">This is also the XML request that the EWS Managed API sends when you bind to a folder by using the [Folder.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) method.</span></span> 
  
<span data-ttu-id="ab7eb-170">Pour obtenir plusieurs dossiers, incluez plusieurs éléments [FolderIds](https://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) dans le message de demande d’opération **GetFolder** .</span><span class="sxs-lookup"><span data-stu-id="ab7eb-170">To get multiple folders, include multiple [FolderIds](https://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) elements in the **GetFolder** operation request message.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:GetFolder>
      <m:FolderShape>
        <t:BaseShape>IdOnly</t:BaseShape>
      </m:FolderShape>
      <m:FolderIds>
        <t:DistinguishedFolderId Id="inbox" />
      </m:FolderIds>
    </m:GetFolder>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="ab7eb-171">L’exemple de code XML suivant montre le message [GetFolderResponse](https://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) envoyé par le serveur au client en réponse à la demande d’opération **GetFolder** .</span><span class="sxs-lookup"><span data-stu-id="ab7eb-171">The following XML example shows the [GetFolderResponse](https://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) message that is sent from the server to the client in response to the **GetFolder** operation request.</span></span> <span data-ttu-id="ab7eb-172">Il contient uniquement la valeur [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) du dossier boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="ab7eb-172">It only contains the [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) value of the Inbox folder.</span></span> <span data-ttu-id="ab7eb-173">Les valeurs de certains attributs et éléments ont été raccourcies pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="ab7eb-173">The values of some attributes and elements have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="800"
                         MinorBuildNumber="16"
                         Version="V2_6"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="AAAENAAA=" ChangeKey="AQAAABYAAAAPxolXAHv3TaHUnjW8wWqXAAAEkbCr"/>
            </t:Folder>
          </m:Folders>
        </m:GetFolderResponseMessage>
      </m:ResponseMessages>
    </m:GetFolderResponse>
  </s:Body>
</s:Envelope>
```

## <a name="get-a-folder-hierarchy-by-using-the-ews-managed-api"></a><span data-ttu-id="ab7eb-174">Obtenir une hiérarchie de dossiers à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="ab7eb-174">Get a folder hierarchy by using the EWS Managed API</span></span>
<span data-ttu-id="ab7eb-175"><a name="bk_getfolderhierarchyewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="ab7eb-175"><a name="bk_getfolderhierarchyewsma"> </a></span></span>

<span data-ttu-id="ab7eb-176">L’exemple de code suivant montre comment récupérer les sous-dossiers d’un dossier racine spécifié.</span><span class="sxs-lookup"><span data-stu-id="ab7eb-176">The following code example shows how to retrieve the subfolders for a specified root folder.</span></span> <span data-ttu-id="ab7eb-177">Cet exemple récupère les sous-dossiers du dossier **MsgFolderRoot** , qui est la racine de la sous-arborescence IPM (où sont stockés vos dossiers et éléments de boîte aux lettres).</span><span class="sxs-lookup"><span data-stu-id="ab7eb-177">This example retrieves the subfolders of the **MsgFolderRoot** folder, which is the root of the IPM Subtree (where your mailbox folders and items are stored).</span></span> 
  
<span data-ttu-id="ab7eb-178">Dans cet exemple, un objet de classe [folderview](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderview%28v=exchg.80%29.aspx) est créé pour limiter les résultats de la réponse de la méthode [Folder. FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="ab7eb-178">In this example, a [FolderView](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderview%28v=exchg.80%29.aspx) class object is created to limit the results of the [Folder.FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) method response.</span></span> <span data-ttu-id="ab7eb-179">Ce scénario limite les propriétés à renvoyer aux éléments suivants : [ID](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx), [DisplayName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.displayname%28v=exchg.80%29.aspx)et la propriété étendue qui indique si le dossier est un dossier masqué.</span><span class="sxs-lookup"><span data-stu-id="ab7eb-179">This scenario limits the properties to return to the following: [Id](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx), [DisplayName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.displayname%28v=exchg.80%29.aspx), and the extended property that indicates whether the folder is a hidden folder.</span></span> <span data-ttu-id="ab7eb-180">Définissez la valeur [folderview. Traversal](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderview.traversal%28v=EXCHG.80%29.aspx) sur Deep pour effectuer une recherche récursive afin que le serveur récupère les sous-dossiers et définissez le dossier racine sur **MsgFolderRoot**, de sorte que le serveur renvoie tous les dossiers de l’utilisateur (et que le serveur ne retourne pas les dossiers système dans la sous-arborescence non IPM).</span><span class="sxs-lookup"><span data-stu-id="ab7eb-180">Set the [FolderView.Traversal](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderview.traversal%28v=EXCHG.80%29.aspx) value to Deep to perform a recursive search so that the server retrieves the subfolders, and set the root folder to **MsgFolderRoot**, so that the server returns all the user's folders (and the server does not return system folders in the Non-IPM Subtree).</span></span>
  
<span data-ttu-id="ab7eb-181">Cet exemple suppose que le **service** est un objet[ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur a bien été authentifié pour un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="ab7eb-181">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```XML
// Create a new folder view, and pass in the maximum number of folders to return.
FolderView view = new FolderView(folderViewSize);
// Create an extended property definition for the PR_ATTR_HIDDEN property,
// so that your results will indicate whether the folder is a hidden folder.
ExtendedPropertyDefinition isHiddenProp = new ExtendedPropertyDefinition(0x10f4, MapiPropertyType.Boolean);
// As a best practice, limit the properties returned to only those required.
// In this case, return the folder ID, DisplayName, and the value of the isHiddenProp
// extended property.
view.PropertySet = new PropertySet(BasePropertySet.IdOnly, FolderSchema.DisplayName, isHiddenProp);
// Indicate a Traversal value of Deep, so that all subfolders are retrieved.
view.Traversal = FolderTraversal.Deep;
// Call FindFolders to retrieve the folder hierarchy, starting with the MsgFolderRoot folder.
// This method call results in a FindFolder call to EWS.
FindFoldersResults findFolderResults = service.FindFolders(WellKnownFolderName.MsgFolderRoot, view);
```

## <a name="get-a-folder-hierarchy-by-using-ews"></a><span data-ttu-id="ab7eb-182">Obtenir une hiérarchie de dossiers à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="ab7eb-182">Get a folder hierarchy by using EWS</span></span>
<span data-ttu-id="ab7eb-183"><a name="bk_getfolderhierarchyews"> </a></span><span class="sxs-lookup"><span data-stu-id="ab7eb-183"><a name="bk_getfolderhierarchyews"> </a></span></span>

<span data-ttu-id="ab7eb-184">Les exemples XML suivants montrent comment utiliser l’opération [FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) pour récupérer une hiérarchie de dossiers à l’aide d’EWS.</span><span class="sxs-lookup"><span data-stu-id="ab7eb-184">The following XML examples show how to use the [FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) operation to retrieve a folder hierarchy by using EWS.</span></span> <span data-ttu-id="ab7eb-185">Cet exemple récupère le dossier **msgfolderroot** , qui est la racine de la sous-arborescence IPM et tous ses sous-dossiers.</span><span class="sxs-lookup"><span data-stu-id="ab7eb-185">This example retrieves the **msgfolderroot** folder, which is the root of the IPM Subtree, and all its subfolders.</span></span> <span data-ttu-id="ab7eb-186">L’attribut **Traversal** est défini sur **Deep** afin que le serveur effectue une recherche récursive de la hiérarchie de dossiers et renvoie uniquement les dossiers et sous-dossiers sous la racine spécifiée dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="ab7eb-186">The **Traversal** attribute is set to **Deep** so that the server performs a recursive search of the folder hierarchy and only returns folders and subfolders under the specified root in the response.</span></span> <span data-ttu-id="ab7eb-187">Dans cet exemple, l’élément [BaseShape](https://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) est défini sur **IdOnly** de sorte que le serveur ne renvoie que l’élément [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="ab7eb-187">In this example, the [BaseShape](https://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) element is set to **IdOnly** so that the server only returns the [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) element.</span></span> <span data-ttu-id="ab7eb-188">Pour faciliter la compréhension de la sortie, incluez l’élément **DisplayName** dans vos résultats en l’incluant dans l’élément [AdditionalProperties](https://msdn.microsoft.com/library/7a269aed-dcfd-4c3e-9e14-094e53828101%28Office.15%29.aspx) de la demande, ainsi que la valeur **ExtendedFieldURI** pour la propriété **PR_ATTR_HIDDEN** , afin de savoir si les dossiers sont des dossiers cachés.</span><span class="sxs-lookup"><span data-stu-id="ab7eb-188">To make the output easier to understand, include the **DisplayName** element in your results by including it in the [AdditionalProperties](https://msdn.microsoft.com/library/7a269aed-dcfd-4c3e-9e14-094e53828101%28Office.15%29.aspx) element in the request, along with the **ExtendedFieldURI** value for the **PR_ATTR_HIDDEN** property, so that you know whether the folders are hidden folders.</span></span> 
  
<span data-ttu-id="ab7eb-189">Il s’agit également de la demande XML que l’API managée EWS envoie lorsque vous appelez la méthode [FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="ab7eb-189">This is also the XML request that the EWS Managed API sends when you call the [FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx) method.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:FindFolder Traversal="Deep">
      <m:FolderShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="folder:DisplayName" />
          <t:ExtendedFieldURI PropertyTag="4340"
                              PropertyType="Boolean" />
        </t:AdditionalProperties>
      </m:FolderShape>
      <m:IndexedPageFolderView MaxEntriesReturned="100"
                               Offset="0"
                               BasePoint="Beginning" />
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="msgfolderroot" />
      </m:ParentFolderIds>
    </m:FindFolder>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="ab7eb-190">L’exemple de code XML suivant montre le message [FindFolderResponse](https://msdn.microsoft.com/library/f5dd813c-9698-4a39-8fca-3a825df365ed%28Office.15%29.aspx) envoyé par le serveur au client en réponse à la demande d’opération **FindFolder** .</span><span class="sxs-lookup"><span data-stu-id="ab7eb-190">The following XML example shows the [FindFolderResponse](https://msdn.microsoft.com/library/f5dd813c-9698-4a39-8fca-3a825df365ed%28Office.15%29.aspx) message that is sent from the server to the client in response to the **FindFolder** operation request.</span></span> <span data-ttu-id="ab7eb-191">Il contient uniquement les [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx), [DisplayName](https://msdn.microsoft.com/library/e7efbbe1-6629-4d11-bed1-ed899e3f9d77%28Office.15%29.aspx)et la valeur de la propriété étendue **PR_ATTR_HIDDEN** pour tous les sous-dossiers sous le dossier **msgrootfolder**</span><span class="sxs-lookup"><span data-stu-id="ab7eb-191">It contains only the [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx), the [DisplayName](https://msdn.microsoft.com/library/e7efbbe1-6629-4d11-bed1-ed899e3f9d77%28Office.15%29.aspx), and the value of the **PR_ATTR_HIDDEN** extended property for all the subfolders under the **msgrootfolder** folder.</span></span> <span data-ttu-id="ab7eb-192">Si l’élément [value](https://msdn.microsoft.com/library/9a30cadd-909e-41b1-b4e9-291643dd89c6%28Office.15%29.aspx) est défini sur true, le dossier doit être masqué dans l’affichage client.</span><span class="sxs-lookup"><span data-stu-id="ab7eb-192">If the [Value](https://msdn.microsoft.com/library/9a30cadd-909e-41b1-b4e9-291643dd89c6%28Office.15%29.aspx) element is set to true, the folder should be hidden in the client view.</span></span> 
  
<span data-ttu-id="ab7eb-193">Il s’agit également de la réponse XML que l’API managée EWS envoie lorsque vous obtenez plusieurs dossiers à l’aide de la méthode [FindFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="ab7eb-193">This is also the XML response that the EWS Managed API sends when you get multiple folders by using the [FindFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) method.</span></span> <span data-ttu-id="ab7eb-194">Les valeurs de certains attributs et éléments ont été raccourcies pour des raisons de lisibilité, et certains dossiers n’ont pas été inclus à des fins de concision.</span><span class="sxs-lookup"><span data-stu-id="ab7eb-194">The values of some attributes and elements have been shortened for readability, and some folders have not been included for brevity.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?><s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="815"
                         MinorBuildNumber="6"
                         Version="V2_7"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="16"
                        TotalItemsInView="16"
                        IncludesLastItemInRange="true">
            <t:Folders>
              <t:CalendarFolder>
                <t:FolderId Id="AAAEOAAA="
                            ChangeKey="AgAAABYAAAAPxolXAHv3TaHUnjW8wWqXAAAAAAA3"/>
                <t:DisplayName>Calendar</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean"/>
                  <t:Value>false</t:Value>
                </t:ExtendedProperty>
              </t:CalendarFolder>
              <t:ContactsFolder>
                <t:FolderId Id="AAAEPAAA="
                            ChangeKey="AwAAABYAAAAPxolXAHv3TaHUnjW8wWqXAAAAAAA4"/>
                <t:DisplayName>Contacts</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean"/>
                  <t:Value>false</t:Value>
                </t:ExtendedProperty>
              </t:ContactsFolder>
              <t:ContactsFolder>
                <t:FolderId Id="AAAUKAAA="
                            ChangeKey="AwAAABYAAAAPxolXAHv3TaHUnjW8wWqXAAAAAAS5"/>
                <t:DisplayName>Recipient Cache</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean"/>
                  <t:Value>true</t:Value>
                </t:ExtendedProperty>
              </t:ContactsFolder>
              <t:Folder>
                <t:FolderId Id="AAAUJAAA="
                            ChangeKey="AQAAABYAAAAPxolXAHv3TaHUnjW8wWqXAAAAAASx"/>
                <t:DisplayName>Conversation Action Settings</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean"/>
                  <t:Value>true</t:Value>
                </t:ExtendedProperty>
              </t:Folder>
…
            </t:Folders>
          </m:RootFolder>
        </m:FindFolderResponseMessage>
      </m:ResponseMessages>
    </m:FindFolderResponse>
  </s:Body>
</s:Envelope>
```

## <a name="update-a-folder-by-using-the-ews-managed-api"></a><span data-ttu-id="ab7eb-195">Mettre à jour un dossier à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="ab7eb-195">Update a folder by using the EWS Managed API</span></span>
<span data-ttu-id="ab7eb-196"><a name="bk_updatefolderewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="ab7eb-196"><a name="bk_updatefolderewsma"> </a></span></span>

<span data-ttu-id="ab7eb-197">L’exemple de code suivant montre comment mettre à jour le nom d’affichage d’un dossier à l’aide de l’API managée EWS.</span><span class="sxs-lookup"><span data-stu-id="ab7eb-197">The following code example shows how to update the display name of a folder by using the EWS Managed API.</span></span>
  
<span data-ttu-id="ab7eb-198">Tout d’abord, créez un [PropertySet](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) pour limiter le nombre de propriétés renvoyées par le serveur dans la réponse [Folder. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="ab7eb-198">First, create a [PropertySet](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) to limit the number of properties that the server returns in the [Folder.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) response.</span></span> <span data-ttu-id="ab7eb-199">Nous vous recommandons d’utiliser le **IdOnly** **BasePropertySet** pour réduire les appels à la base de données Exchange.</span><span class="sxs-lookup"><span data-stu-id="ab7eb-199">We recommend that you use the **IdOnly** **BasePropertySet** to reduce calls to the Exchange database.</span></span> <span data-ttu-id="ab7eb-200">Ensuite, utilisez la méthode **Bind** pour établir une liaison avec le dossier à mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="ab7eb-200">Next, use the **Bind** method to bind to the folder to update.</span></span> <span data-ttu-id="ab7eb-201">Ensuite, mettez à jour la propriété [DisplayName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.displayname%28v=exchg.80%29.aspx) et utilisez la méthode [Folder. Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) pour enregistrer les modifications.</span><span class="sxs-lookup"><span data-stu-id="ab7eb-201">Then, update the [DisplayName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.displayname%28v=exchg.80%29.aspx) property, and use the [Folder.Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) method to save the changes.</span></span> 
  
<span data-ttu-id="ab7eb-202">Dans cet exemple, nous partons du principe que le **service** est un objet [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur a été authentifié auprès d’un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="ab7eb-202">In this example, we assume that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> <span data-ttu-id="ab7eb-203">La variable locale *FolderId* est l' [ID](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx) du dossier à mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="ab7eb-203">The local variable  *folderId*  is the [Id](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx) of the folder to update.</span></span> 
  
```cs
// As a best practice, only include the ID value in the PropertySet.
PropertySet propertySet = new PropertySet(BasePropertySet.IdOnly);
// Bind to an existing folder and get the FolderId.
// This method call results in a GetFolder call to EWS.
Folder folder = Folder.Bind(service, folderId, propertySet);
// Update the display name of the folder.
folder.DisplayName = "Updated folder name";
// Save the updates.
// This method call results in an UpdateFolder call to EWS.
folder.Update();

```

## <a name="update-a-folder-by-using-ews"></a><span data-ttu-id="ab7eb-204">Mettre à jour un dossier à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="ab7eb-204">Update a folder by using EWS</span></span>
<span data-ttu-id="ab7eb-205"><a name="bk_updatefolderews"> </a></span><span class="sxs-lookup"><span data-stu-id="ab7eb-205"><a name="bk_updatefolderews"> </a></span></span>

<span data-ttu-id="ab7eb-206">Les exemples XML suivants montrent comment mettre à jour le nom d’affichage d’un dossier à l’aide d’EWS.</span><span class="sxs-lookup"><span data-stu-id="ab7eb-206">The following XML examples show how to update the display name of a folder by using EWS.</span></span>
  
<span data-ttu-id="ab7eb-207">Tout d’abord, envoyez un message de demande d’opération [GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) pour obtenir le dossier à mettre à jour, comme illustré dans [obtenir une hiérarchie de dossiers à l’aide d’EWS](#bk_getfolderhierarchyews).</span><span class="sxs-lookup"><span data-stu-id="ab7eb-207">First, send a [GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) operation request message to get the folder to update, as shown in [Get a folder hierarchy by using EWS](#bk_getfolderhierarchyews).</span></span>
  
<span data-ttu-id="ab7eb-208">Ensuite, envoyez un message de demande d’opération [UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) au serveur pour mettre à jour un dossier.</span><span class="sxs-lookup"><span data-stu-id="ab7eb-208">Next, send an [UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) operation request message to the server to update a folder.</span></span> <span data-ttu-id="ab7eb-209">La demande d’opération **UpdateFolder** met à jour la valeur [DisplayName](https://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) sur « mise à jour du dossier personnalisé ».</span><span class="sxs-lookup"><span data-stu-id="ab7eb-209">The **UpdateFolder** operation request updates the [DisplayName](https://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) to "Updated Custom Folder".</span></span> 
  
<span data-ttu-id="ab7eb-210">Il s’agit également de la demande XML que l’API managée EWS envoie lorsque vous mettez à jour un dossier à l’aide de la méthode [Folder. Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="ab7eb-210">This is also the XML request that the EWS Managed API sends when you update a folder by using the [Folder.Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) method.</span></span> <span data-ttu-id="ab7eb-211">Les valeurs de certains attributs et éléments ont été raccourcies pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="ab7eb-211">The values of some attributes and elements have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:UpdateFolder>
      <m:FolderChanges>
        <t:FolderChange>
          <t:FolderId Id="OrV9ZAAA=" ChangeKey="AQAAABYAAABVzRdyy/cHS4XTC9itCRdUAAAOrXWb" />
          <t:Updates>
            <t:SetFolderField>
              <t:FieldURI FieldURI="folder:DisplayName" />
              <t:Folder>
                <t:DisplayName>Updated Custom Folder</t:DisplayName>
              </t:Folder>
            </t:SetFolderField>
          </t:Updates>
        </t:FolderChange>
      </m:FolderChanges>
    </m:UpdateFolder>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="ab7eb-212">Le serveur répond à la demande **UpdateFolder** avec un message [UpdateFolderResponse](https://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx) qui inclut la valeur [ResponseCode](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) de la propriété **NOERROR**et la [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) du dossier qui a été mise à jour avec une valeur d’attribut **ChangeKey** mise à jour.</span><span class="sxs-lookup"><span data-stu-id="ab7eb-212">The server responds to the **UpdateFolder** request with a [UpdateFolderResponse](https://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx) message that includes the a [ResponseCode](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, and the [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) of the folder that was updated with an updated **ChangeKey** attribute value.</span></span> 
  
## <a name="delete-a-folder-by-using-the-ews-managed-api"></a><span data-ttu-id="ab7eb-213">Supprimer un dossier à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="ab7eb-213">Delete a folder by using the EWS Managed API</span></span>
<span data-ttu-id="ab7eb-214"><a name="bk_deletefolderewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="ab7eb-214"><a name="bk_deletefolderewsma"> </a></span></span>

<span data-ttu-id="ab7eb-215">Cet article fournit un exemple de base qui vous montre comment supprimer un dossier à l’aide de l’API managée EWS.</span><span class="sxs-lookup"><span data-stu-id="ab7eb-215">This article provides a basic example that shows you how to delete a folder by using the EWS Managed API.</span></span> <span data-ttu-id="ab7eb-216">Pour plus d’informations sur la suppression de dossiers, consultez [la rubrique Suppression d’éléments à l’aide d’EWS dans Exchange](deleting-items-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="ab7eb-216">For more details about deleting folders, see [Deleting items by using EWS in Exchange](deleting-items-by-using-ews-in-exchange.md).</span></span>
  
<span data-ttu-id="ab7eb-217">Pour supprimer un dossier à l’aide de l’API managée EWS, commencez par utiliser la méthode [Folder. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) pour établir une liaison avec l’objet service au dossier à supprimer.</span><span class="sxs-lookup"><span data-stu-id="ab7eb-217">To delete a folder by using the EWS Managed API, first, use the [Folder.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) method to bind to the service object to the folder to delete.</span></span> <span data-ttu-id="ab7eb-218">Ensuite, utilisez la méthode [Folder. Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) pour supprimer le dossier à l’aide du mode de suppression de [HardDelete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.deletemode%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="ab7eb-218">Next, use the [Folder.Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) method to delete the folder by using the [HardDelete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.deletemode%28v=exchg.80%29.aspx) deletion mode.</span></span> 
  
<span data-ttu-id="ab7eb-219">Cet exemple suppose que le **service** est un objet[ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur a bien été authentifié pour un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="ab7eb-219">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> <span data-ttu-id="ab7eb-220">La variable locale *FolderId* est l' [ID](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx) du dossier à supprimer.</span><span class="sxs-lookup"><span data-stu-id="ab7eb-220">The local variable  *folderId*  is the [Id](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx) of the folder to delete.</span></span> 
  
```cs
// Bind to an existing folder and get all its properties.
// This method call results in a GetFolder call to EWS.
Folder folder = Folder.Bind(service, folderId);
// HardDelete the folder.
// This method call results in a DeleteFolder call to EWS.
folder.Delete(DeleteMode.HardDelete);
```

## <a name="delete-a-folder-by-using-ews"></a><span data-ttu-id="ab7eb-221">Supprimer un dossier à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="ab7eb-221">Delete a folder by using EWS</span></span>
<span data-ttu-id="ab7eb-222"><a name="bk_deletefolderews"> </a></span><span class="sxs-lookup"><span data-stu-id="ab7eb-222"><a name="bk_deletefolderews"> </a></span></span>

<span data-ttu-id="ab7eb-223">Cet article fournit un exemple XML de base qui vous montre comment supprimer un dossier à l’aide d’EWS.</span><span class="sxs-lookup"><span data-stu-id="ab7eb-223">This article provides a basic XML example that shows you how to delete a folder by using EWS.</span></span> <span data-ttu-id="ab7eb-224">Pour plus d’informations sur la suppression de dossiers, consultez [la rubrique Suppression d’éléments à l’aide d’EWS dans Exchange](deleting-items-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="ab7eb-224">For more details about deleting folders, see [Deleting items by using EWS in Exchange](deleting-items-by-using-ews-in-exchange.md).</span></span>
  
<span data-ttu-id="ab7eb-225">Pour supprimer un dossier à l’aide d’EWS, envoyez d’abord un message de demande d’opération [GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) pour obtenir le dossier à mettre à jour, comme indiqué dans [Get a folder by using EWS](#bk_getfolderews).</span><span class="sxs-lookup"><span data-stu-id="ab7eb-225">To delete a folder by using EWS, first, send a [GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) operation request message to get the folder to update as shown in [Get a folder by using EWS](#bk_getfolderews).</span></span> 
  
<span data-ttu-id="ab7eb-226">Ensuite, envoyez un message de demande d’opération [DeleteFolder](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) au serveur pour supprimer le dossier.</span><span class="sxs-lookup"><span data-stu-id="ab7eb-226">Next, send a [DeleteFolder](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) operation request message to the server to delete the folder.</span></span> <span data-ttu-id="ab7eb-227">La demande d’opération **DeleteFolder** indique que le **DeleteType** est **HardDelete** et qu’il inclut le [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) du dossier à supprimer.</span><span class="sxs-lookup"><span data-stu-id="ab7eb-227">The **DeleteFolder** operation request indicates that the **DeleteType** is **HardDelete** and it includes the [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) of the folder to delete.</span></span> 
  
<span data-ttu-id="ab7eb-228">Il s’agit également de la demande XML que l’API managée EWS envoie lorsque vous supprimez un dossier à l’aide de la méthode [Folder. Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="ab7eb-228">This is also the XML request that the EWS Managed API sends when you delete a folder by using the [Folder.Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) method.</span></span> <span data-ttu-id="ab7eb-229">Les valeurs de certains attributs et éléments ont été raccourcies pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="ab7eb-229">The values of some attributes and elements have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:DeleteFolder DeleteType="HardDelete">
      <m:FolderIds>
        <t:FolderId Id="OrV9ZAAA=" ChangeKey="AQAAABYAAABVzRdyy/cHS4XTC9itCRdUAAAOrXWf" />
      </m:FolderIds>
    </m:DeleteFolder>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="ab7eb-230">Le serveur répond à la demande **DeleteFolder** avec un message [DeleteFolderResponse](https://msdn.microsoft.com/library/27578bda-ef0a-4a33-bccc-2c1bc1735424%28Office.15%29.aspx) qui inclut la valeur [ResponseCode](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) de **NOERROR**, ce qui indique que la suppression du dossier a réussi.</span><span class="sxs-lookup"><span data-stu-id="ab7eb-230">The server responds to the **DeleteFolder** request with a [DeleteFolderResponse](https://msdn.microsoft.com/library/27578bda-ef0a-4a33-bccc-2c1bc1735424%28Office.15%29.aspx) message that includes the a [ResponseCode](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the folder deletion was successful.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="ab7eb-231">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="ab7eb-231">Next steps</span></span>
<span data-ttu-id="ab7eb-232"><a name="bk_nextsteps"> </a></span><span class="sxs-lookup"><span data-stu-id="ab7eb-232"><a name="bk_nextsteps"> </a></span></span>

<span data-ttu-id="ab7eb-233">Une fois que vous avez récupéré les dossiers sur le serveur ou apporté des modifications aux dossiers, vous pouvez [synchroniser votre hiérarchie de dossiers](how-to-synchronize-folders-by-using-ews-in-exchange.md) ou vous [abonner aux notifications concernant les modifications apportées aux dossiers](notification-subscriptions-mailbox-events-and-ews-in-exchange.md) sur le serveur.</span><span class="sxs-lookup"><span data-stu-id="ab7eb-233">After you have retrieved the folders on the server, or made changes to folders, you might want to [synchronize your folder hierarchy](how-to-synchronize-folders-by-using-ews-in-exchange.md) or [subscribe to notifications about folder changes](notification-subscriptions-mailbox-events-and-ews-in-exchange.md) on the server.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="ab7eb-234">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ab7eb-234">See also</span></span>

- [<span data-ttu-id="ab7eb-235">Dossiers et éléments dans EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ab7eb-235">Folders and items in EWS in Exchange</span></span>](folders-and-items-in-ews-in-exchange.md)   
- [<span data-ttu-id="ab7eb-236">Utilisations d’éléments de boîte aux lettres Exchange à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ab7eb-236">Work with Exchange mailbox items by using EWS in Exchange</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md)    
- [<span data-ttu-id="ab7eb-237">Supprimer des éléments à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ab7eb-237">Deleting items by using EWS in Exchange</span></span>](deleting-items-by-using-ews-in-exchange.md)   
- [<span data-ttu-id="ab7eb-238">Développer des clients de service web pour Exchange</span><span class="sxs-lookup"><span data-stu-id="ab7eb-238">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    

