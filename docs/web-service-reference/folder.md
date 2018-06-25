---
title: Folder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Folder
api_type:
- schema
ms.assetid: 812948d8-c7db-45ce-bb3a-77233a53a974
description: L’élément de dossier définit un dossier pour créer, obtenir, recherchez, synchroniser ou mettre à jour.
ms.openlocfilehash: ecfea52d2105599372a22b78778ac0d0d066bc60
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756448"
---
# <a name="folder"></a><span data-ttu-id="73f88-103">Folder</span><span class="sxs-lookup"><span data-stu-id="73f88-103">Folder</span></span>

<span data-ttu-id="73f88-104">L’élément de **dossier** définit un dossier pour créer, obtenir, recherchez, synchroniser ou mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="73f88-104">The **Folder** element defines a folder to create, get, find, synchronize, or update.</span></span> 
  
```xml
<Folder>
   <FolderId/>
   <ParentFolderId/>
   <FolderClass/>
   <DisplayName/>
   <TotalCount/>
   <ChildFolderCount/>
   <ExtendedProperty/>
   <ManagedFolderInformation/>
   <UnreadCount/>
   <PermissionSet/>
      <EffectiveRights/>
</Folder>
```

 <span data-ttu-id="73f88-105">**FolderType**</span><span class="sxs-lookup"><span data-stu-id="73f88-105">**FolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="73f88-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="73f88-106">Attributes and elements</span></span>

<span data-ttu-id="73f88-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="73f88-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="73f88-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="73f88-108">Attributes</span></span>

<span data-ttu-id="73f88-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="73f88-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="73f88-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="73f88-110">Child elements</span></span>

