---
title: Supprimer (ItemSync)
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
ms.assetid: 4f372d57-2e39-46af-9d83-6c8c55108587
description: L’élément delete identifie un élément unique à supprimer dans le magasin client local.
ms.openlocfilehash: 6e30ddc7f7248fe7ff7136e19ba58c7d5d8a800f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44454679"
---
# <a name="delete-itemsync"></a><span data-ttu-id="7b335-103">Supprimer (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="7b335-103">Delete (ItemSync)</span></span>

<span data-ttu-id="7b335-104">L’élément **Delete** identifie un élément unique à supprimer dans le magasin client local.</span><span class="sxs-lookup"><span data-stu-id="7b335-104">The **Delete** element identifies a single item to delete in the local client store.</span></span> 
  
- [<span data-ttu-id="7b335-105">SyncFolderItemsResponse</span><span class="sxs-lookup"><span data-stu-id="7b335-105">SyncFolderItemsResponse</span></span>](syncfolderitemsresponse.md)  
- [<span data-ttu-id="7b335-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="7b335-106">ResponseMessages</span></span>](responsemessages.md) 
- [<span data-ttu-id="7b335-107">SyncFolderItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="7b335-107">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md)  
- [<span data-ttu-id="7b335-108">Changes (éléments)</span><span class="sxs-lookup"><span data-stu-id="7b335-108">Changes (Items)</span></span>](changes-items.md)  
- [<span data-ttu-id="7b335-109">Supprimer (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="7b335-109">Delete (ItemSync)</span></span>](delete-itemsync.md)
  
```xml
<Delete>
   <ItemId/>
</Delete>
```

<span data-ttu-id="7b335-110">**SyncFolderItemsDeleteType**</span><span class="sxs-lookup"><span data-stu-id="7b335-110">**SyncFolderItemsDeleteType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="7b335-111">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="7b335-111">Attributes and elements</span></span>

<span data-ttu-id="7b335-112">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="7b335-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7b335-113">Attributs</span><span class="sxs-lookup"><span data-stu-id="7b335-113">Attributes</span></span>

<span data-ttu-id="7b335-114">Aucune.</span><span class="sxs-lookup"><span data-stu-id="7b335-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7b335-115">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="7b335-115">Child elements</span></span>

|<span data-ttu-id="7b335-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7b335-116">**Element**</span></span>|<span data-ttu-id="7b335-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="7b335-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7b335-118">ItemId</span><span class="sxs-lookup"><span data-stu-id="7b335-118">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="7b335-119">Contient l'identificateur unique et la clé de modification d'un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="7b335-119">Contains the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7b335-120">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="7b335-120">Parent elements</span></span>

|<span data-ttu-id="7b335-121">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7b335-121">**Element**</span></span>|<span data-ttu-id="7b335-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="7b335-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7b335-123">Changes (éléments)</span><span class="sxs-lookup"><span data-stu-id="7b335-123">Changes (Items)</span></span>](changes-items.md) <br/> |<span data-ttu-id="7b335-124">Contient un tableau de séquence de types de modifications qui représentent le type de différences entre les éléments sur le client et les éléments sur le serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="7b335-124">Contains a sequence array of change types that represent the type of differences between the items on the client and the items on the Exchange server.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7b335-125">Remarques</span><span class="sxs-lookup"><span data-stu-id="7b335-125">Remarks</span></span>

<span data-ttu-id="7b335-126">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="7b335-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7b335-127">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="7b335-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7b335-128">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="7b335-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7b335-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="7b335-129">Schema name</span></span>  <br/> |<span data-ttu-id="7b335-130">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="7b335-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="7b335-131">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="7b335-131">Validation file</span></span>  <br/> |<span data-ttu-id="7b335-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7b335-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7b335-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="7b335-133">Can be empty</span></span>  <br/> |<span data-ttu-id="7b335-134">False</span><span class="sxs-lookup"><span data-stu-id="7b335-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7b335-135">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7b335-135">See also</span></span>

- [<span data-ttu-id="7b335-136">Opération SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="7b335-136">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)
- [<span data-ttu-id="7b335-137">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="7b335-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

