---
title: MessageTrackingReport
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MessageTrackingReport
api_type:
- schema
ms.assetid: 2740bcf6-f86d-4756-a0f2-24ed6e9b75f7
description: L’élément MessageTrackingReport contient un seul message est retourné dans une opération GetMessageTrackingReport.
ms.openlocfilehash: d01e0fbf099d096c7f255a8e94070e330577e6ca
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828457"
---
# <a name="messagetrackingreport"></a><span data-ttu-id="89f51-103">MessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="89f51-103">MessageTrackingReport</span></span>

<span data-ttu-id="89f51-104">L’élément **MessageTrackingReport** contient un seul message est retourné dans une [opération GetMessageTrackingReport](getmessagetrackingreport-operation.md).</span><span class="sxs-lookup"><span data-stu-id="89f51-104">The **MessageTrackingReport** element contains a single message that is returned in a [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>
  
```XML
<MessageTrackingReport>
   <Sender/>
   <PurportedSender/>
   <Subject/>
   <SubmitTime/>
   <OriginalRecipients/>
   <RecipientTrackingEvents/>
   <Properties/>
</MessageTrackingReport>
```

 <span data-ttu-id="89f51-105">**MessageTrackingReportType**</span><span class="sxs-lookup"><span data-stu-id="89f51-105">**MessageTrackingReportType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="89f51-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="89f51-106">Attributes and elements</span></span>

<span data-ttu-id="89f51-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="89f51-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="89f51-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="89f51-108">Attributes</span></span>

<span data-ttu-id="89f51-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="89f51-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="89f51-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="89f51-110">Child elements</span></span>

|<span data-ttu-id="89f51-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="89f51-111">**Element**</span></span>|<span data-ttu-id="89f51-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="89f51-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="89f51-113">Expéditeur (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="89f51-113">Sender (EmailAddressType)</span></span>](sender-emailaddresstype.md) <br/> |<span data-ttu-id="89f51-114">Contient des informations de contact pour l’expéditeur du message électronique.</span><span class="sxs-lookup"><span data-stu-id="89f51-114">Contains contact information for the sender of the e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="89f51-115">PurportedSender</span><span class="sxs-lookup"><span data-stu-id="89f51-115">PurportedSender</span></span>](purportedsender.md) <br/> |<span data-ttu-id="89f51-116">Contient des informations de contact pour l’expéditeur présumé d’un message électronique.</span><span class="sxs-lookup"><span data-stu-id="89f51-116">Contains contact information for the alleged sender of an e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="89f51-117">Objet</span><span class="sxs-lookup"><span data-stu-id="89f51-117">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="89f51-118">Contient l’objet du message électronique.</span><span class="sxs-lookup"><span data-stu-id="89f51-118">Contains the subject of the e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="89f51-119">SubmitTime</span><span class="sxs-lookup"><span data-stu-id="89f51-119">SubmitTime</span></span>](submittime.md) <br/> |<span data-ttu-id="89f51-120">Indique l’heure du jour à laquelle le message électronique a été envoyé.</span><span class="sxs-lookup"><span data-stu-id="89f51-120">Contains the time of day that the e-mail message was submitted.</span></span>  <br/> |
|[<span data-ttu-id="89f51-121">OriginalRecipients</span><span class="sxs-lookup"><span data-stu-id="89f51-121">OriginalRecipients</span></span>](originalrecipients.md) <br/> |<span data-ttu-id="89f51-122">Contient une liste des destinataires du message électronique.</span><span class="sxs-lookup"><span data-stu-id="89f51-122">Contains a list of the recipients of the e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="89f51-123">RecipientTrackingEvents</span><span class="sxs-lookup"><span data-stu-id="89f51-123">RecipientTrackingEvents</span></span>](recipienttrackingevents.md) <br/> |<span data-ttu-id="89f51-124">Contient une liste d’un ou plusieurs événements de suivi pour les destinataires.</span><span class="sxs-lookup"><span data-stu-id="89f51-124">Contains a list of one or more tracking events for the recipients.</span></span>  <br/> |
|[<span data-ttu-id="89f51-125">Propriétés (ArrayOfTrackingPropertiesType)</span><span class="sxs-lookup"><span data-stu-id="89f51-125">Properties (ArrayOfTrackingPropertiesType)</span></span>](properties-arrayoftrackingpropertiestype.md) <br/> |<span data-ttu-id="89f51-126">Contient une liste d’un ou plusieurs des propriétés de suivi.</span><span class="sxs-lookup"><span data-stu-id="89f51-126">Contains a list of one or more tracking properties.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="89f51-127">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="89f51-127">Parent elements</span></span>

|<span data-ttu-id="89f51-128">**Élément**</span><span class="sxs-lookup"><span data-stu-id="89f51-128">**Element**</span></span>|<span data-ttu-id="89f51-129">**Description**</span><span class="sxs-lookup"><span data-stu-id="89f51-129">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="89f51-130">GetMessageTrackingReportResponse</span><span class="sxs-lookup"><span data-stu-id="89f51-130">GetMessageTrackingReportResponse</span></span>](getmessagetrackingreportresponse.md) <br/> |<span data-ttu-id="89f51-131">Contient le résultat d’une seule demande [d’opération GetMessageTrackingReport](getmessagetrackingreport-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="89f51-131">Contains the result of a single [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="89f51-132">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="89f51-132">Text value</span></span>

<span data-ttu-id="89f51-133">Aucun.</span><span class="sxs-lookup"><span data-stu-id="89f51-133">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="89f51-134">Remarques</span><span class="sxs-lookup"><span data-stu-id="89f51-134">Remarks</span></span>

<span data-ttu-id="89f51-135">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="89f51-135">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="89f51-136">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="89f51-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="89f51-137">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="89f51-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="89f51-138">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="89f51-138">Schema Name</span></span>  <br/> |<span data-ttu-id="89f51-139">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="89f51-139">Messages schema</span></span>  <br/> |
|<span data-ttu-id="89f51-140">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="89f51-140">Validation File</span></span>  <br/> |<span data-ttu-id="89f51-141">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="89f51-141">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="89f51-142">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="89f51-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="89f51-143">False</span><span class="sxs-lookup"><span data-stu-id="89f51-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="89f51-144">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="89f51-144">See also</span></span>



[<span data-ttu-id="89f51-145">Opération FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="89f51-145">FindMessageTrackingReport operation</span></span>](findmessagetrackingreport-operation.md)
  
[<span data-ttu-id="89f51-146">Opération de GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="89f51-146">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="89f51-147">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="89f51-147">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
  
- [<span data-ttu-id="89f51-148">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="89f51-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

