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
description: L’élément IsCancelled indique si un rendez-vous ou une réunion a été annulé.
ms.openlocfilehash: 946c9d956da9cf31e9fa08d4ab6f4950b11214b9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455568"
---
# <a name="iscancelled"></a><span data-ttu-id="310f0-103">IsCancelled</span><span class="sxs-lookup"><span data-stu-id="310f0-103">IsCancelled</span></span>

<span data-ttu-id="310f0-104">L’élément **IsCancelled** indique si un rendez-vous ou une réunion a été annulé.</span><span class="sxs-lookup"><span data-stu-id="310f0-104">The **IsCancelled** element indicates whether an appointment or meeting has been canceled.</span></span> 
  
```xml
<IsCancelled/>
```

 <span data-ttu-id="310f0-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="310f0-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="310f0-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="310f0-106">Attributes and elements</span></span>

<span data-ttu-id="310f0-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="310f0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="310f0-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="310f0-108">Attributes</span></span>

<span data-ttu-id="310f0-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="310f0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="310f0-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="310f0-110">Child elements</span></span>

<span data-ttu-id="310f0-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="310f0-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="310f0-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="310f0-112">Parent elements</span></span>

|<span data-ttu-id="310f0-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="310f0-113">**Element**</span></span>|<span data-ttu-id="310f0-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="310f0-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="310f0-115">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="310f0-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="310f0-116">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="310f0-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="310f0-117">Propriété meetingrequest</span><span class="sxs-lookup"><span data-stu-id="310f0-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="310f0-118">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="310f0-118">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="310f0-119">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="310f0-119">Text value</span></span>

<span data-ttu-id="310f0-120">Une valeur de texte qui représente une valeur booléenne est requise si cet élément est inclus.</span><span class="sxs-lookup"><span data-stu-id="310f0-120">A text value that represents a Boolean value is required if this element is included.</span></span> <span data-ttu-id="310f0-121">La valeur **true** indique que l’élément de calendrier a été annulé.</span><span class="sxs-lookup"><span data-stu-id="310f0-121">A value of **true** indicates that the calendar item has been canceled.</span></span> <span data-ttu-id="310f0-122">La valeur **false** indique qu’un élément de calendrier n’a pas été annulé.</span><span class="sxs-lookup"><span data-stu-id="310f0-122">A value of **false** indicates that a calendar item has not been canceled.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="310f0-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="310f0-123">Remarks</span></span>

<span data-ttu-id="310f0-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="310f0-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="310f0-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="310f0-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="310f0-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="310f0-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="310f0-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="310f0-127">Schema name</span></span>  <br/> |<span data-ttu-id="310f0-128">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="310f0-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="310f0-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="310f0-129">Validation file</span></span>  <br/> |<span data-ttu-id="310f0-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="310f0-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="310f0-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="310f0-131">Can be empty</span></span>  <br/> |<span data-ttu-id="310f0-132">False</span><span class="sxs-lookup"><span data-stu-id="310f0-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="310f0-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="310f0-133">See also</span></span>



- [<span data-ttu-id="310f0-134">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="310f0-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

