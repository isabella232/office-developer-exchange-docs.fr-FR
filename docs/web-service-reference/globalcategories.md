---
title: GlobalCategories
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GlobalCategories
api_type:
- schema
ms.assetid: 7a1d3f04-4ada-4a31-845e-f1f1ff6e136f
description: L’élément GlobalCategories contient la liste des catégories pour tous les éléments de conversation dans une boîte aux lettres.
ms.openlocfilehash: 5cedea821b14264f15026c2d297c3017534ca354
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19827711"
---
# <a name="globalcategories"></a><span data-ttu-id="f82a7-103">GlobalCategories</span><span class="sxs-lookup"><span data-stu-id="f82a7-103">GlobalCategories</span></span>

<span data-ttu-id="f82a7-104">L’élément **GlobalCategories** contient la liste des catégories pour tous les éléments de conversation dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="f82a7-104">The **GlobalCategories** element contains the category list for all conversation items in a mailbox.</span></span> 
  
[<span data-ttu-id="f82a7-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="f82a7-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="f82a7-106">Conversations</span><span class="sxs-lookup"><span data-stu-id="f82a7-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="f82a7-107">Conversation (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="f82a7-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="f82a7-108">GlobalCategories</span><span class="sxs-lookup"><span data-stu-id="f82a7-108">GlobalCategories</span></span>](globalcategories.md)
  
```XML
<GlobalCategories>
   <String/>
</GlobalCategories>
```

 <span data-ttu-id="f82a7-109">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="f82a7-109">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f82a7-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f82a7-110">Attributes and elements</span></span>

<span data-ttu-id="f82a7-111">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f82a7-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f82a7-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="f82a7-112">Attributes</span></span>

<span data-ttu-id="f82a7-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f82a7-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f82a7-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f82a7-114">Child elements</span></span>

|<span data-ttu-id="f82a7-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f82a7-115">**Element**</span></span>|<span data-ttu-id="f82a7-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="f82a7-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f82a7-117">String</span><span class="sxs-lookup"><span data-stu-id="f82a7-117">String</span></span>](string.md) <br/> |<span data-ttu-id="f82a7-118">Contient une seule catégorie.</span><span class="sxs-lookup"><span data-stu-id="f82a7-118">Contains a single category.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f82a7-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f82a7-119">Parent elements</span></span>

|<span data-ttu-id="f82a7-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f82a7-120">**Element**</span></span>|<span data-ttu-id="f82a7-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="f82a7-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f82a7-122">Conversation (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="f82a7-122">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="f82a7-123">Représente une conversation unique.</span><span class="sxs-lookup"><span data-stu-id="f82a7-123">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f82a7-124">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="f82a7-124">Text value</span></span>

<span data-ttu-id="f82a7-125">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f82a7-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f82a7-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="f82a7-126">Remarks</span></span>

<span data-ttu-id="f82a7-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="f82a7-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f82a7-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f82a7-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f82a7-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f82a7-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f82a7-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f82a7-130">Schema name</span></span>  <br/> |<span data-ttu-id="f82a7-131">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="f82a7-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="f82a7-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="f82a7-132">Validation file</span></span>  <br/> |<span data-ttu-id="f82a7-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f82a7-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f82a7-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f82a7-134">Can be empty</span></span>  <br/> |<span data-ttu-id="f82a7-135">False</span><span class="sxs-lookup"><span data-stu-id="f82a7-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f82a7-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f82a7-136">See also</span></span>



[<span data-ttu-id="f82a7-137">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="f82a7-137">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="f82a7-138">Opération de ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="f82a7-138">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="f82a7-139">Conversations in EWS</span><span class="sxs-lookup"><span data-stu-id="f82a7-139">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

