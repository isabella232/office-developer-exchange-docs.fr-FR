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
description: L’élément MaximumResultsByDay spécifie le nombre de réunions suggérées par jour renvoyées dans la réponse.
ms.openlocfilehash: 46d5c35a83034b8b968901fbc4ee57d046b6c164
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468417"
---
# <a name="maximumresultsbyday"></a><span data-ttu-id="6137b-103">MaximumResultsByDay</span><span class="sxs-lookup"><span data-stu-id="6137b-103">MaximumResultsByDay</span></span>

<span data-ttu-id="6137b-104">L’élément **MaximumResultsByDay** spécifie le nombre de réunions suggérées par jour renvoyées dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="6137b-104">The **MaximumResultsByDay** element specifies the number of suggested meeting times per a day returned in the response.</span></span> 
  
[<span data-ttu-id="6137b-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="6137b-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="6137b-106">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="6137b-106">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md)
  
[<span data-ttu-id="6137b-107">MaximumResultsByDay</span><span class="sxs-lookup"><span data-stu-id="6137b-107">MaximumResultsByDay</span></span>](maximumresultsbyday.md)
  
```xml
<MaximumResultsByDay>...</MaximumResultsByDay>
```

<span data-ttu-id="6137b-108">**int**</span><span class="sxs-lookup"><span data-stu-id="6137b-108">**int**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="6137b-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="6137b-109">Attributes and elements</span></span>

<span data-ttu-id="6137b-110">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="6137b-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6137b-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="6137b-111">Attributes</span></span>

<span data-ttu-id="6137b-112">Aucune.</span><span class="sxs-lookup"><span data-stu-id="6137b-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6137b-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="6137b-113">Child elements</span></span>

<span data-ttu-id="6137b-114">Aucun.</span><span class="sxs-lookup"><span data-stu-id="6137b-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6137b-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="6137b-115">Parent elements</span></span>

|<span data-ttu-id="6137b-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="6137b-116">**Element**</span></span>|<span data-ttu-id="6137b-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="6137b-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6137b-118">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="6137b-118">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md) <br/> |<span data-ttu-id="6137b-119">Contient les options permettant d’obtenir des informations sur les suggestions de réunion.</span><span class="sxs-lookup"><span data-stu-id="6137b-119">Contains the options for obtaining meeting suggestion information.</span></span>  <br/> <span data-ttu-id="6137b-120">Voici le XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="6137b-120">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6137b-121">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="6137b-121">Text value</span></span>

<span data-ttu-id="6137b-122">Une valeur de texte est requise.</span><span class="sxs-lookup"><span data-stu-id="6137b-122">A text value is required.</span></span> <span data-ttu-id="6137b-123">La valeur texte représente un entier.</span><span class="sxs-lookup"><span data-stu-id="6137b-123">The text value represents an integer.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6137b-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="6137b-124">Remarks</span></span>

<span data-ttu-id="6137b-125">Cet élément est requis si l’élément [SuggestionsViewOptions](suggestionsviewoptions.md) est utilisé.</span><span class="sxs-lookup"><span data-stu-id="6137b-125">This element is required if the [SuggestionsViewOptions](suggestionsviewoptions.md) element is used.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="6137b-126">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur exécutant Microsoft® Exchange Server 2007 sur lequel le rôle serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="6137b-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft® Exchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="6137b-127">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="6137b-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6137b-128">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="6137b-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6137b-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="6137b-129">Schema Name</span></span>  <br/> |<span data-ttu-id="6137b-130">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="6137b-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="6137b-131">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="6137b-131">Validation File</span></span>  <br/> |<span data-ttu-id="6137b-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6137b-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6137b-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="6137b-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="6137b-134">False</span><span class="sxs-lookup"><span data-stu-id="6137b-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6137b-135">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="6137b-135">See also</span></span>

- [<span data-ttu-id="6137b-136">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="6137b-136">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="6137b-137">Obtention de la disponibilité des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="6137b-137">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

