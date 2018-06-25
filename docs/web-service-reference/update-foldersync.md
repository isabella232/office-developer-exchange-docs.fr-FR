---
title: Mise à jour (FolderSync)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Update
api_type:
- schema
ms.assetid: 47ed8edb-2a94-471b-b965-93f91456252e
description: L’élément de mise à jour identifie un seul dossier pour mettre à jour dans le magasin de client local.
ms.openlocfilehash: 6d4a6233df41ea95e1fd9b394502bfb2728bddb6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838849"
---
# <a name="update-foldersync"></a><span data-ttu-id="6b0c8-103">Mise à jour (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="6b0c8-103">Update (FolderSync)</span></span>

<span data-ttu-id="6b0c8-104">L’élément de **mise à jour** identifie un seul dossier pour mettre à jour dans le magasin de client local.</span><span class="sxs-lookup"><span data-stu-id="6b0c8-104">The **Update** element identifies a single folder to update in the local client store.</span></span> 
  
[<span data-ttu-id="6b0c8-105">SyncFolderHierarchyResponse</span><span class="sxs-lookup"><span data-stu-id="6b0c8-105">SyncFolderHierarchyResponse</span></span>](syncfolderhierarchyresponse.md)
  
[<span data-ttu-id="6b0c8-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="6b0c8-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="6b0c8-107">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="6b0c8-107">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md)
  
[<span data-ttu-id="6b0c8-108">Modifications (hiérarchie)</span><span class="sxs-lookup"><span data-stu-id="6b0c8-108">Changes (Hierarchy)</span></span>](changes-hierarchy.md)
  
[<span data-ttu-id="6b0c8-109">Mise à jour (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="6b0c8-109">Update (FolderSync)</span></span>](update-foldersync.md)
  
```xml
<Update>
   <Folder/>
</Update>
```

 <span data-ttu-id="6b0c8-110">**SyncFolderHierarchyCreateOrUpdateType**</span><span class="sxs-lookup"><span data-stu-id="6b0c8-110">**SyncFolderHierarchyCreateOrUpdateType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6b0c8-111">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="6b0c8-111">Attributes and elements</span></span>

<span data-ttu-id="6b0c8-112">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="6b0c8-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6b0c8-113">Attributs</span><span class="sxs-lookup"><span data-stu-id="6b0c8-113">Attributes</span></span>

<span data-ttu-id="6b0c8-114">Aucun.</span><span class="sxs-lookup"><span data-stu-id="6b0c8-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6b0c8-115">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="6b0c8-115">Child elements</span></span>

|<span data-ttu-id="6b0c8-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="6b0c8-116">**Element**</span></span>|<span data-ttu-id="6b0c8-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="6b0c8-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6b0c8-118">Folder</span><span class="sxs-lookup"><span data-stu-id="6b0c8-118">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="6b0c8-119">Définit le dossier pour créer, obtenir, recherchez, synchroniser ou mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="6b0c8-119">Defines the folder to create, get, find, synchronize, or update.</span></span>  <br/> |
|[<span data-ttu-id="6b0c8-120">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="6b0c8-120">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="6b0c8-121">Représente un dossier contenant principalement des éléments de calendrier.</span><span class="sxs-lookup"><span data-stu-id="6b0c8-121">Represents a folder that primarily contains calendar items.</span></span>  <br/> |
|[<span data-ttu-id="6b0c8-122">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="6b0c8-122">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="6b0c8-123">Représente un dossier de contacts dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="6b0c8-123">Represents a contact folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="6b0c8-124">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="6b0c8-124">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="6b0c8-125">Représente un dossier de recherche qui se trouve dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="6b0c8-125">Represents a search folder that is contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="6b0c8-126">Dossier tâches</span><span class="sxs-lookup"><span data-stu-id="6b0c8-126">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="6b0c8-127">Représente une tâche du dossier t est thcontained dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="6b0c8-127">Represents a task folder t is thcontained in a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6b0c8-128">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="6b0c8-128">Parent elements</span></span>

|<span data-ttu-id="6b0c8-129">**Élément**</span><span class="sxs-lookup"><span data-stu-id="6b0c8-129">**Element**</span></span>|<span data-ttu-id="6b0c8-130">**Description**</span><span class="sxs-lookup"><span data-stu-id="6b0c8-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6b0c8-131">Modifications (hiérarchie)</span><span class="sxs-lookup"><span data-stu-id="6b0c8-131">Changes (Hierarchy)</span></span>](changes-hierarchy.md) <br/> |<span data-ttu-id="6b0c8-132">Contient un tableau séquencé de types de modification qui représente le type des différences entre les dossiers sur le client et les dossiers sur le serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="6b0c8-132">Contains a sequenced array of change types that represent the type of differences between the folders on the client and the folders on the Exchange server.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6b0c8-133">Remarques</span><span class="sxs-lookup"><span data-stu-id="6b0c8-133">Remarks</span></span>

<span data-ttu-id="6b0c8-134">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="6b0c8-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6b0c8-135">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="6b0c8-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6b0c8-136">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="6b0c8-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6b0c8-137">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="6b0c8-137">Schema name</span></span>  <br/> |<span data-ttu-id="6b0c8-138">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="6b0c8-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="6b0c8-139">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="6b0c8-139">Validation file</span></span>  <br/> |<span data-ttu-id="6b0c8-140">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6b0c8-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6b0c8-141">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="6b0c8-141">Can be empty</span></span>  <br/> |<span data-ttu-id="6b0c8-142">False</span><span class="sxs-lookup"><span data-stu-id="6b0c8-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6b0c8-143">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="6b0c8-143">See also</span></span>



[<span data-ttu-id="6b0c8-144">Opération SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="6b0c8-144">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="6b0c8-145">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="6b0c8-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

