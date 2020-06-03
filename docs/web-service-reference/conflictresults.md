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
description: L’élément ConflictResults contient le nombre de conflits dans une réponse de l’opération UpdateItem.
ms.openlocfilehash: 923c7950e21039adf28e232486f4df5fc04889d1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460168"
---
# <a name="conflictresults"></a><span data-ttu-id="4a63d-103">ConflictResults</span><span class="sxs-lookup"><span data-stu-id="4a63d-103">ConflictResults</span></span>

<span data-ttu-id="4a63d-104">L’élément [ConflictResults](conflictresults.md) contient le nombre de conflits dans une réponse de l' [opération UpdateItem](updateitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="4a63d-104">The [ConflictResults](conflictresults.md) element contains the number of conflicts in an [UpdateItem operation](updateitem-operation.md) response.</span></span> 
  
[<span data-ttu-id="4a63d-105">UpdateItemResponse</span><span class="sxs-lookup"><span data-stu-id="4a63d-105">UpdateItemResponse</span></span>](updateitemresponse.md)
  
[<span data-ttu-id="4a63d-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="4a63d-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="4a63d-107">UpdateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="4a63d-107">UpdateItemResponseMessage</span></span>](updateitemresponsemessage.md)
  
[<span data-ttu-id="4a63d-108">ConflictResults</span><span class="sxs-lookup"><span data-stu-id="4a63d-108">ConflictResults</span></span>](conflictresults.md)
  
```xml
<ConflictResults>
   <Count/>
</ConflictResults>
```

 <span data-ttu-id="4a63d-109">**ConflictResultsType**</span><span class="sxs-lookup"><span data-stu-id="4a63d-109">**ConflictResultsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4a63d-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="4a63d-110">Attributes and elements</span></span>

<span data-ttu-id="4a63d-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="4a63d-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4a63d-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="4a63d-112">Attributes</span></span>

<span data-ttu-id="4a63d-113">Aucune.</span><span class="sxs-lookup"><span data-stu-id="4a63d-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4a63d-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="4a63d-114">Child elements</span></span>

|<span data-ttu-id="4a63d-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4a63d-115">**Element**</span></span>|<span data-ttu-id="4a63d-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="4a63d-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4a63d-117">Count</span><span class="sxs-lookup"><span data-stu-id="4a63d-117">Count</span></span>](count.md) <br/> |<span data-ttu-id="4a63d-118">Contient le nombre de conflits dans une réponse d' [opération UpdateItem](updateitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="4a63d-118">Contains the number of conflicts in an [UpdateItem operation](updateitem-operation.md) response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4a63d-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="4a63d-119">Parent elements</span></span>

|<span data-ttu-id="4a63d-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4a63d-120">**Element**</span></span>|<span data-ttu-id="4a63d-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="4a63d-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4a63d-122">UpdateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="4a63d-122">UpdateItemResponseMessage</span></span>](updateitemresponsemessage.md) <br/> |<span data-ttu-id="4a63d-123">Contient l’État et le résultat d’une seule demande d' [opération UpdateItem](updateitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="4a63d-123">Contains the status and result of a single [UpdateItem operation](updateitem-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4a63d-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="4a63d-124">Remarks</span></span>

<span data-ttu-id="4a63d-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Exchange Server et sur lequel le rôle serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="4a63d-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4a63d-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="4a63d-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4a63d-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="4a63d-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4a63d-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="4a63d-128">Schema Name</span></span>  <br/> |<span data-ttu-id="4a63d-129">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="4a63d-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="4a63d-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="4a63d-130">Validation File</span></span>  <br/> |<span data-ttu-id="4a63d-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4a63d-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4a63d-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="4a63d-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="4a63d-133">False</span><span class="sxs-lookup"><span data-stu-id="4a63d-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4a63d-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4a63d-134">See also</span></span>



[<span data-ttu-id="4a63d-135">Opération UpdateItem</span><span class="sxs-lookup"><span data-stu-id="4a63d-135">UpdateItem operation</span></span>](updateitem-operation.md)
  
 <span data-ttu-id="4a63d-136">**ConflictResultsType**</span><span class="sxs-lookup"><span data-stu-id="4a63d-136">**ConflictResultsType**</span></span>

