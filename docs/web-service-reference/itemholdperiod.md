---
title: ItemHoldPeriod
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 30369db5-4d45-40e8-bc83-3236667fc404
description: L’élément ItemHoldPeriod spécifie la durée de conservation du contenu qui correspond à la requête de boîte aux lettres.
ms.openlocfilehash: 185666b72cc96dd88605b7baa6433d070e7ebc91
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44452285"
---
# <a name="itemholdperiod"></a><span data-ttu-id="c2a89-103">ItemHoldPeriod</span><span class="sxs-lookup"><span data-stu-id="c2a89-103">ItemHoldPeriod</span></span>

<span data-ttu-id="c2a89-104">L’élément **ItemHoldPeriod** spécifie la durée de conservation du contenu qui correspond à la requête de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="c2a89-104">The **ItemHoldPeriod** element specifies the amount of time to hold content that matches the mailbox query.</span></span> 
  
```XML
<ItemHoldPeriod/>
```

 <span data-ttu-id="c2a89-105">**chaîne**</span><span class="sxs-lookup"><span data-stu-id="c2a89-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c2a89-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="c2a89-106">Attributes and elements</span></span>

<span data-ttu-id="c2a89-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="c2a89-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c2a89-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="c2a89-108">Attributes</span></span>

<span data-ttu-id="c2a89-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="c2a89-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c2a89-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="c2a89-110">Child elements</span></span>

<span data-ttu-id="c2a89-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c2a89-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c2a89-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="c2a89-112">Parent elements</span></span>

[<span data-ttu-id="c2a89-113">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="c2a89-113">SetHoldOnMailboxes</span></span>](setholdonmailboxes.md)
  
## <a name="text-value"></a><span data-ttu-id="c2a89-114">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="c2a89-114">Text value</span></span>

<span data-ttu-id="c2a89-115">La valeur de texte peut être « Unlimited » ou la valeur de la chaîne de n’importe quelle valeur [TimeSpan](https://msdn.microsoft.com/library/1ecy8h51%28v=vs.110%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="c2a89-115">The text value can be "Unlimited" or the string value of any [Timespan](https://msdn.microsoft.com/library/1ecy8h51%28v=vs.110%29.aspx) value.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="c2a89-116">Remarques</span><span class="sxs-lookup"><span data-stu-id="c2a89-116">Remarks</span></span>

<span data-ttu-id="c2a89-117">Cet élément est une nouveauté d'Exchange Server 2013 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="c2a89-117">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="c2a89-118">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="c2a89-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c2a89-119">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="c2a89-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c2a89-120">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="c2a89-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c2a89-121">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="c2a89-121">Schema Name</span></span>  <br/> |<span data-ttu-id="c2a89-122">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="c2a89-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c2a89-123">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="c2a89-123">Validation File</span></span>  <br/> |<span data-ttu-id="c2a89-124">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="c2a89-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c2a89-125">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="c2a89-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="c2a89-126">True</span><span class="sxs-lookup"><span data-stu-id="c2a89-126">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c2a89-127">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c2a89-127">See also</span></span>



[<span data-ttu-id="c2a89-128">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="c2a89-128">SetHoldOnMailboxes</span></span>](setholdonmailboxes.md)


- [<span data-ttu-id="c2a89-129">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="c2a89-129">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

