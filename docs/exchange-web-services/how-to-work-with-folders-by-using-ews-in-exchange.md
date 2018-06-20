---
title: Utilisation de dossiers à l’aide de EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 4b3eb746-74c4-42a0-aa2c-742c147f1871
description: Découvrez comment créer, obtenir, mettre à jour et supprimer des dossiers à l’aide de l’API managée EWS ou EWS dans Exchange.
ms.openlocfilehash: a9a9e5974b2751268f37a1c9faacce43a333bcdb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19754975"
---
# <a name="work-with-folders-by-using-ews-in-exchange"></a><span data-ttu-id="8ee82-103">Utilisation de dossiers à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="8ee82-103">Work with folders by using EWS in Exchange</span></span>

<span data-ttu-id="8ee82-104">Découvrez comment créer, obtenir, mettre à jour et supprimer des dossiers à l’aide de l’API managée EWS ou EWS dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="8ee82-104">Learn how to create, get, update, and delete folders by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="8ee82-105">EWS dans Exchange utilise des dossiers à la structure et organiser des boîtes aux lettres.</span><span class="sxs-lookup"><span data-stu-id="8ee82-105">EWS in Exchange uses folders to structure and organize mailboxes.</span></span> <span data-ttu-id="8ee82-106">Peut créer, obtenir, mettre à jour et supprimer des dossiers à l’aide de l’API managée EWS ou EWS.</span><span class="sxs-lookup"><span data-stu-id="8ee82-106">You can create new, get, update, and delete folders by using the EWS Managed API or EWS.</span></span> <span data-ttu-id="8ee82-107">Chacune des méthodes ou des opérations répertoriées dans le tableau suivant est effectuée sur un objet [Folder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx) , un type de [dossier](http://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) ou [une des classes dérivées des dossiers ou types](folders-and-items-in-ews-in-exchange.md#bk_folders).</span><span class="sxs-lookup"><span data-stu-id="8ee82-107">Each of the methods or operations listed in the following table is performed on a [Folder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx) object, a [Folder](http://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) type, or [one of the derived folder classes or types](folders-and-items-in-ews-in-exchange.md#bk_folders).</span></span>
  
<span data-ttu-id="8ee82-108">**Le tableau 1. Méthodes et les opérations de création, l’obtention, mise à jour et suppression de dossiers**</span><span class="sxs-lookup"><span data-stu-id="8ee82-108">**Table 1. Methods and operations for creating, getting, updating and deleting folders**</span></span>

|<span data-ttu-id="8ee82-109">**Pour...**</span><span class="sxs-lookup"><span data-stu-id="8ee82-109">**In order to…**</span></span>|<span data-ttu-id="8ee82-110">**Méthode d'API managée EWS**</span><span class="sxs-lookup"><span data-stu-id="8ee82-110">**EWS Managed API method**</span></span>|<span data-ttu-id="8ee82-111">**Opération EWS**</span><span class="sxs-lookup"><span data-stu-id="8ee82-111">**EWS operation**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="8ee82-112">Créez un dossier</span><span class="sxs-lookup"><span data-stu-id="8ee82-112">Create a folder</span></span>  <br/> |[<span data-ttu-id="8ee82-113">Folder.Save</span><span class="sxs-lookup"><span data-stu-id="8ee82-113">Folder.Save</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.save%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="8ee82-114">CreateFolder</span><span class="sxs-lookup"><span data-stu-id="8ee82-114">CreateFolder</span></span>](http://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="8ee82-115">Créer une hiérarchie de dossiers</span><span class="sxs-lookup"><span data-stu-id="8ee82-115">Create a folder hierarchy</span></span>  <br/> |<span data-ttu-id="8ee82-116">Non disponible</span><span class="sxs-lookup"><span data-stu-id="8ee82-116">Not available</span></span>  <br/> |[<span data-ttu-id="8ee82-117">CreateFolderPath</span><span class="sxs-lookup"><span data-stu-id="8ee82-117">CreateFolderPath</span></span>](http://msdn.microsoft.com/library/5a10aa5e-3f25-4ec3-a0b9-284c30918a1f%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="8ee82-118">Obtenir un dossier</span><span class="sxs-lookup"><span data-stu-id="8ee82-118">Get a folder</span></span>  <br/> |[<span data-ttu-id="8ee82-119">Folder.Bind</span><span class="sxs-lookup"><span data-stu-id="8ee82-119">Folder.Bind</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="8ee82-120">GetFolder</span><span class="sxs-lookup"><span data-stu-id="8ee82-120">GetFolder</span></span>](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="8ee82-121">Obtenir une hiérarchie de dossiers</span><span class="sxs-lookup"><span data-stu-id="8ee82-121">Get a folder hierarchy</span></span>  <br/> |[<span data-ttu-id="8ee82-122">Folder.FindFolders</span><span class="sxs-lookup"><span data-stu-id="8ee82-122">Folder.FindFolders</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="8ee82-123">FindFolder</span><span class="sxs-lookup"><span data-stu-id="8ee82-123">FindFolder</span></span>](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="8ee82-124">Mettre à jour un dossier</span><span class="sxs-lookup"><span data-stu-id="8ee82-124">Update a folder</span></span>  <br/> |[<span data-ttu-id="8ee82-125">Folder.Update</span><span class="sxs-lookup"><span data-stu-id="8ee82-125">Folder.Update</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="8ee82-126">UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="8ee82-126">UpdateFolder</span></span>](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="8ee82-127">Supprimer un dossier</span><span class="sxs-lookup"><span data-stu-id="8ee82-127">Delete a folder</span></span>  <br/> |[<span data-ttu-id="8ee82-128">Folder.Delete</span><span class="sxs-lookup"><span data-stu-id="8ee82-128">Folder.Delete</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="8ee82-129">DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="8ee82-129">DeleteFolder</span></span>](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |

<span data-ttu-id="8ee82-130"><a name="bk_createfolderewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="8ee82-130"></span></span>

## <a name="create-a-folder-by-using-the-ews-managed-api"></a><span data-ttu-id="8ee82-131">Créez un dossier à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="8ee82-131">Create a folder by using the EWS Managed API</span></span>

<span data-ttu-id="8ee82-132">L’exemple de code suivant montre comment utiliser la classe de [dossier](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx) pour créer un nouveau dossier générique avec un [DisplayName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.displayname%28v=exchg.80%29.aspx) de « Dossier personnalisé » et une valeur de propriété de [classe FolderClass](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.folderclass%28v=exchg.80%29.aspx) de l’erreur. Note.</span><span class="sxs-lookup"><span data-stu-id="8ee82-132">The following code example shows how to use the [Folder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx) class to create a new generic folder with a [DisplayName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.displayname%28v=exchg.80%29.aspx) of "Custom Folder" and a [FolderClass](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.folderclass%28v=exchg.80%29.aspx) property value of IPF.Note.</span></span> <span data-ttu-id="8ee82-133">La méthode [Folder.Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.save%28v=exchg.80%29.aspx) enregistre le dossier sous un dossier enfant du dossier boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="8ee82-133">The [Folder.Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.save%28v=exchg.80%29.aspx) method saves the folder as a child folder of the Inbox folder.</span></span> 
  
<span data-ttu-id="8ee82-134">Les exemples suivants supposent que ce **service** est un objet [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur a été authentifié sur un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="8ee82-134">These examples assume that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
// Create a custom folder.
Folder folder = new Folder(service);
folder.DisplayName = "Custom Folder";
folder.FolderClass = "IPF.Note";
// Save the folder as a child folder of the Inbox.
folder.Save(WellKnownFolderName.Inbox);
```

<span data-ttu-id="8ee82-135">Pour créer un autre type de dossier, comme un [CalendarFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.calendarfolder%28v=exchg.80%29.aspx), [ContactsFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contactsfolder%28v=exchg.80%29.aspx), [SearchFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx)ou [dossier tâches](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.tasksfolder%28v=exchg.80%29.aspx), créez une nouvelle instance de la classe spécifique (au lieu de la classe générique de **dossier** ) et ne définissez pas la Propriété de la **classe FolderClass** .</span><span class="sxs-lookup"><span data-stu-id="8ee82-135">To create a different type of folder, such as a [CalendarFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.calendarfolder%28v=exchg.80%29.aspx), [ContactsFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contactsfolder%28v=exchg.80%29.aspx), [SearchFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx), or [TasksFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.tasksfolder%28v=exchg.80%29.aspx), create a new instance of the specific class (instead of the generic **Folder** class) and do not set the **FolderClass** property.</span></span> <span data-ttu-id="8ee82-136">Par exemple, l’exemple de code suivant montre comment créer un nouveau [dossier tâches](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.tasksfolder%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="8ee82-136">For example, the following code example shows how to create a new [TasksFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.tasksfolder%28v=exchg.80%29.aspx).</span></span>
  
```cs
// Create a custom Tasks folder.
TasksFolder folder = new TasksFolder(service);
folder.DisplayName = "Custom Tasks";
// Save the folder as a child folder in the Inbox folder.
// This method call results in a CreateFolder call to EWS.
folder.Save(WellKnownFolderName.Inbox);
```

<span data-ttu-id="8ee82-137">Si vous essayez de créer une instance d’une classe spécifique et également définir la propriété de la **classe FolderClass** , l’erreur [ErrorNoFolderClassOverride](http://msdn.microsoft.com/en-us/library/exchangewebservices.responsecodetype%28v=exchg.80%29.aspx) est levée.</span><span class="sxs-lookup"><span data-stu-id="8ee82-137">If you try to create an instance of a specific class and also set the **FolderClass** property, the [ErrorNoFolderClassOverride](http://msdn.microsoft.com/en-us/library/exchangewebservices.responsecodetype%28v=exchg.80%29.aspx) error is thrown.</span></span> 
  
<span data-ttu-id="8ee82-138">Notez que la création de plusieurs dossiers dans un seul appel de méthode ne peut pas par lot à l’aide de l’API managée EWS.</span><span class="sxs-lookup"><span data-stu-id="8ee82-138">Note that you cannot batch the creation of multiple folders in a single method call by using the EWS Managed API.</span></span>
  
## <a name="create-a-folder-by-using-ews"></a><span data-ttu-id="8ee82-139">Créez un dossier à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="8ee82-139">Create a folder by using EWS</span></span>
<span data-ttu-id="8ee82-140"><a name="bk_createfolderews"> </a></span><span class="sxs-lookup"><span data-stu-id="8ee82-140"></span></span>

<span data-ttu-id="8ee82-141">Vous pouvez créer un dossier unique ou multiple de dossiers à l’aide de EWS.</span><span class="sxs-lookup"><span data-stu-id="8ee82-141">You can create a single folder or multiple of folders by using EWS.</span></span>
  
<span data-ttu-id="8ee82-142">Pour créer un dossier unique, envoyer un message de demande d’opération [CreateFolder](http://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="8ee82-142">To create a single folder, send a [CreateFolder](http://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) operation request message.</span></span> <span data-ttu-id="8ee82-143">La requête d’opération **CreateFolder** indique que le dossier parent est la boîte de réception, [DisplayName](http://msdn.microsoft.com/library/e7efbbe1-6629-4d11-bed1-ed899e3f9d77%28Office.15%29.aspx) est « Dossier personnalisé », et la valeur de l’élément [classe FolderClass](http://msdn.microsoft.com/library/0041d135-2869-4612-89a5-d1aa86aa1093%28Office.15%29.aspx) est l’erreur. Note.</span><span class="sxs-lookup"><span data-stu-id="8ee82-143">The **CreateFolder** operation request indicates that the parent folder is the Inbox, the [DisplayName](http://msdn.microsoft.com/library/e7efbbe1-6629-4d11-bed1-ed899e3f9d77%28Office.15%29.aspx) is "Custom Folder", and the [FolderClass](http://msdn.microsoft.com/library/0041d135-2869-4612-89a5-d1aa86aa1093%28Office.15%29.aspx) element value is IPF.Note.</span></span> 
  
<span data-ttu-id="8ee82-144">C’est également la demande XML qui envoie de l’API managée EWS lorsque vous créez un nouveau dossier et que vous appelez la méthode [Folder.Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.save%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="8ee82-144">This is also the XML request that the EWS Managed API sends when you create a new folder and call the [Folder.Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.save%28v=exchg.80%29.aspx) method.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="8ee82-145">Le serveur répond à la demande **CreateFolder** avec un message [CreateFolderResponse](http://msdn.microsoft.com/library/158adecc-491a-47d9-af73-acc2cd3f8566%28Office.15%29.aspx) qui contient une valeur [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) **NoError**, ce qui indique que le dossier a été créé avec succès et l' [ID FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) de le message nouvellement créé.</span><span class="sxs-lookup"><span data-stu-id="8ee82-145">The server responds to the **CreateFolder** request with a [CreateFolderResponse](http://msdn.microsoft.com/library/158adecc-491a-47d9-af73-acc2cd3f8566%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the folder was created successfully, and the [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) of the newly created message.</span></span> 
  
<span data-ttu-id="8ee82-146">Pour créer plusieurs dossiers, incluez plusieurs éléments du [dossier](http://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) dans le message de demande d’opération **CreateFolder** .</span><span class="sxs-lookup"><span data-stu-id="8ee82-146">To create multiple folders, include multiple [Folder](http://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) elements in the **CreateFolder** operation request message.</span></span> <span data-ttu-id="8ee82-147">Tous les nouveaux dossiers doivent être dans le même dossier parent.</span><span class="sxs-lookup"><span data-stu-id="8ee82-147">All the new folders must be in the same parent folder.</span></span> 
  
## <a name="create-a-folder-hierarchy-by-using-ews"></a><span data-ttu-id="8ee82-148">Créer une hiérarchie de dossiers à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="8ee82-148">Create a folder hierarchy by using EWS</span></span>
<span data-ttu-id="8ee82-149"><a name="bk_createfolderhierarchy"> </a></span><span class="sxs-lookup"><span data-stu-id="8ee82-149"></span></span>

<span data-ttu-id="8ee82-150">Vous pouvez créer une hiérarchie de dossiers dans un seul appel à l’aide de l’opération EWS [CreateFolderPath](http://msdn.microsoft.com/library/5a10aa5e-3f25-4ec3-a0b9-284c30918a1f%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="8ee82-150">You can create a folder hierarchy in a single call by using the EWS [CreateFolderPath](http://msdn.microsoft.com/library/5a10aa5e-3f25-4ec3-a0b9-284c30918a1f%28Office.15%29.aspx) operation.</span></span> <span data-ttu-id="8ee82-151">La même fonctionnalité n’est pas disponible dans l’API managée EWS.</span><span class="sxs-lookup"><span data-stu-id="8ee82-151">The same functionality is not available in the EWS Managed API.</span></span> <span data-ttu-id="8ee82-152">Au lieu de cela, si vous utilisez l’API managée EWS, vous pouvez créer les dossiers un par un, comme indiqué dans [créer un dossier à l’aide de EWS](#bk_createfolderews).</span><span class="sxs-lookup"><span data-stu-id="8ee82-152">Instead, if you are using the EWS Managed API, you can create folders one by one, as shown in [Create a folder by using EWS](#bk_createfolderews).</span></span>
  
> [!NOTE]
> <span data-ttu-id="8ee82-153">L’API managée EWS n’implémente pas cette fonctionnalité.</span><span class="sxs-lookup"><span data-stu-id="8ee82-153">The EWS Managed API does not implement this functionality.</span></span> 
  
## <a name="get-a-folder-by-using-the-ews-managed-api"></a><span data-ttu-id="8ee82-154">Obtenir un dossier à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="8ee82-154">Get a folder by using the EWS Managed API</span></span>
<span data-ttu-id="8ee82-155"><a name="bk_getfolderewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="8ee82-155"></span></span>

<span data-ttu-id="8ee82-156">L’exemple de code suivant montre comment utiliser la méthode [Folder.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) pour obtenir le dossier boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="8ee82-156">The following code example shows how to use the [Folder.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) method to get the Inbox folder.</span></span> <span data-ttu-id="8ee82-157">Meilleure pratique, limitez les propriétés renvoyées uniquement à ceux requis pour votre application.</span><span class="sxs-lookup"><span data-stu-id="8ee82-157">As a best practice, limit the properties returned to only those required for your application.</span></span> <span data-ttu-id="8ee82-158">Cet exemple limite les propriétés de retour pour n’inclure que la propriété [Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx) en créant un objet [PropertySet](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) et en appliquant la valeur [IdOnly](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.basepropertyset%28v=exchg.80%29.aspx) à la propriété [BasePropertySet](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.propertyset.basepropertyset%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="8ee82-158">This example limits the return properties to only include the [Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx) property by creating a [PropertySet](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) object and applying the [IdOnly](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.basepropertyset%28v=exchg.80%29.aspx) value to the [BasePropertySet](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.propertyset.basepropertyset%28v=exchg.80%29.aspx) property.</span></span> 
  
<span data-ttu-id="8ee82-159">Cet exemple suppose que ce **service** est un objet [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur a été authentifié sur un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="8ee82-159">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
// As a best practice, limit the properties returned to only those that are required.
// In this scenario, you only need the FolderId.
PropertySet propSet = new PropertySet(BasePropertySet.IdOnly);
// Bind to an existing folder and get only the properties specified in the PropertySet.
// This method call results in a GetFolder call to EWS.
Folder rootfolder = Folder.Bind(service, WellKnownFolderName.Inbox, propSet);
```

<span data-ttu-id="8ee82-160">Si vous avez besoin renvoyer les propriétés supplémentaires, ajouter des propriétés de la classe [FolderSchema](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderschema%28v=exchg.80%29.aspx) à **PropertySet**, ou utilisez une des surchargées [lier](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) des méthodes qui retourne toutes les propriétés de première classes.</span><span class="sxs-lookup"><span data-stu-id="8ee82-160">If you need to return additional properties, add properties from the [FolderSchema](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderschema%28v=exchg.80%29.aspx) class to the **PropertySet**, or use one of the overloaded [Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) methods that returns all first class properties.</span></span> 
  
<span data-ttu-id="8ee82-161">Notez que vous ne pouvez pas obtenir plusieurs dossiers en même temps à l’aide de l’API managée EWS.</span><span class="sxs-lookup"><span data-stu-id="8ee82-161">Note that you cannot get multiple folders at one time by using the EWS Managed API.</span></span> <span data-ttu-id="8ee82-162">Vous devez appeler la méthode **Bind** sur chaque dossier séparément.</span><span class="sxs-lookup"><span data-stu-id="8ee82-162">You have to call the **Bind** method on each folder separately.</span></span> 
  
## <a name="get-a-folder-by-using-ews"></a><span data-ttu-id="8ee82-163">Obtenir un dossier à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="8ee82-163">Get a folder by using EWS</span></span>
<span data-ttu-id="8ee82-164"><a name="bk_getfolderews"> </a></span><span class="sxs-lookup"><span data-stu-id="8ee82-164"></span></span>

<span data-ttu-id="8ee82-165">Vous pouvez obtenir un dossier unique ou à plusieurs dossiers à l’aide de EWS.</span><span class="sxs-lookup"><span data-stu-id="8ee82-165">You can get a single folder or multiple folders by using EWS.</span></span>
  
<span data-ttu-id="8ee82-166">Pour obtenir un seul dossier, envoyez un message de demande d’opération [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) sur le serveur.</span><span class="sxs-lookup"><span data-stu-id="8ee82-166">To get a single folder, send a [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) operation request message to the server.</span></span> <span data-ttu-id="8ee82-167">Dans l’exemple suivant, la [BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) est définie à **IdOnly**, ainsi que la [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) du dossier spécifié est retourné.</span><span class="sxs-lookup"><span data-stu-id="8ee82-167">In the following example, the [BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) is set to **IdOnly**, so only the [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) of the specified folder is returned.</span></span> <span data-ttu-id="8ee82-168">L’élément [FolderIds](http://msdn.microsoft.com/library/3ff9d15a-7220-4785-ae6b-583a7eb82005%28Office.15%29.aspx) indique que le dossier à récupérer est le dossier boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="8ee82-168">The [FolderIds](http://msdn.microsoft.com/library/3ff9d15a-7220-4785-ae6b-583a7eb82005%28Office.15%29.aspx) element indicates that the folder to retrieve is the Inbox folder.</span></span> 
  
<span data-ttu-id="8ee82-169">C’est également la demande XML qui envoie de l’API managée EWS lorsque vous liez à un dossier à l’aide de la méthode [Folder.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="8ee82-169">This is also the XML request that the EWS Managed API sends when you bind to a folder by using the [Folder.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) method.</span></span> 
  
<span data-ttu-id="8ee82-170">Pour obtenir plusieurs dossiers, inclure plusieurs éléments [FolderIds](http://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) dans le message de demande d’opération **GetFolder** .</span><span class="sxs-lookup"><span data-stu-id="8ee82-170">To get multiple folders, include multiple [FolderIds](http://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) elements in the **GetFolder** operation request message.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="8ee82-171">L’exemple XML suivant montre le message est envoyé à partir du serveur au client en réponse à la requête d’opération **GetFolder** [GetFolderResponse](http://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="8ee82-171">The following XML example shows the [GetFolderResponse](http://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) message that is sent from the server to the client in response to the **GetFolder** operation request.</span></span> <span data-ttu-id="8ee82-172">Il contient uniquement la valeur [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) du dossier boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="8ee82-172">It only contains the [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) value of the Inbox folder.</span></span> <span data-ttu-id="8ee82-173">Les valeurs de certains attributs et éléments ont été raccourcies pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="8ee82-173">The values of some attributes and elements have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="800"
                         MinorBuildNumber="16"
                         Version="V2_6"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="get-a-folder-hierarchy-by-using-the-ews-managed-api"></a><span data-ttu-id="8ee82-174">Obtenir une hiérarchie de dossiers à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="8ee82-174">Get a folder hierarchy by using the EWS Managed API</span></span>
<span data-ttu-id="8ee82-175"><a name="bk_getfolderhierarchyewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="8ee82-175"></span></span>

<span data-ttu-id="8ee82-176">L’exemple de code suivant montre comment récupérer les sous-dossiers d’un dossier racine spécifié.</span><span class="sxs-lookup"><span data-stu-id="8ee82-176">The following code example shows how to retrieve the subfolders for a specified root folder.</span></span> <span data-ttu-id="8ee82-177">Cet exemple récupère les sous-dossiers du dossier **MsgFolderRoot** , qui est la racine de la sous-arborescence IPM (où sont stockés vos dossiers de boîte aux lettres et éléments).</span><span class="sxs-lookup"><span data-stu-id="8ee82-177">This example retrieves the subfolders of the **MsgFolderRoot** folder, which is the root of the IPM Subtree (where your mailbox folders and items are stored).</span></span> 
  
<span data-ttu-id="8ee82-178">Dans cet exemple, un objet de classe [FolderView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderview%28v=exchg.80%29.aspx) est créé pour limiter les résultats de la réponse de la méthode [Folder.FindFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="8ee82-178">In this example, a [FolderView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderview%28v=exchg.80%29.aspx) class object is created to limit the results of the [Folder.FindFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) method response.</span></span> <span data-ttu-id="8ee82-179">Ce scénario limite les propriétés pour revenir à ce qui suit : [Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx), [DisplayName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.displayname%28v=exchg.80%29.aspx)et la propriété étendue qui indique si le dossier est un dossier masqué.</span><span class="sxs-lookup"><span data-stu-id="8ee82-179">This scenario limits the properties to return to the following: [Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx), [DisplayName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.displayname%28v=exchg.80%29.aspx), and the extended property that indicates whether the folder is a hidden folder.</span></span> <span data-ttu-id="8ee82-180">Définissez la valeur de [FolderView.Traversal](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderview.traversal%28v=EXCHG.80%29.aspx) profondeur pour effectuer une recherche récursive afin que le serveur récupère les sous-dossiers et affecter le dossier racine **MsgFolderRoot**, afin que le serveur renvoie tous les dossiers de l’utilisateur (et le serveur ne retourne pas dossiers système dans la sous-arborescence Non-IPM).</span><span class="sxs-lookup"><span data-stu-id="8ee82-180">Set the [FolderView.Traversal](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderview.traversal%28v=EXCHG.80%29.aspx) value to Deep to perform a recursive search so that the server retrieves the subfolders, and set the root folder to **MsgFolderRoot**, so that the server returns all the user's folders (and the server does not return system folders in the Non-IPM Subtree).</span></span>
  
<span data-ttu-id="8ee82-181">Cet exemple suppose que ce **service** est un objet [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur a été authentifié sur un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="8ee82-181">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
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

## <a name="get-a-folder-hierarchy-by-using-ews"></a><span data-ttu-id="8ee82-182">Obtenir une hiérarchie de dossiers à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="8ee82-182">Get a folder hierarchy by using EWS</span></span>
<span data-ttu-id="8ee82-183"><a name="bk_getfolderhierarchyews"> </a></span><span class="sxs-lookup"><span data-stu-id="8ee82-183"></span></span>

<span data-ttu-id="8ee82-184">Les exemples de code XML suivants montrent comment utiliser l’opération [FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) pour récupérer une hiérarchie de dossiers à l’aide de EWS.</span><span class="sxs-lookup"><span data-stu-id="8ee82-184">The following XML examples show how to use the [FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) operation to retrieve a folder hierarchy by using EWS.</span></span> <span data-ttu-id="8ee82-185">Cet exemple récupère le dossier **msgfolderroot** , qui est la racine de la sous-arborescence IPM et tous ses sous-dossiers.</span><span class="sxs-lookup"><span data-stu-id="8ee82-185">This example retrieves the **msgfolderroot** folder, which is the root of the IPM Subtree, and all its subfolders.</span></span> <span data-ttu-id="8ee82-186">L’attribut de **parcours** est défini sur **approfondie** afin que le serveur effectue une recherche récursive de la hiérarchie de dossiers et renvoie uniquement les dossiers et les sous-dossiers sous la racine spécifiée dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="8ee82-186">The **Traversal** attribute is set to **Deep** so that the server performs a recursive search of the folder hierarchy and only returns folders and subfolders under the specified root in the response.</span></span> <span data-ttu-id="8ee82-187">Dans cet exemple, l’élément [BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) est définie à **IdOnly** afin que le serveur renvoie uniquement l’élément [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="8ee82-187">In this example, the [BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) element is set to **IdOnly** so that the server only returns the [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) element.</span></span> <span data-ttu-id="8ee82-188">Pour faciliter la compréhension de la sortie, inclure l’élément **DisplayName** dans les résultats en y compris dans l’élément [AdditionalProperties](http://msdn.microsoft.com/library/7a269aed-dcfd-4c3e-9e14-094e53828101%28Office.15%29.aspx) dans la demande, ainsi que la valeur **ExtendedFieldURI** pour la **PR_ATTR_HIDDEN** propriété, afin que vous savez si les dossiers sont masquées.</span><span class="sxs-lookup"><span data-stu-id="8ee82-188">To make the output easier to understand, include the **DisplayName** element in your results by including it in the [AdditionalProperties](http://msdn.microsoft.com/library/7a269aed-dcfd-4c3e-9e14-094e53828101%28Office.15%29.aspx) element in the request, along with the **ExtendedFieldURI** value for the **PR_ATTR_HIDDEN** property, so that you know whether the folders are hidden folders.</span></span> 
  
<span data-ttu-id="8ee82-189">C’est également la demande XML qui envoie de l’API managée EWS lorsque vous appelez la méthode [FindFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="8ee82-189">This is also the XML request that the EWS Managed API sends when you call the [FindFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx) method.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="8ee82-190">L’exemple XML suivant montre le message est envoyé à partir du serveur au client en réponse à la requête d’opération **FindFolder** [FindFolderResponse](http://msdn.microsoft.com/library/f5dd813c-9698-4a39-8fca-3a825df365ed%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="8ee82-190">The following XML example shows the [FindFolderResponse](http://msdn.microsoft.com/library/f5dd813c-9698-4a39-8fca-3a825df365ed%28Office.15%29.aspx) message that is sent from the server to the client in response to the **FindFolder** operation request.</span></span> <span data-ttu-id="8ee82-191">Il contient uniquement le [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx), [DisplayName](http://msdn.microsoft.com/library/e7efbbe1-6629-4d11-bed1-ed899e3f9d77%28Office.15%29.aspx), et la valeur de la **PR_ATTR_HIDDEN** étendu de propriété pour tous les sous-dossiers sous le dossier **msgrootfolder** .</span><span class="sxs-lookup"><span data-stu-id="8ee82-191">It contains only the [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx), the [DisplayName](http://msdn.microsoft.com/library/e7efbbe1-6629-4d11-bed1-ed899e3f9d77%28Office.15%29.aspx), and the value of the **PR_ATTR_HIDDEN** extended property for all the subfolders under the **msgrootfolder** folder.</span></span> <span data-ttu-id="8ee82-192">Si l’élément de la [valeur](http://msdn.microsoft.com/library/9a30cadd-909e-41b1-b4e9-291643dd89c6%28Office.15%29.aspx) est définie sur true, le dossier doit être masqué dans l’affichage du client.</span><span class="sxs-lookup"><span data-stu-id="8ee82-192">If the [Value](http://msdn.microsoft.com/library/9a30cadd-909e-41b1-b4e9-291643dd89c6%28Office.15%29.aspx) element is set to true, the folder should be hidden in the client view.</span></span> 
  
<span data-ttu-id="8ee82-193">C’est également la réponse XML de l’API managée EWS envoie lorsque vous récupérez plusieurs dossiers à l’aide de la méthode [FindFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="8ee82-193">This is also the XML response that the EWS Managed API sends when you get multiple folders by using the [FindFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) method.</span></span> <span data-ttu-id="8ee82-194">Les valeurs de certains attributs et éléments ont été raccourcies pour des raisons de lisibilité, et certains dossiers n’ont pas été inclus par souci de concision.</span><span class="sxs-lookup"><span data-stu-id="8ee82-194">The values of some attributes and elements have been shortened for readability, and some folders have not been included for brevity.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?><s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="815"
                         MinorBuildNumber="6"
                         Version="V2_7"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="update-a-folder-by-using-the-ews-managed-api"></a><span data-ttu-id="8ee82-195">Mettre à jour un dossier à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="8ee82-195">Update a folder by using the EWS Managed API</span></span>
<span data-ttu-id="8ee82-196"><a name="bk_updatefolderewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="8ee82-196"></span></span>

<span data-ttu-id="8ee82-197">L’exemple de code suivant montre comment mettre à jour le nom complet d’un dossier à l’aide de l’API managée EWS.</span><span class="sxs-lookup"><span data-stu-id="8ee82-197">The following code example shows how to update the display name of a folder by using the EWS Managed API.</span></span>
  
<span data-ttu-id="8ee82-198">Tout d’abord, créez une [classe PropertySet](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) pour limiter le nombre de propriétés renvoyant le serveur dans la réponse [Folder.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="8ee82-198">First, create a [PropertySet](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) to limit the number of properties that the server returns in the [Folder.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) response.</span></span> <span data-ttu-id="8ee82-199">Nous recommandons d’utiliser le **IdOnly** **BasePropertySet** afin de réduire les appels vers la base de données Exchange.</span><span class="sxs-lookup"><span data-stu-id="8ee82-199">We recommend that you use the **IdOnly** **BasePropertySet** to reduce calls to the Exchange database.</span></span> <span data-ttu-id="8ee82-200">Ensuite, utilisez la méthode de **liaison** pour lier au dossier à mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="8ee82-200">Next, use the **Bind** method to bind to the folder to update.</span></span> <span data-ttu-id="8ee82-201">Ensuite, mettre à jour la propriété [DisplayName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.displayname%28v=exchg.80%29.aspx) et utilisez la méthode [Folder.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) pour enregistrer les modifications.</span><span class="sxs-lookup"><span data-stu-id="8ee82-201">Then, update the [DisplayName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.displayname%28v=exchg.80%29.aspx) property, and use the [Folder.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) method to save the changes.</span></span> 
  
<span data-ttu-id="8ee82-202">Dans cet exemple, nous partons du principe que **service** est un objet [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur a été authentifié sur un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="8ee82-202">In this example, we assume that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> <span data-ttu-id="8ee82-203">La variable locale *folderId* est l' [Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx) du dossier à mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="8ee82-203">The local variable  *folderId*  is the [Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx) of the folder to update.</span></span> 
  
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

## <a name="update-a-folder-by-using-ews"></a><span data-ttu-id="8ee82-204">Mettre à jour un dossier à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="8ee82-204">Update a folder by using EWS</span></span>
<span data-ttu-id="8ee82-205"><a name="bk_updatefolderews"> </a></span><span class="sxs-lookup"><span data-stu-id="8ee82-205"></span></span>

<span data-ttu-id="8ee82-206">Les exemples de code XML suivants montrent comment mettre à jour le nom complet d’un dossier à l’aide de EWS.</span><span class="sxs-lookup"><span data-stu-id="8ee82-206">The following XML examples show how to update the display name of a folder by using EWS.</span></span>
  
<span data-ttu-id="8ee82-207">Tout d’abord, envoyer un message de demande d’opération [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) pour obtenir le dossier à mettre à jour, comme indiqué dans [obtenir une hiérarchie de dossiers à l’aide de EWS](#bk_getfolderhierarchyews).</span><span class="sxs-lookup"><span data-stu-id="8ee82-207">First, send a [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) operation request message to get the folder to update, as shown in [Get a folder hierarchy by using EWS](#bk_getfolderhierarchyews).</span></span>
  
<span data-ttu-id="8ee82-208">Ensuite, envoyer un message de demande d’opération [UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) au serveur pour mettre à jour un dossier.</span><span class="sxs-lookup"><span data-stu-id="8ee82-208">Next, send an [UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) operation request message to the server to update a folder.</span></span> <span data-ttu-id="8ee82-209">La requête d’opération **UpdateFolder** met à jour le [DisplayName](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) à « Mise à jour de dossier personnalisé ».</span><span class="sxs-lookup"><span data-stu-id="8ee82-209">The **UpdateFolder** operation request updates the [DisplayName](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) to "Updated Custom Folder".</span></span> 
  
<span data-ttu-id="8ee82-210">C’est également la demande XML qui envoie de l’API managée EWS lorsque vous mettez à jour un dossier à l’aide de la méthode [Folder.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="8ee82-210">This is also the XML request that the EWS Managed API sends when you update a folder by using the [Folder.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) method.</span></span> <span data-ttu-id="8ee82-211">Les valeurs de certains attributs et éléments ont été raccourcies pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="8ee82-211">The values of some attributes and elements have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="8ee82-212">Le serveur répond à la demande **UpdateFolder** avec un message [UpdateFolderResponse](http://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx) qui inclut la valeur [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) **NoError**et l' [ID FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) du dossier qui a été mis à jour avec une mise à jour ** ChangeKey** valeur d’attribut.</span><span class="sxs-lookup"><span data-stu-id="8ee82-212">The server responds to the **UpdateFolder** request with a [UpdateFolderResponse](http://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx) message that includes the a [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, and the [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) of the folder that was updated with an updated **ChangeKey** attribute value.</span></span> 
  
## <a name="delete-a-folder-by-using-the-ews-managed-api"></a><span data-ttu-id="8ee82-213">Supprimer un dossier à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="8ee82-213">Delete a folder by using the EWS Managed API</span></span>
<span data-ttu-id="8ee82-214"><a name="bk_deletefolderewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="8ee82-214"></span></span>

<span data-ttu-id="8ee82-215">Cet article fournit un exemple de base qui vous montre comment supprimer un dossier à l’aide de l’API managée EWS.</span><span class="sxs-lookup"><span data-stu-id="8ee82-215">This article provides a basic example that shows you how to delete a folder by using the EWS Managed API.</span></span> <span data-ttu-id="8ee82-216">Pour plus d’informations sur la suppression des dossiers, voir [suppression d’éléments à l’aide de EWS dans Exchange](deleting-items-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="8ee82-216">For more details about deleting folders, see [Deleting items by using EWS in Exchange](deleting-items-by-using-ews-in-exchange.md).</span></span>
  
<span data-ttu-id="8ee82-217">Pour supprimer un dossier à l’aide de l’API managée EWS, tout d’abord, utilisez la méthode [Folder.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) pour lier à l’objet de service pour le dossier à supprimer.</span><span class="sxs-lookup"><span data-stu-id="8ee82-217">To delete a folder by using the EWS Managed API, first, use the [Folder.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) method to bind to the service object to the folder to delete.</span></span> <span data-ttu-id="8ee82-218">Ensuite, utilisez la méthode [Folder.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) pour supprimer le dossier en utilisant le mode de suppression [HardDelete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.deletemode%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="8ee82-218">Next, use the [Folder.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) method to delete the folder by using the [HardDelete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.deletemode%28v=exchg.80%29.aspx) deletion mode.</span></span> 
  
<span data-ttu-id="8ee82-219">Cet exemple suppose que ce **service** est un objet [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur a été authentifié sur un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="8ee82-219">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> <span data-ttu-id="8ee82-220">La variable locale *folderId* est l' [Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx) du dossier à supprimer.</span><span class="sxs-lookup"><span data-stu-id="8ee82-220">The local variable  *folderId*  is the [Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx) of the folder to delete.</span></span> 
  
```cs
// Bind to an existing folder and get all its properties.
// This method call results in a GetFolder call to EWS.
Folder folder = Folder.Bind(service, folderId);
// HardDelete the folder.
// This method call results in a DeleteFolder call to EWS.
folder.Delete(DeleteMode.HardDelete);
```

## <a name="delete-a-folder-by-using-ews"></a><span data-ttu-id="8ee82-221">Supprimer un dossier à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="8ee82-221">Delete a folder by using EWS</span></span>
<span data-ttu-id="8ee82-222"><a name="bk_deletefolderews"> </a></span><span class="sxs-lookup"><span data-stu-id="8ee82-222"></span></span>

<span data-ttu-id="8ee82-223">Cet article fournit un exemple de base XML qui vous montre comment supprimer un dossier à l’aide de EWS.</span><span class="sxs-lookup"><span data-stu-id="8ee82-223">This article provides a basic XML example that shows you how to delete a folder by using EWS.</span></span> <span data-ttu-id="8ee82-224">Pour plus d’informations sur la suppression des dossiers, voir [suppression d’éléments à l’aide de EWS dans Exchange](deleting-items-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="8ee82-224">For more details about deleting folders, see [Deleting items by using EWS in Exchange](deleting-items-by-using-ews-in-exchange.md).</span></span>
  
<span data-ttu-id="8ee82-225">Pour supprimer un dossier à l’aide de EWS, tout d’abord, envoyer un message de demande d’opération [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) pour obtenir le dossier à mettre à jour comme indiqué dans [obtenir un dossier à l’aide de EWS](#bk_getfolderews).</span><span class="sxs-lookup"><span data-stu-id="8ee82-225">To delete a folder by using EWS, first, send a [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) operation request message to get the folder to update as shown in [Get a folder by using EWS](#bk_getfolderews).</span></span> 
  
<span data-ttu-id="8ee82-226">Ensuite, envoyer un message de demande d’opération [DeleteFolder](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) au serveur pour supprimer le dossier.</span><span class="sxs-lookup"><span data-stu-id="8ee82-226">Next, send a [DeleteFolder](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) operation request message to the server to delete the folder.</span></span> <span data-ttu-id="8ee82-227">La requête d’opération **DeleteFolder** indique que le **DeleType** est **HardDelete** et il inclut [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) du dossier à supprimer.</span><span class="sxs-lookup"><span data-stu-id="8ee82-227">The **DeleteFolder** operation request indicates that the **DeleteType** is **HardDelete** and it includes the [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) of the folder to delete.</span></span> 
  
<span data-ttu-id="8ee82-228">C’est également la demande XML qui envoie de l’API managée EWS lorsque vous supprimez un dossier à l’aide de la méthode [Folder.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="8ee82-228">This is also the XML request that the EWS Managed API sends when you delete a folder by using the [Folder.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) method.</span></span> <span data-ttu-id="8ee82-229">Les valeurs de certains attributs et éléments ont été raccourcies pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="8ee82-229">The values of some attributes and elements have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="8ee82-230">Le serveur répond à la demande **DeleteFolder** avec un message [DeleteFolderResponse](http://msdn.microsoft.com/library/27578bda-ef0a-4a33-bccc-2c1bc1735424%28Office.15%29.aspx) qui inclut la valeur [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) **NoError**, ce qui indique que la suppression du dossier a réussi.</span><span class="sxs-lookup"><span data-stu-id="8ee82-230">The server responds to the **DeleteFolder** request with a [DeleteFolderResponse](http://msdn.microsoft.com/library/27578bda-ef0a-4a33-bccc-2c1bc1735424%28Office.15%29.aspx) message that includes the a [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the folder deletion was successful.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="8ee82-231">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="8ee82-231">Next steps</span></span>
<span data-ttu-id="8ee82-232"><a name="bk_nextsteps"> </a></span><span class="sxs-lookup"><span data-stu-id="8ee82-232"></span></span>

<span data-ttu-id="8ee82-233">Après avoir récupéré les dossiers sur le serveur, ou apporté des modifications aux dossiers, vous voudrez [synchroniser votre hiérarchie de dossiers](how-to-synchronize-folders-by-using-ews-in-exchange.md) ou [s’abonner aux notifications sur les modifications du dossier](notification-subscriptions-mailbox-events-and-ews-in-exchange.md) sur le serveur.</span><span class="sxs-lookup"><span data-stu-id="8ee82-233">After you have retrieved the folders on the server, or made changes to folders, you might want to [synchronize your folder hierarchy](how-to-synchronize-folders-by-using-ews-in-exchange.md) or [subscribe to notifications about folder changes](notification-subscriptions-mailbox-events-and-ews-in-exchange.md) on the server.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="8ee82-234">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="8ee82-234">See also</span></span>

- [<span data-ttu-id="8ee82-235">Dossiers et éléments dans EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="8ee82-235">Folders and items in EWS in Exchange</span></span>](folders-and-items-in-ews-in-exchange.md)   
- [<span data-ttu-id="8ee82-236">Travailler avec des éléments de boîte aux lettres Exchange à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="8ee82-236">Work with Exchange mailbox items by using EWS in Exchange</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md)    
- [<span data-ttu-id="8ee82-237">Suppression d’éléments à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="8ee82-237">Deleting items by using EWS in Exchange</span></span>](deleting-items-by-using-ews-in-exchange.md)   
- [<span data-ttu-id="8ee82-238">Développer des clients de service web pour Exchange</span><span class="sxs-lookup"><span data-stu-id="8ee82-238">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    

