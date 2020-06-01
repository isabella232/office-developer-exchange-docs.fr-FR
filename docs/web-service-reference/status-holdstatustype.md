---
title: État (HoldStatusType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fee3f1f9-e868-49fa-a554-7ff096964718
description: L’élément Status spécifie l’état de conservation d’une boîte aux lettres.
ms.openlocfilehash: cecfdfaf67b00b6f8cf02188e7a4df7062a732e4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459986"
---
# <a name="status-holdstatustype"></a><span data-ttu-id="0de56-103">État (HoldStatusType)</span><span class="sxs-lookup"><span data-stu-id="0de56-103">Status (HoldStatusType)</span></span>

<span data-ttu-id="0de56-104">L’élément **Status** spécifie l’état de conservation d’une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="0de56-104">The **Status** element specifies the hold status for a mailbox.</span></span> 
  
```XML
<Status> NotOnHold | Pending | OnHold | PartialHold | Failed </Status>
```

 <span data-ttu-id="0de56-105">**HoldStatusType**</span><span class="sxs-lookup"><span data-stu-id="0de56-105">**HoldStatusType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0de56-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="0de56-106">Attributes and elements</span></span>

<span data-ttu-id="0de56-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="0de56-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0de56-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="0de56-108">Attributes</span></span>

<span data-ttu-id="0de56-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="0de56-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0de56-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="0de56-110">Child elements</span></span>

<span data-ttu-id="0de56-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="0de56-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0de56-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="0de56-112">Parent elements</span></span>

[<span data-ttu-id="0de56-113">MailboxHoldStatus</span><span class="sxs-lookup"><span data-stu-id="0de56-113">MailboxHoldStatus</span></span>](mailboxholdstatus.md)
  
## <a name="text-value"></a><span data-ttu-id="0de56-114">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="0de56-114">Text value</span></span>

<span data-ttu-id="0de56-115">La valeur de texte de l’élément **Status** est l’état de conservation d’une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="0de56-115">The text value of the **Status** element is the hold status of a mailbox.</span></span> <span data-ttu-id="0de56-116">L’élément **Status** peut avoir les valeurs répertoriées dans la liste suivante.</span><span class="sxs-lookup"><span data-stu-id="0de56-116">The **Status** element can have the values in the following list.</span></span> 
  
> <span data-ttu-id="0de56-117">NotOnHold-la boîte aux lettres n’est pas en attente.</span><span class="sxs-lookup"><span data-stu-id="0de56-117">NotOnHold - The mailbox is not on hold.</span></span>
    
> <span data-ttu-id="0de56-118">En attente : la boîte aux lettres est en attente d’être placée ou libérée en conservation.</span><span class="sxs-lookup"><span data-stu-id="0de56-118">Pending - The mailbox is pending either being placed or released on hold.</span></span> 
    
> <span data-ttu-id="0de56-119">OnHold-la suspension a été appliquée à la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="0de56-119">OnHold - The hold was successfully applied to the mailbox.</span></span> 
    
> <span data-ttu-id="0de56-120">PartialHold-la conservation a été appliquée avec succès à certaines boîtes aux lettres, mais pas à toutes les boîtes aux lettres.</span><span class="sxs-lookup"><span data-stu-id="0de56-120">PartialHold - The hold was successfully applied to some mailboxes but not to all mailboxes.</span></span>
    
> <span data-ttu-id="0de56-121">Failed : la conservation n’a pas pu s’appliquer à la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="0de56-121">Failed - The hold failed to apply to the mailbox.</span></span>
    
## <a name="remarks"></a><span data-ttu-id="0de56-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="0de56-122">Remarks</span></span>

<span data-ttu-id="0de56-123">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="0de56-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="0de56-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="0de56-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0de56-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="0de56-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0de56-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="0de56-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0de56-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="0de56-127">Schema name</span></span>  <br/> |<span data-ttu-id="0de56-128">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="0de56-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="0de56-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="0de56-129">Validation file</span></span>  <br/> |<span data-ttu-id="0de56-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0de56-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0de56-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="0de56-131">Can be empty</span></span>  <br/> ||
   

