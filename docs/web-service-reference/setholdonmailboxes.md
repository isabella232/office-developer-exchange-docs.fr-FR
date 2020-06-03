---
title: SetHoldOnMailboxes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fd5b9f0e-23e8-428c-8168-2d6b4ecd6beb
description: L’élément SetHoldOnMailboxes contient une requête SetHoldOnMailboxes.
ms.openlocfilehash: c96ff50cb1204d86abc66829e1c5da7124f407f1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44448351"
---
# <a name="setholdonmailboxes"></a><span data-ttu-id="4d8f0-103">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="4d8f0-103">SetHoldOnMailboxes</span></span>

<span data-ttu-id="4d8f0-104">L’élément **SetHoldOnMailboxes** contient une requête **SetHoldOnMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="4d8f0-104">The **SetHoldOnMailboxes** element contains a **SetHoldOnMailboxes** request.</span></span> 
  
```XML
<SetHoldOnMailboxes>
   <ActionType/>
   <HoldId/>
   <Query/>
   <Mailboxes/>
   <Language/>
   <IncludeNonIndexableItems/>
   <Deduplication/>
   <InPlaceHoldIdentity/>
</SetHoldOnMailboxes>
```

 <span data-ttu-id="4d8f0-105">**SetHoldOnMailboxesType**</span><span class="sxs-lookup"><span data-stu-id="4d8f0-105">**SetHoldOnMailboxesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4d8f0-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="4d8f0-106">Attributes and elements</span></span>

<span data-ttu-id="4d8f0-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="4d8f0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4d8f0-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="4d8f0-108">Attributes</span></span>

<span data-ttu-id="4d8f0-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="4d8f0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4d8f0-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="4d8f0-110">Child elements</span></span>

<span data-ttu-id="4d8f0-111">[ActionType (HoldActionType)](actiontype-holdactiontype.md)  |  [HoldId](holdid.md)  |  [Requête](query.md)  |  [Boîtes aux lettres (ArrayOfStringsType)](mailboxes-arrayofstringstype.md)  |  [Langue](language.md)  |  [IncludeNonIndexableItems](includenonindexableitems.md)  |  [Déduplication](deduplication.md)  |  [InPlaceHoldIdentity](inplaceholdidentity.md)</span><span class="sxs-lookup"><span data-stu-id="4d8f0-111">[ActionType (HoldActionType)](actiontype-holdactiontype.md) | [HoldId](holdid.md) | [Query](query.md) | [Mailboxes (ArrayOfStringsType)](mailboxes-arrayofstringstype.md) | [Language](language.md) | [IncludeNonIndexableItems](includenonindexableitems.md) | [Deduplication](deduplication.md) | [InPlaceHoldIdentity](inplaceholdidentity.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4d8f0-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="4d8f0-112">Parent elements</span></span>

<span data-ttu-id="4d8f0-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="4d8f0-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4d8f0-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="4d8f0-114">Remarks</span></span>

<span data-ttu-id="4d8f0-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="4d8f0-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="4d8f0-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="4d8f0-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4d8f0-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="4d8f0-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4d8f0-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="4d8f0-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4d8f0-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="4d8f0-119">Schema name</span></span>  <br/> |<span data-ttu-id="4d8f0-120">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="4d8f0-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4d8f0-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="4d8f0-121">Validation file</span></span>  <br/> |<span data-ttu-id="4d8f0-122">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="4d8f0-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4d8f0-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="4d8f0-123">Can be empty</span></span>  <br/> ||
   

