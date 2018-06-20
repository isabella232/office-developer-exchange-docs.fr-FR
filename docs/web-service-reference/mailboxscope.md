---
title: MailboxScope
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c9778823-f290-4827-ba19-5f391ed4f877
description: L’élément MailboxScope indique si une recherche ou extraction d’une conversation doit s’étendent à la boîte aux lettres principale, boîte aux lettres d’archivage ou à la fois le serveur principal et d’archivage de boîte aux lettres.
ms.openlocfilehash: 89c9776079d686b114d6b744150f1c6df3711eab
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828293"
---
# <a name="mailboxscope"></a><span data-ttu-id="757af-103">MailboxScope</span><span class="sxs-lookup"><span data-stu-id="757af-103">MailboxScope</span></span>

<span data-ttu-id="757af-104">L’élément **MailboxScope** indique si une recherche ou extraction d’une conversation doit s’étendent à la boîte aux lettres principale, boîte aux lettres d’archivage ou à la fois le serveur principal et d’archivage de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="757af-104">The **MailboxScope** element identifies whether a search or fetch for a conversation should span either the primary mailbox, archive mailbox, or both the primary and archive mailbox.</span></span> 
  
```XML
<MailboxScope> PrimaryOnly | ArchiveOnly | All </MailboxScope>
```

<span data-ttu-id="757af-105">**MailboxSearchLocationType**</span><span class="sxs-lookup"><span data-stu-id="757af-105">**MailboxSearchLocationType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="757af-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="757af-106">Attributes and elements</span></span>

<span data-ttu-id="757af-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="757af-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="757af-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="757af-108">Attributes</span></span>

<span data-ttu-id="757af-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="757af-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="757af-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="757af-110">Child elements</span></span>

<span data-ttu-id="757af-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="757af-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="757af-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="757af-112">Parent elements</span></span>

<span data-ttu-id="757af-113">[FindConversation](findconversation.md) | [GetConversationItems](getconversationitems.md) | [Conversation (ConversationType)](conversation-conversationtype.md)</span><span class="sxs-lookup"><span data-stu-id="757af-113">[FindConversation](findconversation.md) | [GetConversationItems](getconversationitems.md) | [Conversation (ConversationType)](conversation-conversationtype.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="757af-114">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="757af-114">Text value</span></span>

<span data-ttu-id="757af-115">La valeur de texte de l’élément **MailboxScope** est l’étendue de recherche ou de l’obtention d’éléments dans une conversation entre deux boîtes aux lettres principales, archiver des boîtes aux lettres ou les deux principal et archiver des boîtes aux lettres.</span><span class="sxs-lookup"><span data-stu-id="757af-115">The text value of the **MailboxScope** element is the scope for finding or getting items in a conversation across either primary mailboxes, archive mailboxes, or both primary and archive mailboxes.</span></span> <span data-ttu-id="757af-116">La valeur texte **PrimaryOnly** indique une étendue qui cible la boîte aux lettres principale pour un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="757af-116">A text value of **PrimaryOnly** indicates a scope that targets the primary mailbox for a user.</span></span> <span data-ttu-id="757af-117">La valeur texte **ArchiveOnly** indique une étendue qui cible la boîte aux lettres d’archivage pour un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="757af-117">A text value of **ArchiveOnly** indicates a scope that targets the archive mailbox for a user.</span></span> <span data-ttu-id="757af-118">Une valeur de texte de **toutes les** indique une étendue qui cible la boîte aux lettres principale et la boîte aux lettres d’archive.</span><span class="sxs-lookup"><span data-stu-id="757af-118">A text value of **All** indicates a scope that targets both the primary mailbox and archive mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="757af-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="757af-119">Remarks</span></span>

<span data-ttu-id="757af-120">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="757af-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="757af-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="757af-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="757af-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="757af-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="757af-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="757af-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="757af-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="757af-124">Schema name</span></span>  <br/> |<span data-ttu-id="757af-125">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="757af-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="757af-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="757af-126">Validation file</span></span>  <br/> |<span data-ttu-id="757af-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="757af-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="757af-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="757af-128">Can be empty</span></span>  <br/> |<span data-ttu-id="757af-129">false</span><span class="sxs-lookup"><span data-stu-id="757af-129">false</span></span>  <br/> |
   

