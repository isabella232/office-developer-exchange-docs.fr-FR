---
title: TransitionsGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TransitionsGroup
api_type:
- schema
ms.assetid: 19d56080-546a-4d53-929e-363d56186759
description: L’élément TransitionsGroup représente un tableau des transitions de fuseau horaire.
ms.openlocfilehash: e5991ad7f73a1694e0d4abadd8d252acc04970e5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838774"
---
# <a name="transitionsgroup"></a><span data-ttu-id="5ea7a-103">TransitionsGroup</span><span class="sxs-lookup"><span data-stu-id="5ea7a-103">TransitionsGroup</span></span>

<span data-ttu-id="5ea7a-104">L’élément **TransitionsGroup** représente un tableau des transitions de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="5ea7a-104">The **TransitionsGroup** element represents an array of time zone transitions.</span></span> 
  
```xml
<TransitionsGroup Id="">
   <AbsoluteDateTransition/>
   <RecurringDayTransition/>
   <RecurringDateTransition/>
</TransitionsGroup>
```

 <span data-ttu-id="5ea7a-105">**ArrayOfTransitionsType**</span><span class="sxs-lookup"><span data-stu-id="5ea7a-105">**ArrayOfTransitionsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5ea7a-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="5ea7a-106">Attributes and elements</span></span>

<span data-ttu-id="5ea7a-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="5ea7a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5ea7a-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="5ea7a-108">Attributes</span></span>

|<span data-ttu-id="5ea7a-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="5ea7a-109">**Attribute**</span></span>|<span data-ttu-id="5ea7a-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="5ea7a-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5ea7a-111">ID</span><span class="sxs-lookup"><span data-stu-id="5ea7a-111">Id</span></span>  <br/> |<span data-ttu-id="5ea7a-112">Une valeur de type string qui représente l’identificateur unique du groupe transitions.</span><span class="sxs-lookup"><span data-stu-id="5ea7a-112">A string value that represents the unique identifier of the transitions group.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="5ea7a-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="5ea7a-113">Child elements</span></span>

|<span data-ttu-id="5ea7a-114">**Élément**</span><span class="sxs-lookup"><span data-stu-id="5ea7a-114">**Element**</span></span>|<span data-ttu-id="5ea7a-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="5ea7a-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5ea7a-116">AbsoluteDateTransition</span><span class="sxs-lookup"><span data-stu-id="5ea7a-116">AbsoluteDateTransition</span></span>](absolutedatetransition.md) <br/> |<span data-ttu-id="5ea7a-117">Représente une transition de fuseau horaire qui se produit à une date spécifique, à un moment spécifique.</span><span class="sxs-lookup"><span data-stu-id="5ea7a-117">Represents a time zone transition that occurs on a specific date and at a specific time.</span></span>  <br/> |
|[<span data-ttu-id="5ea7a-118">RecurringDayTransition</span><span class="sxs-lookup"><span data-stu-id="5ea7a-118">RecurringDayTransition</span></span>](recurringdaytransition.md) <br/> |<span data-ttu-id="5ea7a-119">Représente une transition de fuseau horaire qui se produit sur le même jour tous les ans.</span><span class="sxs-lookup"><span data-stu-id="5ea7a-119">Represents a time zone transition that occurs on the same day each year.</span></span>  <br/> |
|[<span data-ttu-id="5ea7a-120">RecurringDateTransition</span><span class="sxs-lookup"><span data-stu-id="5ea7a-120">RecurringDateTransition</span></span>](recurringdatetransition.md) <br/> |<span data-ttu-id="5ea7a-121">Représente une transition de fuseau horaire qui se produit sur un jour spécifié de l’année.</span><span class="sxs-lookup"><span data-stu-id="5ea7a-121">Represents a time zone transition that occurs on a specified day of the year.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5ea7a-122">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="5ea7a-122">Parent elements</span></span>

|<span data-ttu-id="5ea7a-123">**Élément**</span><span class="sxs-lookup"><span data-stu-id="5ea7a-123">**Element**</span></span>|<span data-ttu-id="5ea7a-124">**Description**</span><span class="sxs-lookup"><span data-stu-id="5ea7a-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5ea7a-125">TransitionsGroups</span><span class="sxs-lookup"><span data-stu-id="5ea7a-125">TransitionsGroups</span></span>](transitionsgroups.md) <br/> |<span data-ttu-id="5ea7a-126">Représente un tableau de groupes de transition de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="5ea7a-126">Represents an array of time zone transition groups.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5ea7a-127">Remarques</span><span class="sxs-lookup"><span data-stu-id="5ea7a-127">Remarks</span></span>

<span data-ttu-id="5ea7a-128">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server qui a le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="5ea7a-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5ea7a-129">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="5ea7a-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5ea7a-130">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="5ea7a-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5ea7a-131">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="5ea7a-131">Schema Name</span></span>  <br/> |<span data-ttu-id="5ea7a-132">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="5ea7a-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="5ea7a-133">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="5ea7a-133">Validation File</span></span>  <br/> |<span data-ttu-id="5ea7a-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="5ea7a-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5ea7a-135">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="5ea7a-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="5ea7a-136">False</span><span class="sxs-lookup"><span data-stu-id="5ea7a-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5ea7a-137">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="5ea7a-137">See also</span></span>



- [<span data-ttu-id="5ea7a-138">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="5ea7a-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

