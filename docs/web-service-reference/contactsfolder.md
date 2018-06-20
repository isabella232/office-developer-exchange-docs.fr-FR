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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755565"
---
# <a name="contactsfolder"></a><span data-ttu-id="20172-103">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="20172-103">ContactsFolder</span></span>

<span data-ttu-id="20172-104">L’élément **ContactsFolder** représente un dossier de contacts qui se trouve dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="20172-104">The **ContactsFolder** element represents a contacts folder that is contained in a mailbox.</span></span> 
  
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

 <span data-ttu-id="20172-105">**ContactsFolderType**</span><span class="sxs-lookup"><span data-stu-id="20172-105">**ContactsFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="20172-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="20172-106">Attributes and elements</span></span>

<span data-ttu-id="20172-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="20172-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="20172-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="20172-108">Attributes</span></span>

<span data-ttu-id="20172-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="20172-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="20172-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="20172-110">Child elements</span></span>

|<span data-ttu-id="20172-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="20172-111">**Element**</span></span>|<span data-ttu-id="20172-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="20172-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="20172-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="20172-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="20172-114">Contient la clé d’identificateur et de modification d’un dossier contacts.</span><span class="sxs-lookup"><span data-stu-id="20172-114">Contains the identifier and change key of a contacts folder.</span></span>  <br/> |
|[<span data-ttu-id="20172-115">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="20172-115">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="20172-116">Représente l’identificateur du dossier parent qui contient le dossier contacts.</span><span class="sxs-lookup"><span data-stu-id="20172-116">Represents the identifier of the parent folder that contains the contacts folder.</span></span>  <br/> |
|[<span data-ttu-id="20172-117">Classe FolderClass</span><span class="sxs-lookup"><span data-stu-id="20172-117">FolderClass</span></span>](folderclass.md) <br/> |<span data-ttu-id="20172-118">Représente la classe de dossier pour un dossier contacts.</span><span class="sxs-lookup"><span data-stu-id="20172-118">Represents the folder class for a contacts folder.</span></span>  <br/> |
|[<span data-ttu-id="20172-119">DisplayName (chaîne)</span><span class="sxs-lookup"><span data-stu-id="20172-119">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="20172-120">Contient le nom complet d’un dossier contacts.</span><span class="sxs-lookup"><span data-stu-id="20172-120">Contains the display name of a contacts folder.</span></span>  <br/> |
|[<span data-ttu-id="20172-121">TotalCount</span><span class="sxs-lookup"><span data-stu-id="20172-121">TotalCount</span></span>](totalcount.md) <br/> |<span data-ttu-id="20172-122">Représente le nombre total d’éléments dans un dossier contacts.</span><span class="sxs-lookup"><span data-stu-id="20172-122">Represents the total count of items within a contacts folder.</span></span>  <br/> |
|[<span data-ttu-id="20172-123">ChildFolderCount</span><span class="sxs-lookup"><span data-stu-id="20172-123">ChildFolderCount</span></span>](childfoldercount.md) <br/> |<span data-ttu-id="20172-124">Représente le nombre de dossiers enfants qui sont contenues dans un dossier contacts.</span><span class="sxs-lookup"><span data-stu-id="20172-124">Represents the number of child folders that are contained within a contacts folder.</span></span> <span data-ttu-id="20172-125">Cette propriété est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="20172-125">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="20172-126">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="20172-126">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="20172-127">Identifie les propriétés étendues dans les dossiers de contacts.</span><span class="sxs-lookup"><span data-stu-id="20172-127">Identifies extended properties on contacts folders.</span></span>  <br/> |
|[<span data-ttu-id="20172-128">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="20172-128">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="20172-129">Contient des informations sur un dossier géré.</span><span class="sxs-lookup"><span data-stu-id="20172-129">Contains information about a managed folder.</span></span>  <br/> |
|[<span data-ttu-id="20172-130">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="20172-130">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="20172-131">Contient les droits du client en fonction des paramètres d'autorisation pour l'élément ou le dossier.</span><span class="sxs-lookup"><span data-stu-id="20172-131">Contains the client's rights based on the permission settings for the item or folder.</span></span>  <br/> |
|[<span data-ttu-id="20172-132">SharingEffectiveRights (PermissionReadAccessType)</span><span class="sxs-lookup"><span data-stu-id="20172-132">SharingEffectiveRights (PermissionReadAccessType)</span></span>](sharingeffectiverights-permissionreadaccesstype.md) <br/> |<span data-ttu-id="20172-133">Indique les autorisations dont dispose l’utilisateur pour les données de contact qui sont partagées.</span><span class="sxs-lookup"><span data-stu-id="20172-133">Indicates the permissions that the user has for the contact data that is being shared.</span></span>  <br/> |
|[<span data-ttu-id="20172-134">PermissionSet (PermissionSetType)</span><span class="sxs-lookup"><span data-stu-id="20172-134">PermissionSet (PermissionSetType)</span></span>](permissionset-permissionsettype.md) <br/> |<span data-ttu-id="20172-135">Contient toutes les autorisations configurées pour un dossier.</span><span class="sxs-lookup"><span data-stu-id="20172-135">Contains all the configured permissions for a folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="20172-136">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="20172-136">Parent elements</span></span>

|<span data-ttu-id="20172-137">**Élément**</span><span class="sxs-lookup"><span data-stu-id="20172-137">**Element**</span></span>|<span data-ttu-id="20172-138">**Description**</span><span class="sxs-lookup"><span data-stu-id="20172-138">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="20172-139">AppendToFolderField</span><span class="sxs-lookup"><span data-stu-id="20172-139">AppendToFolderField</span></span>](appendtofolderfield.md) <br/> |<span data-ttu-id="20172-140">Spécifie les données à ajouter à une propriété de dossier lors d’une [opération UpdateFolder](updatefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="20172-140">Specifies data to append to a folder property during an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="20172-141">Créer (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="20172-141">Create (FolderSync)</span></span>](create-foldersync.md) <br/> |<span data-ttu-id="20172-142">Identifie un dossier unique à créer dans le magasin de client local.</span><span class="sxs-lookup"><span data-stu-id="20172-142">Identifies a single folder to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="20172-143">SetFolderField</span><span class="sxs-lookup"><span data-stu-id="20172-143">SetFolderField</span></span>](setfolderfield.md) <br/> |<span data-ttu-id="20172-144">Représente une mise à jour d’une propriété donnée sur un dossier dans une [opération UpdateFolder](updatefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="20172-144">Represents an update to a single property on a folder in an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="20172-145">Mise à jour (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="20172-145">Update (FolderSync)</span></span>](update-foldersync.md) <br/> |<span data-ttu-id="20172-146">Identifie un seul dossier pour mettre à jour dans le magasin de client local.</span><span class="sxs-lookup"><span data-stu-id="20172-146">Identifies a single folder to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="20172-147">Dossiers</span><span class="sxs-lookup"><span data-stu-id="20172-147">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="20172-148">Contient un tableau des dossiers qui sont utilisés dans les opérations de dossier.</span><span class="sxs-lookup"><span data-stu-id="20172-148">Contains an array of folders that are used in folder operations.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="20172-149">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="20172-149">Text value</span></span>

<span data-ttu-id="20172-150">Aucun.</span><span class="sxs-lookup"><span data-stu-id="20172-150">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="20172-151">Remarques</span><span class="sxs-lookup"><span data-stu-id="20172-151">Remarks</span></span>

<span data-ttu-id="20172-152">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="20172-152">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="20172-153">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="20172-153">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="20172-154">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="20172-154">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="20172-155">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="20172-155">Schema Name</span></span>  <br/> |<span data-ttu-id="20172-156">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="20172-156">Types schema</span></span>  <br/> |
|<span data-ttu-id="20172-157">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="20172-157">Validation File</span></span>  <br/> |<span data-ttu-id="20172-158">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="20172-158">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="20172-159">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="20172-159">Can be Empty</span></span>  <br/> |<span data-ttu-id="20172-160">False</span><span class="sxs-lookup"><span data-stu-id="20172-160">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="20172-161">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="20172-161">See also</span></span>



- [<span data-ttu-id="20172-162">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="20172-162">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

