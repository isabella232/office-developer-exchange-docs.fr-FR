---
title: Année
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Year
api_type:
- schema
ms.assetid: 93bf2847-53fa-496c-9a1e-dc9a9ffd0b9f
description: L’élément Year est utilisé pour définir un fuseau horaire qui change en fonction de l’année. Cet élément est facultatif. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 95d75f9c6166fc26e86534346fb07292a7fb3dcd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839077"
---
# <a name="year"></a><span data-ttu-id="6bc55-105">Année</span><span class="sxs-lookup"><span data-stu-id="6bc55-105">Year</span></span>

<span data-ttu-id="6bc55-106">L’élément **Year** est utilisé pour définir un fuseau horaire qui change en fonction de l’année.</span><span class="sxs-lookup"><span data-stu-id="6bc55-106">The **Year** element is used to define a time zone that changes depending on the year.</span></span> <span data-ttu-id="6bc55-107">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="6bc55-107">This element is optional.</span></span> <span data-ttu-id="6bc55-108">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="6bc55-108">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<Year/>
```

<span data-ttu-id="6bc55-109">**string**</span><span class="sxs-lookup"><span data-stu-id="6bc55-109">**string**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="6bc55-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="6bc55-110">Attributes and elements</span></span>

<span data-ttu-id="6bc55-111">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="6bc55-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6bc55-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="6bc55-112">Attributes</span></span>

<span data-ttu-id="6bc55-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="6bc55-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6bc55-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="6bc55-114">Child elements</span></span>

<span data-ttu-id="6bc55-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="6bc55-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6bc55-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="6bc55-116">Parent elements</span></span>

|<span data-ttu-id="6bc55-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="6bc55-117">**Element**</span></span>|<span data-ttu-id="6bc55-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="6bc55-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6bc55-119">StandardTime</span><span class="sxs-lookup"><span data-stu-id="6bc55-119">StandardTime</span></span>](standardtime.md) <br/> |<span data-ttu-id="6bc55-120">Représente un décalage de l’heure par rapport à temps universel coordonné (UTC) qui est représenté par l’élément [Bias (UTC)](bias-utc.md) .</span><span class="sxs-lookup"><span data-stu-id="6bc55-120">Represents an offset from the time relative to Coordinated Universal Time (UTC) that is represented by the [Bias (UTC)](bias-utc.md) element.</span></span>  <br/> |
|[<span data-ttu-id="6bc55-121">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="6bc55-121">DaylightTime</span></span>](daylighttime.md) <br/> |<span data-ttu-id="6bc55-122">Représente un décalage de l’heure par rapport à temps universel coordonné (UTC) qui est représenté par l’élément [Bias (UTC)](bias-utc.md) dans les zones où l’heure d’été est respectée.</span><span class="sxs-lookup"><span data-stu-id="6bc55-122">Represents an offset from the time relative to Coordinated Universal Time (UTC) that is represented by the [Bias (UTC)](bias-utc.md) element in regions where daylight saving time is observed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6bc55-123">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="6bc55-123">Text value</span></span>

<span data-ttu-id="6bc55-124">L’élément Year accepte une chaîne qui représente une année.</span><span class="sxs-lookup"><span data-stu-id="6bc55-124">The Year element accepts a string that represents a year.</span></span> <span data-ttu-id="6bc55-125">Le format d’année est aaaa.</span><span class="sxs-lookup"><span data-stu-id="6bc55-125">The year format is YYYY.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6bc55-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="6bc55-126">Remarks</span></span>

<span data-ttu-id="6bc55-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="6bc55-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6bc55-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="6bc55-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6bc55-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="6bc55-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6bc55-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="6bc55-130">Schema Name</span></span>  <br/> |<span data-ttu-id="6bc55-131">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="6bc55-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="6bc55-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="6bc55-132">Validation File</span></span>  <br/> |<span data-ttu-id="6bc55-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6bc55-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6bc55-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="6bc55-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="6bc55-135">False</span><span class="sxs-lookup"><span data-stu-id="6bc55-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6bc55-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="6bc55-136">See also</span></span>

- [<span data-ttu-id="6bc55-137">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="6bc55-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

