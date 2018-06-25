---
title: Les infos-courrier
manager: sethgros
ms.date: 09/17/2015
ms.audience: ITPro
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailTips
api_type:
- schema
ms.assetid: c1cba493-bccc-4b8e-be8e-bfa8a8b10882
description: L’élément Infos-courrier représente les valeurs pour les différents types d’astuces de la messagerie.
ms.openlocfilehash: 3a2e95225b09fd2d81db32f821ea3069ab7e7852
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828311"
---
# <a name="mailtips"></a><span data-ttu-id="8afcd-103">Les infos-courrier</span><span class="sxs-lookup"><span data-stu-id="8afcd-103">MailTips</span></span>

<span data-ttu-id="8afcd-104">L’élément **Infos-courrier** représente les valeurs pour les différents types d’astuces de la messagerie.</span><span class="sxs-lookup"><span data-stu-id="8afcd-104">The **MailTips** element represents values for various types of mail tips.</span></span> 
  
```XML
<MailTips>
   <RecipientAddress/>
   <PendingMailTips/>
   <OutOfOffice/>
   <MailboxFull/>
   <CustomMailTip/>
   <TotalMemberCount/>
   <ExternalMemberCount/>
   <MaxMessageSize/>
   <DeliveryRestricted/>
   <IsModerated/>
   <InvalidRecipient/>
</MailTips>
```

 <span data-ttu-id="8afcd-105">**Les infos-courrier**</span><span class="sxs-lookup"><span data-stu-id="8afcd-105">**MailTips**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8afcd-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="8afcd-106">Attributes and elements</span></span>

<span data-ttu-id="8afcd-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="8afcd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8afcd-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="8afcd-108">Attributes</span></span>

<span data-ttu-id="8afcd-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="8afcd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8afcd-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="8afcd-110">Child elements</span></span>

