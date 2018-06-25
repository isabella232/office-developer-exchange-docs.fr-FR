---
title: SuggestionDayResultArray
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SuggestionDayResultArray
api_type:
- schema
ms.assetid: eeba9eff-5eca-4002-b5a5-8fb794feaba1
description: L’élément SuggestionDayResultArray contient un tableau de suggestions organisées par date de réunion.
ms.openlocfilehash: c208104356606a5d9961461ad8743a772d2410d8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838649"
---
# <a name="suggestiondayresultarray"></a><span data-ttu-id="f8aef-103">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="f8aef-103">SuggestionDayResultArray</span></span>

<span data-ttu-id="f8aef-104">L’élément **SuggestionDayResultArray** contient un tableau de suggestions organisées par date de réunion.</span><span class="sxs-lookup"><span data-stu-id="f8aef-104">The **SuggestionDayResultArray** element contains an array of meeting suggestions organized by date.</span></span> 
  
[<span data-ttu-id="f8aef-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="f8aef-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="f8aef-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="f8aef-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="f8aef-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="f8aef-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
```xml
<SuggestionDayResultArray>
   <SuggestionDayResult>...</SuggestionDayResult>
</SuggestionDayResultArray>
```

 <span data-ttu-id="f8aef-108">**ArrayOfSuggestionDayResult**</span><span class="sxs-lookup"><span data-stu-id="f8aef-108">**ArrayOfSuggestionDayResult**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f8aef-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f8aef-109">Attributes and elements</span></span>

<span data-ttu-id="f8aef-110">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f8aef-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f8aef-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="f8aef-111">Attributes</span></span>

<span data-ttu-id="f8aef-112">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f8aef-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f8aef-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f8aef-113">Child elements</span></span>

|<span data-ttu-id="f8aef-114">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f8aef-114">**Element**</span></span>|<span data-ttu-id="f8aef-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="f8aef-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f8aef-116">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="f8aef-116">SuggestionDayResult</span></span>](suggestiondayresult.md) <br/> |<span data-ttu-id="f8aef-117">Représente un seul jour qui contient les heures de réunion proposée.</span><span class="sxs-lookup"><span data-stu-id="f8aef-117">Represents a single day that contains suggested meeting times.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f8aef-118">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f8aef-118">Parent elements</span></span>

|<span data-ttu-id="f8aef-119">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f8aef-119">**Element**</span></span>|<span data-ttu-id="f8aef-120">**Description**</span><span class="sxs-lookup"><span data-stu-id="f8aef-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f8aef-121">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="f8aef-121">SuggestionsResponse</span></span>](suggestionsresponse.md) <br/> |<span data-ttu-id="f8aef-122">Contient des données de suggestion et les informations de réponse pour la demande de suggestions de réunion</span><span class="sxs-lookup"><span data-stu-id="f8aef-122">Contains response information and suggestion data for requested meeting suggestions</span></span>  <br/> <span data-ttu-id="f8aef-123">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="f8aef-123">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f8aef-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="f8aef-124">Remarks</span></span>

<span data-ttu-id="f8aef-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="f8aef-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f8aef-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f8aef-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f8aef-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f8aef-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f8aef-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f8aef-128">Schema Name</span></span>  <br/> |<span data-ttu-id="f8aef-129">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="f8aef-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f8aef-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="f8aef-130">Validation File</span></span>  <br/> |<span data-ttu-id="f8aef-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="f8aef-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f8aef-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f8aef-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="f8aef-133">False</span><span class="sxs-lookup"><span data-stu-id="f8aef-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f8aef-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f8aef-134">See also</span></span>



[<span data-ttu-id="f8aef-135">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="f8aef-135">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="f8aef-136">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="f8aef-136">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="f8aef-137">Obtention de disponibilité de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="f8aef-137">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

