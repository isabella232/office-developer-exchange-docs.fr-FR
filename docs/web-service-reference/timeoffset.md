---
title: TimeOffset
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TimeOffset
api_type:
- schema
ms.assetid: b70bf498-cc3a-4fa6-8236-514acb973b33
description: L’élément TimeOffset représente le décalage du temps universel coordonné (UTC) pour la transition de fuseau horaire.
ms.openlocfilehash: 46b1b2c8eec9bae871b4dafe43036e9d725075ae
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838701"
---
# <a name="timeoffset"></a><span data-ttu-id="37a08-103">TimeOffset</span><span class="sxs-lookup"><span data-stu-id="37a08-103">TimeOffset</span></span>

<span data-ttu-id="37a08-104">L’élément **TimeOffset** représente le décalage du temps universel coordonné (UTC) pour la transition de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="37a08-104">The **TimeOffset** element represents the time offset from Coordinated Universal Time (UTC) for the time zone transition.</span></span> 
  
```XML
<TimeOffset/>
```

 <span data-ttu-id="37a08-105">**duration**</span><span class="sxs-lookup"><span data-stu-id="37a08-105">**duration**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="37a08-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="37a08-106">Attributes and elements</span></span>

<span data-ttu-id="37a08-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="37a08-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="37a08-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="37a08-108">Attributes</span></span>

<span data-ttu-id="37a08-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="37a08-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="37a08-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="37a08-110">Child elements</span></span>

<span data-ttu-id="37a08-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="37a08-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="37a08-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="37a08-112">Parent elements</span></span>

|<span data-ttu-id="37a08-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="37a08-113">**Element**</span></span>|<span data-ttu-id="37a08-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="37a08-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="37a08-115">RecurringDateTransition</span><span class="sxs-lookup"><span data-stu-id="37a08-115">RecurringDateTransition</span></span>](recurringdatetransition.md) <br/> |<span data-ttu-id="37a08-116">Représente une transition de fuseau horaire qui se produit à une date spécifique chaque année.</span><span class="sxs-lookup"><span data-stu-id="37a08-116">Represents a time zone transition that occurs on a specific date each year.</span></span>  <br/> |
|[<span data-ttu-id="37a08-117">RecurringDayTransition</span><span class="sxs-lookup"><span data-stu-id="37a08-117">RecurringDayTransition</span></span>](recurringdaytransition.md) <br/> |<span data-ttu-id="37a08-118">Représente une transition de fuseau horaire qui se produit sur le même jour tous les ans.</span><span class="sxs-lookup"><span data-stu-id="37a08-118">Represents a time zone transition that occurs on the same day each year.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="37a08-119">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="37a08-119">Text value</span></span>

<span data-ttu-id="37a08-120">La valeur de texte de l’élément **TimeOffset** est une durée qui spécifie le décalage de l’heure UTC pour la transition de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="37a08-120">The text value of the **TimeOffset** element is a duration that specifies the time offset from UTC for the time zone transition.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="37a08-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="37a08-121">Remarks</span></span>

<span data-ttu-id="37a08-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="37a08-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="37a08-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="37a08-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="37a08-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="37a08-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="37a08-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="37a08-125">Schema Name</span></span>  <br/> |<span data-ttu-id="37a08-126">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="37a08-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="37a08-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="37a08-127">Validation File</span></span>  <br/> |<span data-ttu-id="37a08-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="37a08-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="37a08-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="37a08-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="37a08-130">False</span><span class="sxs-lookup"><span data-stu-id="37a08-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="37a08-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="37a08-131">See also</span></span>



- [<span data-ttu-id="37a08-132">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="37a08-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
