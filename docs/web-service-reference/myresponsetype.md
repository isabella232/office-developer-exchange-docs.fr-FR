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
description: L’élément MyResponseType contient l’état d’ou une réponse à un élément de calendrier.
ms.openlocfilehash: 3be900ed6d2932699e3e83a0bca2918c016eb689
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828497"
---
# <a name="myresponsetype"></a><span data-ttu-id="98443-103">MyResponseType</span><span class="sxs-lookup"><span data-stu-id="98443-103">MyResponseType</span></span>

<span data-ttu-id="98443-104">L’élément **MyResponseType** contient l’état d’ou une réponse à un élément de calendrier.</span><span class="sxs-lookup"><span data-stu-id="98443-104">The **MyResponseType** element contains the status of or response to a calendar item.</span></span> 
  
```xml
<MyResponseType/>
```

 <span data-ttu-id="98443-105">**ResponseTypeType**</span><span class="sxs-lookup"><span data-stu-id="98443-105">**ResponseTypeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="98443-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="98443-106">Attributes and elements</span></span>

<span data-ttu-id="98443-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="98443-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="98443-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="98443-108">Attributes</span></span>

<span data-ttu-id="98443-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="98443-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="98443-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="98443-110">Child elements</span></span>

<span data-ttu-id="98443-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="98443-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="98443-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="98443-112">Parent elements</span></span>

|<span data-ttu-id="98443-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="98443-113">**Element**</span></span>|<span data-ttu-id="98443-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="98443-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="98443-115">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="98443-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="98443-116">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="98443-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="98443-117">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="98443-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="98443-118">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="98443-118">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="98443-119">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="98443-119">Text value</span></span>

<span data-ttu-id="98443-120">Une valeur texte est requise.</span><span class="sxs-lookup"><span data-stu-id="98443-120">A text value is required.</span></span> <span data-ttu-id="98443-121">Les valeurs de texte possibles de cet élément sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="98443-121">The following are the possible text values for this element:</span></span>
  
- <span data-ttu-id="98443-122">Inconnu</span><span class="sxs-lookup"><span data-stu-id="98443-122">Unknown</span></span>
    
- <span data-ttu-id="98443-123">Organisateur</span><span class="sxs-lookup"><span data-stu-id="98443-123">Organizer</span></span>
    
- <span data-ttu-id="98443-124">Provisoire</span><span class="sxs-lookup"><span data-stu-id="98443-124">Tentative</span></span>
    
- <span data-ttu-id="98443-125">Accepter</span><span class="sxs-lookup"><span data-stu-id="98443-125">Accept</span></span>
    
- <span data-ttu-id="98443-126">Refuser</span><span class="sxs-lookup"><span data-stu-id="98443-126">Decline</span></span>
    
- <span data-ttu-id="98443-127">NoResponseReceived</span><span class="sxs-lookup"><span data-stu-id="98443-127">NoResponseReceived</span></span>
    
## <a name="remarks"></a><span data-ttu-id="98443-128">Remarques</span><span class="sxs-lookup"><span data-stu-id="98443-128">Remarks</span></span>

<span data-ttu-id="98443-129">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="98443-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="98443-130">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="98443-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="98443-131">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="98443-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="98443-132">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="98443-132">Schema name</span></span>  <br/> |<span data-ttu-id="98443-133">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="98443-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="98443-134">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="98443-134">Validation file</span></span>  <br/> |<span data-ttu-id="98443-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="98443-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="98443-136">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="98443-136">Can be empty</span></span>  <br/> |<span data-ttu-id="98443-137">False</span><span class="sxs-lookup"><span data-stu-id="98443-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="98443-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="98443-138">See also</span></span>



- [<span data-ttu-id="98443-139">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="98443-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

