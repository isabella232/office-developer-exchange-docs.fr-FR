---
title: ErrorSubscriptionIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ErrorSubscriptionIds
api_type:
- schema
ms.assetid: e64e76ff-4d98-4082-9acc-a1114ae45f44
description: L’élément ErrorSubscriptionIds contient un tableau d’ID d’abonnement non valide.
ms.openlocfilehash: 5cdbbeb1083754510f431bc092bb67dc0addecab
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756218"
---
# <a name="errorsubscriptionids"></a><span data-ttu-id="e7265-103">ErrorSubscriptionIds</span><span class="sxs-lookup"><span data-stu-id="e7265-103">ErrorSubscriptionIds</span></span>

<span data-ttu-id="e7265-104">L’élément **ErrorSubscriptionIds** contient un tableau d’ID d’abonnement non valide.</span><span class="sxs-lookup"><span data-stu-id="e7265-104">The **ErrorSubscriptionIds** element contains an array of invalid subscription IDs.</span></span> 
  
```xml
<ErrorSubscriptionIds>
   <SubscriptionId/>
</ErrorSubscriptionIds>
```

 <span data-ttu-id="e7265-105">**NonEmptyArrayOfSubscriptionIdsType**</span><span class="sxs-lookup"><span data-stu-id="e7265-105">**NonEmptyArrayOfSubscriptionIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e7265-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="e7265-106">Attributes and elements</span></span>

<span data-ttu-id="e7265-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="e7265-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e7265-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="e7265-108">Attributes</span></span>

<span data-ttu-id="e7265-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="e7265-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e7265-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="e7265-110">Child elements</span></span>

|<span data-ttu-id="e7265-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e7265-111">**Element**</span></span>|<span data-ttu-id="e7265-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="e7265-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e7265-113">SubscriptionId (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="e7265-113">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md) <br/> |<span data-ttu-id="e7265-114">Représente l’identificateur d’un abonnement.</span><span class="sxs-lookup"><span data-stu-id="e7265-114">Represents the identifier for a subscription.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e7265-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="e7265-115">Parent elements</span></span>

|<span data-ttu-id="e7265-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e7265-116">**Element**</span></span>|<span data-ttu-id="e7265-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="e7265-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e7265-118">GetStreamingEventsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="e7265-118">GetStreamingEventsResponseMessage</span></span>](getstreamingeventsresponsemessage.md) <br/> |<span data-ttu-id="e7265-119">Contient l’état et les résultats d’une seule demande [d’opération GetStreamingEvents](getstreamingevents-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="e7265-119">Contains the status and result of a single [GetStreamingEvents operation](getstreamingevents-operation.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e7265-120">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="e7265-120">Text value</span></span>

<span data-ttu-id="e7265-121">Aucun.</span><span class="sxs-lookup"><span data-stu-id="e7265-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e7265-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="e7265-122">Remarks</span></span>

<span data-ttu-id="e7265-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="e7265-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e7265-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="e7265-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e7265-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="e7265-125">Namespace</span></span>  <br/> |<span data-ttu-id="e7265-126">http://schemas.microsoft.com/exchange/services/2006/messages et http://schemas.microsoft.com/exchange/services/2006/types</span><span class="sxs-lookup"><span data-stu-id="e7265-126">http://schemas.microsoft.com/exchange/services/2006/messages and http://schemas.microsoft.com/exchange/services/2006/types</span></span>  <br/> |
|<span data-ttu-id="e7265-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="e7265-127">Schema Name</span></span>  <br/> |<span data-ttu-id="e7265-128">Schéma des messages ; Schéma de types</span><span class="sxs-lookup"><span data-stu-id="e7265-128">Messages schema; Types schema</span></span>  <br/> |
|<span data-ttu-id="e7265-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="e7265-129">Validation File</span></span>  <br/> |<span data-ttu-id="e7265-130">Messages.xsd ; Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e7265-130">Messages.xsd; Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e7265-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="e7265-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="e7265-132">False</span><span class="sxs-lookup"><span data-stu-id="e7265-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e7265-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e7265-133">See also</span></span>



[<span data-ttu-id="e7265-134">Opération de GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="e7265-134">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)


- [<span data-ttu-id="e7265-135">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="e7265-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

