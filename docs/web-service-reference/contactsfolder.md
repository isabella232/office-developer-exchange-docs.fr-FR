---
title: ContactsFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ContactsFolder
api_type:
- schema
ms.assetid: 6c299de8-2087-4aeb-8e66-2bc7586509a6
description: L’élément ContactsFolder représente un dossier de contacts qui se trouve dans une boîte aux lettres.
ms.openlocfilehash: 01302f00d84cfff9713e3b188b7799c537fc0629
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755565"
---
# <a name="contactsfolder"></a><span data-ttu-id="28b63-103">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="28b63-103">ContactsFolder</span></span>

<span data-ttu-id="28b63-104">L’élément **ContactsFolder** représente un dossier de contacts qui se trouve dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="28b63-104">The **ContactsFolder** element represents a contacts folder that is contained in a mailbox.</span></span> 
  
```xml
<ContactsFolder>
   <FolderId/>
   <ParentFolderId/>
   <FolderClass/>
   <DisplayName/>
   <TotalCount/>
   <ChildFolderCount/>
   <ExtendedProperty/>
   <ManagedFolderInformation/>
   <EffectiveRights/>
   <SharingEffectiveRights/>
   <PermissionSet/>
</ContactsFolder>
```

 <span data-ttu-id="28b63-105">**ContactsFolderType**</span><span class="sxs-lookup"><span data-stu-id="28b63-105">**ContactsFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="28b63-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="28b63-106">Attributes and elements</span></span>

<span data-ttu-id="28b63-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="28b63-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="28b63-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="28b63-108">Attributes</span></span>

<span data-ttu-id="28b63-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="28b63-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="28b63-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="28b63-110">Child elements</span></span>

