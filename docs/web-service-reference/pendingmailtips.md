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
description: L’élément PendingMailTips indique que les conseils de messagerie de cet élément n’ont pas pu être évalués avant l’expiration du délai de traitement du serveur.
ms.openlocfilehash: 715d68b367c3b7251c7406c10c1ec52dcd992a59
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529965"
---
# <a name="pendingmailtips"></a><span data-ttu-id="23c64-103">PendingMailTips</span><span class="sxs-lookup"><span data-stu-id="23c64-103">PendingMailTips</span></span>

<span data-ttu-id="23c64-104">L’élément **PendingMailTips** indique que les conseils de messagerie de cet élément n’ont pas pu être évalués avant l’expiration du délai de traitement du serveur.</span><span class="sxs-lookup"><span data-stu-id="23c64-104">The **PendingMailTips** element indicates that the mail tips in this element could not be evaluated before the server's processing timeout expired.</span></span> 
  
```XML
<PendingMailTips>All | OutOfOfficeMessage | MailboxFullStatus | CustomMailTip | ExternalMemberCount | TotalMemberCount | MaxMessageSize | DeliveryRestriction | ModerateStatus | InvalidRecipient</PendingMailTips>
```

 <span data-ttu-id="23c64-105">**MailTipTypes**</span><span class="sxs-lookup"><span data-stu-id="23c64-105">**MailTipTypes**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="23c64-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="23c64-106">Attributes and elements</span></span>

<span data-ttu-id="23c64-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="23c64-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="23c64-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="23c64-108">Attributes</span></span>

<span data-ttu-id="23c64-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="23c64-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="23c64-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="23c64-110">Child elements</span></span>

<span data-ttu-id="23c64-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="23c64-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="23c64-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="23c64-112">Parent elements</span></span>

|<span data-ttu-id="23c64-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="23c64-113">**Element**</span></span>|<span data-ttu-id="23c64-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="23c64-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="23c64-115">Infos-courrier</span><span class="sxs-lookup"><span data-stu-id="23c64-115">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="23c64-116">Représente les valeurs de différents types de conseils de courrier.</span><span class="sxs-lookup"><span data-stu-id="23c64-116">Represents values for various types of mail tips.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="23c64-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="23c64-117">Text value</span></span>

<span data-ttu-id="23c64-118">Le tableau suivant répertorie les valeurs possibles pour l’élément **PendingMailTips** .</span><span class="sxs-lookup"><span data-stu-id="23c64-118">The following table lists the possible values for the **PendingMailTips** element.</span></span> 
  
