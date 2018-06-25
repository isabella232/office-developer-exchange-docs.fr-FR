---
title: Dossiers
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Folders
api_type:
- schema
ms.assetid: 8e71cb44-1df6-444a-add7-0c1363863f65
description: L’élément dossiers contient un tableau des dossiers qui sont utilisés dans les opérations de dossier.
ms.openlocfilehash: e1b9e337f633dbf6fda159c28725d3fb8dcd55a6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756454"
---
# <a name="folders"></a><span data-ttu-id="dadc6-103">Dossiers</span><span class="sxs-lookup"><span data-stu-id="dadc6-103">Folders</span></span>

<span data-ttu-id="dadc6-104">L’élément **dossiers** contient un tableau des dossiers qui sont utilisés dans les opérations de dossier.</span><span class="sxs-lookup"><span data-stu-id="dadc6-104">The **Folders** element contains an array of folders that are used in folder operations.</span></span> 
  
```xml
<Folders>
   <Folder/>
</Folders>
```

 <span data-ttu-id="dadc6-105">**ArrayOfFoldersType** ou **NonEmptyArrayOfFoldersType**</span><span class="sxs-lookup"><span data-stu-id="dadc6-105">**ArrayOfFoldersType** or **NonEmptyArrayOfFoldersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dadc6-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="dadc6-106">Attributes and elements</span></span>

<span data-ttu-id="dadc6-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="dadc6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dadc6-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="dadc6-108">Attributes</span></span>

<span data-ttu-id="dadc6-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="dadc6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dadc6-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="dadc6-110">Child elements</span></span>

