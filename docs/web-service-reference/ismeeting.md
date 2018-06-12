---
title: IsMeeting
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsMeeting
api_type:
- schema
ms.assetid: 6ce22f17-7a31-46c4-b643-0894d087e852
description: L’élément IsMeeting indique si l’élément de calendrier est une réunion ou un rendez-vous.
ms.openlocfilehash: bb1349a8690450882e6beac0ccd84a8d03272a7d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828051"
---
# <a name="ismeeting"></a><span data-ttu-id="ec322-103">IsMeeting</span><span class="sxs-lookup"><span data-stu-id="ec322-103">IsMeeting</span></span>

<span data-ttu-id="ec322-104">L’élément **IsMeeting** indique si l’élément de calendrier est une réunion ou un rendez-vous.</span><span class="sxs-lookup"><span data-stu-id="ec322-104">The **IsMeeting** element indicates whether the calendar item is a meeting or an appointment.</span></span> 
  
```xml
<IsMeeting/>
```

 <span data-ttu-id="ec322-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="ec322-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ec322-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ec322-106">Attributes and elements</span></span>

<span data-ttu-id="ec322-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ec322-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ec322-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="ec322-108">Attributes</span></span>

<span data-ttu-id="ec322-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ec322-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ec322-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ec322-110">Child elements</span></span>

<span data-ttu-id="ec322-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ec322-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ec322-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ec322-112">Parent elements</span></span>

|<span data-ttu-id="ec322-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ec322-113">**Element**</span></span>|<span data-ttu-id="ec322-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="ec322-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ec322-115">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="ec322-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="ec322-116">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="ec322-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="ec322-117">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="ec322-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="ec322-118">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="ec322-118">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ec322-119">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="ec322-119">Text value</span></span>

<span data-ttu-id="ec322-120">Une valeur de texte qui représente une valeur Boolean est requise si cet élément est inclus.</span><span class="sxs-lookup"><span data-stu-id="ec322-120">A text value that represents a Boolean value is required if this element is included.</span></span> <span data-ttu-id="ec322-121">La valeur **true** indique que l’élément de calendrier est une réunion.</span><span class="sxs-lookup"><span data-stu-id="ec322-121">A value of **true** indicates that the calendar item is a meeting.</span></span> <span data-ttu-id="ec322-122">La valeur **false** indique que l’élément de calendrier est un rendez-vous.</span><span class="sxs-lookup"><span data-stu-id="ec322-122">A value of **false** indicates that the calendar item is an appointment.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="ec322-123">Note</span><span class="sxs-lookup"><span data-stu-id="ec322-123">Remarks</span></span>

<span data-ttu-id="ec322-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="ec322-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ec322-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ec322-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ec322-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ec322-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ec322-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ec322-127">Schema name</span></span>  <br/> |<span data-ttu-id="ec322-128">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="ec322-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="ec322-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ec322-129">Validation file</span></span>  <br/> |<span data-ttu-id="ec322-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ec322-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ec322-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ec322-131">Can be empty</span></span>  <br/> |<span data-ttu-id="ec322-132">False</span><span class="sxs-lookup"><span data-stu-id="ec322-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ec322-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ec322-133">See also</span></span>



- [<span data-ttu-id="ec322-134">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ec322-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

