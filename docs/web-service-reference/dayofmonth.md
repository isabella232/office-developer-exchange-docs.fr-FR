---
title: DayOfMonth
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DayOfMonth
api_type:
- schema
ms.assetid: 09b7504e-08d8-42f9-88cc-a2a37a2e2b8b
description: L’élément DayOfMonth décrit le jour d’un mois pendant lequel un élément périodique se produit.
ms.openlocfilehash: dc333a46283d5e8eba3a79f62f8c22c22f56e190
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44442828"
---
# <a name="dayofmonth"></a><span data-ttu-id="03136-103">DayOfMonth</span><span class="sxs-lookup"><span data-stu-id="03136-103">DayOfMonth</span></span>

<span data-ttu-id="03136-104">L’élément **DayOfMonth** décrit le jour d’un mois pendant lequel un élément périodique se produit.</span><span class="sxs-lookup"><span data-stu-id="03136-104">The **DayOfMonth** element describes the day in a month that a recurring item occurs.</span></span> 
  
```xml
<DayOfMonth/>
```

<span data-ttu-id="03136-105">**int**</span><span class="sxs-lookup"><span data-stu-id="03136-105">**int**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="03136-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="03136-106">Attributes and elements</span></span>

<span data-ttu-id="03136-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="03136-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="03136-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="03136-108">Attributes</span></span>

<span data-ttu-id="03136-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="03136-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="03136-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="03136-110">Child elements</span></span>

<span data-ttu-id="03136-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="03136-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="03136-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="03136-112">Parent elements</span></span>

|<span data-ttu-id="03136-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="03136-113">**Element**</span></span>|<span data-ttu-id="03136-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="03136-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="03136-115">AbsoluteYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="03136-115">AbsoluteYearlyRecurrence</span></span>](absoluteyearlyrecurrence.md) <br/> |<span data-ttu-id="03136-116">Représente une périodicité annuelle.</span><span class="sxs-lookup"><span data-stu-id="03136-116">Represents a yearly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="03136-117">AbsoluteMonthlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="03136-117">AbsoluteMonthlyRecurrence</span></span>](absolutemonthlyrecurrence.md) <br/> |<span data-ttu-id="03136-118">Représente une périodicité mensuelle.</span><span class="sxs-lookup"><span data-stu-id="03136-118">Represents a monthly recurrence pattern.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="03136-119">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="03136-119">Text value</span></span>

<span data-ttu-id="03136-120">Une valeur de texte qui représente un nombre entier compris entre 1 et 31 est requise.</span><span class="sxs-lookup"><span data-stu-id="03136-120">A text value that represents an integer in the range of 1 to 31 is required.</span></span> <span data-ttu-id="03136-121">Si, pour un mois donné, cette valeur est supérieure au nombre de jours du mois, le dernier jour du mois est supposé.</span><span class="sxs-lookup"><span data-stu-id="03136-121">If for a particular month this value is larger than the number of days in the month, the last day of the month is assumed.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="03136-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="03136-122">Remarks</span></span>

<span data-ttu-id="03136-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="03136-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="03136-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="03136-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="03136-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="03136-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="03136-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="03136-126">Schema name</span></span>  <br/> |<span data-ttu-id="03136-127">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="03136-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="03136-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="03136-128">Validation file</span></span>  <br/> |<span data-ttu-id="03136-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="03136-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="03136-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="03136-130">Can be empty</span></span>  <br/> |<span data-ttu-id="03136-131">False</span><span class="sxs-lookup"><span data-stu-id="03136-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="03136-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="03136-132">See also</span></span>

- [<span data-ttu-id="03136-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="03136-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

