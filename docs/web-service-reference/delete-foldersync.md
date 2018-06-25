---
title: Supprimer (FolderSync)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Delete
api_type:
- schema
ms.assetid: c4397d91-43ef-40a9-a80e-d31501a33caa
description: L’élément Supprimer identifie un seul dossier à supprimer dans le magasin de client local.
ms.openlocfilehash: 5cad36c6fcff782195fdb285e2d3c4f3c5ec0f1e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755841"
---
# <a name="delete-foldersync"></a><span data-ttu-id="00a72-103">Supprimer (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="00a72-103">Delete (FolderSync)</span></span>

<span data-ttu-id="00a72-104">L’élément **Supprimer** identifie un seul dossier à supprimer dans le magasin de client local.</span><span class="sxs-lookup"><span data-stu-id="00a72-104">The **Delete** element identifies a single folder to delete in the local client store.</span></span> 
  
- [<span data-ttu-id="00a72-105">SyncFolderHierarchyResponse</span><span class="sxs-lookup"><span data-stu-id="00a72-105">SyncFolderHierarchyResponse</span></span>](syncfolderhierarchyresponse.md)  
- [<span data-ttu-id="00a72-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="00a72-106">ResponseMessages</span></span>](responsemessages.md)  
- [<span data-ttu-id="00a72-107">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="00a72-107">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md)  
- [<span data-ttu-id="00a72-108">Modifications (hiérarchie)</span><span class="sxs-lookup"><span data-stu-id="00a72-108">Changes (Hierarchy)</span></span>](changes-hierarchy.md)  
- [<span data-ttu-id="00a72-109">Supprimer (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="00a72-109">Delete (FolderSync)</span></span>](delete-foldersync.md)
  
```xml
<Delete>
   <FolderId/>
</Delete>
```

<span data-ttu-id="00a72-110">**SyncFolderHierarchyDeleteType**</span><span class="sxs-lookup"><span data-stu-id="00a72-110">**SyncFolderHierarchyDeleteType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="00a72-111">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="00a72-111">Attributes and elements</span></span>

<span data-ttu-id="00a72-112">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="00a72-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="00a72-113">Attributs</span><span class="sxs-lookup"><span data-stu-id="00a72-113">Attributes</span></span>

<span data-ttu-id="00a72-114">Aucun.</span><span class="sxs-lookup"><span data-stu-id="00a72-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="00a72-115">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="00a72-115">Child elements</span></span>

|<span data-ttu-id="00a72-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="00a72-116">**Element**</span></span>|<span data-ttu-id="00a72-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="00a72-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="00a72-118">FolderId</span><span class="sxs-lookup"><span data-stu-id="00a72-118">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="00a72-119">Contient la clé d’identificateur et de modification d’un dossier.</span><span class="sxs-lookup"><span data-stu-id="00a72-119">Contains the identifier and change key of a folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="00a72-120">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="00a72-120">Parent elements</span></span>

|<span data-ttu-id="00a72-121">**Élément**</span><span class="sxs-lookup"><span data-stu-id="00a72-121">**Element**</span></span>|<span data-ttu-id="00a72-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="00a72-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="00a72-123">Modifications (hiérarchie)</span><span class="sxs-lookup"><span data-stu-id="00a72-123">Changes (Hierarchy)</span></span>](changes-hierarchy.md) <br/> |<span data-ttu-id="00a72-124">Contient un tableau de types de modification qui représente le type des différences entre les dossiers sur le client et les dossiers sur l’ordinateur qui exécute Microsoft Exchange Server 2007 séquencé.</span><span class="sxs-lookup"><span data-stu-id="00a72-124">Contains a sequenced array of change types that represent the type of differences between the folders on the client and the folders on the computer that is running Microsoft Exchange Server 2007.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="00a72-125">Remarques</span><span class="sxs-lookup"><span data-stu-id="00a72-125">Remarks</span></span>

<span data-ttu-id="00a72-126">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur Exchange 2007 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="00a72-126">The schema that describes this element is located in the EWS virtual directory of the Exchange 2007 computer that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="00a72-127">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="00a72-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="00a72-128">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="00a72-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="00a72-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="00a72-129">Schema name</span></span>  <br/> |<span data-ttu-id="00a72-130">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="00a72-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="00a72-131">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="00a72-131">Validation file</span></span>  <br/> |<span data-ttu-id="00a72-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="00a72-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="00a72-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="00a72-133">Can be empty</span></span>  <br/> |<span data-ttu-id="00a72-134">False</span><span class="sxs-lookup"><span data-stu-id="00a72-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="00a72-135">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="00a72-135">See also</span></span>

- [<span data-ttu-id="00a72-136">Opération SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="00a72-136">SyncFolderHierarchy operation</span></span>](syncfolderhierarchy-operation.md)
- [<span data-ttu-id="00a72-137">Référence EWS pour Exchange</span><span class="sxs-lookup"><span data-stu-id="00a72-137">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)
- [<span data-ttu-id="00a72-138">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="00a72-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

