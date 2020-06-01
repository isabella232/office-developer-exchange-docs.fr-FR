---
title: MaximumNonWorkHourResultsByDay
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MaximumNonWorkHourResultsByDay
api_type:
- schema
ms.assetid: 9fb7314d-779c-4b1f-9d7c-b5cb092ed134
description: L’élément MaximumNonWorkHourResultsByDay spécifie le nombre de résultats suggérés pour les heures de travail en dehors des heures ouvrées normales par jour.
ms.openlocfilehash: 410d6bd84838d979af6bc53ca47f445ae55a09e6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465498"
---
# <a name="maximumnonworkhourresultsbyday"></a><span data-ttu-id="9d627-103">MaximumNonWorkHourResultsByDay</span><span class="sxs-lookup"><span data-stu-id="9d627-103">MaximumNonWorkHourResultsByDay</span></span>

<span data-ttu-id="9d627-104">L’élément **MaximumNonWorkHourResultsByDay** spécifie le nombre de résultats suggérés pour les heures de travail en dehors des heures ouvrées normales par jour.</span><span class="sxs-lookup"><span data-stu-id="9d627-104">The **MaximumNonWorkHourResultsByDay** element specifies the number of suggested results for meeting times outside regular working hours per day.</span></span> 
  
[<span data-ttu-id="9d627-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="9d627-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="9d627-106">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="9d627-106">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md)
  
[<span data-ttu-id="9d627-107">MaximumNonWorkHourResultsByDay</span><span class="sxs-lookup"><span data-stu-id="9d627-107">MaximumNonWorkHourResultsByDay</span></span>](maximumnonworkhourresultsbyday.md)
  
```xml
<MaximumNonWorkHourResultsByDay>...</MaximumNonWorkHourResultsByDay>
```

 <span data-ttu-id="9d627-108">**int**</span><span class="sxs-lookup"><span data-stu-id="9d627-108">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9d627-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="9d627-109">Attributes and elements</span></span>

<span data-ttu-id="9d627-110">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="9d627-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9d627-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="9d627-111">Attributes</span></span>

<span data-ttu-id="9d627-112">Aucune.</span><span class="sxs-lookup"><span data-stu-id="9d627-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9d627-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="9d627-113">Child elements</span></span>

<span data-ttu-id="9d627-114">Aucun.</span><span class="sxs-lookup"><span data-stu-id="9d627-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9d627-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="9d627-115">Parent elements</span></span>

|<span data-ttu-id="9d627-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9d627-116">**Element**</span></span>|<span data-ttu-id="9d627-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="9d627-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9d627-118">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="9d627-118">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md) <br/> |<span data-ttu-id="9d627-119">Contient les options permettant d’obtenir des informations sur les suggestions de réunion.</span><span class="sxs-lookup"><span data-stu-id="9d627-119">Contains the options for obtaining meeting suggestion information.</span></span>  <br/> <span data-ttu-id="9d627-120">Voici le XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="9d627-120">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9d627-121">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="9d627-121">Text value</span></span>

<span data-ttu-id="9d627-122">Une valeur de texte est requise.</span><span class="sxs-lookup"><span data-stu-id="9d627-122">A text value is required.</span></span> <span data-ttu-id="9d627-123">La valeur texte représente un entier.</span><span class="sxs-lookup"><span data-stu-id="9d627-123">The text value represents an integer.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9d627-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="9d627-124">Remarks</span></span>

<span data-ttu-id="9d627-125">Cet élément est requis si l’élément [SuggestionsViewOptions](suggestionsviewoptions.md) est utilisé.</span><span class="sxs-lookup"><span data-stu-id="9d627-125">This element is required if the [SuggestionsViewOptions](suggestionsviewoptions.md) element is used.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="9d627-126">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="9d627-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="9d627-127">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="9d627-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9d627-128">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="9d627-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9d627-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="9d627-129">Schema Name</span></span>  <br/> |<span data-ttu-id="9d627-130">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="9d627-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="9d627-131">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="9d627-131">Validation File</span></span>  <br/> |<span data-ttu-id="9d627-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9d627-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9d627-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="9d627-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="9d627-134">False</span><span class="sxs-lookup"><span data-stu-id="9d627-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9d627-135">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="9d627-135">See also</span></span>



[<span data-ttu-id="9d627-136">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="9d627-136">GetUserAvailability operation</span></span>](getuseravailability-operation.md)


[<span data-ttu-id="9d627-137">Obtention de la disponibilité des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="9d627-137">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

