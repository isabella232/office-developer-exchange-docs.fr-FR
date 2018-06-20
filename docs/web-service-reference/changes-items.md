---
title: Modifications (éléments)
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
ms.assetid: d3139fef-0455-4b89-babd-5d6783b50a58
description: L’élément de modifications contient un tableau de séquence de types de modification qui représentent les types de différences entre les éléments sur le client et les éléments sur le serveur Exchange.
ms.openlocfilehash: 8e38597276e3e3051a5c1494619d3220280e401f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755503"
---
# <a name="changes-items"></a><span data-ttu-id="04a02-103">Modifications (éléments)</span><span class="sxs-lookup"><span data-stu-id="04a02-103">Changes (Items)</span></span>

<span data-ttu-id="04a02-104">L’élément de **modifications** contient un tableau de séquence de types de modification qui représentent les types de différences entre les éléments sur le client et les éléments sur le serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="04a02-104">The **Changes** element contains a sequence array of change types that represent the types of differences between the items on the client and the items on the Exchange server.</span></span> 
  
[<span data-ttu-id="04a02-105">SyncFolderItemsResponse</span><span class="sxs-lookup"><span data-stu-id="04a02-105">SyncFolderItemsResponse</span></span>](syncfolderitemsresponse.md)
  
[<span data-ttu-id="04a02-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="04a02-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="04a02-107">SyncFolderItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="04a02-107">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md)
  
[<span data-ttu-id="04a02-108">Modifications (éléments)</span><span class="sxs-lookup"><span data-stu-id="04a02-108">Changes (Items)</span></span>](changes-items.md)
  
```xml
<Changes>
   <Create/>
   <Update/>
   <Delete/>
</Changes>
```

 <span data-ttu-id="04a02-109">**SyncFolderItemsChangesType**</span><span class="sxs-lookup"><span data-stu-id="04a02-109">**SyncFolderItemsChangesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="04a02-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="04a02-110">Attributes and elements</span></span>

<span data-ttu-id="04a02-111">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="04a02-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="04a02-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="04a02-112">Attributes</span></span>

<span data-ttu-id="04a02-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="04a02-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="04a02-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="04a02-114">Child elements</span></span>

|<span data-ttu-id="04a02-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="04a02-115">**Element**</span></span>|<span data-ttu-id="04a02-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="04a02-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="04a02-117">Créer (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="04a02-117">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="04a02-118">Identifie un élément unique à créer dans le magasin du client local.</span><span class="sxs-lookup"><span data-stu-id="04a02-118">Identifies a single item to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="04a02-119">Mise à jour (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="04a02-119">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="04a02-120">Identifie un élément unique à mettre à jour dans le magasin de client local.</span><span class="sxs-lookup"><span data-stu-id="04a02-120">Identifies a single item to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="04a02-121">Supprimer (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="04a02-121">Delete (ItemSync)</span></span>](delete-itemsync.md) <br/> |<span data-ttu-id="04a02-122">Identifie un seul élément à supprimer dans le magasin de client local.</span><span class="sxs-lookup"><span data-stu-id="04a02-122">Identifies a single item to delete in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="04a02-123">ReadFlagChange</span><span class="sxs-lookup"><span data-stu-id="04a02-123">ReadFlagChange</span></span>](readflagchange.md) <br/> |<span data-ttu-id="04a02-124">Renvoyées dans les réponses [SyncFolderItems opération](syncfolderitems-operation.md) lorsqu’un élément a été lu.</span><span class="sxs-lookup"><span data-stu-id="04a02-124">Returned in [SyncFolderItems operation](syncfolderitems-operation.md) responses when an item has been read.</span></span> <span data-ttu-id="04a02-125">Cette propriété est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="04a02-125">This property is read-only.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="04a02-126">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="04a02-126">Parent elements</span></span>

|<span data-ttu-id="04a02-127">**Élément**</span><span class="sxs-lookup"><span data-stu-id="04a02-127">**Element**</span></span>|<span data-ttu-id="04a02-128">**Description**</span><span class="sxs-lookup"><span data-stu-id="04a02-128">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="04a02-129">SyncFolderItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="04a02-129">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md) <br/> |<span data-ttu-id="04a02-130">Contient l’état et les résultats d’une demande [d’opération SyncFolderItems](syncfolderitems-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="04a02-130">Contains the status and result of a [SyncFolderItems operation](syncfolderitems-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="04a02-131">Remarques</span><span class="sxs-lookup"><span data-stu-id="04a02-131">Remarks</span></span>

<span data-ttu-id="04a02-132">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="04a02-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="04a02-133">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="04a02-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="04a02-134">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="04a02-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="04a02-135">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="04a02-135">Schema name</span></span>  <br/> |<span data-ttu-id="04a02-136">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="04a02-136">Messages schema</span></span>  <br/> |
|<span data-ttu-id="04a02-137">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="04a02-137">Validation file</span></span>  <br/> |<span data-ttu-id="04a02-138">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="04a02-138">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="04a02-139">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="04a02-139">Can be empty</span></span>  <br/> |<span data-ttu-id="04a02-140">False</span><span class="sxs-lookup"><span data-stu-id="04a02-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="04a02-141">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="04a02-141">See also</span></span>



[<span data-ttu-id="04a02-142">Opération SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="04a02-142">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="04a02-143">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="04a02-143">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

