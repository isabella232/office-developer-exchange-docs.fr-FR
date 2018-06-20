---
title: DetailedSuggestionsWindow
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DetailedSuggestionsWindow
api_type:
- schema
ms.assetid: 7b348d63-6a7d-45f4-9562-5c42243d63a5
description: L’élément DetailedSuggestionsWindow identifie l’intervalle de temps qui est interrogé pour des informations détaillées sur les heures de réunion suggérée.
ms.openlocfilehash: 8a3af0178d0c96b50f4dd641716a9f7a7be8f7a2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755908"
---
# <a name="detailedsuggestionswindow"></a><span data-ttu-id="50391-103">DetailedSuggestionsWindow</span><span class="sxs-lookup"><span data-stu-id="50391-103">DetailedSuggestionsWindow</span></span>

<span data-ttu-id="50391-104">L’élément **DetailedSuggestionsWindow** identifie l’intervalle de temps qui est interrogé pour des informations détaillées sur les heures de réunion suggérée.</span><span class="sxs-lookup"><span data-stu-id="50391-104">The **DetailedSuggestionsWindow** element identifies the time span that is queried for detailed information about suggested meeting times.</span></span> 
  
- [<span data-ttu-id="50391-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="50391-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md) 
- [<span data-ttu-id="50391-106">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="50391-106">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md) 
- [<span data-ttu-id="50391-107">DetailedSuggestionsWindow</span><span class="sxs-lookup"><span data-stu-id="50391-107">DetailedSuggestionsWindow</span></span>](detailedsuggestionswindow.md)
  
```xml
<DetailedSuggestionsWindow>
   <StartTime>...</StartTime>
   <EndTime>...</EndTime>
</DetailedSuggestionsWindow>
```

 <span data-ttu-id="50391-108">**Durée**</span><span class="sxs-lookup"><span data-stu-id="50391-108">**Duration**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="50391-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="50391-109">Attributes and elements</span></span>

<span data-ttu-id="50391-110">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="50391-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="50391-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="50391-111">Attributes</span></span>

<span data-ttu-id="50391-112">Aucun.</span><span class="sxs-lookup"><span data-stu-id="50391-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="50391-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="50391-113">Child elements</span></span>

|<span data-ttu-id="50391-114">**Élément**</span><span class="sxs-lookup"><span data-stu-id="50391-114">**Element**</span></span>|<span data-ttu-id="50391-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="50391-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="50391-116">Heure de début</span><span class="sxs-lookup"><span data-stu-id="50391-116">StartTime</span></span>](starttime.md) <br/> |<span data-ttu-id="50391-117">Représente le début de la période effectuées et pour plus d’informations sur les heures de réunion suggérée.</span><span class="sxs-lookup"><span data-stu-id="50391-117">Represents the start of the time span queried for detailed information about suggested meeting times.</span></span>  <br/> |
|[<span data-ttu-id="50391-118">Heure de fin</span><span class="sxs-lookup"><span data-stu-id="50391-118">EndTime</span></span>](endtime.md) <br/> |<span data-ttu-id="50391-119">Représente la fin de la période effectuées et pour plus d’informations sur les heures de réunion suggérée.</span><span class="sxs-lookup"><span data-stu-id="50391-119">Represents the end of the time span queried for detailed information about suggested meeting times.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="50391-120">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="50391-120">Parent elements</span></span>

|<span data-ttu-id="50391-121">**Élément**</span><span class="sxs-lookup"><span data-stu-id="50391-121">**Element**</span></span>|<span data-ttu-id="50391-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="50391-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="50391-123">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="50391-123">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md) <br/> |<span data-ttu-id="50391-124">Contient les options permettant d’obtenir des informations de suggestion de réunion.</span><span class="sxs-lookup"><span data-stu-id="50391-124">Contains the options for obtaining meeting suggestion information.</span></span>  <br/> <span data-ttu-id="50391-125">Vous trouverez ci-dessous le XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="50391-125">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="50391-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="50391-126">Remarks</span></span>

<span data-ttu-id="50391-127">Cet élément n’est pas obligatoire.</span><span class="sxs-lookup"><span data-stu-id="50391-127">This element is not required.</span></span>
  
> [!NOTE]
> <span data-ttu-id="50391-128">Le schéma qui décrit cet élément se trouve dans le répertoire /EWS/ de l’ordinateur qui exécute MicrosoftExchange Server 2007 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="50391-128">The schema that describes this element is located in the /EWS/ directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="50391-129">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="50391-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="50391-130">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="50391-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="50391-131">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="50391-131">Schema Name</span></span>  <br/> |<span data-ttu-id="50391-132">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="50391-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="50391-133">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="50391-133">Validation File</span></span>  <br/> |<span data-ttu-id="50391-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="50391-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="50391-135">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="50391-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="50391-136">False</span><span class="sxs-lookup"><span data-stu-id="50391-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="50391-137">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="50391-137">See also</span></span>

- [<span data-ttu-id="50391-138">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="50391-138">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="50391-139">Obtention de disponibilité de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="50391-139">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

