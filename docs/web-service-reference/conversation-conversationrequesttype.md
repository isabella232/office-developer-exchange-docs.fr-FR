---
title: Conversation (ConversationRequestType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0308b71c-d4ff-44a8-b9ca-d5965291ee1d
description: L’élément conversation représente une conversation unique renvoyée dans une réponse GetConversationItems.
ms.openlocfilehash: 925fd6fce83cad36f4a0e95bb6228ba65e4e9c43
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466779"
---
# <a name="conversation-conversationrequesttype"></a><span data-ttu-id="58d04-103">Conversation (ConversationRequestType)</span><span class="sxs-lookup"><span data-stu-id="58d04-103">Conversation (ConversationRequestType)</span></span>

<span data-ttu-id="58d04-104">L’élément **conversation** représente une conversation unique renvoyée dans une réponse **GetConversationItems** .</span><span class="sxs-lookup"><span data-stu-id="58d04-104">The **Conversation** element represents a single conversation returned in a **GetConversationItems** response.</span></span> 
  
```XML
<Conversation>
   <ConversationId/>
   <SyncState/>
</Conversation>
```

 ****
## <a name="attributes-and-elements"></a><span data-ttu-id="58d04-105">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="58d04-105">Attributes and elements</span></span>

<span data-ttu-id="58d04-106">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="58d04-106">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="58d04-107">Attributs</span><span class="sxs-lookup"><span data-stu-id="58d04-107">Attributes</span></span>

<span data-ttu-id="58d04-108">Aucune.</span><span class="sxs-lookup"><span data-stu-id="58d04-108">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="58d04-109">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="58d04-109">Child elements</span></span>

<span data-ttu-id="58d04-110">[ConversationId](conversationid.md)  |  [SyncState (base64Binary)](syncstate-base64binary.md)</span><span class="sxs-lookup"><span data-stu-id="58d04-110">[ConversationId](conversationid.md) | [SyncState (base64Binary)](syncstate-base64binary.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="58d04-111">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="58d04-111">Parent elements</span></span>

[<span data-ttu-id="58d04-112">Conversations</span><span class="sxs-lookup"><span data-stu-id="58d04-112">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
## <a name="remarks"></a><span data-ttu-id="58d04-113">Remarques</span><span class="sxs-lookup"><span data-stu-id="58d04-113">Remarks</span></span>

<span data-ttu-id="58d04-114">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="58d04-114">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="58d04-115">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="58d04-115">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="58d04-116">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="58d04-116">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="58d04-117">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="58d04-117">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="58d04-118">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="58d04-118">Schema name</span></span>  <br/> |<span data-ttu-id="58d04-119">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="58d04-119">Types schema</span></span>  <br/> |
|<span data-ttu-id="58d04-120">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="58d04-120">Validation file</span></span>  <br/> |<span data-ttu-id="58d04-121">types. xsd</span><span class="sxs-lookup"><span data-stu-id="58d04-121">types.xsd</span></span>  <br/> |
|<span data-ttu-id="58d04-122">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="58d04-122">Can be empty</span></span>  <br/> |<span data-ttu-id="58d04-123">false</span><span class="sxs-lookup"><span data-stu-id="58d04-123">false</span></span>  <br/> |
   

