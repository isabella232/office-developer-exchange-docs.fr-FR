---
title: IsOutOfDate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsOutOfDate
api_type:
- schema
ms.assetid: 2b6005a6-56a9-4848-b998-32908c13e2e2
description: L’élément IsOutOfDate indique si un message de réunion, demande, réponse ou annulation est obsolète.
ms.openlocfilehash: 0a6b2670cc3eb260002821bab31d652177902de1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828110"
---
# <a name="isoutofdate"></a><span data-ttu-id="37bcf-103">IsOutOfDate</span><span class="sxs-lookup"><span data-stu-id="37bcf-103">IsOutOfDate</span></span>

<span data-ttu-id="37bcf-104">L’élément **IsOutOfDate** indique si un message de réunion, demande, réponse ou annulation est obsolète.</span><span class="sxs-lookup"><span data-stu-id="37bcf-104">The **IsOutOfDate** element indicates whether a meeting message, request, response, or cancellation is out-of-date.</span></span> 
  
```xml
<IsOutOfDate/>
```

 <span data-ttu-id="37bcf-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="37bcf-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="37bcf-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="37bcf-106">Attributes and elements</span></span>

<span data-ttu-id="37bcf-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="37bcf-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="37bcf-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="37bcf-108">Attributes</span></span>

<span data-ttu-id="37bcf-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="37bcf-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="37bcf-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="37bcf-110">Child elements</span></span>

<span data-ttu-id="37bcf-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="37bcf-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="37bcf-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="37bcf-112">Parent elements</span></span>

|<span data-ttu-id="37bcf-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="37bcf-113">**Element**</span></span>|<span data-ttu-id="37bcf-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="37bcf-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="37bcf-115">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="37bcf-115">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="37bcf-116">Représente une annulation de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="37bcf-116">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="37bcf-117">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="37bcf-117">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="37bcf-118">Représente une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="37bcf-118">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="37bcf-119">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="37bcf-119">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="37bcf-120">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="37bcf-120">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="37bcf-121">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="37bcf-121">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="37bcf-122">Représente une réponse à une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="37bcf-122">Represents a meeting response in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="37bcf-123">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="37bcf-123">Text value</span></span>

<span data-ttu-id="37bcf-124">Une valeur de texte de **la valeur true** indique que l’élément de réunion est obsolète.</span><span class="sxs-lookup"><span data-stu-id="37bcf-124">A text value of **true** indicates that the meeting item is out-of-date.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="37bcf-125">Remarques</span><span class="sxs-lookup"><span data-stu-id="37bcf-125">Remarks</span></span>

<span data-ttu-id="37bcf-126">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="37bcf-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="37bcf-127">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="37bcf-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="37bcf-128">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="37bcf-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="37bcf-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="37bcf-129">Schema Name</span></span>  <br/> |<span data-ttu-id="37bcf-130">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="37bcf-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="37bcf-131">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="37bcf-131">Validation File</span></span>  <br/> |<span data-ttu-id="37bcf-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="37bcf-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="37bcf-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="37bcf-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="37bcf-134">False</span><span class="sxs-lookup"><span data-stu-id="37bcf-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="37bcf-135">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="37bcf-135">See also</span></span>



- [<span data-ttu-id="37bcf-136">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="37bcf-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

