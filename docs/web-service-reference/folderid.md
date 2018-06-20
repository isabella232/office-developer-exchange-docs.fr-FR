---
title: FolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FolderId
api_type:
- schema
ms.assetid: 00d14e3e-4365-4f21-8f88-eaeea73b9bf7
description: L’élément FolderId contient la clé d’identificateur et de modification d’un dossier.
ms.openlocfilehash: 5764a164d5af183b8f313955ace5274dc6023a6a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756451"
---
# <a name="folderid"></a><span data-ttu-id="6ed79-103">FolderId</span><span class="sxs-lookup"><span data-stu-id="6ed79-103">FolderId</span></span>

<span data-ttu-id="6ed79-104">L’élément **FolderId** contient la clé d’identificateur et de modification d’un dossier.</span><span class="sxs-lookup"><span data-stu-id="6ed79-104">The **FolderId** element contains the identifier and change key of a folder.</span></span> 
  
```XML
<FolderId Id="" ChangeKey="" />
```

 <span data-ttu-id="6ed79-105">**FolderIdType**</span><span class="sxs-lookup"><span data-stu-id="6ed79-105">**FolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6ed79-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="6ed79-106">Attributes and elements</span></span>

<span data-ttu-id="6ed79-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="6ed79-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6ed79-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="6ed79-108">Attributes</span></span>

|<span data-ttu-id="6ed79-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="6ed79-109">**Attribute**</span></span>|<span data-ttu-id="6ed79-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="6ed79-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6ed79-111">ID</span><span class="sxs-lookup"><span data-stu-id="6ed79-111">Id</span></span>  <br/> |<span data-ttu-id="6ed79-112">Contient une chaîne qui identifie un dossier dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="6ed79-112">Contains a string that identifies a folder in the Exchange store.</span></span> <span data-ttu-id="6ed79-113">Cet attribut est requis.</span><span class="sxs-lookup"><span data-stu-id="6ed79-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="6ed79-114">ChangeKey</span><span class="sxs-lookup"><span data-stu-id="6ed79-114">ChangeKey</span></span>  <br/> |<span data-ttu-id="6ed79-115">Contient une chaîne qui identifie une version d’un dossier qui est identifié par l’attribut Id.</span><span class="sxs-lookup"><span data-stu-id="6ed79-115">Contains a string that identifies a version of a folder that is identified by the Id attribute.</span></span> <span data-ttu-id="6ed79-116">Cet attribut est facultatif.</span><span class="sxs-lookup"><span data-stu-id="6ed79-116">This attribute is optional.</span></span> <span data-ttu-id="6ed79-117">Utilisez cet attribut pour vous assurer que la version correcte d’un dossier est utilisée.</span><span class="sxs-lookup"><span data-stu-id="6ed79-117">Use this attribute to make sure that the correct version of a folder is used.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="6ed79-118">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="6ed79-118">Child elements</span></span>

<span data-ttu-id="6ed79-119">Aucun.</span><span class="sxs-lookup"><span data-stu-id="6ed79-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6ed79-120">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="6ed79-120">Parent elements</span></span>

