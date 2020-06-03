---
title: EventData
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EventData
api_type:
- schema
ms.assetid: 74acdbad-d6ee-47e6-82fb-e45ecaaa0500
description: L’élément EventData représente les données associées à l’étape de traitement de l’événement.
ms.openlocfilehash: ef5da21a3300a6939c60d62584b46ca48b071853
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526178"
---
# <a name="eventdata"></a><span data-ttu-id="a7007-103">EventData</span><span class="sxs-lookup"><span data-stu-id="a7007-103">EventData</span></span>

<span data-ttu-id="a7007-104">L’élément **EventData** représente les données associées à l’étape de traitement de l’événement.</span><span class="sxs-lookup"><span data-stu-id="a7007-104">The **EventData** element represents data that is associated with the processing step for the event.</span></span> 
  
```XML
<EventData>
   <String/>
</EventData>
```

 <span data-ttu-id="a7007-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="a7007-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a7007-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a7007-106">Attributes and elements</span></span>

<span data-ttu-id="a7007-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a7007-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a7007-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="a7007-108">Attributes</span></span>

<span data-ttu-id="a7007-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="a7007-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a7007-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a7007-110">Child elements</span></span>

|<span data-ttu-id="a7007-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a7007-111">**Element**</span></span>|<span data-ttu-id="a7007-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="a7007-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a7007-113">String</span><span class="sxs-lookup"><span data-stu-id="a7007-113">String</span></span>](string.md) <br/> |<span data-ttu-id="a7007-114">Contient une chaîne qui identifie un événement.</span><span class="sxs-lookup"><span data-stu-id="a7007-114">Contains a string that identifies an event.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a7007-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a7007-115">Parent elements</span></span>

|<span data-ttu-id="a7007-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a7007-116">**Element**</span></span>|<span data-ttu-id="a7007-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="a7007-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a7007-118">RecipientTrackingEvent</span><span class="sxs-lookup"><span data-stu-id="a7007-118">RecipientTrackingEvent</span></span>](recipienttrackingevent.md) <br/> |<span data-ttu-id="a7007-119">Contient des informations pour un seul événement pour un destinataire.</span><span class="sxs-lookup"><span data-stu-id="a7007-119">Contains information for a single event for a recipient.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a7007-120">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="a7007-120">Text value</span></span>

<span data-ttu-id="a7007-121">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a7007-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a7007-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="a7007-122">Remarks</span></span>

<span data-ttu-id="a7007-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="a7007-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a7007-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a7007-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a7007-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a7007-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a7007-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a7007-126">Schema Name</span></span>  <br/> |<span data-ttu-id="a7007-127">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="a7007-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="a7007-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="a7007-128">Validation File</span></span>  <br/> |<span data-ttu-id="a7007-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a7007-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a7007-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a7007-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="a7007-131">False</span><span class="sxs-lookup"><span data-stu-id="a7007-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a7007-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a7007-132">See also</span></span>



- [<span data-ttu-id="a7007-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="a7007-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

