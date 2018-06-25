---
title: IsDelegated
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsDelegated
api_type:
- schema
ms.assetid: c12907db-be80-4924-9469-8e58612cf42c
description: L’élément IsDelegated indique si une réunion a été gérée par un compte qui dispose d’un accès délégué.
ms.openlocfilehash: a6f42a57b2d0fdb760e4c36d3211ba57289a3c7c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828005"
---
# <a name="isdelegated"></a><span data-ttu-id="0dbe6-103">IsDelegated</span><span class="sxs-lookup"><span data-stu-id="0dbe6-103">IsDelegated</span></span>

<span data-ttu-id="0dbe6-104">L’élément **IsDelegated** indique si une réunion a été gérée par un compte qui dispose d’un accès délégué.</span><span class="sxs-lookup"><span data-stu-id="0dbe6-104">The **IsDelegated** element indicates whether a meeting was handled by an account that has delegate access.</span></span> 
  
```xml
<IsDelegated/>
```

 <span data-ttu-id="0dbe6-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="0dbe6-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0dbe6-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="0dbe6-106">Attributes and elements</span></span>

<span data-ttu-id="0dbe6-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="0dbe6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0dbe6-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="0dbe6-108">Attributes</span></span>

<span data-ttu-id="0dbe6-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="0dbe6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0dbe6-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="0dbe6-110">Child elements</span></span>

<span data-ttu-id="0dbe6-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="0dbe6-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0dbe6-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="0dbe6-112">Parent elements</span></span>

|<span data-ttu-id="0dbe6-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0dbe6-113">**Element**</span></span>|<span data-ttu-id="0dbe6-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="0dbe6-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0dbe6-115">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="0dbe6-115">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="0dbe6-116">Représente une annulation de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="0dbe6-116">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0dbe6-117">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="0dbe6-117">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="0dbe6-118">Représente une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="0dbe6-118">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0dbe6-119">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="0dbe6-119">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="0dbe6-120">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="0dbe6-120">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0dbe6-121">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="0dbe6-121">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="0dbe6-122">Représente une réponse à une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="0dbe6-122">Represents a meeting response in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0dbe6-123">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="0dbe6-123">Text value</span></span>

<span data-ttu-id="0dbe6-124">Une valeur de texte de **la valeur true** indique que la réunion a été gérée par un compte qui dispose d’un accès délégué.</span><span class="sxs-lookup"><span data-stu-id="0dbe6-124">A text value of **true** indicates that the meeting was handled by an account that has delegate access.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="0dbe6-125">Remarques</span><span class="sxs-lookup"><span data-stu-id="0dbe6-125">Remarks</span></span>

<span data-ttu-id="0dbe6-126">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="0dbe6-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0dbe6-127">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="0dbe6-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0dbe6-128">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="0dbe6-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0dbe6-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="0dbe6-129">Schema Name</span></span>  <br/> |<span data-ttu-id="0dbe6-130">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="0dbe6-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="0dbe6-131">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="0dbe6-131">Validation File</span></span>  <br/> |<span data-ttu-id="0dbe6-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0dbe6-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0dbe6-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="0dbe6-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="0dbe6-134">False</span><span class="sxs-lookup"><span data-stu-id="0dbe6-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0dbe6-135">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="0dbe6-135">See also</span></span>



- [<span data-ttu-id="0dbe6-136">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="0dbe6-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

