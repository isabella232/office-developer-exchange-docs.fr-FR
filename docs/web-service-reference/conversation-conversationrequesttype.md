---
title: Conversation (ConversationRequestType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0308b71c-d4ff-44a8-b9ca-d5965291ee1d
description: L’élément de Conversation représente une conversation unique retournée dans la réponse GetConversationItems.
ms.openlocfilehash: ef56e26fda7d2bf6556069355918aa576ce14cb6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755630"
---
# <a name="conversation-conversationrequesttype"></a><span data-ttu-id="c0f12-103">Conversation (ConversationRequestType)</span><span class="sxs-lookup"><span data-stu-id="c0f12-103">Conversation (ConversationRequestType)</span></span>

<span data-ttu-id="c0f12-104">L’élément de **Conversation** représente une conversation unique retournée dans la réponse **GetConversationItems** .</span><span class="sxs-lookup"><span data-stu-id="c0f12-104">The **Conversation** element represents a single conversation returned in a **GetConversationItems** response.</span></span> 
  
```XML
<Conversation>
   <ConversationId/>
   <SyncState/>
</Conversation>
```

 ****
## <a name="attributes-and-elements"></a><span data-ttu-id="c0f12-105">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="c0f12-105">Attributes and elements</span></span>

<span data-ttu-id="c0f12-106">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="c0f12-106">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c0f12-107">Attributs</span><span class="sxs-lookup"><span data-stu-id="c0f12-107">Attributes</span></span>

<span data-ttu-id="c0f12-108">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c0f12-108">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c0f12-109">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="c0f12-109">Child elements</span></span>

<span data-ttu-id="c0f12-110">[ConversationId](conversationid.md) | [SyncState (base64Binary)](syncstate-base64binary.md)</span><span class="sxs-lookup"><span data-stu-id="c0f12-110">[ConversationId](conversationid.md) | [SyncState (base64Binary)](syncstate-base64binary.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c0f12-111">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="c0f12-111">Parent elements</span></span>

[<span data-ttu-id="c0f12-112">Conversations</span><span class="sxs-lookup"><span data-stu-id="c0f12-112">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
## <a name="remarks"></a><span data-ttu-id="c0f12-113">Remarques</span><span class="sxs-lookup"><span data-stu-id="c0f12-113">Remarks</span></span>

<span data-ttu-id="c0f12-114">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="c0f12-114">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="c0f12-115">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="c0f12-115">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c0f12-116">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="c0f12-116">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c0f12-117">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="c0f12-117">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c0f12-118">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="c0f12-118">Schema name</span></span>  <br/> |<span data-ttu-id="c0f12-119">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="c0f12-119">Types schema</span></span>  <br/> |
|<span data-ttu-id="c0f12-120">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="c0f12-120">Validation file</span></span>  <br/> |<span data-ttu-id="c0f12-121">types.xsd</span><span class="sxs-lookup"><span data-stu-id="c0f12-121">types.xsd</span></span>  <br/> |
|<span data-ttu-id="c0f12-122">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="c0f12-122">Can be empty</span></span>  <br/> |<span data-ttu-id="c0f12-123">false</span><span class="sxs-lookup"><span data-stu-id="c0f12-123">false</span></span>  <br/> |
   

