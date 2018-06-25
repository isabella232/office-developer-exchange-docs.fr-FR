---
title: ReferenceItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ReferenceItemId
api_type:
- schema
ms.assetid: 8fd4bb12-a94b-43f5-be3b-f435684e311d
description: L’élément ReferenceItemId identifie l’élément auquel fait référence l’objet de réponse.
ms.openlocfilehash: d29f2dfec8f2c23fe0ac8c84d2bb9029fce613d2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829032"
---
# <a name="referenceitemid"></a><span data-ttu-id="9fe2e-103">ReferenceItemId</span><span class="sxs-lookup"><span data-stu-id="9fe2e-103">ReferenceItemId</span></span>

<span data-ttu-id="9fe2e-104">L’élément **ReferenceItemId** identifie l’élément auquel fait référence l’objet de réponse.</span><span class="sxs-lookup"><span data-stu-id="9fe2e-104">The **ReferenceItemId** element identifies the item to which the response object refers.</span></span> 
  
```xml
<ReferenceItemId Id="" ChangeKey="" />
```

 <span data-ttu-id="9fe2e-105">**ItemIdType**</span><span class="sxs-lookup"><span data-stu-id="9fe2e-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9fe2e-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="9fe2e-106">Attributes and elements</span></span>

<span data-ttu-id="9fe2e-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="9fe2e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9fe2e-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="9fe2e-108">Attributes</span></span>

|<span data-ttu-id="9fe2e-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="9fe2e-109">**Attribute**</span></span>|<span data-ttu-id="9fe2e-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="9fe2e-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9fe2e-111">
  **Id**</span><span class="sxs-lookup"><span data-stu-id="9fe2e-111">**Id**</span></span> <br/> |<span data-ttu-id="9fe2e-112">Identifie un élément spécifique dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="9fe2e-112">Identifies a specific item in the Exchange store.</span></span>  <br/> |
|<span data-ttu-id="9fe2e-113">**ChangeKey**</span><span class="sxs-lookup"><span data-stu-id="9fe2e-113">**ChangeKey**</span></span> <br/> |<span data-ttu-id="9fe2e-114">Identifie une version spécifique d’un élément.</span><span class="sxs-lookup"><span data-stu-id="9fe2e-114">Identifies a specific version of an item.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="9fe2e-115">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="9fe2e-115">Child elements</span></span>

<span data-ttu-id="9fe2e-116">Aucun.</span><span class="sxs-lookup"><span data-stu-id="9fe2e-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9fe2e-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="9fe2e-117">Parent elements</span></span>

|<span data-ttu-id="9fe2e-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9fe2e-118">**Element**</span></span>|<span data-ttu-id="9fe2e-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="9fe2e-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9fe2e-120">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="9fe2e-120">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="9fe2e-121">Représente une réponse à accepter à une demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="9fe2e-121">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="9fe2e-122">AcceptSharingInvitation</span><span class="sxs-lookup"><span data-stu-id="9fe2e-122">AcceptSharingInvitation</span></span>](acceptsharinginvitation.md) <br/> |<span data-ttu-id="9fe2e-123">Représente une réponse accepter une invitation de partage.</span><span class="sxs-lookup"><span data-stu-id="9fe2e-123">Represents an Accept reply to a sharing invitation.</span></span>  <br/> |
|[<span data-ttu-id="9fe2e-124">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="9fe2e-124">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="9fe2e-125">Représente l'objet de réponse qui est utilisé pour annuler une réunion.</span><span class="sxs-lookup"><span data-stu-id="9fe2e-125">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
|[<span data-ttu-id="9fe2e-126">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="9fe2e-126">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="9fe2e-127">Représente une réponse de refus à une demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="9fe2e-127">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="9fe2e-128">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="9fe2e-128">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="9fe2e-129">Contient un élément de la banque Exchange pour transférer à des destinataires.</span><span class="sxs-lookup"><span data-stu-id="9fe2e-129">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="9fe2e-130">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="9fe2e-130">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="9fe2e-131">Supprime un élément de la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="9fe2e-131">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="9fe2e-132">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="9fe2e-132">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="9fe2e-133">Contient une réponse destinée à tous les destinataires identifiés d'un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="9fe2e-133">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="9fe2e-134">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="9fe2e-134">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="9fe2e-135">Contient une réponse à l'auteur d'un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="9fe2e-135">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="9fe2e-136">SuppressReadReceipt</span><span class="sxs-lookup"><span data-stu-id="9fe2e-136">SuppressReadReceipt</span></span>](suppressreadreceipt.md) <br/> |<span data-ttu-id="9fe2e-137">Utilisé pour répondre aux demandes de confirmation de lecture.</span><span class="sxs-lookup"><span data-stu-id="9fe2e-137">Used to respond to read receipt requests.</span></span>  <br/> |
|[<span data-ttu-id="9fe2e-138">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="9fe2e-138">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="9fe2e-139">Représente un provisoire répond à une demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="9fe2e-139">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9fe2e-140">Remarques</span><span class="sxs-lookup"><span data-stu-id="9fe2e-140">Remarks</span></span>

<span data-ttu-id="9fe2e-141">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS que héberge Exchange Web Services de l’ordinateur qui exécute Microsoft Exchange Server qui a le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="9fe2e-141">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9fe2e-142">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="9fe2e-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9fe2e-143">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="9fe2e-143">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9fe2e-144">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="9fe2e-144">Schema Name</span></span>  <br/> |<span data-ttu-id="9fe2e-145">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="9fe2e-145">Types schema</span></span>  <br/> |
|<span data-ttu-id="9fe2e-146">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="9fe2e-146">Validation File</span></span>  <br/> |<span data-ttu-id="9fe2e-147">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9fe2e-147">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9fe2e-148">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="9fe2e-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="9fe2e-149">False</span><span class="sxs-lookup"><span data-stu-id="9fe2e-149">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9fe2e-150">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="9fe2e-150">See also</span></span>



- [<span data-ttu-id="9fe2e-151">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="9fe2e-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

