---
title: FailedMailboxes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f34fb6f6-057e-4ae3-8e10-bc92112eafba
description: L’élément FailedMailboxes spécifie un tableau de boîtes aux lettres ayant échoué sur la recherche.
ms.openlocfilehash: f68cc29dc9da3b1b74369aa21cde65866e42f3b8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756347"
---
# <a name="failedmailboxes"></a><span data-ttu-id="e7acd-103">FailedMailboxes</span><span class="sxs-lookup"><span data-stu-id="e7acd-103">FailedMailboxes</span></span>

<span data-ttu-id="e7acd-104">L’élément **FailedMailboxes** spécifie un tableau de boîtes aux lettres ayant échoué sur la recherche.</span><span class="sxs-lookup"><span data-stu-id="e7acd-104">The **FailedMailboxes** element specifies an array of mailboxes that failed on search.</span></span> 
  
```XML
<FailedMailboxes>
    <FailedMailbox/>
<FailedMailboxes>
```

 <span data-ttu-id="e7acd-105">**ArrayOfFailedSearchMailboxesType**</span><span class="sxs-lookup"><span data-stu-id="e7acd-105">**ArrayOfFailedSearchMailboxesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e7acd-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="e7acd-106">Attributes and elements</span></span>

<span data-ttu-id="e7acd-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="e7acd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e7acd-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="e7acd-108">Attributes</span></span>

<span data-ttu-id="e7acd-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="e7acd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e7acd-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="e7acd-110">Child elements</span></span>

|<span data-ttu-id="e7acd-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e7acd-111">**Element**</span></span>|<span data-ttu-id="e7acd-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="e7acd-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e7acd-113">FailedMailbox</span><span class="sxs-lookup"><span data-stu-id="e7acd-113">FailedMailbox</span></span>](failedmailbox.md) <br/> |<span data-ttu-id="e7acd-114">Spécifie le message d’erreur pour une boîte aux lettres ayant échoué sur la recherche.</span><span class="sxs-lookup"><span data-stu-id="e7acd-114">Specifies the error message for a mailbox that failed on search.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e7acd-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="e7acd-115">Parent elements</span></span>

|<span data-ttu-id="e7acd-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e7acd-116">**Element**</span></span>|<span data-ttu-id="e7acd-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="e7acd-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e7acd-118">SearchMailboxesResult</span><span class="sxs-lookup"><span data-stu-id="e7acd-118">SearchMailboxesResult</span></span>](searchmailboxesresult.md) <br/> |<span data-ttu-id="e7acd-119">Contient le résultat de la demande **SearchMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="e7acd-119">Contains the result of the **SearchMailboxes** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e7acd-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="e7acd-120">Remarks</span></span>

<span data-ttu-id="e7acd-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="e7acd-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e7acd-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="e7acd-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e7acd-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="e7acd-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e7acd-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="e7acd-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e7acd-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="e7acd-125">Schema Name</span></span>  <br/> |<span data-ttu-id="e7acd-126">Schéma type</span><span class="sxs-lookup"><span data-stu-id="e7acd-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="e7acd-127">Validation File</span><span class="sxs-lookup"><span data-stu-id="e7acd-127">Validation File</span></span>  <br/> |<span data-ttu-id="e7acd-128">types.xsd</span><span class="sxs-lookup"><span data-stu-id="e7acd-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="e7acd-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="e7acd-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="e7acd-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e7acd-130">See also</span></span>



- [<span data-ttu-id="e7acd-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="e7acd-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

