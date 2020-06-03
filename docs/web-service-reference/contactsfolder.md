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
description: L’élément ContactsFolder représente un dossier de contacts contenu dans une boîte aux lettres.
ms.openlocfilehash: 997b4f603198e6d05a011c4ef6bac7fe4dfbfe52
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529433"
---
# <a name="contactsfolder"></a><span data-ttu-id="ae8f6-103">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="ae8f6-103">ContactsFolder</span></span>

<span data-ttu-id="ae8f6-104">L’élément **ContactsFolder** représente un dossier de contacts contenu dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="ae8f6-104">The **ContactsFolder** element represents a contacts folder that is contained in a mailbox.</span></span> 
  
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

 <span data-ttu-id="ae8f6-105">**ContactsFolderType**</span><span class="sxs-lookup"><span data-stu-id="ae8f6-105">**ContactsFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ae8f6-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ae8f6-106">Attributes and elements</span></span>

<span data-ttu-id="ae8f6-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ae8f6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ae8f6-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="ae8f6-108">Attributes</span></span>

<span data-ttu-id="ae8f6-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="ae8f6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ae8f6-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ae8f6-110">Child elements</span></span>

|<span data-ttu-id="ae8f6-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ae8f6-111">**Element**</span></span>|<span data-ttu-id="ae8f6-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="ae8f6-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ae8f6-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="ae8f6-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="ae8f6-114">Contient l’identificateur et la clé de modification d’un dossier de contacts.</span><span class="sxs-lookup"><span data-stu-id="ae8f6-114">Contains the identifier and change key of a contacts folder.</span></span>  <br/> |
|[<span data-ttu-id="ae8f6-115">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="ae8f6-115">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="ae8f6-116">Représente l’identificateur du dossier parent qui contient le dossier contacts.</span><span class="sxs-lookup"><span data-stu-id="ae8f6-116">Represents the identifier of the parent folder that contains the contacts folder.</span></span>  <br/> |
|[<span data-ttu-id="ae8f6-117">FolderClass</span><span class="sxs-lookup"><span data-stu-id="ae8f6-117">FolderClass</span></span>](folderclass.md) <br/> |<span data-ttu-id="ae8f6-118">Représente la classe Folder d’un dossier contacts.</span><span class="sxs-lookup"><span data-stu-id="ae8f6-118">Represents the folder class for a contacts folder.</span></span>  <br/> |
|[<span data-ttu-id="ae8f6-119">DisplayName (chaîne)</span><span class="sxs-lookup"><span data-stu-id="ae8f6-119">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="ae8f6-120">Contient le nom complet d’un dossier de contacts.</span><span class="sxs-lookup"><span data-stu-id="ae8f6-120">Contains the display name of a contacts folder.</span></span>  <br/> |
|[<span data-ttu-id="ae8f6-121">TotalCount</span><span class="sxs-lookup"><span data-stu-id="ae8f6-121">TotalCount</span></span>](totalcount.md) <br/> |<span data-ttu-id="ae8f6-122">Représente le nombre total d’éléments au sein d’un dossier de contacts.</span><span class="sxs-lookup"><span data-stu-id="ae8f6-122">Represents the total count of items within a contacts folder.</span></span>  <br/> |
|[<span data-ttu-id="ae8f6-123">ChildFolderCount</span><span class="sxs-lookup"><span data-stu-id="ae8f6-123">ChildFolderCount</span></span>](childfoldercount.md) <br/> |<span data-ttu-id="ae8f6-124">Représente le nombre de dossiers enfants contenus dans un dossier contacts.</span><span class="sxs-lookup"><span data-stu-id="ae8f6-124">Represents the number of child folders that are contained within a contacts folder.</span></span> <span data-ttu-id="ae8f6-125">Cette propriété est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="ae8f6-125">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="ae8f6-126">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="ae8f6-126">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="ae8f6-127">Identifie les propriétés étendues dans les dossiers de contacts.</span><span class="sxs-lookup"><span data-stu-id="ae8f6-127">Identifies extended properties on contacts folders.</span></span>  <br/> |
|[<span data-ttu-id="ae8f6-128">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="ae8f6-128">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="ae8f6-129">Contient des informations sur un dossier géré.</span><span class="sxs-lookup"><span data-stu-id="ae8f6-129">Contains information about a managed folder.</span></span>  <br/> |
|[<span data-ttu-id="ae8f6-130">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="ae8f6-130">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="ae8f6-131">Contient les droits du client en fonction des paramètres d'autorisation pour l'élément ou le dossier.</span><span class="sxs-lookup"><span data-stu-id="ae8f6-131">Contains the client's rights based on the permission settings for the item or folder.</span></span>  <br/> |
|[<span data-ttu-id="ae8f6-132">SharingEffectiveRights (PermissionReadAccessType)</span><span class="sxs-lookup"><span data-stu-id="ae8f6-132">SharingEffectiveRights (PermissionReadAccessType)</span></span>](sharingeffectiverights-permissionreadaccesstype.md) <br/> |<span data-ttu-id="ae8f6-133">Indique les autorisations dont dispose l’utilisateur pour les données de contact partagées.</span><span class="sxs-lookup"><span data-stu-id="ae8f6-133">Indicates the permissions that the user has for the contact data that is being shared.</span></span>  <br/> |
|[<span data-ttu-id="ae8f6-134">PermissionSet (PermissionSetType)</span><span class="sxs-lookup"><span data-stu-id="ae8f6-134">PermissionSet (PermissionSetType)</span></span>](permissionset-permissionsettype.md) <br/> |<span data-ttu-id="ae8f6-135">Contient toutes les autorisations configurées pour un dossier.</span><span class="sxs-lookup"><span data-stu-id="ae8f6-135">Contains all the configured permissions for a folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ae8f6-136">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ae8f6-136">Parent elements</span></span>

|<span data-ttu-id="ae8f6-137">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ae8f6-137">**Element**</span></span>|<span data-ttu-id="ae8f6-138">**Description**</span><span class="sxs-lookup"><span data-stu-id="ae8f6-138">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ae8f6-139">AppendToFolderField</span><span class="sxs-lookup"><span data-stu-id="ae8f6-139">AppendToFolderField</span></span>](appendtofolderfield.md) <br/> |<span data-ttu-id="ae8f6-140">Spécifie les données à ajouter à une propriété de dossier lors d’une [opération UpdateFolder](updatefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="ae8f6-140">Specifies data to append to a folder property during an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="ae8f6-141">Créer (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="ae8f6-141">Create (FolderSync)</span></span>](create-foldersync.md) <br/> |<span data-ttu-id="ae8f6-142">Identifie un dossier unique à créer dans le magasin de client local.</span><span class="sxs-lookup"><span data-stu-id="ae8f6-142">Identifies a single folder to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="ae8f6-143">SetFolderField</span><span class="sxs-lookup"><span data-stu-id="ae8f6-143">SetFolderField</span></span>](setfolderfield.md) <br/> |<span data-ttu-id="ae8f6-144">Représente une mise à jour d’une propriété unique sur un dossier dans une [opération UpdateFolder](updatefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="ae8f6-144">Represents an update to a single property on a folder in an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="ae8f6-145">Mise à jour (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="ae8f6-145">Update (FolderSync)</span></span>](update-foldersync.md) <br/> |<span data-ttu-id="ae8f6-146">Identifie un dossier unique à mettre à jour dans le magasin client local.</span><span class="sxs-lookup"><span data-stu-id="ae8f6-146">Identifies a single folder to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="ae8f6-147">Dossiers</span><span class="sxs-lookup"><span data-stu-id="ae8f6-147">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="ae8f6-148">Contient un tableau de dossiers utilisés dans les opérations de dossier.</span><span class="sxs-lookup"><span data-stu-id="ae8f6-148">Contains an array of folders that are used in folder operations.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ae8f6-149">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="ae8f6-149">Text value</span></span>

<span data-ttu-id="ae8f6-150">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ae8f6-150">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ae8f6-151">Remarques</span><span class="sxs-lookup"><span data-stu-id="ae8f6-151">Remarks</span></span>

<span data-ttu-id="ae8f6-152">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="ae8f6-152">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ae8f6-153">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ae8f6-153">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ae8f6-154">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ae8f6-154">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ae8f6-155">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ae8f6-155">Schema Name</span></span>  <br/> |<span data-ttu-id="ae8f6-156">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="ae8f6-156">Types schema</span></span>  <br/> |
|<span data-ttu-id="ae8f6-157">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ae8f6-157">Validation File</span></span>  <br/> |<span data-ttu-id="ae8f6-158">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ae8f6-158">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ae8f6-159">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ae8f6-159">Can be Empty</span></span>  <br/> |<span data-ttu-id="ae8f6-160">False</span><span class="sxs-lookup"><span data-stu-id="ae8f6-160">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ae8f6-161">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ae8f6-161">See also</span></span>



- [<span data-ttu-id="ae8f6-162">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ae8f6-162">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

