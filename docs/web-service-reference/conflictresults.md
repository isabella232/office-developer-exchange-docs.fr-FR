---
title: ConflictResults
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConflictResults
api_type:
- schema
ms.assetid: 08cdd547-4de7-4c7a-b60f-e618dc217d20
description: L’élément ConflictResults contient le nombre de conflits dans une réponse d’opération UpdateItem.
ms.openlocfilehash: faa6dc6c5fbbe874438a89c810a12fa675e8a1c9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755541"
---
# <a name="conflictresults"></a><span data-ttu-id="89e4c-103">ConflictResults</span><span class="sxs-lookup"><span data-stu-id="89e4c-103">ConflictResults</span></span>

<span data-ttu-id="89e4c-104">L’élément [ConflictResults](conflictresults.md) contient le nombre de conflits dans une réponse [d’opération UpdateItem](updateitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="89e4c-104">The [ConflictResults](conflictresults.md) element contains the number of conflicts in an [UpdateItem operation](updateitem-operation.md) response.</span></span> 
  
[<span data-ttu-id="89e4c-105">UpdateItemResponse</span><span class="sxs-lookup"><span data-stu-id="89e4c-105">UpdateItemResponse</span></span>](updateitemresponse.md)
  
[<span data-ttu-id="89e4c-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="89e4c-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="89e4c-107">UpdateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="89e4c-107">UpdateItemResponseMessage</span></span>](updateitemresponsemessage.md)
  
[<span data-ttu-id="89e4c-108">ConflictResults</span><span class="sxs-lookup"><span data-stu-id="89e4c-108">ConflictResults</span></span>](conflictresults.md)
  
```xml
<ConflictResults>
   <Count/>
</ConflictResults>
```

 <span data-ttu-id="89e4c-109">**ConflictResultsType**</span><span class="sxs-lookup"><span data-stu-id="89e4c-109">**ConflictResultsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="89e4c-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="89e4c-110">Attributes and elements</span></span>

<span data-ttu-id="89e4c-111">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="89e4c-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="89e4c-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="89e4c-112">Attributes</span></span>

<span data-ttu-id="89e4c-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="89e4c-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="89e4c-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="89e4c-114">Child elements</span></span>

|<span data-ttu-id="89e4c-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="89e4c-115">**Element**</span></span>|<span data-ttu-id="89e4c-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="89e4c-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="89e4c-117">Count</span><span class="sxs-lookup"><span data-stu-id="89e4c-117">Count</span></span>](count.md) <br/> |<span data-ttu-id="89e4c-118">Contient le nombre de conflits dans une réponse [d’opération UpdateItem](updateitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="89e4c-118">Contains the number of conflicts in an [UpdateItem operation](updateitem-operation.md) response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="89e4c-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="89e4c-119">Parent elements</span></span>

|<span data-ttu-id="89e4c-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="89e4c-120">**Element**</span></span>|<span data-ttu-id="89e4c-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="89e4c-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="89e4c-122">UpdateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="89e4c-122">UpdateItemResponseMessage</span></span>](updateitemresponsemessage.md) <br/> |<span data-ttu-id="89e4c-123">Contient l’état et les résultats d’une seule demande [d’opération UpdateItem](updateitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="89e4c-123">Contains the status and result of a single [UpdateItem operation](updateitem-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="89e4c-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="89e4c-124">Remarks</span></span>

<span data-ttu-id="89e4c-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Exchange Server avec le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="89e4c-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="89e4c-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="89e4c-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="89e4c-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="89e4c-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="89e4c-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="89e4c-128">Schema Name</span></span>  <br/> |<span data-ttu-id="89e4c-129">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="89e4c-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="89e4c-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="89e4c-130">Validation File</span></span>  <br/> |<span data-ttu-id="89e4c-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="89e4c-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="89e4c-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="89e4c-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="89e4c-133">False</span><span class="sxs-lookup"><span data-stu-id="89e4c-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="89e4c-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="89e4c-134">See also</span></span>



[<span data-ttu-id="89e4c-135">UpdateItem Operation</span><span class="sxs-lookup"><span data-stu-id="89e4c-135">UpdateItem operation</span></span>](updateitem-operation.md)
  
 <span data-ttu-id="89e4c-136">**ConflictResultsType**</span><span class="sxs-lookup"><span data-stu-id="89e4c-136">**ConflictResultsType**</span></span>

