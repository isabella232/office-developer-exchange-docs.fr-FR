---
title: MaximumResultsByDay
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MaximumResultsByDay
api_type:
- schema
ms.assetid: d581a12a-2b8e-4960-ae14-c8c4aa0b1849
description: L’élément MaximumResultsByDay Spécifie le nombre de répétitions de réunion proposée par un jour retourné dans la réponse.
ms.openlocfilehash: 69ab4e0b23f85e5b8786ba2dd934850cadc88f0e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828381"
---
# <a name="maximumresultsbyday"></a><span data-ttu-id="b3e19-103">MaximumResultsByDay</span><span class="sxs-lookup"><span data-stu-id="b3e19-103">MaximumResultsByDay</span></span>

<span data-ttu-id="b3e19-104">L’élément **MaximumResultsByDay** Spécifie le nombre de répétitions de réunion proposée par un jour retourné dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="b3e19-104">The **MaximumResultsByDay** element specifies the number of suggested meeting times per a day returned in the response.</span></span> 
  
[<span data-ttu-id="b3e19-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="b3e19-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="b3e19-106">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="b3e19-106">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md)
  
[<span data-ttu-id="b3e19-107">MaximumResultsByDay</span><span class="sxs-lookup"><span data-stu-id="b3e19-107">MaximumResultsByDay</span></span>](maximumresultsbyday.md)
  
```xml
<MaximumResultsByDay>...</MaximumResultsByDay>
```

<span data-ttu-id="b3e19-108">**int**</span><span class="sxs-lookup"><span data-stu-id="b3e19-108">**int**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="b3e19-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="b3e19-109">Attributes and elements</span></span>

<span data-ttu-id="b3e19-110">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="b3e19-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b3e19-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="b3e19-111">Attributes</span></span>

<span data-ttu-id="b3e19-112">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b3e19-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b3e19-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="b3e19-113">Child elements</span></span>

<span data-ttu-id="b3e19-114">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b3e19-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b3e19-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="b3e19-115">Parent elements</span></span>

|<span data-ttu-id="b3e19-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b3e19-116">**Element**</span></span>|<span data-ttu-id="b3e19-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="b3e19-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b3e19-118">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="b3e19-118">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md) <br/> |<span data-ttu-id="b3e19-119">Contient les options permettant d’obtenir des informations de suggestion de réunion.</span><span class="sxs-lookup"><span data-stu-id="b3e19-119">Contains the options for obtaining meeting suggestion information.</span></span>  <br/> <span data-ttu-id="b3e19-120">Vous trouverez ci-dessous le XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="b3e19-120">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b3e19-121">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="b3e19-121">Text value</span></span>

<span data-ttu-id="b3e19-122">Une valeur texte est requise.</span><span class="sxs-lookup"><span data-stu-id="b3e19-122">A text value is required.</span></span> <span data-ttu-id="b3e19-123">La valeur de texte représente un entier.</span><span class="sxs-lookup"><span data-stu-id="b3e19-123">The text value represents an integer.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b3e19-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="b3e19-124">Remarks</span></span>

<span data-ttu-id="b3e19-125">Cet élément est obligatoire si l’élément [SuggestionsViewOptions](suggestionsviewoptions.md) est utilisé.</span><span class="sxs-lookup"><span data-stu-id="b3e19-125">This element is required if the [SuggestionsViewOptions](suggestionsviewoptions.md) element is used.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="b3e19-126">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft® Exchange Server 2007 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="b3e19-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft® Exchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="b3e19-127">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="b3e19-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b3e19-128">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="b3e19-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b3e19-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="b3e19-129">Schema Name</span></span>  <br/> |<span data-ttu-id="b3e19-130">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="b3e19-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="b3e19-131">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="b3e19-131">Validation File</span></span>  <br/> |<span data-ttu-id="b3e19-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b3e19-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b3e19-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="b3e19-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="b3e19-134">False</span><span class="sxs-lookup"><span data-stu-id="b3e19-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b3e19-135">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b3e19-135">See also</span></span>

- [<span data-ttu-id="b3e19-136">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="b3e19-136">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="b3e19-137">Obtention de disponibilité de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="b3e19-137">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

