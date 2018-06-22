---
title: HasBlockedImages
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ddeb11db-797d-4939-91d5-3e44be5f0778
description: L’élément HasBlockedImages spécifie une valeur de type Boolean qui indique si l’élément a bloqué des images.
ms.openlocfilehash: fbe9967c898016aeef27e3c86e8a1cf603bd87fc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19827795"
---
# <a name="hasblockedimages"></a><span data-ttu-id="7099e-103">HasBlockedImages</span><span class="sxs-lookup"><span data-stu-id="7099e-103">HasBlockedImages</span></span>

<span data-ttu-id="7099e-104">L’élément **HasBlockedImages** spécifie une valeur de type Boolean qui indique si l’élément a bloqué des images.</span><span class="sxs-lookup"><span data-stu-id="7099e-104">The **HasBlockedImages** element specifies a Boolean value that indicates whether the item has blocked images.</span></span> 
  
```XML
<HasBlockedImages> true | false </HasBlockedImages>
```

 <span data-ttu-id="7099e-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="7099e-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7099e-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="7099e-106">Attributes and elements</span></span>

<span data-ttu-id="7099e-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="7099e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7099e-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="7099e-108">Attributes</span></span>

<span data-ttu-id="7099e-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7099e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7099e-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="7099e-110">Child elements</span></span>

<span data-ttu-id="7099e-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7099e-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7099e-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="7099e-112">Parent elements</span></span>

|<span data-ttu-id="7099e-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7099e-113">**Element**</span></span>|<span data-ttu-id="7099e-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="7099e-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7099e-115">Item</span><span class="sxs-lookup"><span data-stu-id="7099e-115">Item</span></span>](item.md) <br/> |<span data-ttu-id="7099e-116">Représente un élément générique dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="7099e-116">Represents a generic item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7099e-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="7099e-117">Text value</span></span>

<span data-ttu-id="7099e-118">Une valeur de texte de **la valeur true** pour l’élément **HasBlockedImages** indique que l’élément a bloqué des images.</span><span class="sxs-lookup"><span data-stu-id="7099e-118">A text value of **true** for the **HasBlockedImages** element indicates that the item has blocked images.</span></span> <span data-ttu-id="7099e-119">La valeur **false** indique que l’élément ne dispose pas des images bloquées.</span><span class="sxs-lookup"><span data-stu-id="7099e-119">A value of **false** indicates that the item does not have any blocked images.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="7099e-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="7099e-120">Remarks</span></span>

<span data-ttu-id="7099e-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="7099e-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="7099e-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="7099e-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7099e-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="7099e-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7099e-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="7099e-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7099e-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="7099e-125">Schema Name</span></span>  <br/> |<span data-ttu-id="7099e-126">Schéma type</span><span class="sxs-lookup"><span data-stu-id="7099e-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="7099e-127">Validation File</span><span class="sxs-lookup"><span data-stu-id="7099e-127">Validation File</span></span>  <br/> |<span data-ttu-id="7099e-128">types.xsd</span><span class="sxs-lookup"><span data-stu-id="7099e-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="7099e-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="7099e-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="7099e-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7099e-130">See also</span></span>



- [<span data-ttu-id="7099e-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="7099e-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