|<span data-ttu-id="6ed79-121">**Élément**</span><span class="sxs-lookup"><span data-stu-id="6ed79-121">**Element**</span></span>|<span data-ttu-id="6ed79-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="6ed79-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6ed79-123">ContextFolderId</span><span class="sxs-lookup"><span data-stu-id="6ed79-123">ContextFolderId</span></span>](contextfolderid.md) <br/> |<span data-ttu-id="6ed79-124">Indique le dossier qui est ciblé pour les actions qui utilisent des dossiers.</span><span class="sxs-lookup"><span data-stu-id="6ed79-124">Indicates the folder that is targeted for actions that use folders.</span></span>  <br/> |
|[<span data-ttu-id="6ed79-125">CopiedEvent</span><span class="sxs-lookup"><span data-stu-id="6ed79-125">CopiedEvent</span></span>](copiedevent.md) <br/> |<span data-ttu-id="6ed79-126">Représente un événement dans lequel un élément ou un dossier est copié.</span><span class="sxs-lookup"><span data-stu-id="6ed79-126">Represents an event in which an item or folder is copied.</span></span>  <br/> |
|[<span data-ttu-id="6ed79-127">DestinationFolderId</span><span class="sxs-lookup"><span data-stu-id="6ed79-127">DestinationFolderId</span></span>](destinationfolderid.md) <br/> |<span data-ttu-id="6ed79-128">Indique le dossier de destination de copie et les actions de déplacement.</span><span class="sxs-lookup"><span data-stu-id="6ed79-128">Indicates the destination folder for copy and move actions.</span></span>  <br/> |
|[<span data-ttu-id="6ed79-129">ParentFolderId (TargetFolderIdType)</span><span class="sxs-lookup"><span data-stu-id="6ed79-129">ParentFolderId (TargetFolderIdType)</span></span>](parentfolderid-targetfolderidtype.md) <br/> | <span data-ttu-id="6ed79-130">Identifie le dossier dans lequel un nouveau dossier ou un élément est créé.</span><span class="sxs-lookup"><span data-stu-id="6ed79-130">Identifies the folder where a new folder or item is created.</span></span>  <br/><br/>  <span data-ttu-id="6ed79-131">Les expressions XPath pour cet élément sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="6ed79-131">The following are the XPath expressions to this element:</span></span><br/>  <br/> `/CreateItem/ParentFolderId` <br/><br/>  `/CreateFolder/ParentFolderId` <br/> |
|[<span data-ttu-id="6ed79-132">BaseFolderIds</span><span class="sxs-lookup"><span data-stu-id="6ed79-132">BaseFolderIds</span></span>](basefolderids.md) <br/> |<span data-ttu-id="6ed79-133">Représente la collection de dossiers qui seront être interrogées pour déterminer le contenu d’un dossier de recherche.</span><span class="sxs-lookup"><span data-stu-id="6ed79-133">Represents the collection of folders that will be mined to determine the contents of a search folder.</span></span>  <br/> |
|[<span data-ttu-id="6ed79-134">Supprimer (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="6ed79-134">Delete (FolderSync)</span></span>](delete-foldersync.md) <br/> |<span data-ttu-id="6ed79-135">Identifie un seul dossier à supprimer dans le magasin de client local.</span><span class="sxs-lookup"><span data-stu-id="6ed79-135">Identifies a single folder to delete in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="6ed79-136">Folder</span><span class="sxs-lookup"><span data-stu-id="6ed79-136">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="6ed79-137">Représente un dossier dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="6ed79-137">Represents a folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="6ed79-138">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="6ed79-138">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="6ed79-139">Représente un dossier de calendrier dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="6ed79-139">Represents a calendar folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="6ed79-140">FolderChange</span><span class="sxs-lookup"><span data-stu-id="6ed79-140">FolderChange</span></span>](folderchange.md) <br/> |<span data-ttu-id="6ed79-141">Représente une collection des modifications à effectuer sur un seul dossier.</span><span class="sxs-lookup"><span data-stu-id="6ed79-141">Represents a collection of changes to be performed on a single folder.</span></span>  <br/> <span data-ttu-id="6ed79-142">Vous trouverez ci-dessous l’expression XPath pour cet élément :`/UpdateFolder/FolderChanges/FolderChange`</span><span class="sxs-lookup"><span data-stu-id="6ed79-142">The following is the XPath expression to this element:  `/UpdateFolder/FolderChanges/FolderChange`</span></span> <br/> |
|[<span data-ttu-id="6ed79-143">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="6ed79-143">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="6ed79-144">Représente un dossier de contacts dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="6ed79-144">Represents a contact folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="6ed79-145">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="6ed79-145">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="6ed79-146">Représente un dossier de recherche dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="6ed79-146">Represents a search folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="6ed79-147">Dossier tâches</span><span class="sxs-lookup"><span data-stu-id="6ed79-147">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="6ed79-148">Représente un dossier de tâches dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="6ed79-148">Represents a task folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="6ed79-149">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="6ed79-149">ToFolderId</span></span>](tofolderid.md) <br/> | <span data-ttu-id="6ed79-150">Représente le dossier de destination pour un dossier ou un élément copié ou déplacé.</span><span class="sxs-lookup"><span data-stu-id="6ed79-150">Represents the destination folder for a copied or moved item or folder.</span></span> <br/> <br/>  <span data-ttu-id="6ed79-151">Les expressions XPath pour cet élément sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="6ed79-151">The following are the XPath expressions to this element:</span></span> <br/> <br/>  `/MoveFolder/ToFolderId` <br/> <br/> `/CopyFolder/ToFolderId` <br/> <br/> `/MoveItem/ToFolderId`<br/> <br/>  `/CopyItem/ToFolderId` <br/> |
|[<span data-ttu-id="6ed79-152">SavedItemFolderId</span><span class="sxs-lookup"><span data-stu-id="6ed79-152">SavedItemFolderId</span></span>](saveditemfolderid.md) <br/> | <span data-ttu-id="6ed79-153">Identifie le dossier cible pour les opérations de mise à jour, d’envoyer et de créer des éléments dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="6ed79-153">Identifies the target folder for operations that update, send, and create items in the Exchange store.</span></span>  <br/><br/>  <span data-ttu-id="6ed79-154">Les expressions XPath pour cet élément sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="6ed79-154">The following are the XPath expressions to this element:</span></span> <br/> <br/>  `/CreateItem/SavedItemFolderId` <br/><br/>  `/UpdateItem/SavedItemFolderId` <br/><br/>  `/SendItem/SavedItemFolderId` <br/> |
|[<span data-ttu-id="6ed79-155">SyncFolderId</span><span class="sxs-lookup"><span data-stu-id="6ed79-155">SyncFolderId</span></span>](syncfolderid.md) <br/> |<span data-ttu-id="6ed79-156">Représente le dossier qui contient les éléments à synchroniser.</span><span class="sxs-lookup"><span data-stu-id="6ed79-156">Represents the folder that contains the items to synchronize.</span></span>  <br/> |
|[<span data-ttu-id="6ed79-157">UserConfigurationName</span><span class="sxs-lookup"><span data-stu-id="6ed79-157">UserConfigurationName</span></span>](userconfigurationname.md) <br/> |<span data-ttu-id="6ed79-158">Représente le nom d’un objet de configuration utilisateur.</span><span class="sxs-lookup"><span data-stu-id="6ed79-158">Represents the name of a user configuration object.</span></span> <span data-ttu-id="6ed79-159">Le nom d’objet de configuration utilisateur est l’identificateur pour un objet de configuration utilisateur.</span><span class="sxs-lookup"><span data-stu-id="6ed79-159">The user configuration object name is the identifier for a user configuration object.</span></span>  <br/> |
|[<span data-ttu-id="6ed79-160">CopyToFolder</span><span class="sxs-lookup"><span data-stu-id="6ed79-160">CopyToFolder</span></span>](copytofolder.md) <br/> |<span data-ttu-id="6ed79-161">Identifie l’ID du dossier qui sont copiées dans les éléments de courrier électronique.</span><span class="sxs-lookup"><span data-stu-id="6ed79-161">Identifies the ID of the folder that e-mail items will be copied to.</span></span>  <br/> |
|[<span data-ttu-id="6ed79-162">MoveToFolder</span><span class="sxs-lookup"><span data-stu-id="6ed79-162">MoveToFolder</span></span>](movetofolder.md) <br/> |<span data-ttu-id="6ed79-163">Identifie l’ID du dossier qui seront déplacées vers des éléments de courrier électronique.</span><span class="sxs-lookup"><span data-stu-id="6ed79-163">Identifies the ID of the folder that e-mail items will be moved to.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6ed79-164">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="6ed79-164">Text value</span></span>

