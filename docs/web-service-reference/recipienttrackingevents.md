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
description: L’élément RecipientTrackingEvents représente une collection d’un ou plusieurs événements pour un message.
ms.openlocfilehash: c0b25a0e22d13bc1f26768b9b7089d96eb2e8cfc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468480"
---
# <a name="recipienttrackingevents"></a><span data-ttu-id="3555f-103">RecipientTrackingEvents</span><span class="sxs-lookup"><span data-stu-id="3555f-103">RecipientTrackingEvents</span></span>

<span data-ttu-id="3555f-104">L’élément **RecipientTrackingEvents** représente une collection d’un ou plusieurs événements pour un message.</span><span class="sxs-lookup"><span data-stu-id="3555f-104">The **RecipientTrackingEvents** element represents a collection of one or more events for a message.</span></span> 
  
```XML
<RecipientTrackingEvents>
   <RecipientTrackingEvent/>
</RecipientTrackingEvents>
```

 <span data-ttu-id="3555f-105">**ArrayOfRecipientTrackingEventType**</span><span class="sxs-lookup"><span data-stu-id="3555f-105">**ArrayOfRecipientTrackingEventType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3555f-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="3555f-106">Attributes and elements</span></span>

<span data-ttu-id="3555f-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="3555f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3555f-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="3555f-108">Attributes</span></span>

<span data-ttu-id="3555f-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="3555f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3555f-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="3555f-110">Child elements</span></span>

|<span data-ttu-id="3555f-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3555f-111">**Element**</span></span>|<span data-ttu-id="3555f-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="3555f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3555f-113">RecipientTrackingEvent</span><span class="sxs-lookup"><span data-stu-id="3555f-113">RecipientTrackingEvent</span></span>](recipienttrackingevent.md) <br/> |<span data-ttu-id="3555f-114">Contient les détails d’un événement spécifique dans le rapport de suivi.</span><span class="sxs-lookup"><span data-stu-id="3555f-114">Contains details for a specific event in the tracking report.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3555f-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="3555f-115">Parent elements</span></span>

|<span data-ttu-id="3555f-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3555f-116">**Element**</span></span>|<span data-ttu-id="3555f-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="3555f-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3555f-118">MessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="3555f-118">MessageTrackingReport</span></span>](messagetrackingreport.md) <br/> |<span data-ttu-id="3555f-119">Contient un seul message renvoyé dans un [Opération de GetMessageTrackingReport](getmessagetrackingreport-operation.md).</span><span class="sxs-lookup"><span data-stu-id="3555f-119">Contains a single message that is returned in a [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3555f-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="3555f-120">Remarks</span></span>

<span data-ttu-id="3555f-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="3555f-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3555f-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="3555f-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3555f-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="3555f-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3555f-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="3555f-124">Schema Name</span></span>  <br/> |<span data-ttu-id="3555f-125">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="3555f-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="3555f-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="3555f-126">Validation File</span></span>  <br/> |<span data-ttu-id="3555f-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3555f-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3555f-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="3555f-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="3555f-129">False</span><span class="sxs-lookup"><span data-stu-id="3555f-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3555f-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="3555f-130">See also</span></span>



[<span data-ttu-id="3555f-131">Opération de GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="3555f-131">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="3555f-132">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="3555f-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

