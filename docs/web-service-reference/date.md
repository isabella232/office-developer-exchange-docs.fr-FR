---
title: Date
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Date
api_type:
- schema
ms.assetid: 2f6bc090-fff4-45b1-8d7e-8fd6e060cce2
description: L’élément Date représente la date qui contient les heures de réunion suggérées.
ms.openlocfilehash: bcc152ed6aba94907189b5579b998815be45db16
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44443787"
---
# <a name="date"></a><span data-ttu-id="de54b-103">Date</span><span class="sxs-lookup"><span data-stu-id="de54b-103">Date</span></span>

<span data-ttu-id="de54b-104">L’élément **Date** représente la date qui contient les heures de réunion suggérées.</span><span class="sxs-lookup"><span data-stu-id="de54b-104">The **Date** element represents the date that contains the suggested meeting times.</span></span> 
  
- [<span data-ttu-id="de54b-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="de54b-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md) 
- [<span data-ttu-id="de54b-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="de54b-106">SuggestionsResponse</span></span>](suggestionsresponse.md) 
- [<span data-ttu-id="de54b-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="de54b-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)  
- [<span data-ttu-id="de54b-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="de54b-108">SuggestionDayResult</span></span>](suggestiondayresult.md)  
- [<span data-ttu-id="de54b-109">Date</span><span class="sxs-lookup"><span data-stu-id="de54b-109">Date</span></span>](date.md)
  
```xml
<Date>...</Date>
```

<span data-ttu-id="de54b-110">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="de54b-110">**dateTime**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="de54b-111">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="de54b-111">Attributes and elements</span></span>

<span data-ttu-id="de54b-112">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="de54b-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="de54b-113">Attributs</span><span class="sxs-lookup"><span data-stu-id="de54b-113">Attributes</span></span>

<span data-ttu-id="de54b-114">Aucune.</span><span class="sxs-lookup"><span data-stu-id="de54b-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="de54b-115">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="de54b-115">Child elements</span></span>

<span data-ttu-id="de54b-116">Aucun.</span><span class="sxs-lookup"><span data-stu-id="de54b-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="de54b-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="de54b-117">Parent elements</span></span>

|<span data-ttu-id="de54b-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="de54b-118">**Element**</span></span>|<span data-ttu-id="de54b-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="de54b-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="de54b-120">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="de54b-120">SuggestionDayResult</span></span>](suggestiondayresult.md) <br/> |<span data-ttu-id="de54b-121">Représente un jour qui contient des heures de réunion suggérées.</span><span class="sxs-lookup"><span data-stu-id="de54b-121">Represents a single day that contains suggested meeting times.</span></span>  <br/><br/><span data-ttu-id="de54b-122">Voici l’expression XPath 2,0 pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="de54b-122">The following is the XPath 2.0 expression to this element:</span></span><br/><br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="de54b-123">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="de54b-123">Text value</span></span>

<span data-ttu-id="de54b-124">Une valeur de texte est requise.</span><span class="sxs-lookup"><span data-stu-id="de54b-124">A text value is required.</span></span> <span data-ttu-id="de54b-125">Consultez les recommandations relatives aux types de données du schéma W3C (World Wide Web Consortium) pour le format du type de données primitif dateTime.</span><span class="sxs-lookup"><span data-stu-id="de54b-125">Review the World Wide Web Consortium (W3C) schema datatype recommendations for the format of the dateTime primitive datatype.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="de54b-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="de54b-126">Remarks</span></span>

<span data-ttu-id="de54b-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="de54b-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="de54b-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="de54b-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="de54b-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="de54b-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="de54b-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="de54b-130">Schema Name</span></span>  <br/> |<span data-ttu-id="de54b-131">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="de54b-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="de54b-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="de54b-132">Validation File</span></span>  <br/> |<span data-ttu-id="de54b-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="de54b-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="de54b-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="de54b-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="de54b-135">False</span><span class="sxs-lookup"><span data-stu-id="de54b-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="de54b-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="de54b-136">See also</span></span>

- [<span data-ttu-id="de54b-137">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="de54b-137">GetUserAvailability operation</span></span>](getuseravailability-operation.md) 
- [<span data-ttu-id="de54b-138">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="de54b-138">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
- [<span data-ttu-id="de54b-139">Obtention de la disponibilité des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="de54b-139">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

