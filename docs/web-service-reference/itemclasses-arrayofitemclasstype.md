---
title: ItemClasses (ArrayOfItemClassType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 971784d1-6860-4833-bb26-0e930fa11c21
description: L’élément ItemClasses contient une liste des classes d’élément qui représente toutes les classes d’élément des éléments de conversation dans le dossier actif.
ms.openlocfilehash: 62ea5b624025b3f012249afd1763e2b393ef5caa
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828150"
---
# <a name="itemclasses-arrayofitemclasstype"></a><span data-ttu-id="2b66b-103">ItemClasses (ArrayOfItemClassType)</span><span class="sxs-lookup"><span data-stu-id="2b66b-103">ItemClasses (ArrayOfItemClassType)</span></span>

<span data-ttu-id="2b66b-104">L’élément **ItemClasses** contient une liste des classes d’élément qui représente toutes les classes d’élément des éléments de conversation dans le dossier actif.</span><span class="sxs-lookup"><span data-stu-id="2b66b-104">The **ItemClasses** element contains a list of item classes that represents all the item classes of the conversation items in the current folder.</span></span> 
  
[<span data-ttu-id="2b66b-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="2b66b-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="2b66b-106">Conversations</span><span class="sxs-lookup"><span data-stu-id="2b66b-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="2b66b-107">Conversation (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="2b66b-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="2b66b-108">ItemClasses (ArrayOfItemClassType)</span><span class="sxs-lookup"><span data-stu-id="2b66b-108">ItemClasses (ArrayOfItemClassType)</span></span>](itemclasses-arrayofitemclasstype.md)
  
```XML
<ItemClasses>
    <String/>
</ItemClasses>
```

 <span data-ttu-id="2b66b-109">**ArrayOfItemClassType**</span><span class="sxs-lookup"><span data-stu-id="2b66b-109">**ArrayOfItemClassType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2b66b-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="2b66b-110">Attributes and elements</span></span>

<span data-ttu-id="2b66b-111">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="2b66b-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2b66b-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="2b66b-112">Attributes</span></span>

<span data-ttu-id="2b66b-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="2b66b-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2b66b-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="2b66b-114">Child elements</span></span>

|<span data-ttu-id="2b66b-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2b66b-115">**Element**</span></span>|<span data-ttu-id="2b66b-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="2b66b-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2b66b-117">ItemClass</span><span class="sxs-lookup"><span data-stu-id="2b66b-117">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="2b66b-118">Représente la classe de message d'un élément.</span><span class="sxs-lookup"><span data-stu-id="2b66b-118">Represents the message class of an item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2b66b-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="2b66b-119">Parent elements</span></span>

|<span data-ttu-id="2b66b-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2b66b-120">**Element**</span></span>|<span data-ttu-id="2b66b-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="2b66b-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2b66b-122">Conversation (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="2b66b-122">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="2b66b-123">Représente une conversation unique.</span><span class="sxs-lookup"><span data-stu-id="2b66b-123">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2b66b-124">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="2b66b-124">Text value</span></span>

<span data-ttu-id="2b66b-125">Aucun.</span><span class="sxs-lookup"><span data-stu-id="2b66b-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2b66b-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="2b66b-126">Remarks</span></span>

<span data-ttu-id="2b66b-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="2b66b-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2b66b-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="2b66b-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2b66b-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="2b66b-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2b66b-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="2b66b-130">Schema name</span></span>  <br/> |<span data-ttu-id="2b66b-131">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="2b66b-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="2b66b-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="2b66b-132">Validation file</span></span>  <br/> |<span data-ttu-id="2b66b-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2b66b-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2b66b-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="2b66b-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="2b66b-135">False</span><span class="sxs-lookup"><span data-stu-id="2b66b-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2b66b-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="2b66b-136">See also</span></span>



[<span data-ttu-id="2b66b-137">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="2b66b-137">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="2b66b-138">Opération de ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="2b66b-138">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="2b66b-139">Conversations in EWS</span><span class="sxs-lookup"><span data-stu-id="2b66b-139">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

