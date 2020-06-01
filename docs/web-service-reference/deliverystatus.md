---
title: DeliveryStatus
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeliveryStatus
api_type:
- schema
ms.assetid: eab55db3-affb-42be-a586-5caa04052433
description: L’élément DeliveryStatus spécifie l’état d’un message.
ms.openlocfilehash: ae32202284d3dd272f693fbb7b76070cb6019d28
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461400"
---
# <a name="deliverystatus"></a><span data-ttu-id="7a59f-103">DeliveryStatus</span><span class="sxs-lookup"><span data-stu-id="7a59f-103">DeliveryStatus</span></span>

<span data-ttu-id="7a59f-104">L’élément **DeliveryStatus** spécifie l’état d’un message.</span><span class="sxs-lookup"><span data-stu-id="7a59f-104">The **DeliveryStatus** element specifies the status for a message.</span></span> 
  
```XML
<DeliveryStatus>Unsuccessful | Pending | Delivered | Transferred | Read</DeliveryStatus>
```

 <span data-ttu-id="7a59f-105">**MessageTrackingDeliveryStatusType**</span><span class="sxs-lookup"><span data-stu-id="7a59f-105">**MessageTrackingDeliveryStatusType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7a59f-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="7a59f-106">Attributes and elements</span></span>

<span data-ttu-id="7a59f-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="7a59f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7a59f-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="7a59f-108">Attributes</span></span>

<span data-ttu-id="7a59f-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="7a59f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7a59f-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="7a59f-110">Child elements</span></span>

<span data-ttu-id="7a59f-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7a59f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7a59f-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="7a59f-112">Parent elements</span></span>

|<span data-ttu-id="7a59f-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7a59f-113">**Element**</span></span>|<span data-ttu-id="7a59f-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="7a59f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7a59f-115">RecipientTrackingEvent</span><span class="sxs-lookup"><span data-stu-id="7a59f-115">RecipientTrackingEvent</span></span>](recipienttrackingevent.md) <br/> |<span data-ttu-id="7a59f-116">Contient des informations pour un seul événement pour un destinataire.</span><span class="sxs-lookup"><span data-stu-id="7a59f-116">Contains information for a single event for a recipient.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7a59f-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="7a59f-117">Text value</span></span>

<span data-ttu-id="7a59f-118">Le tableau suivant répertorie les valeurs de texte possibles pour l’élément **DeliveryStatus** .</span><span class="sxs-lookup"><span data-stu-id="7a59f-118">The following table lists the possible text values for the **DeliveryStatus** element.</span></span> 
  
<span data-ttu-id="7a59f-119">**Valeurs de l’élément DeliveryStatus**</span><span class="sxs-lookup"><span data-stu-id="7a59f-119">**DeliveryStatus element values**</span></span>

|<span data-ttu-id="7a59f-120">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="7a59f-120">**Value**</span></span>|<span data-ttu-id="7a59f-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="7a59f-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7a59f-122">Échoué</span><span class="sxs-lookup"><span data-stu-id="7a59f-122">Unsuccessful</span></span>  <br/> |<span data-ttu-id="7a59f-123">Spécifie qu’un message n’a pas été remis.</span><span class="sxs-lookup"><span data-stu-id="7a59f-123">Specifies that a message was not delivered.</span></span>  <br/> |
|<span data-ttu-id="7a59f-124">Pending</span><span class="sxs-lookup"><span data-stu-id="7a59f-124">Pending</span></span>  <br/> |<span data-ttu-id="7a59f-125">Indique que le message est en attente d’approbation d’un modérateur.</span><span class="sxs-lookup"><span data-stu-id="7a59f-125">Specifies that the message is waiting for approval from a moderator.</span></span>  <br/> |
|<span data-ttu-id="7a59f-126">Cmds</span><span class="sxs-lookup"><span data-stu-id="7a59f-126">Delivered</span></span>  <br/> |<span data-ttu-id="7a59f-127">Indique que le message a été remis à tous les destinataires spécifiés.</span><span class="sxs-lookup"><span data-stu-id="7a59f-127">Specifies that the message was delivered to all of the specified recipients.</span></span>  <br/> |
|<span data-ttu-id="7a59f-128">Transfér</span><span class="sxs-lookup"><span data-stu-id="7a59f-128">Transferred</span></span>  <br/> |<span data-ttu-id="7a59f-129">Spécifie que le message a été transféré vers un serveur en dehors de l’étendue de recherche.</span><span class="sxs-lookup"><span data-stu-id="7a59f-129">Specifies that the message was transferred to a server outside the search scope.</span></span>  <br/> |
|<span data-ttu-id="7a59f-130">Lecture</span><span class="sxs-lookup"><span data-stu-id="7a59f-130">Read</span></span>  <br/> |<span data-ttu-id="7a59f-131">Indique que le message a été remis et lu par les destinataires.</span><span class="sxs-lookup"><span data-stu-id="7a59f-131">Specifies that the message was delivered and read by the recipients.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7a59f-132">Remarques</span><span class="sxs-lookup"><span data-stu-id="7a59f-132">Remarks</span></span>

<span data-ttu-id="7a59f-133">L’élément **DeliveryStatus** était de type **MessageTrackingDeliveryStatusType** dans Exchange Server 2010.</span><span class="sxs-lookup"><span data-stu-id="7a59f-133">The **DeliveryStatus** element was of type **MessageTrackingDeliveryStatusType** in Exchange Server 2010.</span></span> 
  
<span data-ttu-id="7a59f-134">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="7a59f-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7a59f-135">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="7a59f-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7a59f-136">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="7a59f-136">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7a59f-137">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="7a59f-137">Schema Name</span></span>  <br/> |<span data-ttu-id="7a59f-138">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="7a59f-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="7a59f-139">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="7a59f-139">Validation File</span></span>  <br/> |<span data-ttu-id="7a59f-140">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7a59f-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7a59f-141">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="7a59f-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="7a59f-142">False</span><span class="sxs-lookup"><span data-stu-id="7a59f-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7a59f-143">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7a59f-143">See also</span></span>

- [<span data-ttu-id="7a59f-144">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="7a59f-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