<span data-ttu-id="6ed79-165">Aucun.</span><span class="sxs-lookup"><span data-stu-id="6ed79-165">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6ed79-166">Remarques</span><span class="sxs-lookup"><span data-stu-id="6ed79-166">Remarks</span></span>

<span data-ttu-id="6ed79-167">Tous les éléments **FolderId** sont du type **FolderIdType** .</span><span class="sxs-lookup"><span data-stu-id="6ed79-167">All **FolderId** elements are of the **FolderIdType** type.</span></span> <span data-ttu-id="6ed79-168">L’élément **FolderId** est requis dans chaque cas, à l’exception des éléments dont le type étend la **BaseFolderType** ou où l’élément **FolderId** fait partie d’un choix.</span><span class="sxs-lookup"><span data-stu-id="6ed79-168">The **FolderId** element is required in every case except in elements whose type extends the **BaseFolderType** or where the **FolderId** element is a part of a choice.</span></span> <span data-ttu-id="6ed79-169">Passez en revue le schéma pour plus d’informations.</span><span class="sxs-lookup"><span data-stu-id="6ed79-169">Review the schema for more information.</span></span> 
  
<span data-ttu-id="6ed79-170">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="6ed79-170">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6ed79-171">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="6ed79-171">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6ed79-172">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="6ed79-172">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6ed79-173">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="6ed79-173">Schema Name</span></span>  <br/> |<span data-ttu-id="6ed79-174">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="6ed79-174">Types schema</span></span>  <br/> |
|<span data-ttu-id="6ed79-175">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="6ed79-175">Validation File</span></span>  <br/> |<span data-ttu-id="6ed79-176">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6ed79-176">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6ed79-177">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="6ed79-177">Can be Empty</span></span>  <br/> |<span data-ttu-id="6ed79-178">False</span><span class="sxs-lookup"><span data-stu-id="6ed79-178">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6ed79-179">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="6ed79-179">See also</span></span>

- [<span data-ttu-id="6ed79-180">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="6ed79-180">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="6ed79-181">Création de dossiers (Exchange Web Services)</span><span class="sxs-lookup"><span data-stu-id="6ed79-181">Creating Folders (Exchange Web Services)</span></span>](http://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

