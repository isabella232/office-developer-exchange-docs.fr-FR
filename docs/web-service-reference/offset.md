---
title: Offset
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
description: L’élément offset décrit le décalage par rapport à l’BaseOffset. Avec l’élément BaseOffset, l’élément offset identifie s’il s’agit de l’heure standard ou de l’heure d’été.
ms.openlocfilehash: 74ad87026c2cb89f3b0c35218c91f81380029963
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459755"
---
# <a name="offset"></a><span data-ttu-id="75854-104">Offset</span><span class="sxs-lookup"><span data-stu-id="75854-104">Offset</span></span>

<span data-ttu-id="75854-105">L’élément **offset** décrit le décalage par rapport à l' [BaseOffset](baseoffset.md).</span><span class="sxs-lookup"><span data-stu-id="75854-105">The **Offset** element describes the offset from the [BaseOffset](baseoffset.md).</span></span> <span data-ttu-id="75854-106">Avec l’élément **BaseOffset** , l’élément **offset** identifie s’il s’agit de l’heure standard ou de l’heure d’été.</span><span class="sxs-lookup"><span data-stu-id="75854-106">Together with the **BaseOffset** element, the **Offset** element identifies whether the time is standard or daylight saving time.</span></span> 
  
```xml
<Offset/>
```

 <span data-ttu-id="75854-107">**duration**</span><span class="sxs-lookup"><span data-stu-id="75854-107">**duration**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="75854-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="75854-108">Attributes and elements</span></span>

<span data-ttu-id="75854-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="75854-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="75854-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="75854-110">Attributes</span></span>

<span data-ttu-id="75854-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="75854-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="75854-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="75854-112">Child elements</span></span>

<span data-ttu-id="75854-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="75854-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="75854-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="75854-114">Parent elements</span></span>

|<span data-ttu-id="75854-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="75854-115">**Element**</span></span>|<span data-ttu-id="75854-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="75854-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="75854-117">Auxquelles</span><span class="sxs-lookup"><span data-stu-id="75854-117">Daylight</span></span>](daylight.md) <br/> |<span data-ttu-id="75854-118">Représente la date et l’heure auxquelles l’heure passe de l’heure d’été à l’heure standard.</span><span class="sxs-lookup"><span data-stu-id="75854-118">Represents the date and time when the time changes from daylight saving time to standard time.</span></span>  <br/> |
|[<span data-ttu-id="75854-119">Standard</span><span class="sxs-lookup"><span data-stu-id="75854-119">Standard</span></span>](standard.md) <br/> |<span data-ttu-id="75854-120">Représente la date et l’heure auxquelles l’heure passe de l’heure d’été à l’heure standard.</span><span class="sxs-lookup"><span data-stu-id="75854-120">Represents the date and time when the time changes from daylight saving time to standard time.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="75854-121">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="75854-121">Text value</span></span>

<span data-ttu-id="75854-122">La valeur de texte représente le décalage par rapport au temps universel coordonné (UTC).</span><span class="sxs-lookup"><span data-stu-id="75854-122">The text value represents the offset from Coordinated Universal Time (UTC).</span></span>
  
## <a name="remarks"></a><span data-ttu-id="75854-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="75854-123">Remarks</span></span>

<span data-ttu-id="75854-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="75854-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="75854-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="75854-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="75854-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="75854-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="75854-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="75854-127">Schema Name</span></span>  <br/> |<span data-ttu-id="75854-128">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="75854-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="75854-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="75854-129">Validation File</span></span>  <br/> |<span data-ttu-id="75854-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="75854-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="75854-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="75854-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="75854-132">False</span><span class="sxs-lookup"><span data-stu-id="75854-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="75854-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="75854-133">See also</span></span>



- [<span data-ttu-id="75854-134">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="75854-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

