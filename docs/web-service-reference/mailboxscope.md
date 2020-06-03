---
title: MailboxScope
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c9778823-f290-4827-ba19-5f391ed4f877
description: L’élément MailboxScope identifie si une recherche ou une récupération d’une conversation doit s’étendre sur la boîte aux lettres principale, la boîte aux lettres d’archivage ou les deux.
ms.openlocfilehash: 92823c06d4fe186917c3cfb532eda821bd6a95a7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455372"
---
# <a name="mailboxscope"></a><span data-ttu-id="915fe-103">MailboxScope</span><span class="sxs-lookup"><span data-stu-id="915fe-103">MailboxScope</span></span>

<span data-ttu-id="915fe-104">L’élément **MailboxScope** identifie si une recherche ou une récupération d’une conversation doit s’étendre sur la boîte aux lettres principale, la boîte aux lettres d’archivage ou les deux.</span><span class="sxs-lookup"><span data-stu-id="915fe-104">The **MailboxScope** element identifies whether a search or fetch for a conversation should span either the primary mailbox, archive mailbox, or both the primary and archive mailbox.</span></span> 
  
```XML
<MailboxScope> PrimaryOnly | ArchiveOnly | All </MailboxScope>
```

<span data-ttu-id="915fe-105">**MailboxSearchLocationType**</span><span class="sxs-lookup"><span data-stu-id="915fe-105">**MailboxSearchLocationType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="915fe-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="915fe-106">Attributes and elements</span></span>

<span data-ttu-id="915fe-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="915fe-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="915fe-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="915fe-108">Attributes</span></span>

<span data-ttu-id="915fe-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="915fe-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="915fe-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="915fe-110">Child elements</span></span>

<span data-ttu-id="915fe-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="915fe-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="915fe-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="915fe-112">Parent elements</span></span>

<span data-ttu-id="915fe-113">[FindConversation](findconversation.md)  |  [GetConversationItems](getconversationitems.md)  |  [Conversation (ConversationType)](conversation-conversationtype.md)</span><span class="sxs-lookup"><span data-stu-id="915fe-113">[FindConversation](findconversation.md) | [GetConversationItems](getconversationitems.md) | [Conversation (ConversationType)](conversation-conversationtype.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="915fe-114">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="915fe-114">Text value</span></span>

<span data-ttu-id="915fe-115">La valeur de texte de l’élément **MailboxScope** est la portée de la recherche ou de l’obtention d’éléments dans une conversation sur des boîtes aux lettres principales, des boîtes aux lettres d’archivage ou les boîtes aux lettres principales et d’archivage.</span><span class="sxs-lookup"><span data-stu-id="915fe-115">The text value of the **MailboxScope** element is the scope for finding or getting items in a conversation across either primary mailboxes, archive mailboxes, or both primary and archive mailboxes.</span></span> <span data-ttu-id="915fe-116">Une valeur de texte de **PrimaryOnly** indique une étendue qui cible la boîte aux lettres principale d’un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="915fe-116">A text value of **PrimaryOnly** indicates a scope that targets the primary mailbox for a user.</span></span> <span data-ttu-id="915fe-117">Une valeur de texte de **ArchiveOnly** indique une étendue qui cible la boîte aux lettres d’archivage d’un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="915fe-117">A text value of **ArchiveOnly** indicates a scope that targets the archive mailbox for a user.</span></span> <span data-ttu-id="915fe-118">Une valeur de texte de **All** indique une étendue qui cible à la fois la boîte aux lettres principale et la boîte aux lettres d’archivage.</span><span class="sxs-lookup"><span data-stu-id="915fe-118">A text value of **All** indicates a scope that targets both the primary mailbox and archive mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="915fe-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="915fe-119">Remarks</span></span>

<span data-ttu-id="915fe-120">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="915fe-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="915fe-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="915fe-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="915fe-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="915fe-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="915fe-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="915fe-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="915fe-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="915fe-124">Schema name</span></span>  <br/> |<span data-ttu-id="915fe-125">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="915fe-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="915fe-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="915fe-126">Validation file</span></span>  <br/> |<span data-ttu-id="915fe-127">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="915fe-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="915fe-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="915fe-128">Can be empty</span></span>  <br/> |<span data-ttu-id="915fe-129">false</span><span class="sxs-lookup"><span data-stu-id="915fe-129">false</span></span>  <br/> |
   

