---
title: GlobalUniqueRecipients
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GlobalUniqueRecipients
api_type:
- schema
ms.assetid: 67379c1c-85d9-4b11-8f17-ad9d24904788
description: L'élément GlobalUniqueRecipients contient la liste des destinataires d'une conversation regroupée sur une boîte aux lettres.
ms.openlocfilehash: 5eb6e60d3ece8d8369f4603e36ffaaf72a3e459d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19827742"
---
# <a name="globaluniquerecipients"></a><span data-ttu-id="2cf50-103">GlobalUniqueRecipients</span><span class="sxs-lookup"><span data-stu-id="2cf50-103">GlobalUniqueRecipients</span></span>

<span data-ttu-id="2cf50-104">Ce document peut contenir des informations liées aux fonctionnalités ou produits préliminaires qui sont sujettes à modifications avant la sortie de la version définitive. Ce document est fourni "tel quel" à titre indicatif et Microsoft exclut toute garantie, expresse ou implicite, en ce qui concerne ce document. L'élément **GlobalUniqueRecipients** contient la liste des destinataires d'une conversation regroupée sur une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="2cf50-104">The **GlobalUniqueRecipients** element contains the recipient list of a conversation aggregated across a mailbox.</span></span> 
  
[<span data-ttu-id="2cf50-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="2cf50-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="2cf50-106">Conversations</span><span class="sxs-lookup"><span data-stu-id="2cf50-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="2cf50-107">Conversation (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="2cf50-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="2cf50-108">GlobalUniqueRecipients</span><span class="sxs-lookup"><span data-stu-id="2cf50-108">GlobalUniqueRecipients</span></span>](globaluniquerecipients.md)
  
```XML
<GlobalUniqueRecipients>
   <String/>
</GlobalUniqueRecipients>
```

 <span data-ttu-id="2cf50-109">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="2cf50-109">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2cf50-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="2cf50-110">Attributes and elements</span></span>

<span data-ttu-id="2cf50-111">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="2cf50-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2cf50-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="2cf50-112">Attributes</span></span>

<span data-ttu-id="2cf50-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="2cf50-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2cf50-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="2cf50-114">Child elements</span></span>

|<span data-ttu-id="2cf50-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2cf50-115">**Element**</span></span>|<span data-ttu-id="2cf50-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="2cf50-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2cf50-117">String</span><span class="sxs-lookup"><span data-stu-id="2cf50-117">String</span></span>](string.md) <br/> |<span data-ttu-id="2cf50-118">Contient un destinataire unique de conversation.</span><span class="sxs-lookup"><span data-stu-id="2cf50-118">Contains a single conversation recipient.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2cf50-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="2cf50-119">Parent elements</span></span>

|<span data-ttu-id="2cf50-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2cf50-120">**Element**</span></span>|<span data-ttu-id="2cf50-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="2cf50-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2cf50-122">Conversation (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="2cf50-122">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="2cf50-123">Représente une conversation unique.</span><span class="sxs-lookup"><span data-stu-id="2cf50-123">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2cf50-124">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="2cf50-124">Text value</span></span>

<span data-ttu-id="2cf50-125">Aucun.</span><span class="sxs-lookup"><span data-stu-id="2cf50-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2cf50-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="2cf50-126">Remarks</span></span>

<span data-ttu-id="2cf50-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="2cf50-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2cf50-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="2cf50-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2cf50-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="2cf50-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2cf50-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="2cf50-130">Schema name</span></span>  <br/> |<span data-ttu-id="2cf50-131">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="2cf50-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="2cf50-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="2cf50-132">Validation file</span></span>  <br/> |<span data-ttu-id="2cf50-133">types.xsd</span><span class="sxs-lookup"><span data-stu-id="2cf50-133">types.xsd</span></span>  <br/> |
|<span data-ttu-id="2cf50-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="2cf50-134">Can be empty</span></span>  <br/> |<span data-ttu-id="2cf50-135">False</span><span class="sxs-lookup"><span data-stu-id="2cf50-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2cf50-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="2cf50-136">See also</span></span>



[<span data-ttu-id="2cf50-137">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="2cf50-137">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="2cf50-138">Opération de ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="2cf50-138">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="2cf50-139">Conversations in EWS</span><span class="sxs-lookup"><span data-stu-id="2cf50-139">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

