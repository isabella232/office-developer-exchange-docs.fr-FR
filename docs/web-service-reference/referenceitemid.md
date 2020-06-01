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
description: L’élément ReferenceItemId identifie l’élément auquel l’objet Response fait référence.
ms.openlocfilehash: 3b77d75de91af8ec8fb7ae2d507377d1d976febf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457227"
---
# <a name="referenceitemid"></a><span data-ttu-id="837dd-103">ReferenceItemId</span><span class="sxs-lookup"><span data-stu-id="837dd-103">ReferenceItemId</span></span>

<span data-ttu-id="837dd-104">L’élément **ReferenceItemId** identifie l’élément auquel l’objet Response fait référence.</span><span class="sxs-lookup"><span data-stu-id="837dd-104">The **ReferenceItemId** element identifies the item to which the response object refers.</span></span> 
  
```xml
<ReferenceItemId Id="" ChangeKey="" />
```

 <span data-ttu-id="837dd-105">**ItemIdType**</span><span class="sxs-lookup"><span data-stu-id="837dd-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="837dd-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="837dd-106">Attributes and elements</span></span>

<span data-ttu-id="837dd-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="837dd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="837dd-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="837dd-108">Attributes</span></span>

|<span data-ttu-id="837dd-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="837dd-109">**Attribute**</span></span>|<span data-ttu-id="837dd-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="837dd-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="837dd-111">**Id**</span><span class="sxs-lookup"><span data-stu-id="837dd-111">**Id**</span></span> <br/> |<span data-ttu-id="837dd-112">Identifie un élément spécifique dans la Banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="837dd-112">Identifies a specific item in the Exchange store.</span></span>  <br/> |
|<span data-ttu-id="837dd-113">**ChangeKey**</span><span class="sxs-lookup"><span data-stu-id="837dd-113">**ChangeKey**</span></span> <br/> |<span data-ttu-id="837dd-114">Identifie une version spécifique d’un élément.</span><span class="sxs-lookup"><span data-stu-id="837dd-114">Identifies a specific version of an item.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="837dd-115">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="837dd-115">Child elements</span></span>

<span data-ttu-id="837dd-116">Aucun.</span><span class="sxs-lookup"><span data-stu-id="837dd-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="837dd-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="837dd-117">Parent elements</span></span>

|<span data-ttu-id="837dd-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="837dd-118">**Element**</span></span>|<span data-ttu-id="837dd-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="837dd-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="837dd-120">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="837dd-120">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="837dd-121">Représente une réponse à accepter à une demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="837dd-121">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="837dd-122">AcceptSharingInvitation</span><span class="sxs-lookup"><span data-stu-id="837dd-122">AcceptSharingInvitation</span></span>](acceptsharinginvitation.md) <br/> |<span data-ttu-id="837dd-123">Représente une réponse accepter une invitation de partage.</span><span class="sxs-lookup"><span data-stu-id="837dd-123">Represents an Accept reply to a sharing invitation.</span></span>  <br/> |
|[<span data-ttu-id="837dd-124">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="837dd-124">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="837dd-125">Représente l'objet de réponse qui est utilisé pour annuler une réunion.</span><span class="sxs-lookup"><span data-stu-id="837dd-125">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
|[<span data-ttu-id="837dd-126">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="837dd-126">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="837dd-127">Représente une réponse de refus à une demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="837dd-127">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="837dd-128">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="837dd-128">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="837dd-129">Contient un élément de la banque Exchange pour transférer à des destinataires.</span><span class="sxs-lookup"><span data-stu-id="837dd-129">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="837dd-130">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="837dd-130">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="837dd-131">Supprime un élément de la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="837dd-131">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="837dd-132">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="837dd-132">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="837dd-133">Contient une réponse destinée à tous les destinataires identifiés d'un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="837dd-133">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="837dd-134">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="837dd-134">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="837dd-135">Contient une réponse à l'auteur d'un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="837dd-135">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="837dd-136">SuppressReadReceipt</span><span class="sxs-lookup"><span data-stu-id="837dd-136">SuppressReadReceipt</span></span>](suppressreadreceipt.md) <br/> |<span data-ttu-id="837dd-137">Utilisé pour répondre aux demandes de confirmation de lecture.</span><span class="sxs-lookup"><span data-stu-id="837dd-137">Used to respond to read receipt requests.</span></span>  <br/> |
|[<span data-ttu-id="837dd-138">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="837dd-138">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="837dd-139">Représente un provisoire répond à une demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="837dd-139">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="837dd-140">Remarques</span><span class="sxs-lookup"><span data-stu-id="837dd-140">Remarks</span></span>

<span data-ttu-id="837dd-141">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services Web Exchange de l’ordinateur qui exécute Microsoft Exchange Server sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="837dd-141">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="837dd-142">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="837dd-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="837dd-143">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="837dd-143">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="837dd-144">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="837dd-144">Schema Name</span></span>  <br/> |<span data-ttu-id="837dd-145">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="837dd-145">Types schema</span></span>  <br/> |
|<span data-ttu-id="837dd-146">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="837dd-146">Validation File</span></span>  <br/> |<span data-ttu-id="837dd-147">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="837dd-147">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="837dd-148">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="837dd-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="837dd-149">False</span><span class="sxs-lookup"><span data-stu-id="837dd-149">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="837dd-150">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="837dd-150">See also</span></span>



- [<span data-ttu-id="837dd-151">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="837dd-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

