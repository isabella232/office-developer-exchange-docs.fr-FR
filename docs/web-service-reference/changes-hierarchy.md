---
title: Modifications (hiérarchie)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Changes
api_type:
- schema
ms.assetid: 918a0d1f-90a5-4eef-9592-07e15bef94e6
description: L’élément de modifications contient un tableau de types de modification qui représente le type des différences entre les dossiers sur le client et les dossiers sur l’ordinateur qui exécute Microsoft Exchange Server 2007 séquencé.
ms.openlocfilehash: 15e4f9f37c5e4a4083260dcf379a49beb2260030
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755507"
---
# <a name="changes-hierarchy"></a><span data-ttu-id="06bea-103">Modifications (hiérarchie)</span><span class="sxs-lookup"><span data-stu-id="06bea-103">Changes (Hierarchy)</span></span>

<span data-ttu-id="06bea-104">L’élément de **modifications** contient un tableau de types de modification qui représente le type des différences entre les dossiers sur le client et les dossiers sur l’ordinateur qui exécute Microsoft Exchange Server 2007 séquencé.</span><span class="sxs-lookup"><span data-stu-id="06bea-104">The **Changes** element contains a sequenced array of change types that represent the type of differences between the folders on the client and the folders on the computer that is running Microsoft Exchange Server 2007.</span></span> 
  
[<span data-ttu-id="06bea-105">SyncFolderHierarchyResponse</span><span class="sxs-lookup"><span data-stu-id="06bea-105">SyncFolderHierarchyResponse</span></span>](syncfolderhierarchyresponse.md)
  
[<span data-ttu-id="06bea-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="06bea-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="06bea-107">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="06bea-107">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md)
  
[<span data-ttu-id="06bea-108">Modifications (hiérarchie)</span><span class="sxs-lookup"><span data-stu-id="06bea-108">Changes (Hierarchy)</span></span>](changes-hierarchy.md)
  
```xml
<Changes>
   <Create/>
   <Update/>
   <Delete/>
</Changes>
```

 <span data-ttu-id="06bea-109">**SyncFolderHierarchyChangesType**</span><span class="sxs-lookup"><span data-stu-id="06bea-109">**SyncFolderHierarchyChangesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="06bea-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="06bea-110">Attributes and elements</span></span>

<span data-ttu-id="06bea-111">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="06bea-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="06bea-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="06bea-112">Attributes</span></span>

<span data-ttu-id="06bea-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="06bea-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="06bea-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="06bea-114">Child elements</span></span>

|<span data-ttu-id="06bea-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="06bea-115">**Element**</span></span>|<span data-ttu-id="06bea-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="06bea-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="06bea-117">Créer (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="06bea-117">Create (FolderSync)</span></span>](create-foldersync.md) <br/> |<span data-ttu-id="06bea-118">Identifie un dossier unique à créer dans le magasin de client local.</span><span class="sxs-lookup"><span data-stu-id="06bea-118">Identifies a single folder to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="06bea-119">Mise à jour (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="06bea-119">Update (FolderSync)</span></span>](update-foldersync.md) <br/> |<span data-ttu-id="06bea-120">Identifie un seul dossier pour mettre à jour dans le magasin de client local.</span><span class="sxs-lookup"><span data-stu-id="06bea-120">Identifies a single folder to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="06bea-121">Supprimer (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="06bea-121">Delete (FolderSync)</span></span>](delete-foldersync.md) <br/> |<span data-ttu-id="06bea-122">Identifie un seul dossier à supprimer dans le magasin de client local.</span><span class="sxs-lookup"><span data-stu-id="06bea-122">Identifies a single folder to delete in the local client store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="06bea-123">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="06bea-123">Parent elements</span></span>

|<span data-ttu-id="06bea-124">**Élément**</span><span class="sxs-lookup"><span data-stu-id="06bea-124">**Element**</span></span>|<span data-ttu-id="06bea-125">**Description**</span><span class="sxs-lookup"><span data-stu-id="06bea-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="06bea-126">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="06bea-126">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md) <br/> |<span data-ttu-id="06bea-127">Contient l’état et les résultats d’une demande SyncFolderHierarchy.</span><span class="sxs-lookup"><span data-stu-id="06bea-127">Contains the status and result of a SyncFolderHierarchy request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="06bea-128">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="06bea-128">Text value</span></span>

<span data-ttu-id="06bea-129">Une valeur de texte qui représente une valeur Boolean est requise.</span><span class="sxs-lookup"><span data-stu-id="06bea-129">A text value that represents a Boolean value is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="06bea-130">Remarques</span><span class="sxs-lookup"><span data-stu-id="06bea-130">Remarks</span></span>

<span data-ttu-id="06bea-131">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur Exchange 2007 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="06bea-131">The schema that describes this element is located in the EWS virtual directory of the Exchange 2007 computer that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="06bea-132">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="06bea-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="06bea-133">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="06bea-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="06bea-134">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="06bea-134">Schema name</span></span>  <br/> |<span data-ttu-id="06bea-135">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="06bea-135">Messages schema</span></span>  <br/> |
|<span data-ttu-id="06bea-136">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="06bea-136">Validation file</span></span>  <br/> |<span data-ttu-id="06bea-137">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="06bea-137">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="06bea-138">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="06bea-138">Can be empty</span></span>  <br/> |<span data-ttu-id="06bea-139">False</span><span class="sxs-lookup"><span data-stu-id="06bea-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="06bea-140">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="06bea-140">See also</span></span>



[<span data-ttu-id="06bea-141">Opération SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="06bea-141">SyncFolderHierarchy operation</span></span>](syncfolderhierarchy-operation.md)


[<span data-ttu-id="06bea-142">Référence EWS pour Exchange</span><span class="sxs-lookup"><span data-stu-id="06bea-142">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)
  
- [<span data-ttu-id="06bea-143">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="06bea-143">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