|<span data-ttu-id="28b63-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="28b63-111">**Element**</span></span>|<span data-ttu-id="28b63-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="28b63-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="28b63-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="28b63-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="28b63-114">Contient la clé d’identificateur et de modification d’un dossier contacts.</span><span class="sxs-lookup"><span data-stu-id="28b63-114">Contains the identifier and change key of a contacts folder.</span></span>  <br/> |
|[<span data-ttu-id="28b63-115">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="28b63-115">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="28b63-116">Représente l’identificateur du dossier parent qui contient le dossier contacts.</span><span class="sxs-lookup"><span data-stu-id="28b63-116">Represents the identifier of the parent folder that contains the contacts folder.</span></span>  <br/> |
|[<span data-ttu-id="28b63-117">Classe FolderClass</span><span class="sxs-lookup"><span data-stu-id="28b63-117">FolderClass</span></span>](folderclass.md) <br/> |<span data-ttu-id="28b63-118">Représente la classe de dossier pour un dossier contacts.</span><span class="sxs-lookup"><span data-stu-id="28b63-118">Represents the folder class for a contacts folder.</span></span>  <br/> |
|[<span data-ttu-id="28b63-119">DisplayName (chaîne)</span><span class="sxs-lookup"><span data-stu-id="28b63-119">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="28b63-120">Contient le nom complet d’un dossier contacts.</span><span class="sxs-lookup"><span data-stu-id="28b63-120">Contains the display name of a contacts folder.</span></span>  <br/> |
|[<span data-ttu-id="28b63-121">TotalCount</span><span class="sxs-lookup"><span data-stu-id="28b63-121">TotalCount</span></span>](totalcount.md) <br/> |<span data-ttu-id="28b63-122">Représente le nombre total d’éléments dans un dossier contacts.</span><span class="sxs-lookup"><span data-stu-id="28b63-122">Represents the total count of items within a contacts folder.</span></span>  <br/> |
|[<span data-ttu-id="28b63-123">ChildFolderCount</span><span class="sxs-lookup"><span data-stu-id="28b63-123">ChildFolderCount</span></span>](childfoldercount.md) <br/> |<span data-ttu-id="28b63-124">Représente le nombre de dossiers enfants qui sont contenues dans un dossier contacts.</span><span class="sxs-lookup"><span data-stu-id="28b63-124">Represents the number of child folders that are contained within a contacts folder.</span></span> <span data-ttu-id="28b63-125">Cette propriété est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="28b63-125">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="28b63-126">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="28b63-126">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="28b63-127">Identifie les propriétés étendues dans les dossiers de contacts.</span><span class="sxs-lookup"><span data-stu-id="28b63-127">Identifies extended properties on contacts folders.</span></span>  <br/> |
|[<span data-ttu-id="28b63-128">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="28b63-128">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="28b63-129">Contient des informations sur un dossier géré.</span><span class="sxs-lookup"><span data-stu-id="28b63-129">Contains information about a managed folder.</span></span>  <br/> |
|[<span data-ttu-id="28b63-130">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="28b63-130">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="28b63-131">Contient les droits du client en fonction des paramètres d'autorisation pour l'élément ou le dossier.</span><span class="sxs-lookup"><span data-stu-id="28b63-131">Contains the client's rights based on the permission settings for the item or folder.</span></span>  <br/> |
|[<span data-ttu-id="28b63-132">SharingEffectiveRights (PermissionReadAccessType)</span><span class="sxs-lookup"><span data-stu-id="28b63-132">SharingEffectiveRights (PermissionReadAccessType)</span></span>](sharingeffectiverights-permissionreadaccesstype.md) <br/> |<span data-ttu-id="28b63-133">Indique les autorisations dont dispose l’utilisateur pour les données de contact qui sont partagées.</span><span class="sxs-lookup"><span data-stu-id="28b63-133">Indicates the permissions that the user has for the contact data that is being shared.</span></span>  <br/> |
|[<span data-ttu-id="28b63-134">PermissionSet (PermissionSetType)</span><span class="sxs-lookup"><span data-stu-id="28b63-134">PermissionSet (PermissionSetType)</span></span>](permissionset-permissionsettype.md) <br/> |<span data-ttu-id="28b63-135">Contient toutes les autorisations configurées pour un dossier.</span><span class="sxs-lookup"><span data-stu-id="28b63-135">Contains all the configured permissions for a folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="28b63-136">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="28b63-136">Parent elements</span></span>

|<span data-ttu-id="28b63-137">**Élément**</span><span class="sxs-lookup"><span data-stu-id="28b63-137">**Element**</span></span>|<span data-ttu-id="28b63-138">**Description**</span><span class="sxs-lookup"><span data-stu-id="28b63-138">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="28b63-139">AppendToFolderField</span><span class="sxs-lookup"><span data-stu-id="28b63-139">AppendToFolderField</span></span>](appendtofolderfield.md) <br/> |<span data-ttu-id="28b63-140">Spécifie les données à ajouter à une propriété de dossier lors d’une [opération UpdateFolder](updatefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="28b63-140">Specifies data to append to a folder property during an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="28b63-141">Créer (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="28b63-141">Create (FolderSync)</span></span>](create-foldersync.md) <br/> |<span data-ttu-id="28b63-142">Identifie un dossier unique à créer dans le magasin de client local.</span><span class="sxs-lookup"><span data-stu-id="28b63-142">Identifies a single folder to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="28b63-143">SetFolderField</span><span class="sxs-lookup"><span data-stu-id="28b63-143">SetFolderField</span></span>](setfolderfield.md) <br/> |<span data-ttu-id="28b63-144">Représente une mise à jour d’une propriété donnée sur un dossier dans une [opération UpdateFolder](updatefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="28b63-144">Represents an update to a single property on a folder in an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="28b63-145">Mise à jour (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="28b63-145">Update (FolderSync)</span></span>](update-foldersync.md) <br/> |<span data-ttu-id="28b63-146">Identifie un seul dossier pour mettre à jour dans le magasin de client local.</span><span class="sxs-lookup"><span data-stu-id="28b63-146">Identifies a single folder to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="28b63-147">Dossiers</span><span class="sxs-lookup"><span data-stu-id="28b63-147">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="28b63-148">Contient un tableau des dossiers qui sont utilisés dans les opérations de dossier.</span><span class="sxs-lookup"><span data-stu-id="28b63-148">Contains an array of folders that are used in folder operations.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="28b63-149">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="28b63-149">Text value</span></span>

<span data-ttu-id="28b63-150">Aucun.</span><span class="sxs-lookup"><span data-stu-id="28b63-150">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="28b63-151">Remarques</span><span class="sxs-lookup"><span data-stu-id="28b63-151">Remarks</span></span>

<span data-ttu-id="28b63-152">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="28b63-152">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="28b63-153">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="28b63-153">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="28b63-154">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="28b63-154">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="28b63-155">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="28b63-155">Schema Name</span></span>  <br/> |<span data-ttu-id="28b63-156">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="28b63-156">Types schema</span></span>  <br/> |
|<span data-ttu-id="28b63-157">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="28b63-157">Validation File</span></span>  <br/> |<span data-ttu-id="28b63-158">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="28b63-158">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="28b63-159">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="28b63-159">Can be Empty</span></span>  <br/> |<span data-ttu-id="28b63-160">False</span><span class="sxs-lookup"><span data-stu-id="28b63-160">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="28b63-161">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="28b63-161">See also</span></span>



- [<span data-ttu-id="28b63-162">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="28b63-162">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