|<span data-ttu-id="dadc6-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="dadc6-111">**Element**</span></span>|<span data-ttu-id="dadc6-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="dadc6-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dadc6-113">Folder</span><span class="sxs-lookup"><span data-stu-id="dadc6-113">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="dadc6-114">Identifie un dossier pour créer, obtenir, recherchez, synchroniser ou mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="dadc6-114">Identifies a folder to create, get, find, synchronize, or update.</span></span>  <br/> |
|[<span data-ttu-id="dadc6-115">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="dadc6-115">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="dadc6-116">Représente un dossier contenant principalement des éléments de calendrier.</span><span class="sxs-lookup"><span data-stu-id="dadc6-116">Represents a folder that primarily contains calendar items.</span></span>  <br/> |
|[<span data-ttu-id="dadc6-117">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="dadc6-117">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="dadc6-118">Représente un dossier Contacts dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="dadc6-118">Represents a Contacts folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="dadc6-119">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="dadc6-119">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="dadc6-120">Représente un dossier de recherche contenu dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="dadc6-120">Represents a Search folder contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="dadc6-121">Dossier tâches</span><span class="sxs-lookup"><span data-stu-id="dadc6-121">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="dadc6-122">Représente un dossier de tâches dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="dadc6-122">Represents a Tasks folder in a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="dadc6-123">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="dadc6-123">Parent elements</span></span>

|<span data-ttu-id="dadc6-124">**Élément**</span><span class="sxs-lookup"><span data-stu-id="dadc6-124">**Element**</span></span>|<span data-ttu-id="dadc6-125">**Description**</span><span class="sxs-lookup"><span data-stu-id="dadc6-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dadc6-126">CopyFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="dadc6-126">CopyFolderResponseMessage</span></span>](copyfolderresponsemessage.md) <br/> |<span data-ttu-id="dadc6-127">Contient l’état et les résultats d’une seule demande [d’opération CopyFolder](copyfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="dadc6-127">Contains the status and result of a single [CopyFolder operation](copyfolder-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="dadc6-128">CreateFolder</span><span class="sxs-lookup"><span data-stu-id="dadc6-128">CreateFolder</span></span>](createfolder.md) <br/> |<span data-ttu-id="dadc6-129">Définit une demande pour créer un dossier dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="dadc6-129">Defines a request to create a folder in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="dadc6-130">CreateFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="dadc6-130">CreateFolderResponseMessage</span></span>](createfolderresponsemessage.md) <br/> |<span data-ttu-id="dadc6-131">Contient l’état et les résultats d’une seule demande [d’opération CreateFolder](createfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="dadc6-131">Contains the status and result of a single [CreateFolder operation](createfolder-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="dadc6-132">CreateManagedFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="dadc6-132">CreateManagedFolderResponseMessage</span></span>](createmanagedfolderresponsemessage.md) <br/> |<span data-ttu-id="dadc6-133">Contient l’état et les résultats d’une seule demande [d’opération CreateManagedFolder](createmanagedfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="dadc6-133">Contains the status and result of a single [CreateManagedFolder operation](createmanagedfolder-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="dadc6-134">GetFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="dadc6-134">GetFolderResponseMessage</span></span>](getfolderresponsemessage.md) <br/> |<span data-ttu-id="dadc6-135">Contient l’état et les résultats d’une demande [d’opération GetFolder](getfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="dadc6-135">Contains the status and result of a [GetFolder operation](getfolder-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="dadc6-136">MoveFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="dadc6-136">MoveFolderResponseMessage</span></span>](movefolderresponsemessage.md) <br/> |<span data-ttu-id="dadc6-137">Contient l’état et les résultats d’une demande [d’opération MoveFolder](movefolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="dadc6-137">Contains the status and result of a [MoveFolder operation](movefolder-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="dadc6-138">ParentFolderId (TargetFolderIdType)</span><span class="sxs-lookup"><span data-stu-id="dadc6-138">ParentFolderId (TargetFolderIdType)</span></span>](parentfolderid-targetfolderidtype.md) <br/> |<span data-ttu-id="dadc6-139">Identifie le dossier dans lequel un nouveau dossier est créé.</span><span class="sxs-lookup"><span data-stu-id="dadc6-139">Identifies the folder where a new folder is created.</span></span>  <br/> |
|[<span data-ttu-id="dadc6-140">RootFolder (FindFolderResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="dadc6-140">RootFolder (FindFolderResponseMessage)</span></span>](rootfolder-findfolderresponsemessage.md) <br/> |<span data-ttu-id="dadc6-141">Contient les résultats de recherche dans un dossier racine unique lors d’une [opération FindFolder](findfolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="dadc6-141">Contains the results from searching a single root folder during a [FindFolder operation](findfolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="dadc6-142">UpdateFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="dadc6-142">UpdateFolderResponseMessage</span></span>](updatefolderresponsemessage.md) <br/> |<span data-ttu-id="dadc6-143">Contient l’état et les résultats d’une seule demande [d’opération UpdateFolder](updatefolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="dadc6-143">Contains the status and result of a single [UpdateFolder operation](updatefolder-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="dadc6-144">Remarques</span><span class="sxs-lookup"><span data-stu-id="dadc6-144">Remarks</span></span>

<span data-ttu-id="dadc6-145">Cet élément est un élément enfant requis de l’élément [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) .</span><span class="sxs-lookup"><span data-stu-id="dadc6-145">This element is a required child element of the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span> 
  
<span data-ttu-id="dadc6-146">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="dadc6-146">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dadc6-147">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="dadc6-147">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dadc6-148">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="dadc6-148">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="dadc6-149">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="dadc6-149">Schema Name</span></span>  <br/> |<span data-ttu-id="dadc6-150">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="dadc6-150">Types schema</span></span>  <br/> |
|<span data-ttu-id="dadc6-151">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="dadc6-151">Validation File</span></span>  <br/> |<span data-ttu-id="dadc6-152">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="dadc6-152">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="dadc6-153">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="dadc6-153">Can be Empty</span></span>  <br/> |<span data-ttu-id="dadc6-154">False</span><span class="sxs-lookup"><span data-stu-id="dadc6-154">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dadc6-155">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="dadc6-155">See also</span></span>



[<span data-ttu-id="dadc6-156">ParentFolderId (TargetFolderIdType)</span><span class="sxs-lookup"><span data-stu-id="dadc6-156">ParentFolderId (TargetFolderIdType)</span></span>](parentfolderid-targetfolderidtype.md)

