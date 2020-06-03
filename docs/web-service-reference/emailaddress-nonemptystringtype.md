---
title: EmailAddress (NonEmptyStringType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- EmailAddress
api_type:
- schema
ms.assetid: c0c708d1-b016-4902-a294-9af44aea2050
description: L’élément EmailAddress définit l’adresse SMTP principale d’un utilisateur de boîte aux lettres.
ms.openlocfilehash: fcc3e650d5fc32344022ed6f015d4096a4461f63
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463131"
---
# <a name="emailaddress-nonemptystringtype"></a><span data-ttu-id="2611a-103">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="2611a-103">EmailAddress (NonEmptyStringType)</span></span>

<span data-ttu-id="2611a-104">L’élément **EmailAddress** définit l’adresse SMTP principale d’un utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="2611a-104">The **EmailAddress** element defines the primary SMTP address of a mailbox user.</span></span> 
  
```XML
<EmailAddress/>
```

 <span data-ttu-id="2611a-105">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="2611a-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2611a-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="2611a-106">Attributes and elements</span></span>

<span data-ttu-id="2611a-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="2611a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2611a-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="2611a-108">Attributes</span></span>

<span data-ttu-id="2611a-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="2611a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2611a-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="2611a-110">Child elements</span></span>

<span data-ttu-id="2611a-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="2611a-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2611a-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="2611a-112">Parent elements</span></span>

|<span data-ttu-id="2611a-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2611a-113">**Element**</span></span>|<span data-ttu-id="2611a-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="2611a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2611a-115">Actionas</span><span class="sxs-lookup"><span data-stu-id="2611a-115">ActingAs</span></span>](actingas.md) <br/> |<span data-ttu-id="2611a-116">Identifie les personnes qui envoient l’appelant.</span><span class="sxs-lookup"><span data-stu-id="2611a-116">Identifies who the caller is sending as.</span></span>  <br/> |
|[<span data-ttu-id="2611a-117">Boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="2611a-117">Mailbox</span></span>](mailbox.md) <br/> | <span data-ttu-id="2611a-118">Identifie une adresse de messagerie entièrement résolue.</span><span class="sxs-lookup"><span data-stu-id="2611a-118">Identifies a fully resolved e-mail address.</span></span>  <br/><br/><span data-ttu-id="2611a-119">Voici quelques expressions XPath sur cet élément :</span><span class="sxs-lookup"><span data-stu-id="2611a-119">The following are some XPath expressions to this element:</span></span><br/><br/>`/CreateItem/ParentFolderId/DistinguishedFolderId/Mailbox`<br/><br/>`/CreateFolder/ParentFolderId/DistinguishedFolderId/Mailbox`<br/><br/>`CreateItem/Items/AcceptItem/ToRecipients/Mailbox`<br/><br/>`SyncFolderItemsResponseMessage/Changes/Create/CalendarItem/ConflictingMeetings/AcceptItem/CcRecipients/Mailbox`<br/><br/><span data-ttu-id="2611a-120">Les éléments suivants sont des éléments parents supplémentaires de l’élément Mailbox :</span><span class="sxs-lookup"><span data-stu-id="2611a-120">The following are additional parent elements of the Mailbox element:</span></span><br/><br/><span data-ttu-id="2611a-121">- [BccRecipients](bccrecipients.md)</span><span class="sxs-lookup"><span data-stu-id="2611a-121">- [BccRecipients](bccrecipients.md)</span></span> <br/><span data-ttu-id="2611a-122">- [ReplyTo](replyto.md)</span><span class="sxs-lookup"><span data-stu-id="2611a-122">- [ReplyTo](replyto.md)</span></span> <br/><span data-ttu-id="2611a-123">- [Expéditeur](sender.md)</span><span class="sxs-lookup"><span data-stu-id="2611a-123">- [Sender](sender.md)</span></span> <br/><span data-ttu-id="2611a-124">- [De](from.md)</span><span class="sxs-lookup"><span data-stu-id="2611a-124">- [From](from.md)</span></span> <br/><span data-ttu-id="2611a-125">- [Organiser](organizer.md)</span><span class="sxs-lookup"><span data-stu-id="2611a-125">- [Organizer](organizer.md)</span></span> <br/><span data-ttu-id="2611a-126">- [DistinguishedFolderId](distinguishedfolderid.md)</span><span class="sxs-lookup"><span data-stu-id="2611a-126">- [DistinguishedFolderId](distinguishedfolderid.md)</span></span> <br/><span data-ttu-id="2611a-127">- [Résolution](resolution.md)</span><span class="sxs-lookup"><span data-stu-id="2611a-127">- [Resolution](resolution.md)</span></span> <br/><span data-ttu-id="2611a-128">- [DLExpansion](dlexpansion.md)</span><span class="sxs-lookup"><span data-stu-id="2611a-128">- [DLExpansion](dlexpansion.md)</span></span> <br/><span data-ttu-id="2611a-129">- [Participant](attendee.md)</span><span class="sxs-lookup"><span data-stu-id="2611a-129">- [Attendee](attendee.md)</span></span> <br/> |
|[<span data-ttu-id="2611a-130">RoomList</span><span class="sxs-lookup"><span data-stu-id="2611a-130">RoomList</span></span>](roomlist.md) <br/> |<span data-ttu-id="2611a-131">Identifie une liste de salles de réunion par adresse de messagerie.</span><span class="sxs-lookup"><span data-stu-id="2611a-131">Identifies a list of meeting rooms by email address.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2611a-132">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="2611a-132">Text value</span></span>

<span data-ttu-id="2611a-133">Une valeur de texte qui représente une adresse SMTP est requise.</span><span class="sxs-lookup"><span data-stu-id="2611a-133">A text value that represents an SMTP address is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2611a-134">Remarques</span><span class="sxs-lookup"><span data-stu-id="2611a-134">Remarks</span></span>

<span data-ttu-id="2611a-135">L’élément **EmailAddress** peut représenter des adresses SMTP ou des noms uniques Exchange hérités (également appelés DN).</span><span class="sxs-lookup"><span data-stu-id="2611a-135">The **EmailAddress** element can represent SMTP or legacy Exchange distinguished name (also known as DN) addresses.</span></span> <span data-ttu-id="2611a-136">L’élément **EmailAddress** est le seul élément de [boîte aux lettres](mailbox.md) obligatoire.</span><span class="sxs-lookup"><span data-stu-id="2611a-136">The **EmailAddress** element is the only required [Mailbox](mailbox.md) element.</span></span> 
  
<span data-ttu-id="2611a-137">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="2611a-137">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2611a-138">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="2611a-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2611a-139">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="2611a-139">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2611a-140">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="2611a-140">Schema Name</span></span>  <br/> |<span data-ttu-id="2611a-141">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="2611a-141">Types schema</span></span>  <br/> |
|<span data-ttu-id="2611a-142">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="2611a-142">Validation File</span></span>  <br/> |<span data-ttu-id="2611a-143">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2611a-143">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2611a-144">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="2611a-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="2611a-145">False</span><span class="sxs-lookup"><span data-stu-id="2611a-145">False</span></span>  <br/> |
   

