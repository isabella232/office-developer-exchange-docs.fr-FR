---
title: État (HoldStatusType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fee3f1f9-e868-49fa-a554-7ff096964718
description: L’élément Status spécifie l’état de conservation pour une boîte aux lettres.
ms.openlocfilehash: c40dc865d2b305ac86fa40d536e2d516a14260ab
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829579"
---
# <a name="status-holdstatustype"></a><span data-ttu-id="b59b8-103">État (HoldStatusType)</span><span class="sxs-lookup"><span data-stu-id="b59b8-103">Status (HoldStatusType)</span></span>

<span data-ttu-id="b59b8-104">L’élément **Status** Spécifie l’état de conservation pour une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="b59b8-104">The **Status** element specifies the hold status for a mailbox.</span></span> 
  
```XML
<Status> NotOnHold | Pending | OnHold | PartialHold | Failed </Status>
```

 <span data-ttu-id="b59b8-105">**HoldStatusType**</span><span class="sxs-lookup"><span data-stu-id="b59b8-105">**HoldStatusType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b59b8-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="b59b8-106">Attributes and elements</span></span>

<span data-ttu-id="b59b8-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="b59b8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b59b8-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="b59b8-108">Attributes</span></span>

<span data-ttu-id="b59b8-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b59b8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b59b8-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="b59b8-110">Child elements</span></span>

<span data-ttu-id="b59b8-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b59b8-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b59b8-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="b59b8-112">Parent elements</span></span>

[<span data-ttu-id="b59b8-113">MailboxHoldStatus</span><span class="sxs-lookup"><span data-stu-id="b59b8-113">MailboxHoldStatus</span></span>](mailboxholdstatus.md)
  
## <a name="text-value"></a><span data-ttu-id="b59b8-114">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="b59b8-114">Text value</span></span>

<span data-ttu-id="b59b8-115">La valeur de texte de l’élément **Status** est l’état de conservation d’une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="b59b8-115">The text value of the **Status** element is the hold status of a mailbox.</span></span> <span data-ttu-id="b59b8-116">L’élément **Status** peut avoir les valeurs dans la liste suivante.</span><span class="sxs-lookup"><span data-stu-id="b59b8-116">The **Status** element can have the values in the following list.</span></span> 
  
> <span data-ttu-id="b59b8-117">NotOnHold - la boîte aux lettres n’est pas en attente.</span><span class="sxs-lookup"><span data-stu-id="b59b8-117">NotOnHold - The mailbox is not on hold.</span></span>
    
> <span data-ttu-id="b59b8-118">En attente - la boîte aux lettres est en attente d’être placé soit publié en attente.</span><span class="sxs-lookup"><span data-stu-id="b59b8-118">Pending - The mailbox is pending either being placed or released on hold.</span></span> 
    
> <span data-ttu-id="b59b8-119">En attente - la suspension a été appliqué à la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="b59b8-119">OnHold - The hold was successfully applied to the mailbox.</span></span> 
    
> <span data-ttu-id="b59b8-120">PartialHold - la suspension a été appliqué à des boîtes aux lettres, mais pas pour toutes les boîtes aux lettres.</span><span class="sxs-lookup"><span data-stu-id="b59b8-120">PartialHold - The hold was successfully applied to some mailboxes but not to all mailboxes.</span></span>
    
> <span data-ttu-id="b59b8-121">Échec - Échec de la suspension à appliquer à la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="b59b8-121">Failed - The hold failed to apply to the mailbox.</span></span>
    
## <a name="remarks"></a><span data-ttu-id="b59b8-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="b59b8-122">Remarks</span></span>

<span data-ttu-id="b59b8-123">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="b59b8-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b59b8-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="b59b8-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b59b8-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="b59b8-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b59b8-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="b59b8-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b59b8-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="b59b8-127">Schema name</span></span>  <br/> |<span data-ttu-id="b59b8-128">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="b59b8-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="b59b8-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="b59b8-129">Validation file</span></span>  <br/> |<span data-ttu-id="b59b8-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b59b8-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b59b8-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="b59b8-131">Can be empty</span></span>  <br/> ||
   

