---
title: RootAddress
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RootAddress
api_type:
- schema
ms.assetid: 1dbb130a-e4eb-4baf-ae07-2568a8375bff
description: L’élément RootAddress représente la première adresse qui démarre l’événement pour un événement RecipientTrackingEvent.
ms.openlocfilehash: afe544d6ee8dea4cb416ad033ed2cd68976ec087
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829250"
---
# <a name="rootaddress"></a><span data-ttu-id="a8c91-103">RootAddress</span><span class="sxs-lookup"><span data-stu-id="a8c91-103">RootAddress</span></span>

<span data-ttu-id="a8c91-104">L’élément **RootAddress** représente la première adresse qui démarre l’événement pour un événement [RecipientTrackingEvent](recipienttrackingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="a8c91-104">The **RootAddress** element represents the first address that starts the event for a [RecipientTrackingEvent](recipienttrackingevent.md) event.</span></span> 
  
```xml
<RootAddress/>
```

 <span data-ttu-id="a8c91-105">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="a8c91-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a8c91-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a8c91-106">Attributes and elements</span></span>

<span data-ttu-id="a8c91-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a8c91-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a8c91-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="a8c91-108">Attributes</span></span>

<span data-ttu-id="a8c91-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a8c91-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a8c91-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a8c91-110">Child elements</span></span>

<span data-ttu-id="a8c91-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a8c91-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a8c91-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a8c91-112">Parent elements</span></span>

|<span data-ttu-id="a8c91-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a8c91-113">**Element**</span></span>|<span data-ttu-id="a8c91-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="a8c91-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a8c91-115">RecipientTrackingEvent</span><span class="sxs-lookup"><span data-stu-id="a8c91-115">RecipientTrackingEvent</span></span>](recipienttrackingevent.md) <br/> |<span data-ttu-id="a8c91-116">Contient des informations pour un seul événement pour un destinataire.</span><span class="sxs-lookup"><span data-stu-id="a8c91-116">Contains information for a single event for a recipient.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a8c91-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="a8c91-117">Text value</span></span>

<span data-ttu-id="a8c91-118">La valeur de text est l’adresse qui démarre l’événement de suivi.</span><span class="sxs-lookup"><span data-stu-id="a8c91-118">The text value is the address that starts the tracking event.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a8c91-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="a8c91-119">Remarks</span></span>

<span data-ttu-id="a8c91-120">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="a8c91-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a8c91-121">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a8c91-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a8c91-122">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a8c91-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a8c91-123">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a8c91-123">Schema Name</span></span>  <br/> |<span data-ttu-id="a8c91-124">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="a8c91-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="a8c91-125">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="a8c91-125">Validation File</span></span>  <br/> |<span data-ttu-id="a8c91-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a8c91-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a8c91-127">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a8c91-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="a8c91-128">False</span><span class="sxs-lookup"><span data-stu-id="a8c91-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a8c91-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a8c91-129">See also</span></span>



[<span data-ttu-id="a8c91-130">Opération de GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="a8c91-130">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="a8c91-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="a8c91-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

