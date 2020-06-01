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
ms.openlocfilehash: fd72766977567210cd08b47d0723cd73aa53a622
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465967"
---
# <a name="ismeeting"></a><span data-ttu-id="5f3a9-103">IsMeeting</span><span class="sxs-lookup"><span data-stu-id="5f3a9-103">IsMeeting</span></span>

<span data-ttu-id="5f3a9-104">L’élément **IsMeeting** indique si l’élément de calendrier est une réunion ou un rendez-vous.</span><span class="sxs-lookup"><span data-stu-id="5f3a9-104">The **IsMeeting** element indicates whether the calendar item is a meeting or an appointment.</span></span> 
  
```xml
<IsMeeting/>
```

 <span data-ttu-id="5f3a9-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="5f3a9-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5f3a9-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="5f3a9-106">Attributes and elements</span></span>

<span data-ttu-id="5f3a9-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="5f3a9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5f3a9-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="5f3a9-108">Attributes</span></span>

<span data-ttu-id="5f3a9-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="5f3a9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5f3a9-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="5f3a9-110">Child elements</span></span>

<span data-ttu-id="5f3a9-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="5f3a9-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5f3a9-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="5f3a9-112">Parent elements</span></span>

|<span data-ttu-id="5f3a9-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="5f3a9-113">**Element**</span></span>|<span data-ttu-id="5f3a9-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="5f3a9-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5f3a9-115">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="5f3a9-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="5f3a9-116">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="5f3a9-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="5f3a9-117">Propriété meetingrequest</span><span class="sxs-lookup"><span data-stu-id="5f3a9-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="5f3a9-118">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="5f3a9-118">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5f3a9-119">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="5f3a9-119">Text value</span></span>

<span data-ttu-id="5f3a9-120">Une valeur de texte qui représente une valeur booléenne est requise si cet élément est inclus.</span><span class="sxs-lookup"><span data-stu-id="5f3a9-120">A text value that represents a Boolean value is required if this element is included.</span></span> <span data-ttu-id="5f3a9-121">La valeur **true** indique que l’élément de calendrier est une réunion.</span><span class="sxs-lookup"><span data-stu-id="5f3a9-121">A value of **true** indicates that the calendar item is a meeting.</span></span> <span data-ttu-id="5f3a9-122">La valeur **false** indique que l’élément de calendrier est un rendez-vous.</span><span class="sxs-lookup"><span data-stu-id="5f3a9-122">A value of **false** indicates that the calendar item is an appointment.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="5f3a9-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="5f3a9-123">Remarks</span></span>

<span data-ttu-id="5f3a9-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="5f3a9-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5f3a9-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="5f3a9-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5f3a9-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="5f3a9-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5f3a9-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="5f3a9-127">Schema name</span></span>  <br/> |<span data-ttu-id="5f3a9-128">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="5f3a9-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="5f3a9-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="5f3a9-129">Validation file</span></span>  <br/> |<span data-ttu-id="5f3a9-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="5f3a9-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5f3a9-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="5f3a9-131">Can be empty</span></span>  <br/> |<span data-ttu-id="5f3a9-132">False</span><span class="sxs-lookup"><span data-stu-id="5f3a9-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5f3a9-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="5f3a9-133">See also</span></span>



- [<span data-ttu-id="5f3a9-134">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="5f3a9-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

