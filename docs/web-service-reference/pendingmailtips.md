---
title: PendingMailTips
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PendingMailTips
api_type:
- schema
ms.assetid: 0cd70eea-8d36-4b1b-bf80-5edf359e7ba7
description: L’élément PendingMailTips indique que les conseils de messagerie de cet élément ne peuvent pas être évaluées avant l’expiration du délai d’attente de traitement du serveur.
ms.openlocfilehash: 73d597f6534ea29f7d26d6526c48631251521ae5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828704"
---
# <a name="pendingmailtips"></a><span data-ttu-id="d6b21-103">PendingMailTips</span><span class="sxs-lookup"><span data-stu-id="d6b21-103">PendingMailTips</span></span>

<span data-ttu-id="d6b21-104">L’élément **PendingMailTips** indique que les conseils de messagerie de cet élément ne peuvent pas être évaluées avant l’expiration du délai d’attente de traitement du serveur.</span><span class="sxs-lookup"><span data-stu-id="d6b21-104">The **PendingMailTips** element indicates that the mail tips in this element could not be evaluated before the server's processing timeout expired.</span></span> 
  
```XML
<PendingMailTips>All | OutOfOfficeMessage | MailboxFullStatus | CustomMailTip | ExternalMemberCount | TotalMemberCount | MaxMessageSize | DeliveryRestriction | ModerateStatus | InvalidRecipient</PendingMailTips>
```

 <span data-ttu-id="d6b21-105">**MailTipTypes**</span><span class="sxs-lookup"><span data-stu-id="d6b21-105">**MailTipTypes**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d6b21-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d6b21-106">Attributes and elements</span></span>

<span data-ttu-id="d6b21-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d6b21-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d6b21-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="d6b21-108">Attributes</span></span>

<span data-ttu-id="d6b21-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d6b21-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d6b21-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d6b21-110">Child elements</span></span>

<span data-ttu-id="d6b21-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d6b21-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d6b21-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d6b21-112">Parent elements</span></span>

|<span data-ttu-id="d6b21-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d6b21-113">**Element**</span></span>|<span data-ttu-id="d6b21-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="d6b21-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d6b21-115">Les infos-courrier</span><span class="sxs-lookup"><span data-stu-id="d6b21-115">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="d6b21-116">Représente les valeurs pour les différents types d’astuces de la messagerie.</span><span class="sxs-lookup"><span data-stu-id="d6b21-116">Represents values for various types of mail tips.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d6b21-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="d6b21-117">Text value</span></span>

<span data-ttu-id="d6b21-118">Le tableau suivant répertorie les valeurs possibles pour l’élément **PendingMailTips** .</span><span class="sxs-lookup"><span data-stu-id="d6b21-118">The following table lists the possible values for the **PendingMailTips** element.</span></span> 
  
