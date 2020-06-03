---
title: SearchMailboxesResult
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ddb276c4-6c8a-46ef-a2eb-46b6a0bfce09
description: L’élément SearchMailboxesResult contient le résultat de la demande SearchMailboxes.
ms.openlocfilehash: 79d593d99762aedc6290578b5458f9ac3cad3d26
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466702"
---
# <a name="searchmailboxesresult"></a><span data-ttu-id="fa13e-103">SearchMailboxesResult</span><span class="sxs-lookup"><span data-stu-id="fa13e-103">SearchMailboxesResult</span></span>

<span data-ttu-id="fa13e-104">L’élément **SearchMailboxesResult** contient le résultat de la demande **SearchMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="fa13e-104">The **SearchMailboxesResult** element contains the result of the **SearchMailboxes** request.</span></span> 
  
```XML
<SearchMailboxesResult>
   <SearchQueries/>
   <ResultType/>
   <ItemCount/>
   <Size/>
   <PageItemCount/>
   <PageItemSize/>
   <KeywordStats/>
   <Items/>
   <FailedMailboxes/>
   <Refiners/>
   <MailboxStats/>
</SearchMailboxesResult>
```

 <span data-ttu-id="fa13e-105">**SearchMailboxesResultType**</span><span class="sxs-lookup"><span data-stu-id="fa13e-105">**SearchMailboxesResultType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fa13e-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="fa13e-106">Attributes and elements</span></span>

<span data-ttu-id="fa13e-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="fa13e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fa13e-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="fa13e-108">Attributes</span></span>

<span data-ttu-id="fa13e-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="fa13e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fa13e-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="fa13e-110">Child elements</span></span>

<span data-ttu-id="fa13e-111">[SearchQueries](searchqueries.md)  |  [ResultType](resulttype.md)  |  [ItemCount](itemcount.md)  |  [Taille (long)](size-long.md)  |  [PageItemCount](pageitemcount.md)  |  [PageItemSize](pageitemsize.md)  |  [KeywordStats](keywordstats.md)  |  [Items (ArrayOfSearchPreviewItemsType)](items-arrayofsearchpreviewitemstype.md)  |  [FailedMailboxes](failedmailboxes.md)  |  [Affinements](refiners.md)  |  [MailboxStats](mailboxstats.md)</span><span class="sxs-lookup"><span data-stu-id="fa13e-111">[SearchQueries](searchqueries.md) | [ResultType](resulttype.md) | [ItemCount](itemcount.md) | [Size (long)](size-long.md) | [PageItemCount](pageitemcount.md) | [PageItemSize](pageitemsize.md) | [KeywordStats](keywordstats.md) | [Items (ArrayOfSearchPreviewItemsType)](items-arrayofsearchpreviewitemstype.md) | [FailedMailboxes](failedmailboxes.md) | [Refiners](refiners.md) | [MailboxStats](mailboxstats.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fa13e-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="fa13e-112">Parent elements</span></span>

[<span data-ttu-id="fa13e-113">SearchMailboxesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="fa13e-113">SearchMailboxesResponseMessage</span></span>](searchmailboxesresponsemessage.md)
  
## <a name="remarks"></a><span data-ttu-id="fa13e-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="fa13e-114">Remarks</span></span>

<span data-ttu-id="fa13e-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="fa13e-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="fa13e-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="fa13e-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fa13e-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="fa13e-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fa13e-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="fa13e-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="fa13e-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="fa13e-119">Schema name</span></span>  <br/> |<span data-ttu-id="fa13e-120">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="fa13e-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="fa13e-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="fa13e-121">Validation file</span></span>  <br/> |<span data-ttu-id="fa13e-122">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="fa13e-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="fa13e-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="fa13e-123">Can be empty</span></span>  <br/> |<span data-ttu-id="fa13e-124">false</span><span class="sxs-lookup"><span data-stu-id="fa13e-124">false</span></span>  <br/> |
   

