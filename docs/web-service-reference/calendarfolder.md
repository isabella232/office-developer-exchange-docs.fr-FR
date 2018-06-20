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
description: L’élément CalendarFolder représente un dossier contenant principalement des éléments de calendrier.
ms.openlocfilehash: 7dc90706eb45eb4617a68b9fdcf37669921af966
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755467"
---
# <a name="calendarfolder"></a><span data-ttu-id="9e067-103">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="9e067-103">CalendarFolder</span></span>

<span data-ttu-id="9e067-104">L’élément **CalendarFolder** représente un dossier contenant principalement des éléments de calendrier.</span><span class="sxs-lookup"><span data-stu-id="9e067-104">The **CalendarFolder** element represents a folder that primarily contains calendar items.</span></span> 
  
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

 <span data-ttu-id="9e067-105">**CalendarFolderType**</span><span class="sxs-lookup"><span data-stu-id="9e067-105">**CalendarFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9e067-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="9e067-106">Attributes and elements</span></span>

<span data-ttu-id="9e067-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="9e067-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9e067-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="9e067-108">Attributes</span></span>

<span data-ttu-id="9e067-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="9e067-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9e067-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="9e067-110">Child elements</span></span>

|<span data-ttu-id="9e067-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9e067-111">**Element**</span></span>|<span data-ttu-id="9e067-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="9e067-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9e067-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="9e067-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="9e067-114">Contient la clé d’identificateur et de modification d’un dossier.</span><span class="sxs-lookup"><span data-stu-id="9e067-114">Contains the identifier and change key of a folder.</span></span>  <br/> |
|[<span data-ttu-id="9e067-115">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="9e067-115">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="9e067-116">Représente l’identificateur du dossier qui contient le dossier parent.</span><span class="sxs-lookup"><span data-stu-id="9e067-116">Represents the identifier of the parent folder that contains the folder.</span></span>  <br/> |
|[<span data-ttu-id="9e067-117">Classe FolderClass</span><span class="sxs-lookup"><span data-stu-id="9e067-117">FolderClass</span></span>](folderclass.md) <br/> |<span data-ttu-id="9e067-118">Représente la classe de dossier pour un dossier donné.</span><span class="sxs-lookup"><span data-stu-id="9e067-118">Represents the folder class for a given folder.</span></span>  <br/> |
|[<span data-ttu-id="9e067-119">DisplayName (chaîne)</span><span class="sxs-lookup"><span data-stu-id="9e067-119">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="9e067-120">Contient le nom complet d’un dossier.</span><span class="sxs-lookup"><span data-stu-id="9e067-120">Contains the display name of a folder.</span></span>  <br/> |
|[<span data-ttu-id="9e067-121">TotalCount</span><span class="sxs-lookup"><span data-stu-id="9e067-121">TotalCount</span></span>](totalcount.md) <br/> |<span data-ttu-id="9e067-122">Représente le nombre total d’éléments dans un dossier donné.</span><span class="sxs-lookup"><span data-stu-id="9e067-122">Represents the total count of items within a given folder.</span></span>  <br/> |
|[<span data-ttu-id="9e067-123">ChildFolderCount</span><span class="sxs-lookup"><span data-stu-id="9e067-123">ChildFolderCount</span></span>](childfoldercount.md) <br/> |<span data-ttu-id="9e067-124">Représente le nombre de dossiers enfants qui sont contenues dans un dossier.</span><span class="sxs-lookup"><span data-stu-id="9e067-124">Represents the number of child folders that are contained within a folder.</span></span> <span data-ttu-id="9e067-125">Cette propriété est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="9e067-125">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="9e067-126">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="9e067-126">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="9e067-127">Identifie les propriétés étendues dans les dossiers.</span><span class="sxs-lookup"><span data-stu-id="9e067-127">Identifies extended properties on folders.</span></span>  <br/> |
|[<span data-ttu-id="9e067-128">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="9e067-128">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="9e067-129">Contient des informations sur un dossier géré.</span><span class="sxs-lookup"><span data-stu-id="9e067-129">Contains information about a managed folder.</span></span>  <br/> |
|[<span data-ttu-id="9e067-130">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="9e067-130">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="9e067-p102">Contient les droits du client en fonction des paramètres d'autorisation pour l'élément ou le dossier. Cet élément est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="9e067-p102">Contains the client's rights based on the permission settings for the item or folder. This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="9e067-133">SharingEffectiveRights (CalendarPermissionReadAccessType)</span><span class="sxs-lookup"><span data-stu-id="9e067-133">SharingEffectiveRights (CalendarPermissionReadAccessType)</span></span>](sharingeffectiverights-calendarpermissionreadaccesstype.md) <br/> |<span data-ttu-id="9e067-134">Indique les autorisations dont dispose l’utilisateur pour les données de calendrier qui sont partagées.</span><span class="sxs-lookup"><span data-stu-id="9e067-134">Indicates the permissions that the user has for the calendar data that is being shared.</span></span>  <br/> |
|[<span data-ttu-id="9e067-135">PermissionSet (CalendarPermissionSetType)</span><span class="sxs-lookup"><span data-stu-id="9e067-135">PermissionSet (CalendarPermissionSetType)</span></span>](permissionset-calendarpermissionsettype.md) <br/> |<span data-ttu-id="9e067-136">Contient toutes les autorisations configurées pour un dossier de calendrier.</span><span class="sxs-lookup"><span data-stu-id="9e067-136">Contains all the configured permissions for a calendar folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9e067-137">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="9e067-137">Parent elements</span></span>

|<span data-ttu-id="9e067-138">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9e067-138">**Element**</span></span>|<span data-ttu-id="9e067-139">**Description**</span><span class="sxs-lookup"><span data-stu-id="9e067-139">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9e067-140">AppendToFolderField</span><span class="sxs-lookup"><span data-stu-id="9e067-140">AppendToFolderField</span></span>](appendtofolderfield.md) <br/> |<span data-ttu-id="9e067-141">Spécifie les données à ajouter à une propriété de dossier lors d’une [opération UpdateFolder](updatefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="9e067-141">Specifies data to append to a folder property during an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="9e067-142">Créer (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="9e067-142">Create (FolderSync)</span></span>](create-foldersync.md) <br/> |<span data-ttu-id="9e067-143">Identifie un dossier unique à créer dans le magasin de client local.</span><span class="sxs-lookup"><span data-stu-id="9e067-143">Identifies a single folder to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="9e067-144">SetFolderField</span><span class="sxs-lookup"><span data-stu-id="9e067-144">SetFolderField</span></span>](setfolderfield.md) <br/> |<span data-ttu-id="9e067-145">Représente une mise à jour d’une propriété donnée sur un dossier dans une [opération UpdateFolder](updatefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="9e067-145">Represents an update to a single property on a folder in an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="9e067-146">Mise à jour (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="9e067-146">Update (FolderSync)</span></span>](update-foldersync.md) <br/> |<span data-ttu-id="9e067-147">Identifie un seul dossier pour mettre à jour dans le magasin de client local.</span><span class="sxs-lookup"><span data-stu-id="9e067-147">Identifies a single folder to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="9e067-148">Dossiers</span><span class="sxs-lookup"><span data-stu-id="9e067-148">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="9e067-149">Contient un tableau des dossiers qui sont utilisés dans les opérations de dossier.</span><span class="sxs-lookup"><span data-stu-id="9e067-149">Contains an array of folders that are used in folder operations.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9e067-150">Remarques</span><span class="sxs-lookup"><span data-stu-id="9e067-150">Remarks</span></span>

<span data-ttu-id="9e067-151">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="9e067-151">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9e067-152">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="9e067-152">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9e067-153">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="9e067-153">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9e067-154">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="9e067-154">Schema Name</span></span>  <br/> |<span data-ttu-id="9e067-155">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="9e067-155">Types schema</span></span>  <br/> |
|<span data-ttu-id="9e067-156">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="9e067-156">Validation File</span></span>  <br/> |<span data-ttu-id="9e067-157">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9e067-157">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9e067-158">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="9e067-158">Can be Empty</span></span>  <br/> |<span data-ttu-id="9e067-159">False</span><span class="sxs-lookup"><span data-stu-id="9e067-159">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9e067-160">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="9e067-160">See also</span></span>



- [<span data-ttu-id="9e067-161">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="9e067-161">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

