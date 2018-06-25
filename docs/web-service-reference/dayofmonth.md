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
description: L’élément DayOfMonth décrit le jour du mois qui se produit un élément périodique.
ms.openlocfilehash: 0d0d95849a2562e06b88872b2857cc5e6ca67af3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755816"
---
# <a name="dayofmonth"></a><span data-ttu-id="b7dfe-103">DayOfMonth</span><span class="sxs-lookup"><span data-stu-id="b7dfe-103">DayOfMonth</span></span>

<span data-ttu-id="b7dfe-104">L’élément **DayOfMonth** décrit le jour du mois qui se produit un élément périodique.</span><span class="sxs-lookup"><span data-stu-id="b7dfe-104">The **DayOfMonth** element describes the day in a month that a recurring item occurs.</span></span> 
  
```xml
<DayOfMonth/>
```

<span data-ttu-id="b7dfe-105">**int**</span><span class="sxs-lookup"><span data-stu-id="b7dfe-105">**int**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="b7dfe-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="b7dfe-106">Attributes and elements</span></span>

<span data-ttu-id="b7dfe-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="b7dfe-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b7dfe-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="b7dfe-108">Attributes</span></span>

<span data-ttu-id="b7dfe-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b7dfe-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b7dfe-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="b7dfe-110">Child elements</span></span>

<span data-ttu-id="b7dfe-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b7dfe-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b7dfe-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="b7dfe-112">Parent elements</span></span>

|<span data-ttu-id="b7dfe-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b7dfe-113">**Element**</span></span>|<span data-ttu-id="b7dfe-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="b7dfe-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b7dfe-115">AbsoluteYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="b7dfe-115">AbsoluteYearlyRecurrence</span></span>](absoluteyearlyrecurrence.md) <br/> |<span data-ttu-id="b7dfe-116">Représente une périodicité annuelle.</span><span class="sxs-lookup"><span data-stu-id="b7dfe-116">Represents a yearly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="b7dfe-117">AbsoluteMonthlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="b7dfe-117">AbsoluteMonthlyRecurrence</span></span>](absolutemonthlyrecurrence.md) <br/> |<span data-ttu-id="b7dfe-118">Représente une périodicité mensuelle.</span><span class="sxs-lookup"><span data-stu-id="b7dfe-118">Represents a monthly recurrence pattern.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b7dfe-119">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="b7dfe-119">Text value</span></span>

<span data-ttu-id="b7dfe-120">Une valeur de texte qui représente un entier dans la plage de 1 à 31 est requise.</span><span class="sxs-lookup"><span data-stu-id="b7dfe-120">A text value that represents an integer in the range of 1 to 31 is required.</span></span> <span data-ttu-id="b7dfe-121">Si pour un mois donné, cette valeur est supérieure au nombre de jours dans le mois, le dernier jour du mois est supposé.</span><span class="sxs-lookup"><span data-stu-id="b7dfe-121">If for a particular month this value is larger than the number of days in the month, the last day of the month is assumed.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b7dfe-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="b7dfe-122">Remarks</span></span>

<span data-ttu-id="b7dfe-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="b7dfe-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b7dfe-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="b7dfe-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b7dfe-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="b7dfe-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b7dfe-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="b7dfe-126">Schema name</span></span>  <br/> |<span data-ttu-id="b7dfe-127">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="b7dfe-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="b7dfe-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="b7dfe-128">Validation file</span></span>  <br/> |<span data-ttu-id="b7dfe-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b7dfe-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b7dfe-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="b7dfe-130">Can be empty</span></span>  <br/> |<span data-ttu-id="b7dfe-131">False</span><span class="sxs-lookup"><span data-stu-id="b7dfe-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b7dfe-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b7dfe-132">See also</span></span>

- [<span data-ttu-id="b7dfe-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="b7dfe-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

