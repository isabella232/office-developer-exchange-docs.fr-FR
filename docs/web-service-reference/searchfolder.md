---
title: SearchFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SearchFolder
api_type:
- schema
ms.assetid: 1a7d408b-2e98-4391-8834-085ed6d5757c
description: L’élément SearchFolder représente un dossier de recherche contenu dans une boîte aux lettres.
ms.openlocfilehash: e1d5893e00f3b199451622061785e2566c6f32e5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464006"
---
# <a name="searchfolder"></a><span data-ttu-id="9a5ff-103">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="9a5ff-103">SearchFolder</span></span>

<span data-ttu-id="9a5ff-104">L’élément **SearchFolder** représente un dossier de recherche contenu dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="9a5ff-104">The **SearchFolder** element represents a search folder that is contained in a mailbox.</span></span> 
  
```xml
<SearchFolder>
   <FolderId/>
   <ParentFolderId/>
   <FolderClass/>
   <DisplayName/>
   <TotalCount/>
   <ChildFolderCount/>
   <ExtendedProperty/>
   <ManagedFolderInformation/>
   <UnreadCount/>
   <SearchParameters/>
   <PermissionSet/>
      <EffectiveRights/>
</SearchFolder>
```

 <span data-ttu-id="9a5ff-105">**SearchFolderType**</span><span class="sxs-lookup"><span data-stu-id="9a5ff-105">**SearchFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9a5ff-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="9a5ff-106">Attributes and elements</span></span>

<span data-ttu-id="9a5ff-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="9a5ff-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9a5ff-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="9a5ff-108">Attributes</span></span>

<span data-ttu-id="9a5ff-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="9a5ff-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9a5ff-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="9a5ff-110">Child elements</span></span>

