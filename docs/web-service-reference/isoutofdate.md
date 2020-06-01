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
description: L’élément IsOutOfDate indique si un message, une demande, une réponse ou une annulation de réunion est obsolète.
ms.openlocfilehash: b50b021e48789ba63016582450404b5da3ff86e1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466548"
---
# <a name="isoutofdate"></a><span data-ttu-id="b7c0e-103">IsOutOfDate</span><span class="sxs-lookup"><span data-stu-id="b7c0e-103">IsOutOfDate</span></span>

<span data-ttu-id="b7c0e-104">L’élément **IsOutOfDate** indique si un message, une demande, une réponse ou une annulation de réunion est obsolète.</span><span class="sxs-lookup"><span data-stu-id="b7c0e-104">The **IsOutOfDate** element indicates whether a meeting message, request, response, or cancellation is out-of-date.</span></span> 
  
```xml
<IsOutOfDate/>
```

 <span data-ttu-id="b7c0e-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="b7c0e-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b7c0e-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="b7c0e-106">Attributes and elements</span></span>

<span data-ttu-id="b7c0e-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="b7c0e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b7c0e-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="b7c0e-108">Attributes</span></span>

<span data-ttu-id="b7c0e-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="b7c0e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b7c0e-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="b7c0e-110">Child elements</span></span>

<span data-ttu-id="b7c0e-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b7c0e-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b7c0e-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="b7c0e-112">Parent elements</span></span>

|<span data-ttu-id="b7c0e-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b7c0e-113">**Element**</span></span>|<span data-ttu-id="b7c0e-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="b7c0e-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b7c0e-115">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="b7c0e-115">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="b7c0e-116">Représente une annulation de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="b7c0e-116">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="b7c0e-117">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="b7c0e-117">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="b7c0e-118">Représente une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="b7c0e-118">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="b7c0e-119">Propriété meetingrequest</span><span class="sxs-lookup"><span data-stu-id="b7c0e-119">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="b7c0e-120">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="b7c0e-120">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="b7c0e-121">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="b7c0e-121">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="b7c0e-122">Représente une réponse à une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="b7c0e-122">Represents a meeting response in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b7c0e-123">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="b7c0e-123">Text value</span></span>

<span data-ttu-id="b7c0e-124">Une valeur de texte **true** indique que l’élément de réunion est obsolète.</span><span class="sxs-lookup"><span data-stu-id="b7c0e-124">A text value of **true** indicates that the meeting item is out-of-date.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="b7c0e-125">Remarques</span><span class="sxs-lookup"><span data-stu-id="b7c0e-125">Remarks</span></span>

<span data-ttu-id="b7c0e-126">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="b7c0e-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b7c0e-127">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="b7c0e-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b7c0e-128">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="b7c0e-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b7c0e-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="b7c0e-129">Schema Name</span></span>  <br/> |<span data-ttu-id="b7c0e-130">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="b7c0e-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="b7c0e-131">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="b7c0e-131">Validation File</span></span>  <br/> |<span data-ttu-id="b7c0e-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b7c0e-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b7c0e-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="b7c0e-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="b7c0e-134">False</span><span class="sxs-lookup"><span data-stu-id="b7c0e-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b7c0e-135">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b7c0e-135">See also</span></span>



- [<span data-ttu-id="b7c0e-136">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="b7c0e-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

