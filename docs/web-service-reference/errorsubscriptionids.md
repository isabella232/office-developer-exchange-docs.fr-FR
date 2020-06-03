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
description: L’élément ErrorSubscriptionIds contient un tableau d’ID d’abonnement non valides.
ms.openlocfilehash: bdc5c86560800464d677a9043607bed3f7872e32
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526185"
---
# <a name="errorsubscriptionids"></a><span data-ttu-id="a2be1-103">ErrorSubscriptionIds</span><span class="sxs-lookup"><span data-stu-id="a2be1-103">ErrorSubscriptionIds</span></span>

<span data-ttu-id="a2be1-104">L’élément **ErrorSubscriptionIds** contient un tableau d’ID d’abonnement non valides.</span><span class="sxs-lookup"><span data-stu-id="a2be1-104">The **ErrorSubscriptionIds** element contains an array of invalid subscription IDs.</span></span> 
  
```xml
<ErrorSubscriptionIds>
   <SubscriptionId/>
</ErrorSubscriptionIds>
```

 <span data-ttu-id="a2be1-105">**NonEmptyArrayOfSubscriptionIdsType**</span><span class="sxs-lookup"><span data-stu-id="a2be1-105">**NonEmptyArrayOfSubscriptionIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a2be1-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a2be1-106">Attributes and elements</span></span>

<span data-ttu-id="a2be1-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a2be1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a2be1-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="a2be1-108">Attributes</span></span>

<span data-ttu-id="a2be1-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="a2be1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a2be1-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a2be1-110">Child elements</span></span>

|<span data-ttu-id="a2be1-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a2be1-111">**Element**</span></span>|<span data-ttu-id="a2be1-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="a2be1-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a2be1-113">SubscriptionId (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="a2be1-113">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md) <br/> |<span data-ttu-id="a2be1-114">Représente l’identificateur d’un abonnement.</span><span class="sxs-lookup"><span data-stu-id="a2be1-114">Represents the identifier for a subscription.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a2be1-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a2be1-115">Parent elements</span></span>

|<span data-ttu-id="a2be1-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a2be1-116">**Element**</span></span>|<span data-ttu-id="a2be1-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="a2be1-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a2be1-118">GetStreamingEventsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="a2be1-118">GetStreamingEventsResponseMessage</span></span>](getstreamingeventsresponsemessage.md) <br/> |<span data-ttu-id="a2be1-119">Contient l’État et le résultat d’une seule demande d' [opération GetStreamingEvents](getstreamingevents-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="a2be1-119">Contains the status and result of a single [GetStreamingEvents operation](getstreamingevents-operation.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a2be1-120">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="a2be1-120">Text value</span></span>

<span data-ttu-id="a2be1-121">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a2be1-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a2be1-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="a2be1-122">Remarks</span></span>

<span data-ttu-id="a2be1-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="a2be1-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a2be1-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a2be1-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a2be1-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a2be1-125">Namespace</span></span>  <br/> |<span data-ttu-id="a2be1-126">https://schemas.microsoft.com/exchange/services/2006/messages et https://schemas.microsoft.com/exchange/services/2006/types</span><span class="sxs-lookup"><span data-stu-id="a2be1-126">https://schemas.microsoft.com/exchange/services/2006/messages and https://schemas.microsoft.com/exchange/services/2006/types</span></span>  <br/> |
|<span data-ttu-id="a2be1-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a2be1-127">Schema Name</span></span>  <br/> |<span data-ttu-id="a2be1-128">Schéma des messages ; Schéma de types</span><span class="sxs-lookup"><span data-stu-id="a2be1-128">Messages schema; Types schema</span></span>  <br/> |
|<span data-ttu-id="a2be1-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="a2be1-129">Validation File</span></span>  <br/> |<span data-ttu-id="a2be1-130">Messages. xsd ; Types. xsd</span><span class="sxs-lookup"><span data-stu-id="a2be1-130">Messages.xsd; Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a2be1-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a2be1-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="a2be1-132">False</span><span class="sxs-lookup"><span data-stu-id="a2be1-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a2be1-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a2be1-133">See also</span></span>



[<span data-ttu-id="a2be1-134">Opération de GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="a2be1-134">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)


- [<span data-ttu-id="a2be1-135">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="a2be1-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

