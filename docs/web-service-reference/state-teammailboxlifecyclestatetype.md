---
title: État (TeamMailboxLifecycleStateType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3b1bc531-6988-41c3-9aad-3f5ad5b732a9
description: L’élément State contient l’état du cycle de vie qui est défini sur une boîte aux lettres de site.
ms.openlocfilehash: 597946b48649d997f8dd57823b4e0fcc091a6f84
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465162"
---
# <a name="state-teammailboxlifecyclestatetype"></a><span data-ttu-id="a0885-103">État (TeamMailboxLifecycleStateType)</span><span class="sxs-lookup"><span data-stu-id="a0885-103">State (TeamMailboxLifecycleStateType)</span></span>

<span data-ttu-id="a0885-104">L’élément **State** contient l’état du cycle de vie qui est défini sur une boîte aux lettres de site.</span><span class="sxs-lookup"><span data-stu-id="a0885-104">The **State** element contains the lifecycle state that is set on a site mailbox.</span></span> 
  
```XML
<State> Active | Closed | Unlinked | PendingDelete </State>
```

<span data-ttu-id="a0885-105">**TeamMailboxLifecycleStateType**</span><span class="sxs-lookup"><span data-stu-id="a0885-105">**TeamMailboxLifecycleStateType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="a0885-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a0885-106">Attributes and elements</span></span>

<span data-ttu-id="a0885-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a0885-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a0885-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="a0885-108">Attributes</span></span>

<span data-ttu-id="a0885-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="a0885-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a0885-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a0885-110">Child elements</span></span>

<span data-ttu-id="a0885-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a0885-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a0885-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a0885-112">Parent elements</span></span>

[<span data-ttu-id="a0885-113">SetTeamMailbox</span><span class="sxs-lookup"><span data-stu-id="a0885-113">SetTeamMailbox</span></span>](setteammailbox.md)
  
## <a name="text-value"></a><span data-ttu-id="a0885-114">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="a0885-114">Text value</span></span>

<span data-ttu-id="a0885-115">La valeur de texte de l’élément **State** est l’état de cycle de vie défini sur une boîte aux lettres de site.</span><span class="sxs-lookup"><span data-stu-id="a0885-115">The text value of the **State** element is the lifecycle state that is set on a site mailbox.</span></span> <span data-ttu-id="a0885-116">Une valeur de texte **active** indique qu’une boîte aux lettres de site est en cours d’utilisation.</span><span class="sxs-lookup"><span data-stu-id="a0885-116">A text value of **Active** indicates that a site mailbox is in active use.</span></span> <span data-ttu-id="a0885-117">Une valeur de texte **fermé** indique qu’une boîte aux lettres de site a été fermée et qu’elle n’est pas en cours d’utilisation.</span><span class="sxs-lookup"><span data-stu-id="a0885-117">A text value of **Closed** indicates that a site mailbox has been closed and is not in active use.</span></span> <span data-ttu-id="a0885-118">Une valeur de texte non **liée indique qu'** une boîte aux lettres de site n’est pas liée à un environnement de collaboration Web.</span><span class="sxs-lookup"><span data-stu-id="a0885-118">A text value of **Unlinked** indicates that a site mailbox is not linked to a web-based collaboration environment.</span></span> <span data-ttu-id="a0885-119">Les valeurs **active**, **Closed**et **PendingDelete** s’excluent mutuellement, mais la valeur non **liée** n’est pas mutuellement exclusive par les autres valeurs.</span><span class="sxs-lookup"><span data-stu-id="a0885-119">The **Active**, **Closed**, and **PendingDelete** values are mutually exclusive, but the **Unlinked** value is not mutually exclusive of the other values.</span></span> <span data-ttu-id="a0885-120">Une valeur de texte de **PendingDelete** indique qu’une boîte aux lettres de site est en attente de suppression.</span><span class="sxs-lookup"><span data-stu-id="a0885-120">A text value of **PendingDelete** indicates that a site mailbox is pending deletion.</span></span> <span data-ttu-id="a0885-121">Une boîte aux lettres de site doit être fermée pour pouvoir être définie comme **PendingDelete**.</span><span class="sxs-lookup"><span data-stu-id="a0885-121">A site mailbox has to be closed before it can be set as **PendingDelete**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a0885-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="a0885-122">Remarks</span></span>

<span data-ttu-id="a0885-123">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="a0885-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="a0885-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="a0885-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a0885-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a0885-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a0885-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a0885-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a0885-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a0885-127">Schema name</span></span>  <br/> |<span data-ttu-id="a0885-128">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="a0885-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a0885-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="a0885-129">Validation file</span></span>  <br/> |<span data-ttu-id="a0885-130">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="a0885-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a0885-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a0885-131">Can be empty</span></span>  <br/> ||
   

