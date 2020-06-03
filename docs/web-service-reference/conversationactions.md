---
title: ConversationActions
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConversationActions
api_type:
- schema
ms.assetid: 3d6c663d-4bd9-4eec-b95a-cd683f592672
description: L’élément ConversationActions contient une collection de conversations et les actions à leur appliquer.
ms.openlocfilehash: 2db84f78b4b8c92e0a6ef7d69fba7c778fb5f96d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527102"
---
# <a name="conversationactions"></a><span data-ttu-id="7ac55-103">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="7ac55-103">ConversationActions</span></span>

<span data-ttu-id="7ac55-104">L’élément **ConversationActions** contient une collection de conversations et les actions à leur appliquer.</span><span class="sxs-lookup"><span data-stu-id="7ac55-104">The **ConversationActions** element contains a collection of conversations and the actions to apply to them.</span></span> 
  
[<span data-ttu-id="7ac55-105">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="7ac55-105">ApplyConversationAction</span></span>](applyconversationaction.md)
  
[<span data-ttu-id="7ac55-106">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="7ac55-106">ConversationActions</span></span>](conversationactions.md)
  
```XML
<ConversationActions>
   <ConversationAction/>
</ConversationActions>
```

 <span data-ttu-id="7ac55-107">**NonEmptyArrayOfApplyConversationActionType**</span><span class="sxs-lookup"><span data-stu-id="7ac55-107">**NonEmptyArrayOfApplyConversationActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7ac55-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="7ac55-108">Attributes and elements</span></span>

<span data-ttu-id="7ac55-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="7ac55-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7ac55-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="7ac55-110">Attributes</span></span>

<span data-ttu-id="7ac55-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="7ac55-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7ac55-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="7ac55-112">Child elements</span></span>

|<span data-ttu-id="7ac55-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7ac55-113">**Element**</span></span>|<span data-ttu-id="7ac55-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="7ac55-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7ac55-115">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="7ac55-115">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="7ac55-116">Contient une seule action à appliquer à une conversation unique.</span><span class="sxs-lookup"><span data-stu-id="7ac55-116">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7ac55-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="7ac55-117">Parent elements</span></span>

|<span data-ttu-id="7ac55-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7ac55-118">**Element**</span></span>|<span data-ttu-id="7ac55-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="7ac55-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7ac55-120">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="7ac55-120">ApplyConversationAction</span></span>](applyconversationaction.md) <br/> |<span data-ttu-id="7ac55-121">Définit une demande d’application d’actions à des éléments d’une conversation.</span><span class="sxs-lookup"><span data-stu-id="7ac55-121">Defines a request to apply actions to items in a conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7ac55-122">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="7ac55-122">Text value</span></span>

<span data-ttu-id="7ac55-123">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7ac55-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7ac55-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="7ac55-124">Remarks</span></span>

<span data-ttu-id="7ac55-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="7ac55-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7ac55-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="7ac55-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7ac55-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="7ac55-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7ac55-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="7ac55-128">Schema Name</span></span>  <br/> |<span data-ttu-id="7ac55-129">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="7ac55-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7ac55-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="7ac55-130">Validation File</span></span>  <br/> |<span data-ttu-id="7ac55-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="7ac55-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7ac55-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="7ac55-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="7ac55-133">False</span><span class="sxs-lookup"><span data-stu-id="7ac55-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7ac55-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7ac55-134">See also</span></span>



[<span data-ttu-id="7ac55-135">Opération de ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="7ac55-135">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)

