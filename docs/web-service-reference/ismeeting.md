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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465967"
---
# <a name="ismeeting"></a><span data-ttu-id="adb35-103">IsMeeting</span><span class="sxs-lookup"><span data-stu-id="adb35-103">IsMeeting</span></span>

<span data-ttu-id="adb35-104">L’élément **IsMeeting** indique si l’élément de calendrier est une réunion ou un rendez-vous.</span><span class="sxs-lookup"><span data-stu-id="adb35-104">The **IsMeeting** element indicates whether the calendar item is a meeting or an appointment.</span></span> 
  
```xml
<IsMeeting/>
```

 <span data-ttu-id="adb35-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="adb35-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="adb35-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="adb35-106">Attributes and elements</span></span>

<span data-ttu-id="adb35-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="adb35-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="adb35-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="adb35-108">Attributes</span></span>

<span data-ttu-id="adb35-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="adb35-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="adb35-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="adb35-110">Child elements</span></span>

<span data-ttu-id="adb35-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="adb35-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="adb35-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="adb35-112">Parent elements</span></span>

|<span data-ttu-id="adb35-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="adb35-113">**Element**</span></span>|<span data-ttu-id="adb35-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="adb35-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="adb35-115">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="adb35-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="adb35-116">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="adb35-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="adb35-117">Propriété meetingrequest</span><span class="sxs-lookup"><span data-stu-id="adb35-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="adb35-118">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="adb35-118">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="adb35-119">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="adb35-119">Text value</span></span>

<span data-ttu-id="adb35-120">Une valeur de texte qui représente une valeur booléenne est requise si cet élément est inclus.</span><span class="sxs-lookup"><span data-stu-id="adb35-120">A text value that represents a Boolean value is required if this element is included.</span></span> <span data-ttu-id="adb35-121">La valeur **true** indique que l’élément de calendrier est une réunion.</span><span class="sxs-lookup"><span data-stu-id="adb35-121">A value of **true** indicates that the calendar item is a meeting.</span></span> <span data-ttu-id="adb35-122">La valeur **false** indique que l’élément de calendrier est un rendez-vous.</span><span class="sxs-lookup"><span data-stu-id="adb35-122">A value of **false** indicates that the calendar item is an appointment.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="adb35-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="adb35-123">Remarks</span></span>

<span data-ttu-id="adb35-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="adb35-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="adb35-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="adb35-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="adb35-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="adb35-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="adb35-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="adb35-127">Schema name</span></span>  <br/> |<span data-ttu-id="adb35-128">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="adb35-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="adb35-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="adb35-129">Validation file</span></span>  <br/> |<span data-ttu-id="adb35-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="adb35-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="adb35-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="adb35-131">Can be empty</span></span>  <br/> |<span data-ttu-id="adb35-132">False</span><span class="sxs-lookup"><span data-stu-id="adb35-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="adb35-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="adb35-133">See also</span></span>



- [<span data-ttu-id="adb35-134">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="adb35-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

