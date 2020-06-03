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
description: L’élément DetailedSuggestionsWindow identifie l’intervalle de temps interrogé pour obtenir des informations détaillées sur les heures de réunion suggérées.
ms.openlocfilehash: 45d582f2642c0e3d8f6330b09946230c8842618d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467843"
---
# <a name="detailedsuggestionswindow"></a><span data-ttu-id="28052-103">DetailedSuggestionsWindow</span><span class="sxs-lookup"><span data-stu-id="28052-103">DetailedSuggestionsWindow</span></span>

<span data-ttu-id="28052-104">L’élément **DetailedSuggestionsWindow** identifie l’intervalle de temps interrogé pour obtenir des informations détaillées sur les heures de réunion suggérées.</span><span class="sxs-lookup"><span data-stu-id="28052-104">The **DetailedSuggestionsWindow** element identifies the time span that is queried for detailed information about suggested meeting times.</span></span> 
  
- [<span data-ttu-id="28052-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="28052-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md) 
- [<span data-ttu-id="28052-106">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="28052-106">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md) 
- [<span data-ttu-id="28052-107">DetailedSuggestionsWindow</span><span class="sxs-lookup"><span data-stu-id="28052-107">DetailedSuggestionsWindow</span></span>](detailedsuggestionswindow.md)
  
```xml
<DetailedSuggestionsWindow>
   <StartTime>...</StartTime>
   <EndTime>...</EndTime>
</DetailedSuggestionsWindow>
```

 <span data-ttu-id="28052-108">**Duration**</span><span class="sxs-lookup"><span data-stu-id="28052-108">**Duration**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="28052-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="28052-109">Attributes and elements</span></span>

<span data-ttu-id="28052-110">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="28052-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="28052-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="28052-111">Attributes</span></span>

<span data-ttu-id="28052-112">Aucune.</span><span class="sxs-lookup"><span data-stu-id="28052-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="28052-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="28052-113">Child elements</span></span>

|<span data-ttu-id="28052-114">**Élément**</span><span class="sxs-lookup"><span data-stu-id="28052-114">**Element**</span></span>|<span data-ttu-id="28052-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="28052-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="28052-116">StartTime</span><span class="sxs-lookup"><span data-stu-id="28052-116">StartTime</span></span>](starttime.md) <br/> |<span data-ttu-id="28052-117">Représente le début de la période interrogée pour obtenir des informations détaillées sur les heures de réunion suggérées.</span><span class="sxs-lookup"><span data-stu-id="28052-117">Represents the start of the time span queried for detailed information about suggested meeting times.</span></span>  <br/> |
|[<span data-ttu-id="28052-118">EndTime</span><span class="sxs-lookup"><span data-stu-id="28052-118">EndTime</span></span>](endtime.md) <br/> |<span data-ttu-id="28052-119">Représente la fin de la période interrogée pour obtenir des informations détaillées sur les heures de réunion suggérées.</span><span class="sxs-lookup"><span data-stu-id="28052-119">Represents the end of the time span queried for detailed information about suggested meeting times.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="28052-120">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="28052-120">Parent elements</span></span>

|<span data-ttu-id="28052-121">**Élément**</span><span class="sxs-lookup"><span data-stu-id="28052-121">**Element**</span></span>|<span data-ttu-id="28052-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="28052-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="28052-123">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="28052-123">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md) <br/> |<span data-ttu-id="28052-124">Contient les options permettant d’obtenir des informations sur les suggestions de réunion.</span><span class="sxs-lookup"><span data-stu-id="28052-124">Contains the options for obtaining meeting suggestion information.</span></span>  <br/> <span data-ttu-id="28052-125">Voici le XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="28052-125">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="28052-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="28052-126">Remarks</span></span>

<span data-ttu-id="28052-127">Cet élément n’est pas obligatoire.</span><span class="sxs-lookup"><span data-stu-id="28052-127">This element is not required.</span></span>
  
> [!NOTE]
> <span data-ttu-id="28052-128">Le schéma qui décrit cet élément se trouve dans le répertoire/EWS/de l’ordinateur exécutant MicrosoftExchange Server 2007 sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="28052-128">The schema that describes this element is located in the /EWS/ directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="28052-129">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="28052-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="28052-130">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="28052-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="28052-131">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="28052-131">Schema Name</span></span>  <br/> |<span data-ttu-id="28052-132">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="28052-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="28052-133">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="28052-133">Validation File</span></span>  <br/> |<span data-ttu-id="28052-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="28052-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="28052-135">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="28052-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="28052-136">False</span><span class="sxs-lookup"><span data-stu-id="28052-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="28052-137">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="28052-137">See also</span></span>

- [<span data-ttu-id="28052-138">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="28052-138">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="28052-139">Obtention de la disponibilité des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="28052-139">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

