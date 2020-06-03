---
title: GlobalHasAttachments
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GlobalHasAttachments
api_type:
- schema
ms.assetid: 3d075e93-14bc-479d-957f-9b7873d1db39
description: L'élément GlobalHasAttachments contient une valeur qui indique si les éléments d'au moins une conversation dans une boîte aux lettres a une pièce jointe.
ms.openlocfilehash: e314e8e5c06ca7d7820b910c05b381765e88911f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459475"
---
# <a name="globalhasattachments"></a><span data-ttu-id="08edb-103">GlobalHasAttachments</span><span class="sxs-lookup"><span data-stu-id="08edb-103">GlobalHasAttachments</span></span>

<span data-ttu-id="08edb-104">Ce document peut contenir des informations liées aux fonctionnalités ou produits préliminaires qui sont sujettes à modifications avant la sortie de la version définitive. Ce document est fourni "tel quel" à titre indicatif et Microsoft exclut toute garantie, expresse ou implicite, en ce qui concerne ce document. L'élément **GlobalHasAttachments** contient une valeur qui indique si les éléments d'au moins une conversation dans une boîte aux lettres a une pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="08edb-104">The **GlobalHasAttachments** element contains a value that indicates whether at least one conversation item in a mailbox has an attachment.</span></span> 
  
[<span data-ttu-id="08edb-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="08edb-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="08edb-106">Conversations</span><span class="sxs-lookup"><span data-stu-id="08edb-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="08edb-107">Conversation (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="08edb-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="08edb-108">GlobalHasAttachments</span><span class="sxs-lookup"><span data-stu-id="08edb-108">GlobalHasAttachments</span></span>](globalhasattachments.md)
  
```XML
<GlobalHasAttachments/>
```

 <span data-ttu-id="08edb-109">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="08edb-109">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="08edb-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="08edb-110">Attributes and elements</span></span>

<span data-ttu-id="08edb-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="08edb-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="08edb-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="08edb-112">Attributes</span></span>

<span data-ttu-id="08edb-113">Aucune.</span><span class="sxs-lookup"><span data-stu-id="08edb-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="08edb-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="08edb-114">Child elements</span></span>

<span data-ttu-id="08edb-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="08edb-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="08edb-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="08edb-116">Parent elements</span></span>

|<span data-ttu-id="08edb-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="08edb-117">**Element**</span></span>|<span data-ttu-id="08edb-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="08edb-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="08edb-119">Conversation (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="08edb-119">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="08edb-120">Représente une conversation unique.</span><span class="sxs-lookup"><span data-stu-id="08edb-120">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="08edb-121">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="08edb-121">Text value</span></span>

<span data-ttu-id="08edb-p101">La valeur de l'élément **GlobalHasAttachments** indique si les éléments au moins une conversation dans une boîte aux lettres comportant une pièce jointe. Une valeur de texte qui représente une valeur Boolean est requise. La valeur **true** signifie que la conversation a au moins un des pièces jointes visible. La valeur **false** signifie que la conversation n'a aucune pièce jointe ou a masqué uniquement les pièces jointes.</span><span class="sxs-lookup"><span data-stu-id="08edb-p101">The value of the **GlobalHasAttachments** element indicates whether at least one conversation item in a mailbox has an attachment. A text value that represents a Boolean value is required. A value of **true** means that the conversation has at least one visible attachment. A value of **false** means that the conversation either has no attachments or has only hidden attachments.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="08edb-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="08edb-126">Remarks</span></span>

<span data-ttu-id="08edb-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="08edb-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="08edb-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="08edb-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="08edb-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="08edb-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="08edb-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="08edb-130">Schema name</span></span>  <br/> |<span data-ttu-id="08edb-131">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="08edb-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="08edb-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="08edb-132">Validation file</span></span>  <br/> |<span data-ttu-id="08edb-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="08edb-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="08edb-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="08edb-134">Can be empty</span></span>  <br/> |<span data-ttu-id="08edb-135">False</span><span class="sxs-lookup"><span data-stu-id="08edb-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="08edb-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="08edb-136">See also</span></span>



[<span data-ttu-id="08edb-137">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="08edb-137">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="08edb-138">Opération de ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="08edb-138">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="08edb-139">Conversations in EWS</span><span class="sxs-lookup"><span data-stu-id="08edb-139">Conversations in EWS</span></span>](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

