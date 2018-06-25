---
title: GetConversationItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4f7bcd0f-140c-4cbc-a5ed-daeffded1df1
description: L’élément GetConversationItems définit une demande pour obtenir un ensemble d’éléments qui sont liés par en cours dans la même conversation.
ms.openlocfilehash: 9be300318a07173e4a8e11e5a6ca78b885de1199
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756548"
---
# <a name="getconversationitems"></a><span data-ttu-id="998be-103">GetConversationItems</span><span class="sxs-lookup"><span data-stu-id="998be-103">GetConversationItems</span></span>

<span data-ttu-id="998be-104">L’élément **GetConversationItems** définit une demande pour obtenir un ensemble d’éléments qui sont liés par en cours dans la même conversation.</span><span class="sxs-lookup"><span data-stu-id="998be-104">The **GetConversationItems** element defines a request to get a set of items that are related by being in the same conversation.</span></span> 
  
```XML
<GetConversationItems>
   <ItemShape/>
   <FoldersToIgnore/>
   <MaxItemsToReturn/>
   <SortOrder/>
   <MailboxScope/>
   <Conversations/>
</GetConversationItems>
```

 <span data-ttu-id="998be-105">**GetConversationItemsType**</span><span class="sxs-lookup"><span data-stu-id="998be-105">**GetConversationItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="998be-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="998be-106">Attributes and elements</span></span>

<span data-ttu-id="998be-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="998be-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="998be-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="998be-108">Attributes</span></span>

<span data-ttu-id="998be-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="998be-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="998be-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="998be-110">Child elements</span></span>

<span data-ttu-id="998be-111">[ItemShape](itemshape.md) | [FoldersToIgnore](folderstoignore.md) | [MaxItemsToReturn](maxitemstoreturn.md) | [SortOrder (ConversationNodeSortOrder)](sortorder-conversationnodesortorder.md) | [MailboxScope](mailboxscope.md) | [Conversations](conversations-ex15websvcsotherref.md)</span><span class="sxs-lookup"><span data-stu-id="998be-111">[ItemShape](itemshape.md) | [FoldersToIgnore](folderstoignore.md) | [MaxItemsToReturn](maxitemstoreturn.md) | [SortOrder (ConversationNodeSortOrder)](sortorder-conversationnodesortorder.md) | [MailboxScope](mailboxscope.md) | [Conversations](conversations-ex15websvcsotherref.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="998be-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="998be-112">Parent elements</span></span>

<span data-ttu-id="998be-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="998be-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="998be-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="998be-114">Remarks</span></span>

<span data-ttu-id="998be-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="998be-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="998be-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="998be-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="998be-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="998be-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="998be-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="998be-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="998be-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="998be-119">Schema name</span></span>  <br/> |<span data-ttu-id="998be-120">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="998be-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="998be-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="998be-121">Validation file</span></span>  <br/> |<span data-ttu-id="998be-122">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="998be-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="998be-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="998be-123">Can be empty</span></span>  <br/> |<span data-ttu-id="998be-124">false</span><span class="sxs-lookup"><span data-stu-id="998be-124">false</span></span>  <br/> |
   

