---
title: IsCancelled
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsCancelled
api_type:
- schema
ms.assetid: 50c1e97f-2913-47a1-8457-60428a3c5b92
description: L’élément IsCancelled indique si un rendez-vous ou une réunion a été annulée.
ms.openlocfilehash: 594b8a9ccb535f074a8cf1da060373f640231a29
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827993"
---
# <a name="iscancelled"></a><span data-ttu-id="a0cf6-103">IsCancelled</span><span class="sxs-lookup"><span data-stu-id="a0cf6-103">IsCancelled</span></span>

<span data-ttu-id="a0cf6-104">L’élément **IsCancelled** indique si un rendez-vous ou une réunion a été annulée.</span><span class="sxs-lookup"><span data-stu-id="a0cf6-104">The **IsCancelled** element indicates whether an appointment or meeting has been canceled.</span></span> 
  
```xml
<IsCancelled/>
```

 <span data-ttu-id="a0cf6-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="a0cf6-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a0cf6-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a0cf6-106">Attributes and elements</span></span>

<span data-ttu-id="a0cf6-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a0cf6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a0cf6-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="a0cf6-108">Attributes</span></span>

<span data-ttu-id="a0cf6-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a0cf6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a0cf6-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a0cf6-110">Child elements</span></span>

<span data-ttu-id="a0cf6-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a0cf6-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a0cf6-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a0cf6-112">Parent elements</span></span>

|<span data-ttu-id="a0cf6-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a0cf6-113">**Element**</span></span>|<span data-ttu-id="a0cf6-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="a0cf6-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a0cf6-115">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="a0cf6-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="a0cf6-116">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="a0cf6-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="a0cf6-117">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="a0cf6-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="a0cf6-118">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="a0cf6-118">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a0cf6-119">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="a0cf6-119">Text value</span></span>

<span data-ttu-id="a0cf6-120">Une valeur de texte qui représente une valeur Boolean est requise si cet élément est inclus.</span><span class="sxs-lookup"><span data-stu-id="a0cf6-120">A text value that represents a Boolean value is required if this element is included.</span></span> <span data-ttu-id="a0cf6-121">La valeur **true** indique que l’élément de calendrier a été annulée.</span><span class="sxs-lookup"><span data-stu-id="a0cf6-121">A value of **true** indicates that the calendar item has been canceled.</span></span> <span data-ttu-id="a0cf6-122">La valeur **false** indique qu’un élément de calendrier n’a pas été annulé.</span><span class="sxs-lookup"><span data-stu-id="a0cf6-122">A value of **false** indicates that a calendar item has not been canceled.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="a0cf6-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="a0cf6-123">Remarks</span></span>

<span data-ttu-id="a0cf6-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="a0cf6-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a0cf6-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a0cf6-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a0cf6-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a0cf6-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a0cf6-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a0cf6-127">Schema name</span></span>  <br/> |<span data-ttu-id="a0cf6-128">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="a0cf6-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="a0cf6-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="a0cf6-129">Validation file</span></span>  <br/> |<span data-ttu-id="a0cf6-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a0cf6-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a0cf6-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a0cf6-131">Can be empty</span></span>  <br/> |<span data-ttu-id="a0cf6-132">False</span><span class="sxs-lookup"><span data-stu-id="a0cf6-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a0cf6-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a0cf6-133">See also</span></span>



- [<span data-ttu-id="a0cf6-134">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="a0cf6-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

