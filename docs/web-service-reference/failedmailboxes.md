---
title: FailedMailboxes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f34fb6f6-057e-4ae3-8e10-bc92112eafba
description: L’élément FailedMailboxes spécifie un tableau de boîtes aux lettres ayant échoué lors de la recherche.
ms.openlocfilehash: 10f10d3f2ac4379d7ddcb3a13019d17a17bb676a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461953"
---
# <a name="failedmailboxes"></a><span data-ttu-id="083c7-103">FailedMailboxes</span><span class="sxs-lookup"><span data-stu-id="083c7-103">FailedMailboxes</span></span>

<span data-ttu-id="083c7-104">L’élément **FailedMailboxes** spécifie un tableau de boîtes aux lettres ayant échoué lors de la recherche.</span><span class="sxs-lookup"><span data-stu-id="083c7-104">The **FailedMailboxes** element specifies an array of mailboxes that failed on search.</span></span> 
  
```XML
<FailedMailboxes>
    <FailedMailbox/>
<FailedMailboxes>
```

 <span data-ttu-id="083c7-105">**ArrayOfFailedSearchMailboxesType**</span><span class="sxs-lookup"><span data-stu-id="083c7-105">**ArrayOfFailedSearchMailboxesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="083c7-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="083c7-106">Attributes and elements</span></span>

<span data-ttu-id="083c7-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="083c7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="083c7-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="083c7-108">Attributes</span></span>

<span data-ttu-id="083c7-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="083c7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="083c7-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="083c7-110">Child elements</span></span>

|<span data-ttu-id="083c7-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="083c7-111">**Element**</span></span>|<span data-ttu-id="083c7-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="083c7-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="083c7-113">FailedMailbox</span><span class="sxs-lookup"><span data-stu-id="083c7-113">FailedMailbox</span></span>](failedmailbox.md) <br/> |<span data-ttu-id="083c7-114">Spécifie le message d’erreur pour une boîte aux lettres ayant échoué lors de la recherche.</span><span class="sxs-lookup"><span data-stu-id="083c7-114">Specifies the error message for a mailbox that failed on search.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="083c7-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="083c7-115">Parent elements</span></span>

|<span data-ttu-id="083c7-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="083c7-116">**Element**</span></span>|<span data-ttu-id="083c7-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="083c7-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="083c7-118">SearchMailboxesResult</span><span class="sxs-lookup"><span data-stu-id="083c7-118">SearchMailboxesResult</span></span>](searchmailboxesresult.md) <br/> |<span data-ttu-id="083c7-119">Contient le résultat de la demande **SearchMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="083c7-119">Contains the result of the **SearchMailboxes** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="083c7-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="083c7-120">Remarks</span></span>

<span data-ttu-id="083c7-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="083c7-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="083c7-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="083c7-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="083c7-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="083c7-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="083c7-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="083c7-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="083c7-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="083c7-125">Schema Name</span></span>  <br/> |<span data-ttu-id="083c7-126">Schéma type</span><span class="sxs-lookup"><span data-stu-id="083c7-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="083c7-127">Validation File</span><span class="sxs-lookup"><span data-stu-id="083c7-127">Validation File</span></span>  <br/> |<span data-ttu-id="083c7-128">types. xsd</span><span class="sxs-lookup"><span data-stu-id="083c7-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="083c7-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="083c7-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="083c7-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="083c7-130">See also</span></span>



- [<span data-ttu-id="083c7-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="083c7-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

