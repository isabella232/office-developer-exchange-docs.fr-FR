---
title: GetNonIndexableItemDetails
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ce3994c1-3bb4-4571-b026-34a6c5705410
description: L’élément GetNonIndexableItemDetails spécifie une requête pour récupérer les détails de l’élément nonindexable.
ms.openlocfilehash: 0aeda85973aa78eff240a017db58ffb57fc0de06
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756676"
---
# <a name="getnonindexableitemdetails"></a><span data-ttu-id="88da1-103">GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="88da1-103">GetNonIndexableItemDetails</span></span>

<span data-ttu-id="88da1-104">L’élément **GetNonIndexableItemDetails** spécifie une requête pour récupérer les détails de l’élément nonindexable.</span><span class="sxs-lookup"><span data-stu-id="88da1-104">The **GetNonIndexableItemDetails** element specifies a request to retrieve nonindexable item details.</span></span> 
  
```XML
<GetNonIndexableItemDetails>
    <Mailboxes/>
    <PageSize/>
    <PageItemReference/>
    <PageDirection/>
</GetNonIndexableItemDetails>
```

 <span data-ttu-id="88da1-105">**GetNonIndexableItemDetailsType**</span><span class="sxs-lookup"><span data-stu-id="88da1-105">**GetNonIndexableItemDetailsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="88da1-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="88da1-106">Attributes and elements</span></span>

<span data-ttu-id="88da1-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="88da1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="88da1-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="88da1-108">Attributes</span></span>

<span data-ttu-id="88da1-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="88da1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="88da1-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="88da1-110">Child elements</span></span>

|<span data-ttu-id="88da1-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="88da1-111">**Element**</span></span>|<span data-ttu-id="88da1-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="88da1-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="88da1-113">Boîtes aux lettres (NonEmptyArrayOfLegacyDNsType)</span><span class="sxs-lookup"><span data-stu-id="88da1-113">Mailboxes (NonEmptyArrayOfLegacyDNsType)</span></span>](mailboxes-nonemptyarrayoflegacydnstype.md) <br/> |<span data-ttu-id="88da1-114">Spécifie un tableau d’éléments de **boîte aux lettres** .</span><span class="sxs-lookup"><span data-stu-id="88da1-114">Specifies an array of **Mailbox** elements.</span></span>  <br/> |
|[<span data-ttu-id="88da1-115">PageSize</span><span class="sxs-lookup"><span data-stu-id="88da1-115">PageSize</span></span>](pagesize.md) <br/> |<span data-ttu-id="88da1-116">Contient le nombre d’éléments à renvoyer dans une seule page pour un résultat de recherche.</span><span class="sxs-lookup"><span data-stu-id="88da1-116">Contains the number of items to be returned in a single page for a search result.</span></span>  <br/> |
|[<span data-ttu-id="88da1-117">PageItemReference</span><span class="sxs-lookup"><span data-stu-id="88da1-117">PageItemReference</span></span>](pageitemreference.md) <br/> |<span data-ttu-id="88da1-118">Spécifie la référence pour un élément de page.</span><span class="sxs-lookup"><span data-stu-id="88da1-118">Specifies the reference for a page item.</span></span>  <br/> |
|[<span data-ttu-id="88da1-119">PageDirection</span><span class="sxs-lookup"><span data-stu-id="88da1-119">PageDirection</span></span>](pagedirection.md) <br/> |<span data-ttu-id="88da1-120">Indique la direction de la pagination dans le résultat de recherche.</span><span class="sxs-lookup"><span data-stu-id="88da1-120">Contains the direction for pagination in the search result.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="88da1-121">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="88da1-121">Parent elements</span></span>

<span data-ttu-id="88da1-122">Aucun.</span><span class="sxs-lookup"><span data-stu-id="88da1-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="88da1-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="88da1-123">Remarks</span></span>

<span data-ttu-id="88da1-124">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="88da1-124">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="88da1-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="88da1-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="88da1-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="88da1-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="88da1-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="88da1-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="88da1-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="88da1-128">Schema Name</span></span>  <br/> |<span data-ttu-id="88da1-129">Schéma des messages</span><span class="sxs-lookup"><span data-stu-id="88da1-129">Message schema</span></span>  <br/> |
|<span data-ttu-id="88da1-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="88da1-130">Validation File</span></span>  <br/> |<span data-ttu-id="88da1-131">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="88da1-131">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="88da1-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="88da1-132">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="88da1-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="88da1-133">See also</span></span>



- [<span data-ttu-id="88da1-134">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="88da1-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

