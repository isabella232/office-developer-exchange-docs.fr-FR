---
title: Changes (hiérarchie)
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
description: L’élément changes contient un tableau séquencé de types de modifications qui représentent le type de différences entre les dossiers sur le client et les dossiers sur l’ordinateur qui exécute Microsoft Exchange Server 2007.
ms.openlocfilehash: a296d87f23e85d42b4c8c858e92eddfb586a8324
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463271"
---
# <a name="changes-hierarchy"></a><span data-ttu-id="74521-103">Changes (hiérarchie)</span><span class="sxs-lookup"><span data-stu-id="74521-103">Changes (Hierarchy)</span></span>

<span data-ttu-id="74521-104">L’élément **changes** contient un tableau séquencé de types de modifications qui représentent le type de différences entre les dossiers sur le client et les dossiers sur l’ordinateur qui exécute Microsoft Exchange Server 2007.</span><span class="sxs-lookup"><span data-stu-id="74521-104">The **Changes** element contains a sequenced array of change types that represent the type of differences between the folders on the client and the folders on the computer that is running Microsoft Exchange Server 2007.</span></span> 
  
[<span data-ttu-id="74521-105">SyncFolderHierarchyResponse</span><span class="sxs-lookup"><span data-stu-id="74521-105">SyncFolderHierarchyResponse</span></span>](syncfolderhierarchyresponse.md)
  
[<span data-ttu-id="74521-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="74521-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="74521-107">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="74521-107">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md)
  
[<span data-ttu-id="74521-108">Changes (hiérarchie)</span><span class="sxs-lookup"><span data-stu-id="74521-108">Changes (Hierarchy)</span></span>](changes-hierarchy.md)
  
```xml
<Changes>
   <Create/>
   <Update/>
   <Delete/>
</Changes>
```

 <span data-ttu-id="74521-109">**SyncFolderHierarchyChangesType**</span><span class="sxs-lookup"><span data-stu-id="74521-109">**SyncFolderHierarchyChangesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="74521-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="74521-110">Attributes and elements</span></span>

<span data-ttu-id="74521-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="74521-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="74521-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="74521-112">Attributes</span></span>

<span data-ttu-id="74521-113">Aucune.</span><span class="sxs-lookup"><span data-stu-id="74521-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="74521-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="74521-114">Child elements</span></span>

|<span data-ttu-id="74521-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="74521-115">**Element**</span></span>|<span data-ttu-id="74521-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="74521-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="74521-117">Créer (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="74521-117">Create (FolderSync)</span></span>](create-foldersync.md) <br/> |<span data-ttu-id="74521-118">Identifie un dossier unique à créer dans le magasin de client local.</span><span class="sxs-lookup"><span data-stu-id="74521-118">Identifies a single folder to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="74521-119">Mise à jour (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="74521-119">Update (FolderSync)</span></span>](update-foldersync.md) <br/> |<span data-ttu-id="74521-120">Identifie un dossier unique à mettre à jour dans le magasin client local.</span><span class="sxs-lookup"><span data-stu-id="74521-120">Identifies a single folder to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="74521-121">Supprimer (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="74521-121">Delete (FolderSync)</span></span>](delete-foldersync.md) <br/> |<span data-ttu-id="74521-122">Identifie un dossier unique à supprimer dans le magasin client local.</span><span class="sxs-lookup"><span data-stu-id="74521-122">Identifies a single folder to delete in the local client store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="74521-123">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="74521-123">Parent elements</span></span>

|<span data-ttu-id="74521-124">**Élément**</span><span class="sxs-lookup"><span data-stu-id="74521-124">**Element**</span></span>|<span data-ttu-id="74521-125">**Description**</span><span class="sxs-lookup"><span data-stu-id="74521-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="74521-126">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="74521-126">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md) <br/> |<span data-ttu-id="74521-127">Contient l’État et le résultat d’une demande Opérationsyncfolderhierarchy.</span><span class="sxs-lookup"><span data-stu-id="74521-127">Contains the status and result of a SyncFolderHierarchy request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="74521-128">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="74521-128">Text value</span></span>

<span data-ttu-id="74521-129">Une valeur de texte qui représente une valeur Boolean est requise.</span><span class="sxs-lookup"><span data-stu-id="74521-129">A text value that represents a Boolean value is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="74521-130">Remarques</span><span class="sxs-lookup"><span data-stu-id="74521-130">Remarks</span></span>

<span data-ttu-id="74521-131">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur Exchange 2007 sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="74521-131">The schema that describes this element is located in the EWS virtual directory of the Exchange 2007 computer that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="74521-132">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="74521-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="74521-133">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="74521-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="74521-134">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="74521-134">Schema name</span></span>  <br/> |<span data-ttu-id="74521-135">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="74521-135">Messages schema</span></span>  <br/> |
|<span data-ttu-id="74521-136">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="74521-136">Validation file</span></span>  <br/> |<span data-ttu-id="74521-137">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="74521-137">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="74521-138">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="74521-138">Can be empty</span></span>  <br/> |<span data-ttu-id="74521-139">False</span><span class="sxs-lookup"><span data-stu-id="74521-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="74521-140">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="74521-140">See also</span></span>



[<span data-ttu-id="74521-141">Opération Opérationsyncfolderhierarchy</span><span class="sxs-lookup"><span data-stu-id="74521-141">SyncFolderHierarchy operation</span></span>](syncfolderhierarchy-operation.md)


[<span data-ttu-id="74521-142">Référence EWS pour Exchange</span><span class="sxs-lookup"><span data-stu-id="74521-142">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)
  
- [<span data-ttu-id="74521-143">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="74521-143">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

