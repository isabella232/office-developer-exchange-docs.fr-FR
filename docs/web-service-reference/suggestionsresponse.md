---
title: SuggestionsResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SuggestionsResponse
api_type:
- schema
ms.assetid: d25ca143-f80c-4458-b669-346fda29a5a7
description: L’élément SuggestionsResponse contient des données de suggestion et les informations de statut pour les suggestions de réunion demandée response.
ms.openlocfilehash: 614b58a1df8e340c6be468ccddd3b37537d32591
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838650"
---
# <a name="suggestionsresponse"></a><span data-ttu-id="d0a91-103">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="d0a91-103">SuggestionsResponse</span></span>

<span data-ttu-id="d0a91-104">L’élément **SuggestionsResponse** contient des données de suggestion et les informations de statut pour les suggestions de réunion demandée response.</span><span class="sxs-lookup"><span data-stu-id="d0a91-104">The **SuggestionsResponse** element contains response status information and suggestion data for requested meeting suggestions.</span></span> 
  
[<span data-ttu-id="d0a91-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="d0a91-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="d0a91-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="d0a91-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
```xml
<SuggestionsResponse>
   <ResponseMessage>...</ResponseMessage>
   <SuggestionDayResultArray>...</SuggestionDayResultArray>
</SuggestionsResponse>
```

 <span data-ttu-id="d0a91-107">**SuggestionsResponseType**</span><span class="sxs-lookup"><span data-stu-id="d0a91-107">**SuggestionsResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d0a91-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d0a91-108">Attributes and elements</span></span>

<span data-ttu-id="d0a91-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d0a91-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d0a91-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="d0a91-110">Attributes</span></span>

<span data-ttu-id="d0a91-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d0a91-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d0a91-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d0a91-112">Child elements</span></span>

|<span data-ttu-id="d0a91-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d0a91-113">**Element**</span></span>|<span data-ttu-id="d0a91-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="d0a91-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d0a91-115">ResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d0a91-115">ResponseMessage</span></span>](responsemessage.md) <br/> |<span data-ttu-id="d0a91-116">Fournit des informations descriptives concernant l’état de réponse.</span><span class="sxs-lookup"><span data-stu-id="d0a91-116">Provides descriptive information about the response status.</span></span>  <br/> |
|[<span data-ttu-id="d0a91-117">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="d0a91-117">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md) <br/> |<span data-ttu-id="d0a91-118">Contient un tableau de suggestions organisées par date de réunion.</span><span class="sxs-lookup"><span data-stu-id="d0a91-118">Contains an array of meeting suggestions organized by date.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d0a91-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d0a91-119">Parent elements</span></span>

|<span data-ttu-id="d0a91-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d0a91-120">**Element**</span></span>|<span data-ttu-id="d0a91-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="d0a91-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d0a91-122">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="d0a91-122">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md) <br/> |<span data-ttu-id="d0a91-123">Contient des informations de disponibilité de l’utilisateur demandé.</span><span class="sxs-lookup"><span data-stu-id="d0a91-123">Contains the requested users' availability information.</span></span>  <br/> <span data-ttu-id="d0a91-124">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="d0a91-124">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d0a91-125">Remarques</span><span class="sxs-lookup"><span data-stu-id="d0a91-125">Remarks</span></span>

<span data-ttu-id="d0a91-126">Cet élément n’est pas inclus dans une réponse GetUserAvailability si [SuggestionsViewOptions](suggestionsviewoptions.md) n’est pas définie dans le message de demande GetUserAvailability.</span><span class="sxs-lookup"><span data-stu-id="d0a91-126">This element is not included in a GetUserAvailability response if [SuggestionsViewOptions](suggestionsviewoptions.md) is not set in the GetUserAvailability request message.</span></span> 
  
<span data-ttu-id="d0a91-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="d0a91-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d0a91-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d0a91-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d0a91-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d0a91-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d0a91-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d0a91-130">Schema Name</span></span>  <br/> |<span data-ttu-id="d0a91-131">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="d0a91-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d0a91-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d0a91-132">Validation File</span></span>  <br/> |<span data-ttu-id="d0a91-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d0a91-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d0a91-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d0a91-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="d0a91-135">False</span><span class="sxs-lookup"><span data-stu-id="d0a91-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d0a91-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d0a91-136">See also</span></span>



[<span data-ttu-id="d0a91-137">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="d0a91-137">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="d0a91-138">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="d0a91-138">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="d0a91-139">Obtention de disponibilité de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="d0a91-139">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

