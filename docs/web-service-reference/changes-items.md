---
title: Changes (éléments)
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
description: L’élément changes contient un tableau de séquence de types de modifications qui représentent les types de différences entre les éléments sur le client et les éléments sur le serveur Exchange.
ms.openlocfilehash: 6fda7b5602f172bae84ad7b211db2811def4f883
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463264"
---
# <a name="changes-items"></a><span data-ttu-id="2c003-103">Changes (éléments)</span><span class="sxs-lookup"><span data-stu-id="2c003-103">Changes (Items)</span></span>

<span data-ttu-id="2c003-104">L’élément **changes** contient un tableau de séquence de types de modifications qui représentent les types de différences entre les éléments sur le client et les éléments sur le serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="2c003-104">The **Changes** element contains a sequence array of change types that represent the types of differences between the items on the client and the items on the Exchange server.</span></span> 
  
[<span data-ttu-id="2c003-105">SyncFolderItemsResponse</span><span class="sxs-lookup"><span data-stu-id="2c003-105">SyncFolderItemsResponse</span></span>](syncfolderitemsresponse.md)
  
[<span data-ttu-id="2c003-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="2c003-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="2c003-107">SyncFolderItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="2c003-107">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md)
  
[<span data-ttu-id="2c003-108">Changes (éléments)</span><span class="sxs-lookup"><span data-stu-id="2c003-108">Changes (Items)</span></span>](changes-items.md)
  
```xml
<Changes>
   <Create/>
   <Update/>
   <Delete/>
</Changes>
```

 <span data-ttu-id="2c003-109">**SyncFolderItemsChangesType**</span><span class="sxs-lookup"><span data-stu-id="2c003-109">**SyncFolderItemsChangesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2c003-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="2c003-110">Attributes and elements</span></span>

<span data-ttu-id="2c003-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="2c003-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2c003-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="2c003-112">Attributes</span></span>

<span data-ttu-id="2c003-113">Aucune.</span><span class="sxs-lookup"><span data-stu-id="2c003-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2c003-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="2c003-114">Child elements</span></span>

|<span data-ttu-id="2c003-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2c003-115">**Element**</span></span>|<span data-ttu-id="2c003-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="2c003-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2c003-117">Créer (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="2c003-117">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="2c003-118">Identifie un élément unique à créer dans le magasin client local.</span><span class="sxs-lookup"><span data-stu-id="2c003-118">Identifies a single item to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="2c003-119">Mise à jour (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="2c003-119">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="2c003-120">Identifie un élément unique à mettre à jour dans le magasin de client local.</span><span class="sxs-lookup"><span data-stu-id="2c003-120">Identifies a single item to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="2c003-121">Supprimer (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="2c003-121">Delete (ItemSync)</span></span>](delete-itemsync.md) <br/> |<span data-ttu-id="2c003-122">Identifie un élément unique à supprimer dans le magasin client local.</span><span class="sxs-lookup"><span data-stu-id="2c003-122">Identifies a single item to delete in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="2c003-123">ReadFlagChange</span><span class="sxs-lookup"><span data-stu-id="2c003-123">ReadFlagChange</span></span>](readflagchange.md) <br/> |<span data-ttu-id="2c003-124">Renvoyée dans les réponses d' [opération SyncFolderItems](syncfolderitems-operation.md) lorsqu’un élément a été lu.</span><span class="sxs-lookup"><span data-stu-id="2c003-124">Returned in [SyncFolderItems operation](syncfolderitems-operation.md) responses when an item has been read.</span></span> <span data-ttu-id="2c003-125">Cette propriété est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="2c003-125">This property is read-only.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2c003-126">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="2c003-126">Parent elements</span></span>

|<span data-ttu-id="2c003-127">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2c003-127">**Element**</span></span>|<span data-ttu-id="2c003-128">**Description**</span><span class="sxs-lookup"><span data-stu-id="2c003-128">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2c003-129">SyncFolderItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="2c003-129">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md) <br/> |<span data-ttu-id="2c003-130">Contient l’État et le résultat d’une demande d' [opération SyncFolderItems](syncfolderitems-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="2c003-130">Contains the status and result of a [SyncFolderItems operation](syncfolderitems-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2c003-131">Remarques</span><span class="sxs-lookup"><span data-stu-id="2c003-131">Remarks</span></span>

<span data-ttu-id="2c003-132">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="2c003-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2c003-133">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="2c003-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2c003-134">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="2c003-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2c003-135">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="2c003-135">Schema name</span></span>  <br/> |<span data-ttu-id="2c003-136">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="2c003-136">Messages schema</span></span>  <br/> |
|<span data-ttu-id="2c003-137">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="2c003-137">Validation file</span></span>  <br/> |<span data-ttu-id="2c003-138">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="2c003-138">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2c003-139">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="2c003-139">Can be empty</span></span>  <br/> |<span data-ttu-id="2c003-140">False</span><span class="sxs-lookup"><span data-stu-id="2c003-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2c003-141">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="2c003-141">See also</span></span>



[<span data-ttu-id="2c003-142">Opération SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="2c003-142">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="2c003-143">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="2c003-143">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