|<span data-ttu-id="d6b21-119">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="d6b21-119">**Value**</span></span>|<span data-ttu-id="d6b21-120">**Description**</span><span class="sxs-lookup"><span data-stu-id="d6b21-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d6b21-121">Tous</span><span class="sxs-lookup"><span data-stu-id="d6b21-121">All</span></span>  <br/> |<span data-ttu-id="d6b21-122">Représente tous les conseils de messagerie disponibles.</span><span class="sxs-lookup"><span data-stu-id="d6b21-122">Represents all available mail tips.</span></span>  <br/> |
|<span data-ttu-id="d6b21-123">OutOfOfficeMessage</span><span class="sxs-lookup"><span data-stu-id="d6b21-123">OutOfOfficeMessage</span></span>  <br/> |<span data-ttu-id="d6b21-124">Représente le message d’absence du bureau (OOF).</span><span class="sxs-lookup"><span data-stu-id="d6b21-124">Represents the Out of Office (OOF) message.</span></span>  <br/> |
|<span data-ttu-id="d6b21-125">MailboxFullStatus</span><span class="sxs-lookup"><span data-stu-id="d6b21-125">MailboxFullStatus</span></span>  <br/> |<span data-ttu-id="d6b21-126">Représente l’état d’une boîte aux lettres en cours complète.</span><span class="sxs-lookup"><span data-stu-id="d6b21-126">Represents the status for a mailbox being full.</span></span>  <br/> |
|<span data-ttu-id="d6b21-127">CustomMailTip</span><span class="sxs-lookup"><span data-stu-id="d6b21-127">CustomMailTip</span></span>  <br/> |<span data-ttu-id="d6b21-128">Représente une info-bulle de messagerie personnalisé.</span><span class="sxs-lookup"><span data-stu-id="d6b21-128">Represents a custom mail tip.</span></span>  <br/> |
|<span data-ttu-id="d6b21-129">ExternalMemberCount</span><span class="sxs-lookup"><span data-stu-id="d6b21-129">ExternalMemberCount</span></span>  <br/> |<span data-ttu-id="d6b21-130">Représente le nombre de membres externes.</span><span class="sxs-lookup"><span data-stu-id="d6b21-130">Represents the count of external members.</span></span>  <br/> |
|<span data-ttu-id="d6b21-131">TotalMemberCount</span><span class="sxs-lookup"><span data-stu-id="d6b21-131">TotalMemberCount</span></span>  <br/> |<span data-ttu-id="d6b21-132">Représente le nombre de tous les membres.</span><span class="sxs-lookup"><span data-stu-id="d6b21-132">Represents the count of all members.</span></span>  <br/> |
|<span data-ttu-id="d6b21-133">MaxMessageSize</span><span class="sxs-lookup"><span data-stu-id="d6b21-133">MaxMessageSize</span></span>  <br/> |<span data-ttu-id="d6b21-134">Représente la taille maximale des messages que le destinataire peut accepter.</span><span class="sxs-lookup"><span data-stu-id="d6b21-134">Represents the maximum message size a recipient can accept.</span></span>  <br/> |
|<span data-ttu-id="d6b21-135">DeliveryRestriction</span><span class="sxs-lookup"><span data-stu-id="d6b21-135">DeliveryRestriction</span></span>  <br/> |<span data-ttu-id="d6b21-136">Indique si les restrictions de remise empêche le message de l’expéditeur d’atteindre le destinataire.</span><span class="sxs-lookup"><span data-stu-id="d6b21-136">Indicates whether delivery restrictions will prevent the sender's message from reaching the recipient.</span></span>  <br/> |
|<span data-ttu-id="d6b21-137">ModerationStatus</span><span class="sxs-lookup"><span data-stu-id="d6b21-137">ModerationStatus</span></span>  <br/> |<span data-ttu-id="d6b21-138">Indique si le message de l’expéditeur s’être révisé par un modérateur.</span><span class="sxs-lookup"><span data-stu-id="d6b21-138">Indicates whether the sender's message will be reviewed by a moderator.</span></span>  <br/> |
|<span data-ttu-id="d6b21-139">InvalidRecipient</span><span class="sxs-lookup"><span data-stu-id="d6b21-139">InvalidRecipient</span></span>  <br/> |<span data-ttu-id="d6b21-140">Indique si le destinataire n’est pas valide.</span><span class="sxs-lookup"><span data-stu-id="d6b21-140">Indicates whether the recipient is invalid.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d6b21-141">Remarques</span><span class="sxs-lookup"><span data-stu-id="d6b21-141">Remarks</span></span>

<span data-ttu-id="d6b21-142">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="d6b21-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d6b21-143">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d6b21-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d6b21-144">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d6b21-144">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d6b21-145">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d6b21-145">Schema Name</span></span>  <br/> |<span data-ttu-id="d6b21-146">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="d6b21-146">Types schema</span></span>  <br/> |
|<span data-ttu-id="d6b21-147">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d6b21-147">Validation File</span></span>  <br/> |<span data-ttu-id="d6b21-148">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d6b21-148">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d6b21-149">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d6b21-149">Can be Empty</span></span>  <br/> |<span data-ttu-id="d6b21-150">False</span><span class="sxs-lookup"><span data-stu-id="d6b21-150">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d6b21-151">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d6b21-151">See also</span></span>



- [<span data-ttu-id="d6b21-152">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="d6b21-152">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

