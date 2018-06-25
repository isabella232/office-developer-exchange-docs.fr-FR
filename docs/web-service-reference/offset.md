---
title: Décalage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Offset
api_type:
- schema
ms.assetid: dcbb9d85-d90c-4363-b4c9-d081ad03f407
description: L’élément de décalage décrit le décalage de le BaseOffset. Avec l’élément BaseOffset, l’élément de décalage indique si l’heure est standard ou l’heure d’été.
ms.openlocfilehash: d85fef0d67633733f6aa1943d70413ea70a528d6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828642"
---
# <a name="offset"></a><span data-ttu-id="4d2d3-104">Décalage</span><span class="sxs-lookup"><span data-stu-id="4d2d3-104">Offset</span></span>

<span data-ttu-id="4d2d3-105">L’élément de **décalage** décrit le décalage de l' [BaseOffset](baseoffset.md).</span><span class="sxs-lookup"><span data-stu-id="4d2d3-105">The **Offset** element describes the offset from the [BaseOffset](baseoffset.md).</span></span> <span data-ttu-id="4d2d3-106">Avec l’élément **BaseOffset** , l’élément **décalage** indique si l’heure est standard ou l’heure d’été.</span><span class="sxs-lookup"><span data-stu-id="4d2d3-106">Together with the **BaseOffset** element, the **Offset** element identifies whether the time is standard or daylight saving time.</span></span> 
  
```xml
<Offset/>
```

 <span data-ttu-id="4d2d3-107">**duration**</span><span class="sxs-lookup"><span data-stu-id="4d2d3-107">**duration**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4d2d3-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="4d2d3-108">Attributes and elements</span></span>

<span data-ttu-id="4d2d3-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="4d2d3-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4d2d3-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="4d2d3-110">Attributes</span></span>

<span data-ttu-id="4d2d3-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="4d2d3-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4d2d3-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="4d2d3-112">Child elements</span></span>

<span data-ttu-id="4d2d3-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="4d2d3-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4d2d3-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="4d2d3-114">Parent elements</span></span>

|<span data-ttu-id="4d2d3-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4d2d3-115">**Element**</span></span>|<span data-ttu-id="4d2d3-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="4d2d3-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4d2d3-117">Heure d’été</span><span class="sxs-lookup"><span data-stu-id="4d2d3-117">Daylight</span></span>](daylight.md) <br/> |<span data-ttu-id="4d2d3-118">Représente la date et l’heure de l’heure de modification de l’heure à l’heure standard.</span><span class="sxs-lookup"><span data-stu-id="4d2d3-118">Represents the date and time when the time changes from daylight saving time to standard time.</span></span>  <br/> |
|[<span data-ttu-id="4d2d3-119">Standard</span><span class="sxs-lookup"><span data-stu-id="4d2d3-119">Standard</span></span>](standard.md) <br/> |<span data-ttu-id="4d2d3-120">Représente la date et l’heure de l’heure de modification de l’heure à l’heure standard.</span><span class="sxs-lookup"><span data-stu-id="4d2d3-120">Represents the date and time when the time changes from daylight saving time to standard time.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4d2d3-121">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="4d2d3-121">Text value</span></span>

<span data-ttu-id="4d2d3-122">La valeur de texte représente le décalage du temps universel coordonné (UTC).</span><span class="sxs-lookup"><span data-stu-id="4d2d3-122">The text value represents the offset from Coordinated Universal Time (UTC).</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4d2d3-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="4d2d3-123">Remarks</span></span>

<span data-ttu-id="4d2d3-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="4d2d3-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4d2d3-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="4d2d3-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4d2d3-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="4d2d3-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4d2d3-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="4d2d3-127">Schema Name</span></span>  <br/> |<span data-ttu-id="4d2d3-128">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="4d2d3-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="4d2d3-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="4d2d3-129">Validation File</span></span>  <br/> |<span data-ttu-id="4d2d3-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4d2d3-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4d2d3-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="4d2d3-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="4d2d3-132">False</span><span class="sxs-lookup"><span data-stu-id="4d2d3-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4d2d3-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4d2d3-133">See also</span></span>



- [<span data-ttu-id="4d2d3-134">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="4d2d3-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

