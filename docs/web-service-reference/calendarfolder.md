---
title: CalendarFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CalendarFolder
api_type:
- schema
ms.assetid: 48687a78-e757-4c04-9641-bf4302c6b565
description: L’élément CalendarFolder représente un dossier qui contient principalement des éléments de calendrier.
ms.openlocfilehash: dcd0ab9d7dea1152766997de0618b3dcceed5567
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461491"
---
# <a name="calendarfolder"></a><span data-ttu-id="06dec-103">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="06dec-103">CalendarFolder</span></span>

<span data-ttu-id="06dec-104">L’élément **CalendarFolder** représente un dossier qui contient principalement des éléments de calendrier.</span><span class="sxs-lookup"><span data-stu-id="06dec-104">The **CalendarFolder** element represents a folder that primarily contains calendar items.</span></span> 
  
```xml
<CalendarFolder>
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
</CalendarFolder>
```

 <span data-ttu-id="06dec-105">**CalendarFolderType**</span><span class="sxs-lookup"><span data-stu-id="06dec-105">**CalendarFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="06dec-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="06dec-106">Attributes and elements</span></span>

<span data-ttu-id="06dec-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="06dec-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="06dec-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="06dec-108">Attributes</span></span>

<span data-ttu-id="06dec-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="06dec-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="06dec-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="06dec-110">Child elements</span></span>

