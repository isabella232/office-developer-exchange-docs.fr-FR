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
description: L’élément SuggestionDayResultArray contient un tableau de suggestions de réunion organisées par date.
ms.openlocfilehash: 277d4cf71c31aba26cbff6f598eaa62769cae552
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457983"
---
# <a name="suggestiondayresultarray"></a><span data-ttu-id="5b347-103">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="5b347-103">SuggestionDayResultArray</span></span>

<span data-ttu-id="5b347-104">L’élément **SuggestionDayResultArray** contient un tableau de suggestions de réunion organisées par date.</span><span class="sxs-lookup"><span data-stu-id="5b347-104">The **SuggestionDayResultArray** element contains an array of meeting suggestions organized by date.</span></span> 
  
[<span data-ttu-id="5b347-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="5b347-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="5b347-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="5b347-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="5b347-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="5b347-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
```xml
<SuggestionDayResultArray>
   <SuggestionDayResult>...</SuggestionDayResult>
</SuggestionDayResultArray>
```

 <span data-ttu-id="5b347-108">**ArrayOfSuggestionDayResult**</span><span class="sxs-lookup"><span data-stu-id="5b347-108">**ArrayOfSuggestionDayResult**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5b347-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="5b347-109">Attributes and elements</span></span>

<span data-ttu-id="5b347-110">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="5b347-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5b347-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="5b347-111">Attributes</span></span>

<span data-ttu-id="5b347-112">Aucune.</span><span class="sxs-lookup"><span data-stu-id="5b347-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5b347-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="5b347-113">Child elements</span></span>

|<span data-ttu-id="5b347-114">**Élément**</span><span class="sxs-lookup"><span data-stu-id="5b347-114">**Element**</span></span>|<span data-ttu-id="5b347-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="5b347-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5b347-116">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="5b347-116">SuggestionDayResult</span></span>](suggestiondayresult.md) <br/> |<span data-ttu-id="5b347-117">Représente un jour qui contient des heures de réunion suggérées.</span><span class="sxs-lookup"><span data-stu-id="5b347-117">Represents a single day that contains suggested meeting times.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5b347-118">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="5b347-118">Parent elements</span></span>

|<span data-ttu-id="5b347-119">**Élément**</span><span class="sxs-lookup"><span data-stu-id="5b347-119">**Element**</span></span>|<span data-ttu-id="5b347-120">**Description**</span><span class="sxs-lookup"><span data-stu-id="5b347-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5b347-121">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="5b347-121">SuggestionsResponse</span></span>](suggestionsresponse.md) <br/> |<span data-ttu-id="5b347-122">Contient des informations de réponse et des suggestions de données pour les suggestions de réunion demandées</span><span class="sxs-lookup"><span data-stu-id="5b347-122">Contains response information and suggestion data for requested meeting suggestions</span></span>  <br/> <span data-ttu-id="5b347-123">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="5b347-123">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5b347-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="5b347-124">Remarks</span></span>

<span data-ttu-id="5b347-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="5b347-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5b347-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="5b347-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5b347-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="5b347-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5b347-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="5b347-128">Schema Name</span></span>  <br/> |<span data-ttu-id="5b347-129">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="5b347-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="5b347-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="5b347-130">Validation File</span></span>  <br/> |<span data-ttu-id="5b347-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="5b347-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5b347-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="5b347-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="5b347-133">False</span><span class="sxs-lookup"><span data-stu-id="5b347-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5b347-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="5b347-134">See also</span></span>



[<span data-ttu-id="5b347-135">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="5b347-135">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="5b347-136">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="5b347-136">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="5b347-137">Obtention de la disponibilité des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="5b347-137">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

