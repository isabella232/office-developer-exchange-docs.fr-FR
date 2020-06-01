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
description: L’élément delete identifie un dossier unique à supprimer dans le magasin client local.
ms.openlocfilehash: 68f8687b8cf0723d7fd63a3d55da8ef7c2f98f8e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44454980"
---
# <a name="delete-foldersync"></a><span data-ttu-id="d22b8-103">Supprimer (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="d22b8-103">Delete (FolderSync)</span></span>

<span data-ttu-id="d22b8-104">L’élément **Delete** identifie un dossier unique à supprimer dans le magasin client local.</span><span class="sxs-lookup"><span data-stu-id="d22b8-104">The **Delete** element identifies a single folder to delete in the local client store.</span></span> 
  
- [<span data-ttu-id="d22b8-105">SyncFolderHierarchyResponse</span><span class="sxs-lookup"><span data-stu-id="d22b8-105">SyncFolderHierarchyResponse</span></span>](syncfolderhierarchyresponse.md)  
- [<span data-ttu-id="d22b8-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="d22b8-106">ResponseMessages</span></span>](responsemessages.md)  
- [<span data-ttu-id="d22b8-107">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d22b8-107">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md)  
- [<span data-ttu-id="d22b8-108">Changes (hiérarchie)</span><span class="sxs-lookup"><span data-stu-id="d22b8-108">Changes (Hierarchy)</span></span>](changes-hierarchy.md)  
- [<span data-ttu-id="d22b8-109">Supprimer (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="d22b8-109">Delete (FolderSync)</span></span>](delete-foldersync.md)
  
```xml
<Delete>
   <FolderId/>
</Delete>
```

<span data-ttu-id="d22b8-110">**SyncFolderHierarchyDeleteType**</span><span class="sxs-lookup"><span data-stu-id="d22b8-110">**SyncFolderHierarchyDeleteType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="d22b8-111">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d22b8-111">Attributes and elements</span></span>

<span data-ttu-id="d22b8-112">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d22b8-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d22b8-113">Attributs</span><span class="sxs-lookup"><span data-stu-id="d22b8-113">Attributes</span></span>

<span data-ttu-id="d22b8-114">Aucune.</span><span class="sxs-lookup"><span data-stu-id="d22b8-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d22b8-115">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d22b8-115">Child elements</span></span>

|<span data-ttu-id="d22b8-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d22b8-116">**Element**</span></span>|<span data-ttu-id="d22b8-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="d22b8-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d22b8-118">FolderId</span><span class="sxs-lookup"><span data-stu-id="d22b8-118">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="d22b8-119">Contient l’identificateur et la clé de modification d’un dossier.</span><span class="sxs-lookup"><span data-stu-id="d22b8-119">Contains the identifier and change key of a folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d22b8-120">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d22b8-120">Parent elements</span></span>

|<span data-ttu-id="d22b8-121">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d22b8-121">**Element**</span></span>|<span data-ttu-id="d22b8-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="d22b8-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d22b8-123">Changes (hiérarchie)</span><span class="sxs-lookup"><span data-stu-id="d22b8-123">Changes (Hierarchy)</span></span>](changes-hierarchy.md) <br/> |<span data-ttu-id="d22b8-124">Contient un tableau séquencé de types de modifications qui représentent le type de différences entre les dossiers sur le client et les dossiers sur l’ordinateur qui exécute Microsoft Exchange Server 2007.</span><span class="sxs-lookup"><span data-stu-id="d22b8-124">Contains a sequenced array of change types that represent the type of differences between the folders on the client and the folders on the computer that is running Microsoft Exchange Server 2007.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d22b8-125">Remarques</span><span class="sxs-lookup"><span data-stu-id="d22b8-125">Remarks</span></span>

<span data-ttu-id="d22b8-126">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur Exchange 2007 sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="d22b8-126">The schema that describes this element is located in the EWS virtual directory of the Exchange 2007 computer that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d22b8-127">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d22b8-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d22b8-128">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d22b8-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d22b8-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d22b8-129">Schema name</span></span>  <br/> |<span data-ttu-id="d22b8-130">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="d22b8-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="d22b8-131">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d22b8-131">Validation file</span></span>  <br/> |<span data-ttu-id="d22b8-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d22b8-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d22b8-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d22b8-133">Can be empty</span></span>  <br/> |<span data-ttu-id="d22b8-134">False</span><span class="sxs-lookup"><span data-stu-id="d22b8-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d22b8-135">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d22b8-135">See also</span></span>

- [<span data-ttu-id="d22b8-136">Opération Opérationsyncfolderhierarchy</span><span class="sxs-lookup"><span data-stu-id="d22b8-136">SyncFolderHierarchy operation</span></span>](syncfolderhierarchy-operation.md)
- [<span data-ttu-id="d22b8-137">Référence EWS pour Exchange</span><span class="sxs-lookup"><span data-stu-id="d22b8-137">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)
- [<span data-ttu-id="d22b8-138">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="d22b8-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

