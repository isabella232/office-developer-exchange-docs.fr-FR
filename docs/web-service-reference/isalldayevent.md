---
title: IsAllDayEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsAllDayEvent
api_type:
- schema
ms.assetid: 29140a64-9d7a-4a14-a10d-c98197c9831b
description: L’élément IsAllDayEvent indique si une demande de réunion ou d’élément de calendrier représente une journée entière.
ms.openlocfilehash: 81cf1e7d8338275540f264de7cbf194005e7770c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827983"
---
# <a name="isalldayevent"></a><span data-ttu-id="d4565-103">IsAllDayEvent</span><span class="sxs-lookup"><span data-stu-id="d4565-103">IsAllDayEvent</span></span>

<span data-ttu-id="d4565-104">L’élément **IsAllDayEvent** indique si une demande de réunion ou d’élément de calendrier représente une journée entière.</span><span class="sxs-lookup"><span data-stu-id="d4565-104">The **IsAllDayEvent** element indicates whether a calendar item or meeting request represents an all-day event.</span></span> 
  
```xml
<IsAllDayEvent/>
```

 <span data-ttu-id="d4565-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="d4565-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d4565-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d4565-106">Attributes and elements</span></span>

<span data-ttu-id="d4565-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d4565-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d4565-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="d4565-108">Attributes</span></span>

<span data-ttu-id="d4565-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d4565-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d4565-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d4565-110">Child elements</span></span>

<span data-ttu-id="d4565-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d4565-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d4565-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d4565-112">Parent elements</span></span>

|<span data-ttu-id="d4565-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d4565-113">**Element**</span></span>|<span data-ttu-id="d4565-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="d4565-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d4565-115">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="d4565-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="d4565-116">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="d4565-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="d4565-117">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="d4565-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="d4565-118">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="d4565-118">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d4565-119">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="d4565-119">Text value</span></span>

<span data-ttu-id="d4565-120">Une valeur de texte qui représente une valeur Boolean est requise si cet élément est inclus.</span><span class="sxs-lookup"><span data-stu-id="d4565-120">A text value that represents a Boolean value is required if this element is included.</span></span> <span data-ttu-id="d4565-121">La valeur **true** indique que l’élément représente une journée entière.</span><span class="sxs-lookup"><span data-stu-id="d4565-121">A value of **true** indicates that the item represents an all-day event.</span></span> <span data-ttu-id="d4565-122">La valeur **false** indique que l’élément s’étend sur moins d’heures de travail d’un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="d4565-122">A value of **false** indicates that the item spans less than a user's working hours.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="d4565-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="d4565-123">Remarks</span></span>

<span data-ttu-id="d4565-124">Un événement d’une journée entière s’étend sur la durée des heures de travail qui est définie pour une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="d4565-124">An all-day event spans the duration of working hours that is defined for a mailbox.</span></span>
  
<span data-ttu-id="d4565-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="d4565-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d4565-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d4565-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d4565-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d4565-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d4565-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d4565-128">Schema name</span></span>  <br/> |<span data-ttu-id="d4565-129">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="d4565-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="d4565-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d4565-130">Validation file</span></span>  <br/> |<span data-ttu-id="d4565-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d4565-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d4565-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d4565-132">Can be empty</span></span>  <br/> |<span data-ttu-id="d4565-133">False</span><span class="sxs-lookup"><span data-stu-id="d4565-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d4565-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d4565-134">See also</span></span>



- [<span data-ttu-id="d4565-135">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="d4565-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

