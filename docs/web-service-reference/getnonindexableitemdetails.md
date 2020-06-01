---
title: GetNonIndexableItemDetails
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ce3994c1-3bb4-4571-b026-34a6c5705410
description: L’élément GetNonIndexableItemDetails spécifie une demande de récupération des détails d’élément non indexable.
ms.openlocfilehash: 1c04b4cd7a86183210be869973c9779188fa0adf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458599"
---
# <a name="getnonindexableitemdetails"></a><span data-ttu-id="85ab1-103">GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="85ab1-103">GetNonIndexableItemDetails</span></span>

<span data-ttu-id="85ab1-104">L’élément **GetNonIndexableItemDetails** spécifie une demande de récupération des détails d’élément non indexable.</span><span class="sxs-lookup"><span data-stu-id="85ab1-104">The **GetNonIndexableItemDetails** element specifies a request to retrieve nonindexable item details.</span></span> 
  
```XML
<GetNonIndexableItemDetails>
    <Mailboxes/>
    <PageSize/>
    <PageItemReference/>
    <PageDirection/>
</GetNonIndexableItemDetails>
```

 <span data-ttu-id="85ab1-105">**GetNonIndexableItemDetailsType**</span><span class="sxs-lookup"><span data-stu-id="85ab1-105">**GetNonIndexableItemDetailsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="85ab1-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="85ab1-106">Attributes and elements</span></span>

<span data-ttu-id="85ab1-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="85ab1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="85ab1-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="85ab1-108">Attributes</span></span>

<span data-ttu-id="85ab1-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="85ab1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="85ab1-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="85ab1-110">Child elements</span></span>

|<span data-ttu-id="85ab1-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="85ab1-111">**Element**</span></span>|<span data-ttu-id="85ab1-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="85ab1-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="85ab1-113">Boîtes aux lettres (NonEmptyArrayOfLegacyDNsType)</span><span class="sxs-lookup"><span data-stu-id="85ab1-113">Mailboxes (NonEmptyArrayOfLegacyDNsType)</span></span>](mailboxes-nonemptyarrayoflegacydnstype.md) <br/> |<span data-ttu-id="85ab1-114">Spécifie un tableau d’éléments de **boîte aux lettres** .</span><span class="sxs-lookup"><span data-stu-id="85ab1-114">Specifies an array of **Mailbox** elements.</span></span>  <br/> |
|[<span data-ttu-id="85ab1-115">PageSize</span><span class="sxs-lookup"><span data-stu-id="85ab1-115">PageSize</span></span>](pagesize.md) <br/> |<span data-ttu-id="85ab1-116">Contient le nombre d’éléments à renvoyer dans une seule page pour un résultat de recherche.</span><span class="sxs-lookup"><span data-stu-id="85ab1-116">Contains the number of items to be returned in a single page for a search result.</span></span>  <br/> |
|[<span data-ttu-id="85ab1-117">PageItemReference</span><span class="sxs-lookup"><span data-stu-id="85ab1-117">PageItemReference</span></span>](pageitemreference.md) <br/> |<span data-ttu-id="85ab1-118">Spécifie la référence d’un élément de page.</span><span class="sxs-lookup"><span data-stu-id="85ab1-118">Specifies the reference for a page item.</span></span>  <br/> |
|[<span data-ttu-id="85ab1-119">PageDirection</span><span class="sxs-lookup"><span data-stu-id="85ab1-119">PageDirection</span></span>](pagedirection.md) <br/> |<span data-ttu-id="85ab1-120">Contient le sens de pagination dans le résultat de la recherche.</span><span class="sxs-lookup"><span data-stu-id="85ab1-120">Contains the direction for pagination in the search result.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="85ab1-121">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="85ab1-121">Parent elements</span></span>

<span data-ttu-id="85ab1-122">Aucun.</span><span class="sxs-lookup"><span data-stu-id="85ab1-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="85ab1-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="85ab1-123">Remarks</span></span>

<span data-ttu-id="85ab1-124">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="85ab1-124">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="85ab1-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="85ab1-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="85ab1-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="85ab1-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="85ab1-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="85ab1-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="85ab1-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="85ab1-128">Schema Name</span></span>  <br/> |<span data-ttu-id="85ab1-129">Schéma de message</span><span class="sxs-lookup"><span data-stu-id="85ab1-129">Message schema</span></span>  <br/> |
|<span data-ttu-id="85ab1-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="85ab1-130">Validation File</span></span>  <br/> |<span data-ttu-id="85ab1-131">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="85ab1-131">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="85ab1-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="85ab1-132">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="85ab1-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="85ab1-133">See also</span></span>



- [<span data-ttu-id="85ab1-134">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="85ab1-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

