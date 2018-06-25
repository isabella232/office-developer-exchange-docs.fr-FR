---
title: RecipientTrackingEvents
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RecipientTrackingEvents
api_type:
- schema
ms.assetid: c4f729aa-674e-43b2-97f2-bf49740b0a34
description: L’élément RecipientTrackingEvents représente une collection d’un ou plusieurs des événements pour un message.
ms.openlocfilehash: 5fa5df422eff533891d021b77d5443b314d36244
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828993"
---
# <a name="recipienttrackingevents"></a><span data-ttu-id="955c0-103">RecipientTrackingEvents</span><span class="sxs-lookup"><span data-stu-id="955c0-103">RecipientTrackingEvents</span></span>

<span data-ttu-id="955c0-104">L’élément **RecipientTrackingEvents** représente une collection d’un ou plusieurs des événements pour un message.</span><span class="sxs-lookup"><span data-stu-id="955c0-104">The **RecipientTrackingEvents** element represents a collection of one or more events for a message.</span></span> 
  
```XML
<RecipientTrackingEvents>
   <RecipientTrackingEvent/>
</RecipientTrackingEvents>
```

 <span data-ttu-id="955c0-105">**ArrayOfRecipientTrackingEventType**</span><span class="sxs-lookup"><span data-stu-id="955c0-105">**ArrayOfRecipientTrackingEventType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="955c0-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="955c0-106">Attributes and elements</span></span>

<span data-ttu-id="955c0-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="955c0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="955c0-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="955c0-108">Attributes</span></span>

<span data-ttu-id="955c0-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="955c0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="955c0-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="955c0-110">Child elements</span></span>

|<span data-ttu-id="955c0-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="955c0-111">**Element**</span></span>|<span data-ttu-id="955c0-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="955c0-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="955c0-113">RecipientTrackingEvent</span><span class="sxs-lookup"><span data-stu-id="955c0-113">RecipientTrackingEvent</span></span>](recipienttrackingevent.md) <br/> |<span data-ttu-id="955c0-114">Contient des détails pour un événement spécifique dans le rapport de suivi.</span><span class="sxs-lookup"><span data-stu-id="955c0-114">Contains details for a specific event in the tracking report.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="955c0-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="955c0-115">Parent elements</span></span>

|<span data-ttu-id="955c0-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="955c0-116">**Element**</span></span>|<span data-ttu-id="955c0-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="955c0-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="955c0-118">MessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="955c0-118">MessageTrackingReport</span></span>](messagetrackingreport.md) <br/> |<span data-ttu-id="955c0-119">Contient un seul message renvoyé dans un [Opération de GetMessageTrackingReport](getmessagetrackingreport-operation.md).</span><span class="sxs-lookup"><span data-stu-id="955c0-119">Contains a single message that is returned in a [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="955c0-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="955c0-120">Remarks</span></span>

<span data-ttu-id="955c0-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="955c0-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="955c0-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="955c0-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="955c0-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="955c0-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="955c0-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="955c0-124">Schema Name</span></span>  <br/> |<span data-ttu-id="955c0-125">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="955c0-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="955c0-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="955c0-126">Validation File</span></span>  <br/> |<span data-ttu-id="955c0-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="955c0-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="955c0-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="955c0-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="955c0-129">False</span><span class="sxs-lookup"><span data-stu-id="955c0-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="955c0-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="955c0-130">See also</span></span>



[<span data-ttu-id="955c0-131">Opération de GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="955c0-131">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="955c0-132">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="955c0-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

