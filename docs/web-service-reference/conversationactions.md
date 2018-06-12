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
description: L’élément ConversationActions contient une collection des conversations et les actions à appliquer à leur.
ms.openlocfilehash: 3dff7ff66f758f1cd2eb3cd7b8126294d2799fc0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755641"
---
# <a name="conversationactions"></a><span data-ttu-id="f919f-103">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="f919f-103">ConversationActions</span></span>

<span data-ttu-id="f919f-104">L’élément **ConversationActions** contient une collection des conversations et les actions à appliquer à leur.</span><span class="sxs-lookup"><span data-stu-id="f919f-104">The **ConversationActions** element contains a collection of conversations and the actions to apply to them.</span></span> 
  
[<span data-ttu-id="f919f-105">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="f919f-105">ApplyConversationAction</span></span>](applyconversationaction.md)
  
[<span data-ttu-id="f919f-106">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="f919f-106">ConversationActions</span></span>](conversationactions.md)
  
```XML
<ConversationActions>
   <ConversationAction/>
</ConversationActions>
```

 <span data-ttu-id="f919f-107">**NonEmptyArrayOfApplyConversationActionType**</span><span class="sxs-lookup"><span data-stu-id="f919f-107">**NonEmptyArrayOfApplyConversationActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f919f-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f919f-108">Attributes and elements</span></span>

<span data-ttu-id="f919f-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f919f-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f919f-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="f919f-110">Attributes</span></span>

<span data-ttu-id="f919f-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f919f-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f919f-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f919f-112">Child elements</span></span>

|<span data-ttu-id="f919f-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f919f-113">**Element**</span></span>|<span data-ttu-id="f919f-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="f919f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f919f-115">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="f919f-115">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="f919f-116">Contient une seule action à appliquer à une même conversation.</span><span class="sxs-lookup"><span data-stu-id="f919f-116">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f919f-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f919f-117">Parent elements</span></span>

|<span data-ttu-id="f919f-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f919f-118">**Element**</span></span>|<span data-ttu-id="f919f-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="f919f-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f919f-120">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="f919f-120">ApplyConversationAction</span></span>](applyconversationaction.md) <br/> |<span data-ttu-id="f919f-121">Définit une demande pour appliquer des actions à des éléments dans une conversation.</span><span class="sxs-lookup"><span data-stu-id="f919f-121">Defines a request to apply actions to items in a conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f919f-122">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="f919f-122">Text value</span></span>

<span data-ttu-id="f919f-123">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f919f-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f919f-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="f919f-124">Remarks</span></span>

<span data-ttu-id="f919f-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="f919f-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f919f-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f919f-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f919f-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f919f-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f919f-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f919f-128">Schema Name</span></span>  <br/> |<span data-ttu-id="f919f-129">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="f919f-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f919f-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="f919f-130">Validation File</span></span>  <br/> |<span data-ttu-id="f919f-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="f919f-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f919f-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f919f-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="f919f-133">False</span><span class="sxs-lookup"><span data-stu-id="f919f-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f919f-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f919f-134">See also</span></span>



[<span data-ttu-id="f919f-135">Opération de ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="f919f-135">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)

