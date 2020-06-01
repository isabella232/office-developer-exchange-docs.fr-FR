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
ms.openlocfilehash: e020ff07f271bdde6c2a4172141097dcba66f64e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465092"
---
# <a name="rootaddress"></a><span data-ttu-id="74296-103">RootAddress</span><span class="sxs-lookup"><span data-stu-id="74296-103">RootAddress</span></span>

<span data-ttu-id="74296-104">L’élément **RootAddress** représente la première adresse qui démarre l’événement pour un événement [RecipientTrackingEvent](recipienttrackingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="74296-104">The **RootAddress** element represents the first address that starts the event for a [RecipientTrackingEvent](recipienttrackingevent.md) event.</span></span> 
  
```xml
<RootAddress/>
```

 <span data-ttu-id="74296-105">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="74296-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="74296-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="74296-106">Attributes and elements</span></span>

<span data-ttu-id="74296-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="74296-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="74296-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="74296-108">Attributes</span></span>

<span data-ttu-id="74296-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="74296-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="74296-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="74296-110">Child elements</span></span>

<span data-ttu-id="74296-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="74296-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="74296-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="74296-112">Parent elements</span></span>

|<span data-ttu-id="74296-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="74296-113">**Element**</span></span>|<span data-ttu-id="74296-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="74296-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="74296-115">RecipientTrackingEvent</span><span class="sxs-lookup"><span data-stu-id="74296-115">RecipientTrackingEvent</span></span>](recipienttrackingevent.md) <br/> |<span data-ttu-id="74296-116">Contient des informations pour un seul événement pour un destinataire.</span><span class="sxs-lookup"><span data-stu-id="74296-116">Contains information for a single event for a recipient.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="74296-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="74296-117">Text value</span></span>

<span data-ttu-id="74296-118">La valeur de texte est l’adresse qui commence l’événement de suivi.</span><span class="sxs-lookup"><span data-stu-id="74296-118">The text value is the address that starts the tracking event.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="74296-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="74296-119">Remarks</span></span>

<span data-ttu-id="74296-120">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="74296-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="74296-121">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="74296-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="74296-122">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="74296-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="74296-123">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="74296-123">Schema Name</span></span>  <br/> |<span data-ttu-id="74296-124">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="74296-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="74296-125">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="74296-125">Validation File</span></span>  <br/> |<span data-ttu-id="74296-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="74296-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="74296-127">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="74296-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="74296-128">False</span><span class="sxs-lookup"><span data-stu-id="74296-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="74296-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="74296-129">See also</span></span>



[<span data-ttu-id="74296-130">Opération de GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="74296-130">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="74296-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="74296-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