|<span data-ttu-id="23c64-119">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="23c64-119">**Value**</span></span>|<span data-ttu-id="23c64-120">**Description**</span><span class="sxs-lookup"><span data-stu-id="23c64-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="23c64-121">Tous</span><span class="sxs-lookup"><span data-stu-id="23c64-121">All</span></span>  <br/> |<span data-ttu-id="23c64-122">Représente tous les conseils de courrier disponibles.</span><span class="sxs-lookup"><span data-stu-id="23c64-122">Represents all available mail tips.</span></span>  <br/> |
|<span data-ttu-id="23c64-123">OutOfOfficeMessage</span><span class="sxs-lookup"><span data-stu-id="23c64-123">OutOfOfficeMessage</span></span>  <br/> |<span data-ttu-id="23c64-124">Représente le message absent (e) du bureau.</span><span class="sxs-lookup"><span data-stu-id="23c64-124">Represents the Out of Office (OOF) message.</span></span>  <br/> |
|<span data-ttu-id="23c64-125">MailboxFullStatus</span><span class="sxs-lookup"><span data-stu-id="23c64-125">MailboxFullStatus</span></span>  <br/> |<span data-ttu-id="23c64-126">Représente l’état d’une boîte aux lettres en cours de remplissage.</span><span class="sxs-lookup"><span data-stu-id="23c64-126">Represents the status for a mailbox being full.</span></span>  <br/> |
|<span data-ttu-id="23c64-127">CustomMailTip</span><span class="sxs-lookup"><span data-stu-id="23c64-127">CustomMailTip</span></span>  <br/> |<span data-ttu-id="23c64-128">Représente une info-bulle personnalisée.</span><span class="sxs-lookup"><span data-stu-id="23c64-128">Represents a custom mail tip.</span></span>  <br/> |
|<span data-ttu-id="23c64-129">ExternalMemberCount</span><span class="sxs-lookup"><span data-stu-id="23c64-129">ExternalMemberCount</span></span>  <br/> |<span data-ttu-id="23c64-130">Représente le nombre de membres externes.</span><span class="sxs-lookup"><span data-stu-id="23c64-130">Represents the count of external members.</span></span>  <br/> |
|<span data-ttu-id="23c64-131">TotalMemberCount</span><span class="sxs-lookup"><span data-stu-id="23c64-131">TotalMemberCount</span></span>  <br/> |<span data-ttu-id="23c64-132">Représente le décompte de tous les membres.</span><span class="sxs-lookup"><span data-stu-id="23c64-132">Represents the count of all members.</span></span>  <br/> |
|<span data-ttu-id="23c64-133">MaxMessageSize</span><span class="sxs-lookup"><span data-stu-id="23c64-133">MaxMessageSize</span></span>  <br/> |<span data-ttu-id="23c64-134">Représente la taille maximale des messages qu’un destinataire peut accepter.</span><span class="sxs-lookup"><span data-stu-id="23c64-134">Represents the maximum message size a recipient can accept.</span></span>  <br/> |
|<span data-ttu-id="23c64-135">DeliveryRestriction</span><span class="sxs-lookup"><span data-stu-id="23c64-135">DeliveryRestriction</span></span>  <br/> |<span data-ttu-id="23c64-136">Indique si les restrictions de remise empêchent le message de l’expéditeur d’atteindre le destinataire.</span><span class="sxs-lookup"><span data-stu-id="23c64-136">Indicates whether delivery restrictions will prevent the sender's message from reaching the recipient.</span></span>  <br/> |
|<span data-ttu-id="23c64-137">ModerationStatus</span><span class="sxs-lookup"><span data-stu-id="23c64-137">ModerationStatus</span></span>  <br/> |<span data-ttu-id="23c64-138">Indique si le message de l’expéditeur est examiné par un modérateur.</span><span class="sxs-lookup"><span data-stu-id="23c64-138">Indicates whether the sender's message will be reviewed by a moderator.</span></span>  <br/> |
|<span data-ttu-id="23c64-139">InvalidRecipient</span><span class="sxs-lookup"><span data-stu-id="23c64-139">InvalidRecipient</span></span>  <br/> |<span data-ttu-id="23c64-140">Indique si le destinataire n’est pas valide.</span><span class="sxs-lookup"><span data-stu-id="23c64-140">Indicates whether the recipient is invalid.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="23c64-141">Remarques</span><span class="sxs-lookup"><span data-stu-id="23c64-141">Remarks</span></span>

<span data-ttu-id="23c64-142">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="23c64-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="23c64-143">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="23c64-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="23c64-144">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="23c64-144">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="23c64-145">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="23c64-145">Schema Name</span></span>  <br/> |<span data-ttu-id="23c64-146">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="23c64-146">Types schema</span></span>  <br/> |
|<span data-ttu-id="23c64-147">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="23c64-147">Validation File</span></span>  <br/> |<span data-ttu-id="23c64-148">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="23c64-148">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="23c64-149">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="23c64-149">Can be Empty</span></span>  <br/> |<span data-ttu-id="23c64-150">False</span><span class="sxs-lookup"><span data-stu-id="23c64-150">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="23c64-151">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="23c64-151">See also</span></span>



- [<span data-ttu-id="23c64-152">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="23c64-152">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