|<span data-ttu-id="8afcd-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="8afcd-111">**Element**</span></span>|<span data-ttu-id="8afcd-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="8afcd-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8afcd-113">RecipientAddress</span><span class="sxs-lookup"><span data-stu-id="8afcd-113">RecipientAddress</span></span>](recipientaddress.md) <br/> |<span data-ttu-id="8afcd-114">Représente la boîte aux lettres du destinataire.</span><span class="sxs-lookup"><span data-stu-id="8afcd-114">Represents the mailbox of the recipient.</span></span>  <br/> |
|[<span data-ttu-id="8afcd-115">PendingMailTips</span><span class="sxs-lookup"><span data-stu-id="8afcd-115">PendingMailTips</span></span>](pendingmailtips.md) <br/> |<span data-ttu-id="8afcd-116">Indique que les conseils de messagerie de cet élément ne peuvent pas être évaluées avant l’expiration du délai d’attente de traitement du serveur.</span><span class="sxs-lookup"><span data-stu-id="8afcd-116">Indicates that the mail tips in this element could not be evaluated before the server's processing timeout expired.</span></span>  <br/> |
|[<span data-ttu-id="8afcd-117">OutOfOffice</span><span class="sxs-lookup"><span data-stu-id="8afcd-117">OutOfOffice</span></span>](outofoffice.md) <br/> |<span data-ttu-id="8afcd-118">Représente le message de réponse et un délai d’expiration pour l’envoi du message de réponse.</span><span class="sxs-lookup"><span data-stu-id="8afcd-118">Represents the response message and a duration time for sending the response message.</span></span>  <br/> |
|[<span data-ttu-id="8afcd-119">MailboxFull</span><span class="sxs-lookup"><span data-stu-id="8afcd-119">MailboxFull</span></span>](mailboxfull.md) <br/> |<span data-ttu-id="8afcd-120">Indique si la boîte aux lettres du destinataire est complète.</span><span class="sxs-lookup"><span data-stu-id="8afcd-120">Indicates whether the mailbox for the recipient is full.</span></span>  <br/> |
|[<span data-ttu-id="8afcd-121">CustomMailTip</span><span class="sxs-lookup"><span data-stu-id="8afcd-121">CustomMailTip</span></span>](custommailtip.md) <br/> |<span data-ttu-id="8afcd-122">Représente un message d’info-bulle personnalisée.</span><span class="sxs-lookup"><span data-stu-id="8afcd-122">Represents a customized mail tip message.</span></span>  <br/> |
|[<span data-ttu-id="8afcd-123">TotalMemberCount</span><span class="sxs-lookup"><span data-stu-id="8afcd-123">TotalMemberCount</span></span>](totalmembercount.md) <br/> |<span data-ttu-id="8afcd-124">Représente le nombre de tous les membres d’un groupe.</span><span class="sxs-lookup"><span data-stu-id="8afcd-124">Represents the count of all members in a group.</span></span>  <br/> |
|[<span data-ttu-id="8afcd-125">ExternalMemberCount</span><span class="sxs-lookup"><span data-stu-id="8afcd-125">ExternalMemberCount</span></span>](externalmembercount.md) <br/> |<span data-ttu-id="8afcd-126">Représente le nombre de membres externes dans un groupe.</span><span class="sxs-lookup"><span data-stu-id="8afcd-126">Represents the count of external members in a group.</span></span>  <br/> |
|[<span data-ttu-id="8afcd-127">MaxMessageSize</span><span class="sxs-lookup"><span data-stu-id="8afcd-127">MaxMessageSize</span></span>](maxmessagesize.md) <br/> |<span data-ttu-id="8afcd-128">Représente la taille maximale des messages que le destinataire peut accepter.</span><span class="sxs-lookup"><span data-stu-id="8afcd-128">Represents the maximum message size the recipient can accept.</span></span>  <br/> |
|[<span data-ttu-id="8afcd-129">DeliveryRestricted</span><span class="sxs-lookup"><span data-stu-id="8afcd-129">DeliveryRestricted</span></span>](deliveryrestricted.md) <br/> |<span data-ttu-id="8afcd-130">Indique si les restrictions de remise empêche le message de l’expéditeur d’atteindre le destinataire.</span><span class="sxs-lookup"><span data-stu-id="8afcd-130">Indicates whether delivery restrictions will prevent the sender's message from reaching the recipient.</span></span>  <br/> |
|[<span data-ttu-id="8afcd-131">IsModerated</span><span class="sxs-lookup"><span data-stu-id="8afcd-131">IsModerated</span></span>](ismoderated.md) <br/> |<span data-ttu-id="8afcd-132">Indique si la boîte aux lettres du destinataire est en cours modéré.</span><span class="sxs-lookup"><span data-stu-id="8afcd-132">Indicates whether the recipient's mailbox is being moderated.</span></span>  <br/> |
|[<span data-ttu-id="8afcd-133">InvalidRecipient (Infos-courrier)</span><span class="sxs-lookup"><span data-stu-id="8afcd-133">InvalidRecipient (MailTips)</span></span>](invalidrecipient-mailtips.md) <br/> |<span data-ttu-id="8afcd-134">Indique si le destinataire n’est pas valide.</span><span class="sxs-lookup"><span data-stu-id="8afcd-134">Indicates whether the recipient is invalid.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8afcd-135">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="8afcd-135">Parent elements</span></span>

|<span data-ttu-id="8afcd-136">**Élément**</span><span class="sxs-lookup"><span data-stu-id="8afcd-136">**Element**</span></span>|<span data-ttu-id="8afcd-137">**Description**</span><span class="sxs-lookup"><span data-stu-id="8afcd-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8afcd-138">MailTipsResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="8afcd-138">MailTipsResponseMessageType</span></span>](mailtipsresponsemessagetype.md) <br/> |<span data-ttu-id="8afcd-139">Représente les paramètres de conseils de messagerie.</span><span class="sxs-lookup"><span data-stu-id="8afcd-139">Represents mail tips settings.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8afcd-140">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="8afcd-140">Text value</span></span>

<span data-ttu-id="8afcd-141">Aucun.</span><span class="sxs-lookup"><span data-stu-id="8afcd-141">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8afcd-142">Remarques</span><span class="sxs-lookup"><span data-stu-id="8afcd-142">Remarks</span></span>

<span data-ttu-id="8afcd-143">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="8afcd-143">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8afcd-144">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="8afcd-144">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8afcd-145">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="8afcd-145">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="8afcd-146">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="8afcd-146">Schema Name</span></span>  <br/> |<span data-ttu-id="8afcd-147">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="8afcd-147">Messages schema</span></span>  <br/> |
|<span data-ttu-id="8afcd-148">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="8afcd-148">Validation File</span></span>  <br/> |<span data-ttu-id="8afcd-149">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="8afcd-149">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="8afcd-150">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="8afcd-150">Can be Empty</span></span>  <br/> |<span data-ttu-id="8afcd-151">False</span><span class="sxs-lookup"><span data-stu-id="8afcd-151">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8afcd-152">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="8afcd-152">See also</span></span>



- [<span data-ttu-id="8afcd-153">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="8afcd-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

