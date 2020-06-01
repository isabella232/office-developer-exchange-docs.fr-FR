---
title: MyResponseType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MyResponseType
api_type:
- schema
ms.assetid: 9741b71d-a310-4520-81d5-3787a1ee630f
description: L’élément MyResponseType contient l’État ou la réponse à un élément de calendrier.
ms.openlocfilehash: 640b0595ac039cc3c119aa52aa6e791e5b695e87
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466625"
---
# <a name="myresponsetype"></a><span data-ttu-id="850d8-103">MyResponseType</span><span class="sxs-lookup"><span data-stu-id="850d8-103">MyResponseType</span></span>

<span data-ttu-id="850d8-104">L’élément **MyResponseType** contient l’État ou la réponse à un élément de calendrier.</span><span class="sxs-lookup"><span data-stu-id="850d8-104">The **MyResponseType** element contains the status of or response to a calendar item.</span></span> 
  
```xml
<MyResponseType/>
```

 <span data-ttu-id="850d8-105">**ResponseTypeType**</span><span class="sxs-lookup"><span data-stu-id="850d8-105">**ResponseTypeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="850d8-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="850d8-106">Attributes and elements</span></span>

<span data-ttu-id="850d8-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="850d8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="850d8-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="850d8-108">Attributes</span></span>

<span data-ttu-id="850d8-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="850d8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="850d8-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="850d8-110">Child elements</span></span>

<span data-ttu-id="850d8-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="850d8-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="850d8-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="850d8-112">Parent elements</span></span>

|<span data-ttu-id="850d8-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="850d8-113">**Element**</span></span>|<span data-ttu-id="850d8-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="850d8-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="850d8-115">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="850d8-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="850d8-116">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="850d8-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="850d8-117">Propriété meetingrequest</span><span class="sxs-lookup"><span data-stu-id="850d8-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="850d8-118">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="850d8-118">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="850d8-119">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="850d8-119">Text value</span></span>

<span data-ttu-id="850d8-120">Une valeur de texte est requise.</span><span class="sxs-lookup"><span data-stu-id="850d8-120">A text value is required.</span></span> <span data-ttu-id="850d8-121">Voici les valeurs de texte possibles pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="850d8-121">The following are the possible text values for this element:</span></span>
  
- <span data-ttu-id="850d8-122">Inconnu</span><span class="sxs-lookup"><span data-stu-id="850d8-122">Unknown</span></span>
    
- <span data-ttu-id="850d8-123">Organisateur</span><span class="sxs-lookup"><span data-stu-id="850d8-123">Organizer</span></span>
    
- <span data-ttu-id="850d8-124">Provisoire</span><span class="sxs-lookup"><span data-stu-id="850d8-124">Tentative</span></span>
    
- <span data-ttu-id="850d8-125">Accepter</span><span class="sxs-lookup"><span data-stu-id="850d8-125">Accept</span></span>
    
- <span data-ttu-id="850d8-126">Amortissement</span><span class="sxs-lookup"><span data-stu-id="850d8-126">Decline</span></span>
    
- <span data-ttu-id="850d8-127">NoResponseReceived</span><span class="sxs-lookup"><span data-stu-id="850d8-127">NoResponseReceived</span></span>
    
## <a name="remarks"></a><span data-ttu-id="850d8-128">Remarques</span><span class="sxs-lookup"><span data-stu-id="850d8-128">Remarks</span></span>

<span data-ttu-id="850d8-129">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="850d8-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="850d8-130">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="850d8-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="850d8-131">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="850d8-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="850d8-132">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="850d8-132">Schema name</span></span>  <br/> |<span data-ttu-id="850d8-133">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="850d8-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="850d8-134">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="850d8-134">Validation file</span></span>  <br/> |<span data-ttu-id="850d8-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="850d8-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="850d8-136">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="850d8-136">Can be empty</span></span>  <br/> |<span data-ttu-id="850d8-137">False</span><span class="sxs-lookup"><span data-stu-id="850d8-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="850d8-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="850d8-138">See also</span></span>



- [<span data-ttu-id="850d8-139">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="850d8-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