|<span data-ttu-id="06dec-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="06dec-111">**Element**</span></span>|<span data-ttu-id="06dec-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="06dec-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="06dec-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="06dec-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="06dec-114">Contient l’identificateur et la clé de modification d’un dossier.</span><span class="sxs-lookup"><span data-stu-id="06dec-114">Contains the identifier and change key of a folder.</span></span>  <br/> |
|[<span data-ttu-id="06dec-115">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="06dec-115">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="06dec-116">Représente l’identificateur du dossier parent qui contient le dossier.</span><span class="sxs-lookup"><span data-stu-id="06dec-116">Represents the identifier of the parent folder that contains the folder.</span></span>  <br/> |
|[<span data-ttu-id="06dec-117">FolderClass</span><span class="sxs-lookup"><span data-stu-id="06dec-117">FolderClass</span></span>](folderclass.md) <br/> |<span data-ttu-id="06dec-118">Représente la classe de dossier pour un dossier donné.</span><span class="sxs-lookup"><span data-stu-id="06dec-118">Represents the folder class for a given folder.</span></span>  <br/> |
|[<span data-ttu-id="06dec-119">DisplayName (chaîne)</span><span class="sxs-lookup"><span data-stu-id="06dec-119">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="06dec-120">Contient le nom complet d’un dossier.</span><span class="sxs-lookup"><span data-stu-id="06dec-120">Contains the display name of a folder.</span></span>  <br/> |
|[<span data-ttu-id="06dec-121">TotalCount</span><span class="sxs-lookup"><span data-stu-id="06dec-121">TotalCount</span></span>](totalcount.md) <br/> |<span data-ttu-id="06dec-122">Représente le nombre total d’éléments dans un dossier donné.</span><span class="sxs-lookup"><span data-stu-id="06dec-122">Represents the total count of items within a given folder.</span></span>  <br/> |
|[<span data-ttu-id="06dec-123">ChildFolderCount</span><span class="sxs-lookup"><span data-stu-id="06dec-123">ChildFolderCount</span></span>](childfoldercount.md) <br/> |<span data-ttu-id="06dec-124">Représente le nombre de dossiers enfants contenus dans un dossier.</span><span class="sxs-lookup"><span data-stu-id="06dec-124">Represents the number of child folders that are contained within a folder.</span></span> <span data-ttu-id="06dec-125">Cette propriété est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="06dec-125">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="06dec-126">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="06dec-126">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="06dec-127">Identifie les propriétés étendues des dossiers.</span><span class="sxs-lookup"><span data-stu-id="06dec-127">Identifies extended properties on folders.</span></span>  <br/> |
|[<span data-ttu-id="06dec-128">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="06dec-128">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="06dec-129">Contient des informations sur un dossier géré.</span><span class="sxs-lookup"><span data-stu-id="06dec-129">Contains information about a managed folder.</span></span>  <br/> |
|[<span data-ttu-id="06dec-130">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="06dec-130">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="06dec-p102">Contient les droits du client en fonction des paramètres d'autorisation pour l'élément ou le dossier. Cet élément est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="06dec-p102">Contains the client's rights based on the permission settings for the item or folder. This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="06dec-133">SharingEffectiveRights (CalendarPermissionReadAccessType)</span><span class="sxs-lookup"><span data-stu-id="06dec-133">SharingEffectiveRights (CalendarPermissionReadAccessType)</span></span>](sharingeffectiverights-calendarpermissionreadaccesstype.md) <br/> |<span data-ttu-id="06dec-134">Indique les autorisations dont dispose l’utilisateur pour les données de calendrier partagées.</span><span class="sxs-lookup"><span data-stu-id="06dec-134">Indicates the permissions that the user has for the calendar data that is being shared.</span></span>  <br/> |
|[<span data-ttu-id="06dec-135">PermissionSet (CalendarPermissionSetType)</span><span class="sxs-lookup"><span data-stu-id="06dec-135">PermissionSet (CalendarPermissionSetType)</span></span>](permissionset-calendarpermissionsettype.md) <br/> |<span data-ttu-id="06dec-136">Contient toutes les autorisations configurées pour un dossier de calendrier.</span><span class="sxs-lookup"><span data-stu-id="06dec-136">Contains all the configured permissions for a calendar folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="06dec-137">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="06dec-137">Parent elements</span></span>

|<span data-ttu-id="06dec-138">**Élément**</span><span class="sxs-lookup"><span data-stu-id="06dec-138">**Element**</span></span>|<span data-ttu-id="06dec-139">**Description**</span><span class="sxs-lookup"><span data-stu-id="06dec-139">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="06dec-140">AppendToFolderField</span><span class="sxs-lookup"><span data-stu-id="06dec-140">AppendToFolderField</span></span>](appendtofolderfield.md) <br/> |<span data-ttu-id="06dec-141">Spécifie les données à ajouter à une propriété de dossier lors d’une [opération UpdateFolder](updatefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="06dec-141">Specifies data to append to a folder property during an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="06dec-142">Créer (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="06dec-142">Create (FolderSync)</span></span>](create-foldersync.md) <br/> |<span data-ttu-id="06dec-143">Identifie un dossier unique à créer dans le magasin de client local.</span><span class="sxs-lookup"><span data-stu-id="06dec-143">Identifies a single folder to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="06dec-144">SetFolderField</span><span class="sxs-lookup"><span data-stu-id="06dec-144">SetFolderField</span></span>](setfolderfield.md) <br/> |<span data-ttu-id="06dec-145">Représente une mise à jour d’une propriété unique sur un dossier dans une [opération UpdateFolder](updatefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="06dec-145">Represents an update to a single property on a folder in an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="06dec-146">Mise à jour (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="06dec-146">Update (FolderSync)</span></span>](update-foldersync.md) <br/> |<span data-ttu-id="06dec-147">Identifie un dossier unique à mettre à jour dans le magasin client local.</span><span class="sxs-lookup"><span data-stu-id="06dec-147">Identifies a single folder to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="06dec-148">Dossiers</span><span class="sxs-lookup"><span data-stu-id="06dec-148">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="06dec-149">Contient un tableau de dossiers utilisés dans les opérations de dossier.</span><span class="sxs-lookup"><span data-stu-id="06dec-149">Contains an array of folders that are used in folder operations.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="06dec-150">Remarques</span><span class="sxs-lookup"><span data-stu-id="06dec-150">Remarks</span></span>

<span data-ttu-id="06dec-151">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="06dec-151">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="06dec-152">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="06dec-152">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="06dec-153">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="06dec-153">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="06dec-154">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="06dec-154">Schema Name</span></span>  <br/> |<span data-ttu-id="06dec-155">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="06dec-155">Types schema</span></span>  <br/> |
|<span data-ttu-id="06dec-156">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="06dec-156">Validation File</span></span>  <br/> |<span data-ttu-id="06dec-157">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="06dec-157">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="06dec-158">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="06dec-158">Can be Empty</span></span>  <br/> |<span data-ttu-id="06dec-159">False</span><span class="sxs-lookup"><span data-stu-id="06dec-159">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="06dec-160">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="06dec-160">See also</span></span>



- [<span data-ttu-id="06dec-161">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="06dec-161">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

