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
description: L’élément TransitionsGroup représente un tableau de transitions de fuseau horaire.
ms.openlocfilehash: 9f08dec048d410dadab9580e7886b2499d943176
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467416"
---
# <a name="transitionsgroup"></a><span data-ttu-id="e9430-103">TransitionsGroup</span><span class="sxs-lookup"><span data-stu-id="e9430-103">TransitionsGroup</span></span>

<span data-ttu-id="e9430-104">L’élément **TransitionsGroup** représente un tableau de transitions de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="e9430-104">The **TransitionsGroup** element represents an array of time zone transitions.</span></span> 
  
```xml
<TransitionsGroup Id="">
   <AbsoluteDateTransition/>
   <RecurringDayTransition/>
   <RecurringDateTransition/>
</TransitionsGroup>
```

 <span data-ttu-id="e9430-105">**ArrayOfTransitionsType**</span><span class="sxs-lookup"><span data-stu-id="e9430-105">**ArrayOfTransitionsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e9430-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="e9430-106">Attributes and elements</span></span>

<span data-ttu-id="e9430-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="e9430-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e9430-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="e9430-108">Attributes</span></span>

|<span data-ttu-id="e9430-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="e9430-109">**Attribute**</span></span>|<span data-ttu-id="e9430-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="e9430-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e9430-111">ID</span><span class="sxs-lookup"><span data-stu-id="e9430-111">Id</span></span>  <br/> |<span data-ttu-id="e9430-112">Valeur de type String qui représente l’identificateur unique du groupe transitions.</span><span class="sxs-lookup"><span data-stu-id="e9430-112">A string value that represents the unique identifier of the transitions group.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="e9430-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="e9430-113">Child elements</span></span>

|<span data-ttu-id="e9430-114">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e9430-114">**Element**</span></span>|<span data-ttu-id="e9430-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="e9430-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e9430-116">AbsoluteDateTransition</span><span class="sxs-lookup"><span data-stu-id="e9430-116">AbsoluteDateTransition</span></span>](absolutedatetransition.md) <br/> |<span data-ttu-id="e9430-117">Représente une transition de fuseau horaire qui se produit à une date et à une heure spécifiques.</span><span class="sxs-lookup"><span data-stu-id="e9430-117">Represents a time zone transition that occurs on a specific date and at a specific time.</span></span>  <br/> |
|[<span data-ttu-id="e9430-118">RecurringDayTransition</span><span class="sxs-lookup"><span data-stu-id="e9430-118">RecurringDayTransition</span></span>](recurringdaytransition.md) <br/> |<span data-ttu-id="e9430-119">Représente une transition de fuseau horaire qui se produit chaque année.</span><span class="sxs-lookup"><span data-stu-id="e9430-119">Represents a time zone transition that occurs on the same day each year.</span></span>  <br/> |
|[<span data-ttu-id="e9430-120">RecurringDateTransition</span><span class="sxs-lookup"><span data-stu-id="e9430-120">RecurringDateTransition</span></span>](recurringdatetransition.md) <br/> |<span data-ttu-id="e9430-121">Représente une transition de fuseau horaire qui se produit un jour de l’année donné.</span><span class="sxs-lookup"><span data-stu-id="e9430-121">Represents a time zone transition that occurs on a specified day of the year.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e9430-122">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="e9430-122">Parent elements</span></span>

|<span data-ttu-id="e9430-123">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e9430-123">**Element**</span></span>|<span data-ttu-id="e9430-124">**Description**</span><span class="sxs-lookup"><span data-stu-id="e9430-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e9430-125">TransitionsGroups</span><span class="sxs-lookup"><span data-stu-id="e9430-125">TransitionsGroups</span></span>](transitionsgroups.md) <br/> |<span data-ttu-id="e9430-126">Représente un tableau de groupes de transition de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="e9430-126">Represents an array of time zone transition groups.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e9430-127">Remarques</span><span class="sxs-lookup"><span data-stu-id="e9430-127">Remarks</span></span>

<span data-ttu-id="e9430-128">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="e9430-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e9430-129">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="e9430-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e9430-130">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="e9430-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e9430-131">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="e9430-131">Schema Name</span></span>  <br/> |<span data-ttu-id="e9430-132">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="e9430-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="e9430-133">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="e9430-133">Validation File</span></span>  <br/> |<span data-ttu-id="e9430-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e9430-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e9430-135">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="e9430-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="e9430-136">False</span><span class="sxs-lookup"><span data-stu-id="e9430-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e9430-137">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e9430-137">See also</span></span>



- [<span data-ttu-id="e9430-138">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="e9430-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

