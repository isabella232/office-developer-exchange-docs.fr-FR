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
description: L’élément SuggestionsResponse contient les informations d’état de réponse et les données de suggestion pour les suggestions de réunion demandées.
ms.openlocfilehash: cba344f3f97777580c2cc6d296f110f20b550063
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466653"
---
# <a name="suggestionsresponse"></a><span data-ttu-id="2523c-103">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="2523c-103">SuggestionsResponse</span></span>

<span data-ttu-id="2523c-104">L’élément **SuggestionsResponse** contient les informations d’état de réponse et les données de suggestion pour les suggestions de réunion demandées.</span><span class="sxs-lookup"><span data-stu-id="2523c-104">The **SuggestionsResponse** element contains response status information and suggestion data for requested meeting suggestions.</span></span> 
  
[<span data-ttu-id="2523c-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="2523c-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="2523c-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="2523c-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
```xml
<SuggestionsResponse>
   <ResponseMessage>...</ResponseMessage>
   <SuggestionDayResultArray>...</SuggestionDayResultArray>
</SuggestionsResponse>
```

 <span data-ttu-id="2523c-107">**SuggestionsResponseType**</span><span class="sxs-lookup"><span data-stu-id="2523c-107">**SuggestionsResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2523c-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="2523c-108">Attributes and elements</span></span>

<span data-ttu-id="2523c-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="2523c-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2523c-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="2523c-110">Attributes</span></span>

<span data-ttu-id="2523c-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="2523c-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2523c-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="2523c-112">Child elements</span></span>

|<span data-ttu-id="2523c-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2523c-113">**Element**</span></span>|<span data-ttu-id="2523c-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="2523c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2523c-115">ResponseMessage</span><span class="sxs-lookup"><span data-stu-id="2523c-115">ResponseMessage</span></span>](responsemessage.md) <br/> |<span data-ttu-id="2523c-116">Fournit des informations descriptives sur l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="2523c-116">Provides descriptive information about the response status.</span></span>  <br/> |
|[<span data-ttu-id="2523c-117">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="2523c-117">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md) <br/> |<span data-ttu-id="2523c-118">Contient un tableau des suggestions de réunion organisées par date.</span><span class="sxs-lookup"><span data-stu-id="2523c-118">Contains an array of meeting suggestions organized by date.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2523c-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="2523c-119">Parent elements</span></span>

|<span data-ttu-id="2523c-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2523c-120">**Element**</span></span>|<span data-ttu-id="2523c-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="2523c-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2523c-122">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="2523c-122">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md) <br/> |<span data-ttu-id="2523c-123">Contient les informations de disponibilité des utilisateurs demandés.</span><span class="sxs-lookup"><span data-stu-id="2523c-123">Contains the requested users' availability information.</span></span>  <br/> <span data-ttu-id="2523c-124">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="2523c-124">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2523c-125">Remarques</span><span class="sxs-lookup"><span data-stu-id="2523c-125">Remarks</span></span>

<span data-ttu-id="2523c-126">Cet élément n’est pas inclus dans une réponse GetUserAvailability si [SuggestionsViewOptions](suggestionsviewoptions.md) n’est pas défini dans le message de demande GetUserAvailability.</span><span class="sxs-lookup"><span data-stu-id="2523c-126">This element is not included in a GetUserAvailability response if [SuggestionsViewOptions](suggestionsviewoptions.md) is not set in the GetUserAvailability request message.</span></span> 
  
<span data-ttu-id="2523c-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="2523c-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2523c-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="2523c-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2523c-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="2523c-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2523c-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="2523c-130">Schema Name</span></span>  <br/> |<span data-ttu-id="2523c-131">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="2523c-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="2523c-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="2523c-132">Validation File</span></span>  <br/> |<span data-ttu-id="2523c-133">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="2523c-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2523c-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="2523c-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="2523c-135">False</span><span class="sxs-lookup"><span data-stu-id="2523c-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2523c-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="2523c-136">See also</span></span>



[<span data-ttu-id="2523c-137">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="2523c-137">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="2523c-138">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="2523c-138">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="2523c-139">Obtention de la disponibilité des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="2523c-139">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

