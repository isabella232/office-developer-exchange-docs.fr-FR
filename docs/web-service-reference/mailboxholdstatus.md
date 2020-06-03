---
title: MailboxHoldStatus
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 92608b77-8aa4-403b-a4de-01e3a60af3e0
description: L’élément MailboxHoldStatus spécifie l’état de conservation de la boîte aux lettres.
ms.openlocfilehash: 2ac575275fc00d2e3ba38cb4ec7335567ee82da6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468809"
---
# <a name="mailboxholdstatus"></a><span data-ttu-id="36626-103">MailboxHoldStatus</span><span class="sxs-lookup"><span data-stu-id="36626-103">MailboxHoldStatus</span></span>

<span data-ttu-id="36626-104">L’élément **MailboxHoldStatus** spécifie l’état de conservation de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="36626-104">The **MailboxHoldStatus** element specifies the hold status of the mailbox.</span></span> 
  
```XML
<MailboxHoldStatus>
   <Mailbox/>
   <Status/>
   <AdditionalInfo/>
</MailboxHoldStatus>
```

<span data-ttu-id="36626-105">**MailboxHoldStatusType**</span><span class="sxs-lookup"><span data-stu-id="36626-105">**MailboxHoldStatusType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="36626-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="36626-106">Attributes and elements</span></span>

<span data-ttu-id="36626-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="36626-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="36626-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="36626-108">Attributes</span></span>

<span data-ttu-id="36626-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="36626-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="36626-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="36626-110">Child elements</span></span>

<span data-ttu-id="36626-111">[Mailbox (String)](mailbox-string.md)  |  [État (HoldStatusType)](status-holdstatustype.md)  |  [AdditionalInfo](additionalinfo.md)</span><span class="sxs-lookup"><span data-stu-id="36626-111">[Mailbox (string)](mailbox-string.md) | [Status (HoldStatusType)](status-holdstatustype.md) | [AdditionalInfo](additionalinfo.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="36626-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="36626-112">Parent elements</span></span>

[<span data-ttu-id="36626-113">MailboxHoldStatuses</span><span class="sxs-lookup"><span data-stu-id="36626-113">MailboxHoldStatuses</span></span>](mailboxholdstatuses.md)
  
## <a name="remarks"></a><span data-ttu-id="36626-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="36626-114">Remarks</span></span>

<span data-ttu-id="36626-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="36626-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="36626-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="36626-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="36626-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="36626-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="36626-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="36626-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="36626-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="36626-119">Schema name</span></span>  <br/> |<span data-ttu-id="36626-120">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="36626-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="36626-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="36626-121">Validation file</span></span>  <br/> |<span data-ttu-id="36626-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="36626-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="36626-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="36626-123">Can be empty</span></span>  <br/> ||
   

