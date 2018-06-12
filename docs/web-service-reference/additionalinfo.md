---
title: AdditionalInfo
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 50bebbab-2fef-4a27-a5a9-32d7200820b6
description: L’élément AdditionalInfo spécifie des informations supplémentaires sur l’état de conservation d’une boîte aux lettres.
ms.openlocfilehash: 6fbe24d5d3e41f2ba9c81657b2c38240d10eefed
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755173"
---
# <a name="additionalinfo"></a><span data-ttu-id="05411-103">AdditionalInfo</span><span class="sxs-lookup"><span data-stu-id="05411-103">AdditionalInfo</span></span>

<span data-ttu-id="05411-104">L’élément **AdditionalInfo** spécifie des informations supplémentaires sur l’état de conservation d’une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="05411-104">The **AdditionalInfo** element specifies additional information about the hold status of a mailbox.</span></span> 
  
```XML
<AdditionalInfo></AdditionalInfo>
```

 <span data-ttu-id="05411-105">**xs : String**</span><span class="sxs-lookup"><span data-stu-id="05411-105">**xs:string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="05411-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="05411-106">Attributes and elements</span></span>

<span data-ttu-id="05411-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="05411-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="05411-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="05411-108">Attributes</span></span>

<span data-ttu-id="05411-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="05411-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="05411-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="05411-110">Child elements</span></span>

<span data-ttu-id="05411-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="05411-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="05411-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="05411-112">Parent elements</span></span>

|<span data-ttu-id="05411-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="05411-113">**Element**</span></span>|<span data-ttu-id="05411-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="05411-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="05411-115">MailboxHoldStatus</span><span class="sxs-lookup"><span data-stu-id="05411-115">MailboxHoldStatus</span></span>](mailboxholdstatus.md) <br/> |<span data-ttu-id="05411-116">Spécifie l’état de conservation de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="05411-116">Specifies the hold status of the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="05411-117">NonIndexableItemDetail</span><span class="sxs-lookup"><span data-stu-id="05411-117">NonIndexableItemDetail</span></span>](nonindexableitemdetail.md) <br/> |<span data-ttu-id="05411-118">Spécifie les détails d’un élément qui ne peuvent pas être indexé.</span><span class="sxs-lookup"><span data-stu-id="05411-118">Specifies detail for an item that cannot be indexed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="05411-119">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="05411-119">Text value</span></span>

<span data-ttu-id="05411-120">La valeur de texte de l’élément AdditionalInfo est plus d’informations sur l’état de conservation d’une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="05411-120">The text value of the AdditionalInfo element is additional information about the hold status of a mailbox.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="05411-121">Note</span><span class="sxs-lookup"><span data-stu-id="05411-121">Remarks</span></span>

<span data-ttu-id="05411-122">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="05411-122">This element is optional.</span></span>
  
<span data-ttu-id="05411-123">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="05411-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="05411-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="05411-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="05411-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="05411-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="05411-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="05411-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="05411-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="05411-127">Schema Name</span></span>  <br/> |<span data-ttu-id="05411-128">Schéma type</span><span class="sxs-lookup"><span data-stu-id="05411-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="05411-129">Validation File</span><span class="sxs-lookup"><span data-stu-id="05411-129">Validation File</span></span>  <br/> |<span data-ttu-id="05411-130">types.xsd</span><span class="sxs-lookup"><span data-stu-id="05411-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="05411-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="05411-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="05411-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="05411-132">See also</span></span>

- [<span data-ttu-id="05411-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="05411-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

