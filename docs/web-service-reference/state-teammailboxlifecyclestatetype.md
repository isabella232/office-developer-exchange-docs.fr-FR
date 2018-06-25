---
title: État (TeamMailboxLifecycleStateType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3b1bc531-6988-41c3-9aad-3f5ad5b732a9
description: L’élément d’état contient l’état du cycle de vie est définie sur une boîte aux lettres du site.
ms.openlocfilehash: accd70d36cc34e7364387b98a2e94c56b91f012f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829571"
---
# <a name="state-teammailboxlifecyclestatetype"></a><span data-ttu-id="7e4bc-103">État (TeamMailboxLifecycleStateType)</span><span class="sxs-lookup"><span data-stu-id="7e4bc-103">State (TeamMailboxLifecycleStateType)</span></span>

<span data-ttu-id="7e4bc-104">L’élément **d’état** contient l’état du cycle de vie est définie sur une boîte aux lettres du site.</span><span class="sxs-lookup"><span data-stu-id="7e4bc-104">The **State** element contains the lifecycle state that is set on a site mailbox.</span></span> 
  
```XML
<State> Active | Closed | Unlinked | PendingDelete </State>
```

<span data-ttu-id="7e4bc-105">**TeamMailboxLifecycleStateType**</span><span class="sxs-lookup"><span data-stu-id="7e4bc-105">**TeamMailboxLifecycleStateType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="7e4bc-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="7e4bc-106">Attributes and elements</span></span>

<span data-ttu-id="7e4bc-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="7e4bc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7e4bc-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="7e4bc-108">Attributes</span></span>

<span data-ttu-id="7e4bc-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7e4bc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7e4bc-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="7e4bc-110">Child elements</span></span>

<span data-ttu-id="7e4bc-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7e4bc-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7e4bc-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="7e4bc-112">Parent elements</span></span>

[<span data-ttu-id="7e4bc-113">SetTeamMailbox</span><span class="sxs-lookup"><span data-stu-id="7e4bc-113">SetTeamMailbox</span></span>](setteammailbox.md)
  
## <a name="text-value"></a><span data-ttu-id="7e4bc-114">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="7e4bc-114">Text value</span></span>

<span data-ttu-id="7e4bc-115">La valeur de texte de l’élément **d’état** est l’état du cycle de vie est définie sur une boîte aux lettres du site.</span><span class="sxs-lookup"><span data-stu-id="7e4bc-115">The text value of the **State** element is the lifecycle state that is set on a site mailbox.</span></span> <span data-ttu-id="7e4bc-116">Une valeur texte **actif** indique qu’une boîte aux lettres du site est en cours d’utilisation.</span><span class="sxs-lookup"><span data-stu-id="7e4bc-116">A text value of **Active** indicates that a site mailbox is in active use.</span></span> <span data-ttu-id="7e4bc-117">Une valeur texte **fermé** indique qu’une boîte aux lettres de site a été fermée et n’est pas en cours d’utilisation.</span><span class="sxs-lookup"><span data-stu-id="7e4bc-117">A text value of **Closed** indicates that a site mailbox has been closed and is not in active use.</span></span> <span data-ttu-id="7e4bc-118">Une valeur texte **non liés** indique qu’une boîte aux lettres du site n’est pas liée à un environnement de collaboration basée sur le web.</span><span class="sxs-lookup"><span data-stu-id="7e4bc-118">A text value of **Unlinked** indicates that a site mailbox is not linked to a web-based collaboration environment.</span></span> <span data-ttu-id="7e4bc-119">Les valeurs **actives**, **fermé**et **PendingDelete** s’excluent mutuellement, mais la valeur **non liés** n’est pas mutuellement, sans compter les autres valeurs.</span><span class="sxs-lookup"><span data-stu-id="7e4bc-119">The **Active**, **Closed**, and **PendingDelete** values are mutually exclusive, but the **Unlinked** value is not mutually exclusive of the other values.</span></span> <span data-ttu-id="7e4bc-120">Une valeur texte **PendingDelete** indique qu’une boîte aux lettres du site est en attente de suppression.</span><span class="sxs-lookup"><span data-stu-id="7e4bc-120">A text value of **PendingDelete** indicates that a site mailbox is pending deletion.</span></span> <span data-ttu-id="7e4bc-121">Une boîte aux lettres de site doit être fermé avant qu’il peut être définie en tant que **PendingDelete**.</span><span class="sxs-lookup"><span data-stu-id="7e4bc-121">A site mailbox has to be closed before it can be set as **PendingDelete**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7e4bc-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="7e4bc-122">Remarks</span></span>

<span data-ttu-id="7e4bc-123">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="7e4bc-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="7e4bc-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="7e4bc-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7e4bc-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="7e4bc-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7e4bc-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="7e4bc-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7e4bc-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="7e4bc-127">Schema name</span></span>  <br/> |<span data-ttu-id="7e4bc-128">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="7e4bc-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7e4bc-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="7e4bc-129">Validation file</span></span>  <br/> |<span data-ttu-id="7e4bc-130">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="7e4bc-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7e4bc-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="7e4bc-131">Can be empty</span></span>  <br/> ||
   

