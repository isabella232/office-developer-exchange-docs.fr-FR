---
title: GetConversationItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4f7bcd0f-140c-4cbc-a5ed-daeffded1df1
description: L’élément GetConversationItems définit une demande pour obtenir un ensemble d’éléments liés par le fait d’être dans la même conversation.
ms.openlocfilehash: cde4bc2c39ccbc51b7436c87c4bc06e3b8d7e52c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457745"
---
# <a name="getconversationitems"></a><span data-ttu-id="997c8-103">GetConversationItems</span><span class="sxs-lookup"><span data-stu-id="997c8-103">GetConversationItems</span></span>

<span data-ttu-id="997c8-104">L’élément **GetConversationItems** définit une demande pour obtenir un ensemble d’éléments liés par le fait d’être dans la même conversation.</span><span class="sxs-lookup"><span data-stu-id="997c8-104">The **GetConversationItems** element defines a request to get a set of items that are related by being in the same conversation.</span></span> 
  
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

 <span data-ttu-id="997c8-105">**GetConversationItemsType**</span><span class="sxs-lookup"><span data-stu-id="997c8-105">**GetConversationItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="997c8-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="997c8-106">Attributes and elements</span></span>

<span data-ttu-id="997c8-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="997c8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="997c8-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="997c8-108">Attributes</span></span>

<span data-ttu-id="997c8-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="997c8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="997c8-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="997c8-110">Child elements</span></span>

<span data-ttu-id="997c8-111">[ItemShape](itemshape.md)  |  [FoldersToIgnore](folderstoignore.md)  |  [MaxItemsToReturn](maxitemstoreturn.md)  |  [OrdreTri (ConversationNodeSortOrder)](sortorder-conversationnodesortorder.md)  |  [MailboxScope](mailboxscope.md)  |  [Conversations](conversations-ex15websvcsotherref.md)</span><span class="sxs-lookup"><span data-stu-id="997c8-111">[ItemShape](itemshape.md) | [FoldersToIgnore](folderstoignore.md) | [MaxItemsToReturn](maxitemstoreturn.md) | [SortOrder (ConversationNodeSortOrder)](sortorder-conversationnodesortorder.md) | [MailboxScope](mailboxscope.md) | [Conversations](conversations-ex15websvcsotherref.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="997c8-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="997c8-112">Parent elements</span></span>

<span data-ttu-id="997c8-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="997c8-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="997c8-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="997c8-114">Remarks</span></span>

<span data-ttu-id="997c8-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="997c8-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="997c8-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="997c8-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="997c8-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="997c8-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="997c8-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="997c8-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="997c8-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="997c8-119">Schema name</span></span>  <br/> |<span data-ttu-id="997c8-120">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="997c8-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="997c8-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="997c8-121">Validation file</span></span>  <br/> |<span data-ttu-id="997c8-122">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="997c8-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="997c8-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="997c8-123">Can be empty</span></span>  <br/> |<span data-ttu-id="997c8-124">false</span><span class="sxs-lookup"><span data-stu-id="997c8-124">false</span></span>  <br/> |
   

