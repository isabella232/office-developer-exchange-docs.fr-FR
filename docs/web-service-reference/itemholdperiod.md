---
title: ItemHoldPeriod
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 30369db5-4d45-40e8-bc83-3236667fc404
description: L’élément ItemHoldPeriod spécifie la quantité de temps pour bloquer le contenu qui correspond à la requête de la boîte aux lettres.
ms.openlocfilehash: 212d765aa3f0493dd4f3051de483fa08a6fa8ac7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828144"
---
# <a name="itemholdperiod"></a><span data-ttu-id="c60d0-103">ItemHoldPeriod</span><span class="sxs-lookup"><span data-stu-id="c60d0-103">ItemHoldPeriod</span></span>

<span data-ttu-id="c60d0-104">L’élément **ItemHoldPeriod** spécifie la quantité de temps pour bloquer le contenu qui correspond à la requête de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="c60d0-104">The **ItemHoldPeriod** element specifies the amount of time to hold content that matches the mailbox query.</span></span> 
  
```XML
<ItemHoldPeriod/>
```

 <span data-ttu-id="c60d0-105">**string**</span><span class="sxs-lookup"><span data-stu-id="c60d0-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c60d0-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="c60d0-106">Attributes and elements</span></span>

<span data-ttu-id="c60d0-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="c60d0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c60d0-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="c60d0-108">Attributes</span></span>

<span data-ttu-id="c60d0-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c60d0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c60d0-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="c60d0-110">Child elements</span></span>

<span data-ttu-id="c60d0-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c60d0-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c60d0-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="c60d0-112">Parent elements</span></span>

[<span data-ttu-id="c60d0-113">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="c60d0-113">SetHoldOnMailboxes</span></span>](setholdonmailboxes.md)
  
## <a name="text-value"></a><span data-ttu-id="c60d0-114">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="c60d0-114">Text value</span></span>

<span data-ttu-id="c60d0-115">La valeur de texte peut être « Unlimited » ou la valeur de chaîne de n’importe quelle valeur [Timespan](http://msdn.microsoft.com/en-us/library/1ecy8h51%28v=vs.110%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="c60d0-115">The text value can be "Unlimited" or the string value of any [Timespan](http://msdn.microsoft.com/en-us/library/1ecy8h51%28v=vs.110%29.aspx) value.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="c60d0-116">Remarques</span><span class="sxs-lookup"><span data-stu-id="c60d0-116">Remarks</span></span>

<span data-ttu-id="c60d0-117">Cet élément est une nouveauté d'Exchange Server 2013 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="c60d0-117">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="c60d0-118">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="c60d0-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c60d0-119">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="c60d0-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c60d0-120">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="c60d0-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c60d0-121">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="c60d0-121">Schema Name</span></span>  <br/> |<span data-ttu-id="c60d0-122">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="c60d0-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c60d0-123">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="c60d0-123">Validation File</span></span>  <br/> |<span data-ttu-id="c60d0-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c60d0-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c60d0-125">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="c60d0-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="c60d0-126">True</span><span class="sxs-lookup"><span data-stu-id="c60d0-126">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c60d0-127">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c60d0-127">See also</span></span>



[<span data-ttu-id="c60d0-128">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="c60d0-128">SetHoldOnMailboxes</span></span>](setholdonmailboxes.md)


- [<span data-ttu-id="c60d0-129">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="c60d0-129">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