|<span data-ttu-id="73f88-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="73f88-111">**Element**</span></span>|<span data-ttu-id="73f88-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="73f88-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="73f88-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="73f88-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="73f88-114">Contient la clé d’identificateur et de modification d’un dossier.</span><span class="sxs-lookup"><span data-stu-id="73f88-114">Contains the identifier and change key of a folder.</span></span>  <br/> |
|[<span data-ttu-id="73f88-115">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="73f88-115">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="73f88-116">Représente l’identificateur du dossier qui contient le dossier parent.</span><span class="sxs-lookup"><span data-stu-id="73f88-116">Represents the identifier of the parent folder that contains the folder.</span></span>  <br/> |
|[<span data-ttu-id="73f88-117">Classe FolderClass</span><span class="sxs-lookup"><span data-stu-id="73f88-117">FolderClass</span></span>](folderclass.md) <br/> |<span data-ttu-id="73f88-118">Représente la classe de dossier pour un dossier donné.</span><span class="sxs-lookup"><span data-stu-id="73f88-118">Represents the folder class for a given folder.</span></span>  <br/> |
|[<span data-ttu-id="73f88-119">DisplayName (chaîne)</span><span class="sxs-lookup"><span data-stu-id="73f88-119">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="73f88-120">Contient le nom complet d’un dossier.</span><span class="sxs-lookup"><span data-stu-id="73f88-120">Contains the display name of a folder.</span></span>  <br/> |
|[<span data-ttu-id="73f88-121">TotalCount</span><span class="sxs-lookup"><span data-stu-id="73f88-121">TotalCount</span></span>](totalcount.md) <br/> |<span data-ttu-id="73f88-122">Représente le nombre total d’éléments dans un dossier donné.</span><span class="sxs-lookup"><span data-stu-id="73f88-122">Represents the total count of items within a given folder.</span></span>  <br/> |
|[<span data-ttu-id="73f88-123">ChildFolderCount</span><span class="sxs-lookup"><span data-stu-id="73f88-123">ChildFolderCount</span></span>](childfoldercount.md) <br/> |<span data-ttu-id="73f88-124">Représente le nombre de dossiers enfants qui sont contenues dans un dossier.</span><span class="sxs-lookup"><span data-stu-id="73f88-124">Represents the number of child folders that are contained within a folder.</span></span> <span data-ttu-id="73f88-125">Cette propriété est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="73f88-125">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="73f88-126">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="73f88-126">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="73f88-127">Identifie les propriétés étendues dans les dossiers.</span><span class="sxs-lookup"><span data-stu-id="73f88-127">Identifies extended properties on folders.</span></span>  <br/> |
|[<span data-ttu-id="73f88-128">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="73f88-128">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="73f88-129">Contient des informations sur un dossier géré.</span><span class="sxs-lookup"><span data-stu-id="73f88-129">Contains information about a managed folder.</span></span>  <br/> |
|[<span data-ttu-id="73f88-130">UnreadCount</span><span class="sxs-lookup"><span data-stu-id="73f88-130">UnreadCount</span></span>](unreadcount.md) <br/> |<span data-ttu-id="73f88-131">Représente le nombre d’éléments non lus dans un dossier donné.</span><span class="sxs-lookup"><span data-stu-id="73f88-131">Represents the count of unread items within a given folder.</span></span>  <br/> |
|[<span data-ttu-id="73f88-132">PermissionSet (PermissionSetType)</span><span class="sxs-lookup"><span data-stu-id="73f88-132">PermissionSet (PermissionSetType)</span></span>](permissionset-permissionsettype.md) <br/> |<span data-ttu-id="73f88-133">Contient toutes les autorisations configurées pour un dossier.</span><span class="sxs-lookup"><span data-stu-id="73f88-133">Contains all the configured permissions for a folder.</span></span> <span data-ttu-id="73f88-134">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="73f88-134">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="73f88-135">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="73f88-135">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="73f88-136">Contient les droits du client en fonction des paramètres d'autorisation pour l'élément ou le dossier.</span><span class="sxs-lookup"><span data-stu-id="73f88-136">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="73f88-137">Cet élément est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="73f88-137">This element is read-only.</span></span> <span data-ttu-id="73f88-138">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="73f88-138">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="73f88-139">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="73f88-139">Parent elements</span></span>

|<span data-ttu-id="73f88-140">**Élément**</span><span class="sxs-lookup"><span data-stu-id="73f88-140">**Element**</span></span>|<span data-ttu-id="73f88-141">**Description**</span><span class="sxs-lookup"><span data-stu-id="73f88-141">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="73f88-142">AppendToFolderField</span><span class="sxs-lookup"><span data-stu-id="73f88-142">AppendToFolderField</span></span>](appendtofolderfield.md) <br/> |<span data-ttu-id="73f88-143">Spécifie les données à ajouter à une propriété de dossier lors d’une [opération UpdateFolder](updatefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="73f88-143">Specifies data to append to a folder property during an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="73f88-144">Créer (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="73f88-144">Create (FolderSync)</span></span>](create-foldersync.md) <br/> |<span data-ttu-id="73f88-145">Identifie un dossier unique à créer dans le magasin de client local.</span><span class="sxs-lookup"><span data-stu-id="73f88-145">Identifies a single folder to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="73f88-146">SetFolderField</span><span class="sxs-lookup"><span data-stu-id="73f88-146">SetFolderField</span></span>](setfolderfield.md) <br/> |<span data-ttu-id="73f88-147">Représente une mise à jour d’une propriété donnée sur un dossier dans une [opération UpdateFolder](updatefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="73f88-147">Represents an update to a single property on a folder in an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="73f88-148">Mise à jour (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="73f88-148">Update (FolderSync)</span></span>](update-foldersync.md) <br/> |<span data-ttu-id="73f88-149">Identifie un seul dossier pour mettre à jour dans le magasin de client local.</span><span class="sxs-lookup"><span data-stu-id="73f88-149">Identifies a single folder to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="73f88-150">Dossiers</span><span class="sxs-lookup"><span data-stu-id="73f88-150">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="73f88-151">Contient un tableau des dossiers qui sont utilisés dans les opérations de dossier.</span><span class="sxs-lookup"><span data-stu-id="73f88-151">Contains an array of folders that are used in folder operations.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="73f88-152">Remarques</span><span class="sxs-lookup"><span data-stu-id="73f88-152">Remarks</span></span>

<span data-ttu-id="73f88-153">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Exchange 2007 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="73f88-153">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="73f88-154">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="73f88-154">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="73f88-155">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="73f88-155">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="73f88-156">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="73f88-156">Schema Name</span></span>  <br/> |<span data-ttu-id="73f88-157">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="73f88-157">Types schema</span></span>  <br/> |
|<span data-ttu-id="73f88-158">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="73f88-158">Validation File</span></span>  <br/> |<span data-ttu-id="73f88-159">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="73f88-159">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="73f88-160">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="73f88-160">Can be Empty</span></span>  <br/> |<span data-ttu-id="73f88-161">False</span><span class="sxs-lookup"><span data-stu-id="73f88-161">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="73f88-162">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="73f88-162">See also</span></span>



[<span data-ttu-id="73f88-163">Opération SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="73f88-163">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="73f88-164">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="73f88-164">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

