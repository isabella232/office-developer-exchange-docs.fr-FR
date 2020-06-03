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
ms.openlocfilehash: 3481c43b99f75a05a8e7fbe5a288e04708290d83
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456037"
---
# <a name="globaluniquerecipients"></a><span data-ttu-id="38c79-103">GlobalUniqueRecipients</span><span class="sxs-lookup"><span data-stu-id="38c79-103">GlobalUniqueRecipients</span></span>

<span data-ttu-id="38c79-104">Ce document peut contenir des informations liées aux fonctionnalités ou produits préliminaires qui sont sujettes à modifications avant la sortie de la version définitive. Ce document est fourni "tel quel" à titre indicatif et Microsoft exclut toute garantie, expresse ou implicite, en ce qui concerne ce document. L'élément **GlobalUniqueRecipients** contient la liste des destinataires d'une conversation regroupée sur une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="38c79-104">The **GlobalUniqueRecipients** element contains the recipient list of a conversation aggregated across a mailbox.</span></span> 
  
[<span data-ttu-id="38c79-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="38c79-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="38c79-106">Conversations</span><span class="sxs-lookup"><span data-stu-id="38c79-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="38c79-107">Conversation (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="38c79-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="38c79-108">GlobalUniqueRecipients</span><span class="sxs-lookup"><span data-stu-id="38c79-108">GlobalUniqueRecipients</span></span>](globaluniquerecipients.md)
  
```XML
<GlobalUniqueRecipients>
   <String/>
</GlobalUniqueRecipients>
```

 <span data-ttu-id="38c79-109">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="38c79-109">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="38c79-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="38c79-110">Attributes and elements</span></span>

<span data-ttu-id="38c79-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="38c79-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="38c79-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="38c79-112">Attributes</span></span>

<span data-ttu-id="38c79-113">Aucune.</span><span class="sxs-lookup"><span data-stu-id="38c79-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="38c79-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="38c79-114">Child elements</span></span>

|<span data-ttu-id="38c79-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="38c79-115">**Element**</span></span>|<span data-ttu-id="38c79-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="38c79-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="38c79-117">String</span><span class="sxs-lookup"><span data-stu-id="38c79-117">String</span></span>](string.md) <br/> |<span data-ttu-id="38c79-118">Contient un destinataire unique de conversation.</span><span class="sxs-lookup"><span data-stu-id="38c79-118">Contains a single conversation recipient.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="38c79-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="38c79-119">Parent elements</span></span>

|<span data-ttu-id="38c79-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="38c79-120">**Element**</span></span>|<span data-ttu-id="38c79-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="38c79-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="38c79-122">Conversation (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="38c79-122">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="38c79-123">Représente une conversation unique.</span><span class="sxs-lookup"><span data-stu-id="38c79-123">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="38c79-124">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="38c79-124">Text value</span></span>

<span data-ttu-id="38c79-125">Aucun.</span><span class="sxs-lookup"><span data-stu-id="38c79-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="38c79-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="38c79-126">Remarks</span></span>

<span data-ttu-id="38c79-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="38c79-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="38c79-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="38c79-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="38c79-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="38c79-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="38c79-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="38c79-130">Schema name</span></span>  <br/> |<span data-ttu-id="38c79-131">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="38c79-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="38c79-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="38c79-132">Validation file</span></span>  <br/> |<span data-ttu-id="38c79-133">types. xsd</span><span class="sxs-lookup"><span data-stu-id="38c79-133">types.xsd</span></span>  <br/> |
|<span data-ttu-id="38c79-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="38c79-134">Can be empty</span></span>  <br/> |<span data-ttu-id="38c79-135">False</span><span class="sxs-lookup"><span data-stu-id="38c79-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="38c79-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="38c79-136">See also</span></span>



[<span data-ttu-id="38c79-137">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="38c79-137">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="38c79-138">Opération de ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="38c79-138">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="38c79-139">Conversations in EWS</span><span class="sxs-lookup"><span data-stu-id="38c79-139">Conversations in EWS</span></span>](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

