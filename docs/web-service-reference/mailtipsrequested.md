---
title: MailTipsRequested
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailTipsRequested
api_type:
- schema
ms.assetid: 8037bbe5-a37f-4f77-8209-27a94f9095ef
description: L’élément MailTipsRequested contient les types de conseils de messagerie demandés par le service.
ms.openlocfilehash: bcb2ebf15e628a04e8507f938d385cf113f2f2a3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465897"
---
# <a name="mailtipsrequested"></a><span data-ttu-id="dbede-103">MailTipsRequested</span><span class="sxs-lookup"><span data-stu-id="dbede-103">MailTipsRequested</span></span>

<span data-ttu-id="dbede-104">L’élément **MailTipsRequested** contient les types de conseils de messagerie demandés par le service.</span><span class="sxs-lookup"><span data-stu-id="dbede-104">The **MailTipsRequested** element contains the types of mail tips requested from the service.</span></span> 
  
```XML
<MailTipsRequested/>
```

 <span data-ttu-id="dbede-105">**MailTipTypes**</span><span class="sxs-lookup"><span data-stu-id="dbede-105">**MailTipTypes**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dbede-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="dbede-106">Attributes and elements</span></span>

<span data-ttu-id="dbede-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="dbede-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dbede-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="dbede-108">Attributes</span></span>

<span data-ttu-id="dbede-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="dbede-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dbede-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="dbede-110">Child elements</span></span>

<span data-ttu-id="dbede-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="dbede-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="dbede-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="dbede-112">Parent elements</span></span>

|<span data-ttu-id="dbede-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="dbede-113">**Element**</span></span>|<span data-ttu-id="dbede-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="dbede-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dbede-115">GetMailTips</span><span class="sxs-lookup"><span data-stu-id="dbede-115">GetMailTips</span></span>](getmailtips.md) <br/> |<span data-ttu-id="dbede-116">Contient les destinataires et les types de conseils de messagerie à récupérer.</span><span class="sxs-lookup"><span data-stu-id="dbede-116">Contains the recipients and types of mail tips to retrieve.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="dbede-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="dbede-117">Text value</span></span>

<span data-ttu-id="dbede-118">Le tableau suivant répertorie les valeurs possibles pour l’élément **MailTipsRequested** .</span><span class="sxs-lookup"><span data-stu-id="dbede-118">The following table lists the possible values for the **MailTipsRequested** element.</span></span> 
  
|<span data-ttu-id="dbede-119">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="dbede-119">**Value**</span></span>|<span data-ttu-id="dbede-120">**Description**</span><span class="sxs-lookup"><span data-stu-id="dbede-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="dbede-121">Tous</span><span class="sxs-lookup"><span data-stu-id="dbede-121">All</span></span>  <br/> |<span data-ttu-id="dbede-122">Représente tous les conseils de courrier disponibles.</span><span class="sxs-lookup"><span data-stu-id="dbede-122">Represents all available mail tips.</span></span>  <br/> |
|<span data-ttu-id="dbede-123">OutOfOfficeMessage</span><span class="sxs-lookup"><span data-stu-id="dbede-123">OutOfOfficeMessage</span></span>  <br/> |<span data-ttu-id="dbede-124">Représente le message absent (e) du bureau.</span><span class="sxs-lookup"><span data-stu-id="dbede-124">Represents the Out of Office (OOF) message.</span></span>  <br/> |
|<span data-ttu-id="dbede-125">MailboxFullStatus</span><span class="sxs-lookup"><span data-stu-id="dbede-125">MailboxFullStatus</span></span>  <br/> |<span data-ttu-id="dbede-126">Représente l’état d’une boîte aux lettres qui est saturée.</span><span class="sxs-lookup"><span data-stu-id="dbede-126">Represents the status for a mailbox that is full.</span></span>  <br/> |
|<span data-ttu-id="dbede-127">CustomMailTip</span><span class="sxs-lookup"><span data-stu-id="dbede-127">CustomMailTip</span></span>  <br/> |<span data-ttu-id="dbede-128">Représente une info-bulle personnalisée.</span><span class="sxs-lookup"><span data-stu-id="dbede-128">Represents a custom mail tip.</span></span>  <br/> |
|<span data-ttu-id="dbede-129">ExternalMemberCount</span><span class="sxs-lookup"><span data-stu-id="dbede-129">ExternalMemberCount</span></span>  <br/> |<span data-ttu-id="dbede-130">Représente le nombre de membres externes.</span><span class="sxs-lookup"><span data-stu-id="dbede-130">Represents the count of external members.</span></span>  <br/> |
|<span data-ttu-id="dbede-131">TotalMemberCount</span><span class="sxs-lookup"><span data-stu-id="dbede-131">TotalMemberCount</span></span>  <br/> |<span data-ttu-id="dbede-132">Représente le décompte de tous les membres.</span><span class="sxs-lookup"><span data-stu-id="dbede-132">Represents the count of all members.</span></span>  <br/> |
|<span data-ttu-id="dbede-133">MaxMessageSize</span><span class="sxs-lookup"><span data-stu-id="dbede-133">MaxMessageSize</span></span>  <br/> |<span data-ttu-id="dbede-134">Représente la taille maximale des messages qu’un destinataire peut accepter.</span><span class="sxs-lookup"><span data-stu-id="dbede-134">Represents the maximum message size a recipient can accept.</span></span>  <br/> |
|<span data-ttu-id="dbede-135">DeliveryRestriction</span><span class="sxs-lookup"><span data-stu-id="dbede-135">DeliveryRestriction</span></span>  <br/> |<span data-ttu-id="dbede-136">Indique si les restrictions de remise empêchent le message de l’expéditeur d’atteindre le destinataire.</span><span class="sxs-lookup"><span data-stu-id="dbede-136">Indicates whether delivery restrictions will prevent the sender's message from reaching the recipient.</span></span>  <br/> |
|<span data-ttu-id="dbede-137">ModerationStatus</span><span class="sxs-lookup"><span data-stu-id="dbede-137">ModerationStatus</span></span>  <br/> |<span data-ttu-id="dbede-138">Indique si le message de l’expéditeur est examiné par un modérateur.</span><span class="sxs-lookup"><span data-stu-id="dbede-138">Indicates whether the sender's message will be reviewed by a moderator.</span></span>  <br/> |
|<span data-ttu-id="dbede-139">InvalidRecipient</span><span class="sxs-lookup"><span data-stu-id="dbede-139">InvalidRecipient</span></span>  <br/> |<span data-ttu-id="dbede-140">Indique si le destinataire n’est pas valide.</span><span class="sxs-lookup"><span data-stu-id="dbede-140">Indicates whether the recipient is invalid.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="dbede-141">Remarques</span><span class="sxs-lookup"><span data-stu-id="dbede-141">Remarks</span></span>

<span data-ttu-id="dbede-142">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="dbede-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dbede-143">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="dbede-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dbede-144">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="dbede-144">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="dbede-145">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="dbede-145">Schema Name</span></span>  <br/> |<span data-ttu-id="dbede-146">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="dbede-146">Messages schema</span></span>  <br/> |
|<span data-ttu-id="dbede-147">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="dbede-147">Validation File</span></span>  <br/> |<span data-ttu-id="dbede-148">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="dbede-148">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="dbede-149">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="dbede-149">Can be Empty</span></span>  <br/> |<span data-ttu-id="dbede-150">False</span><span class="sxs-lookup"><span data-stu-id="dbede-150">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dbede-151">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="dbede-151">See also</span></span>



- [<span data-ttu-id="dbede-152">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="dbede-152">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

