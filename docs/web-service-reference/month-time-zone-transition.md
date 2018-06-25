---
title: Mois (Transition fuseau horaire)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Month
api_type:
- schema
ms.assetid: 5e6aac75-366d-43d0-8ccb-956285474662
description: L’élément Month représente le mois dans laquelle se produit la transition de fuseau horaire.
ms.openlocfilehash: 887bd750b9cad1e28e6f7603c7b3289da8f8dc07
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828483"
---
# <a name="month-time-zone-transition"></a><span data-ttu-id="6d1c4-103">Mois (Transition fuseau horaire)</span><span class="sxs-lookup"><span data-stu-id="6d1c4-103">Month (Time Zone Transition)</span></span>

<span data-ttu-id="6d1c4-104">L’élément **Month** représente le mois dans laquelle se produit la transition de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="6d1c4-104">The **Month** element represents the month in which the time zone transition occurs.</span></span> 
  
```xml
<Month/>
```

 <span data-ttu-id="6d1c4-105">**int**</span><span class="sxs-lookup"><span data-stu-id="6d1c4-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6d1c4-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="6d1c4-106">Attributes and elements</span></span>

<span data-ttu-id="6d1c4-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="6d1c4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6d1c4-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="6d1c4-108">Attributes</span></span>

<span data-ttu-id="6d1c4-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="6d1c4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6d1c4-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="6d1c4-110">Child elements</span></span>

<span data-ttu-id="6d1c4-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="6d1c4-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6d1c4-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="6d1c4-112">Parent elements</span></span>

|<span data-ttu-id="6d1c4-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="6d1c4-113">**Element**</span></span>|<span data-ttu-id="6d1c4-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="6d1c4-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6d1c4-115">RecurringDateTransition</span><span class="sxs-lookup"><span data-stu-id="6d1c4-115">RecurringDateTransition</span></span>](recurringdatetransition.md) <br/> |<span data-ttu-id="6d1c4-116">Représente une transition de fuseau horaire qui se produit à une date spécifique chaque année.</span><span class="sxs-lookup"><span data-stu-id="6d1c4-116">Represents a time zone transition that occurs on a specific date each year.</span></span>  <br/> |
|[<span data-ttu-id="6d1c4-117">RecurringDayTransition</span><span class="sxs-lookup"><span data-stu-id="6d1c4-117">RecurringDayTransition</span></span>](recurringdaytransition.md) <br/> |<span data-ttu-id="6d1c4-118">Représente une transition de fuseau horaire qui se produit sur le même jour tous les ans.</span><span class="sxs-lookup"><span data-stu-id="6d1c4-118">Represents a time zone transition that occurs on the same day each year.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6d1c4-119">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="6d1c4-119">Text value</span></span>

<span data-ttu-id="6d1c4-120">La valeur de texte est un entier qui représente le mois dans laquelle se produit la transition de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="6d1c4-120">The text value is an integer that represents the month in which the time zone transition occurs.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6d1c4-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="6d1c4-121">Remarks</span></span>

<span data-ttu-id="6d1c4-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server qui a le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="6d1c4-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6d1c4-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="6d1c4-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6d1c4-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="6d1c4-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6d1c4-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="6d1c4-125">Schema Name</span></span>  <br/> |<span data-ttu-id="6d1c4-126">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="6d1c4-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="6d1c4-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="6d1c4-127">Validation File</span></span>  <br/> |<span data-ttu-id="6d1c4-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6d1c4-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6d1c4-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="6d1c4-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="6d1c4-130">False</span><span class="sxs-lookup"><span data-stu-id="6d1c4-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6d1c4-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="6d1c4-131">See also</span></span>



- [<span data-ttu-id="6d1c4-132">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="6d1c4-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

