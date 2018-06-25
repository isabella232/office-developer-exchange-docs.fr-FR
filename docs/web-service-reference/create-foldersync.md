---
title: Créer (FolderSync)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Create
api_type:
- schema
ms.assetid: 6b463d0a-70e9-40c5-ade4-c7d9a5f36bc1
description: L’élément créer identifie un seul dossier à créer dans le magasin du client local.
ms.openlocfilehash: 867eecb89c115b008d4828e162b21d078eba695c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755676"
---
# <a name="create-foldersync"></a><span data-ttu-id="c765c-103">Créer (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="c765c-103">Create (FolderSync)</span></span>

<span data-ttu-id="c765c-104">L’élément **créer** identifie un seul dossier à créer dans le magasin du client local.</span><span class="sxs-lookup"><span data-stu-id="c765c-104">The **Create** element identifies a single folder to create in the local client store.</span></span> 
  
[<span data-ttu-id="c765c-105">SyncFolderHierarchyResponse</span><span class="sxs-lookup"><span data-stu-id="c765c-105">SyncFolderHierarchyResponse</span></span>](syncfolderhierarchyresponse.md)
  
[<span data-ttu-id="c765c-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="c765c-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="c765c-107">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="c765c-107">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md)
  
[<span data-ttu-id="c765c-108">Modifications (hiérarchie)</span><span class="sxs-lookup"><span data-stu-id="c765c-108">Changes (Hierarchy)</span></span>](changes-hierarchy.md)
  
[<span data-ttu-id="c765c-109">Créer (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="c765c-109">Create (FolderSync)</span></span>](create-foldersync.md)
  
```xml
<Create>
   <Folder/>
   <CalendarFolder/>
   <ContactsFolder/>
   <SearchFolder/>
   <TasksFolder/>
</Create>
```

 <span data-ttu-id="c765c-110">**SyncFolderHierarchyCreateOrUpdateType**</span><span class="sxs-lookup"><span data-stu-id="c765c-110">**SyncFolderHierarchyCreateOrUpdateType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c765c-111">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="c765c-111">Attributes and elements</span></span>

<span data-ttu-id="c765c-112">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="c765c-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c765c-113">Attributs</span><span class="sxs-lookup"><span data-stu-id="c765c-113">Attributes</span></span>

<span data-ttu-id="c765c-114">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c765c-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c765c-115">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="c765c-115">Child elements</span></span>

|<span data-ttu-id="c765c-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c765c-116">**Element**</span></span>|<span data-ttu-id="c765c-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="c765c-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c765c-118">Folder</span><span class="sxs-lookup"><span data-stu-id="c765c-118">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="c765c-119">Définit le dossier pour créer, obtenir, recherchez, synchroniser ou mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="c765c-119">Defines the folder to create, get, find, synchronize, or update.</span></span>  <br/> |
|[<span data-ttu-id="c765c-120">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="c765c-120">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="c765c-121">Représente un dossier contenant principalement des éléments de calendrier.</span><span class="sxs-lookup"><span data-stu-id="c765c-121">Represents a folder that primarily contains calendar items.</span></span>  <br/> |
|[<span data-ttu-id="c765c-122">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="c765c-122">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="c765c-123">Représente un dossier de contacts dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="c765c-123">Represents a contact folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="c765c-124">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="c765c-124">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="c765c-125">Représente un dossier de recherche contenu dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="c765c-125">Represents a search folder contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="c765c-126">Dossier tâches</span><span class="sxs-lookup"><span data-stu-id="c765c-126">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="c765c-127">Représente un dossier de tâches contenu dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="c765c-127">Represents a task folder contained in a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c765c-128">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="c765c-128">Parent elements</span></span>

|<span data-ttu-id="c765c-129">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c765c-129">**Element**</span></span>|<span data-ttu-id="c765c-130">**Description**</span><span class="sxs-lookup"><span data-stu-id="c765c-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c765c-131">Modifications (hiérarchie)</span><span class="sxs-lookup"><span data-stu-id="c765c-131">Changes (Hierarchy)</span></span>](changes-hierarchy.md) <br/> |<span data-ttu-id="c765c-132">Contient un tableau de séquence de types de modification qui représente le type des différences entre les éléments sur le client et les éléments sur le serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="c765c-132">Contains a sequence array of change types that represent the type of differences between the items on the client and the items on the Exchange server.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c765c-133">Remarques</span><span class="sxs-lookup"><span data-stu-id="c765c-133">Remarks</span></span>

<span data-ttu-id="c765c-134">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="c765c-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c765c-135">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="c765c-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c765c-136">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="c765c-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c765c-137">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="c765c-137">Schema name</span></span>  <br/> |<span data-ttu-id="c765c-138">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="c765c-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="c765c-139">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="c765c-139">Validation file</span></span>  <br/> |<span data-ttu-id="c765c-140">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c765c-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c765c-141">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="c765c-141">Can be empty</span></span>  <br/> |<span data-ttu-id="c765c-142">False</span><span class="sxs-lookup"><span data-stu-id="c765c-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c765c-143">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c765c-143">See also</span></span>



[<span data-ttu-id="c765c-144">Opération SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="c765c-144">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="c765c-145">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="c765c-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