|<span data-ttu-id="9a5ff-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9a5ff-111">**Element**</span></span>|<span data-ttu-id="9a5ff-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="9a5ff-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9a5ff-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="9a5ff-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="9a5ff-114">Contient l’identificateur et la clé de modification d’un dossier.</span><span class="sxs-lookup"><span data-stu-id="9a5ff-114">Contains the identifier and change key of a folder.</span></span>  <br/> |
|[<span data-ttu-id="9a5ff-115">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="9a5ff-115">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="9a5ff-116">Représente l’identificateur du dossier parent qui contient le dossier.</span><span class="sxs-lookup"><span data-stu-id="9a5ff-116">Represents the identifier of the parent folder that contains the folder.</span></span>  <br/> |
|[<span data-ttu-id="9a5ff-117">FolderClass</span><span class="sxs-lookup"><span data-stu-id="9a5ff-117">FolderClass</span></span>](folderclass.md) <br/> |<span data-ttu-id="9a5ff-118">Représente la classe de dossier pour un dossier donné.</span><span class="sxs-lookup"><span data-stu-id="9a5ff-118">Represents the folder class for a given folder.</span></span>  <br/> |
|[<span data-ttu-id="9a5ff-119">DisplayName (chaîne)</span><span class="sxs-lookup"><span data-stu-id="9a5ff-119">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="9a5ff-120">Contient le nom complet d’un dossier.</span><span class="sxs-lookup"><span data-stu-id="9a5ff-120">Contains the display name of a folder.</span></span>  <br/> |
|[<span data-ttu-id="9a5ff-121">TotalCount</span><span class="sxs-lookup"><span data-stu-id="9a5ff-121">TotalCount</span></span>](totalcount.md) <br/> |<span data-ttu-id="9a5ff-122">Représente le nombre total d’éléments dans un dossier donné.</span><span class="sxs-lookup"><span data-stu-id="9a5ff-122">Represents the total count of items within a given folder.</span></span>  <br/> |
|[<span data-ttu-id="9a5ff-123">ChildFolderCount</span><span class="sxs-lookup"><span data-stu-id="9a5ff-123">ChildFolderCount</span></span>](childfoldercount.md) <br/> |<span data-ttu-id="9a5ff-124">Représente le nombre de dossiers enfants contenus dans un dossier.</span><span class="sxs-lookup"><span data-stu-id="9a5ff-124">Represents the number of child folders contained within a folder.</span></span> <span data-ttu-id="9a5ff-125">Cette propriété est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="9a5ff-125">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="9a5ff-126">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="9a5ff-126">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="9a5ff-127">Identifie les propriétés étendues des dossiers.</span><span class="sxs-lookup"><span data-stu-id="9a5ff-127">Identifies extended properties on folders.</span></span>  <br/> |
|[<span data-ttu-id="9a5ff-128">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="9a5ff-128">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="9a5ff-129">Contient des informations sur un dossier géré.</span><span class="sxs-lookup"><span data-stu-id="9a5ff-129">Contains information about a managed folder.</span></span>  <br/> |
|[<span data-ttu-id="9a5ff-130">UnreadCount</span><span class="sxs-lookup"><span data-stu-id="9a5ff-130">UnreadCount</span></span>](unreadcount.md) <br/> |<span data-ttu-id="9a5ff-131">Représente le nombre d’éléments non lus dans un dossier donné.</span><span class="sxs-lookup"><span data-stu-id="9a5ff-131">Represents the count of unread items within a given folder.</span></span>  <br/> |
|[<span data-ttu-id="9a5ff-132">SearchParameters</span><span class="sxs-lookup"><span data-stu-id="9a5ff-132">SearchParameters</span></span>](searchparameters.md) <br/> |<span data-ttu-id="9a5ff-133">Contient les paramètres qui définissent un dossier de recherche.</span><span class="sxs-lookup"><span data-stu-id="9a5ff-133">Contains the parameters that define a search folder.</span></span>  <br/> |
|[<span data-ttu-id="9a5ff-134">PermissionSet (PermissionSetType)</span><span class="sxs-lookup"><span data-stu-id="9a5ff-134">PermissionSet (PermissionSetType)</span></span>](permissionset-permissionsettype.md) <br/> |<span data-ttu-id="9a5ff-135">Contient toutes les autorisations configurées pour un dossier.</span><span class="sxs-lookup"><span data-stu-id="9a5ff-135">Contains all the configured permissions for a folder.</span></span> <span data-ttu-id="9a5ff-136">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="9a5ff-136">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="9a5ff-137">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="9a5ff-137">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="9a5ff-138">Contient les droits du client en fonction des paramètres d'autorisation pour l'élément ou le dossier.</span><span class="sxs-lookup"><span data-stu-id="9a5ff-138">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="9a5ff-139">Cet élément est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="9a5ff-139">This element is read-only.</span></span> <span data-ttu-id="9a5ff-140">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="9a5ff-140">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9a5ff-141">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="9a5ff-141">Parent elements</span></span>

|<span data-ttu-id="9a5ff-142">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9a5ff-142">**Element**</span></span>|<span data-ttu-id="9a5ff-143">**Description**</span><span class="sxs-lookup"><span data-stu-id="9a5ff-143">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9a5ff-144">AppendToFolderField</span><span class="sxs-lookup"><span data-stu-id="9a5ff-144">AppendToFolderField</span></span>](appendtofolderfield.md) <br/> |<span data-ttu-id="9a5ff-145">Spécifie les données à ajouter à une propriété de dossier lors d’une [opération UpdateFolder](updatefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="9a5ff-145">Specifies data to append to a folder property during an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="9a5ff-146">Créer (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="9a5ff-146">Create (FolderSync)</span></span>](create-foldersync.md) <br/> |<span data-ttu-id="9a5ff-147">Identifie un dossier unique à créer dans le magasin de client local.</span><span class="sxs-lookup"><span data-stu-id="9a5ff-147">Identifies a single folder to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="9a5ff-148">SetFolderField</span><span class="sxs-lookup"><span data-stu-id="9a5ff-148">SetFolderField</span></span>](setfolderfield.md) <br/> |<span data-ttu-id="9a5ff-149">Représente une mise à jour d’une propriété unique sur un dossier dans une [opération UpdateFolder](updatefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="9a5ff-149">Represents an update to a single property on a folder in an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="9a5ff-150">Mise à jour (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="9a5ff-150">Update (FolderSync)</span></span>](update-foldersync.md) <br/> |<span data-ttu-id="9a5ff-151">Identifie un dossier unique à mettre à jour dans le magasin client local.</span><span class="sxs-lookup"><span data-stu-id="9a5ff-151">Identifies a single folder to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="9a5ff-152">Dossiers</span><span class="sxs-lookup"><span data-stu-id="9a5ff-152">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="9a5ff-153">Contient un tableau de dossiers utilisés dans les opérations de dossier.</span><span class="sxs-lookup"><span data-stu-id="9a5ff-153">Contains an array of folders used in folder operations.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9a5ff-154">Remarques</span><span class="sxs-lookup"><span data-stu-id="9a5ff-154">Remarks</span></span>

 <span data-ttu-id="9a5ff-155">**SearchFolder** est utilisé pour les dossiers de recherche standard et les dossiers de recherche visibles MicrosoftOfficeOutlook et Outlook Web Access.</span><span class="sxs-lookup"><span data-stu-id="9a5ff-155">**SearchFolder** is used for both regular search folders and MicrosoftOfficeOutlook and Outlook Web Access visible search folders.</span></span> <span data-ttu-id="9a5ff-156">Pour qu’un dossier de recherche soit visible dans Outlook et Outlook Web Access, le dossier doit être créé sous le dossier unique SearchFolders.</span><span class="sxs-lookup"><span data-stu-id="9a5ff-156">For a search folder to be visible to Outlook and Outlook Web Access, the folder must be created under the SearchFolders distinguished folder.</span></span> 
  
<span data-ttu-id="9a5ff-157">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="9a5ff-157">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9a5ff-158">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="9a5ff-158">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9a5ff-159">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="9a5ff-159">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9a5ff-160">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="9a5ff-160">Schema Name</span></span>  <br/> |<span data-ttu-id="9a5ff-161">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="9a5ff-161">Types schema</span></span>  <br/> |
|<span data-ttu-id="9a5ff-162">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="9a5ff-162">Validation File</span></span>  <br/> |<span data-ttu-id="9a5ff-163">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9a5ff-163">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9a5ff-164">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="9a5ff-164">Can be Empty</span></span>  <br/> |<span data-ttu-id="9a5ff-165">False</span><span class="sxs-lookup"><span data-stu-id="9a5ff-165">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9a5ff-166">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="9a5ff-166">See also</span></span>



- [<span data-ttu-id="9a5ff-167">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="9a5ff-167">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

