---
title: DeliverMeetingRequests
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeliverMeetingRequests
api_type:
- schema
ms.assetid: 04b999af-0b27-4e6d-a8b1-400955a1afaa
description: L’élément DeliverMeetingRequests définit la gestion des demandes de réunion entre le délégué et l’entité de sécurité. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 803bd2da72bdb21b507a59cc11635a40d4431acf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755889"
---
# <a name="delivermeetingrequests"></a><span data-ttu-id="300ec-104">DeliverMeetingRequests</span><span class="sxs-lookup"><span data-stu-id="300ec-104">DeliverMeetingRequests</span></span>

<span data-ttu-id="300ec-105">L’élément **DeliverMeetingRequests** définit la gestion des demandes de réunion entre le délégué et l’entité de sécurité.</span><span class="sxs-lookup"><span data-stu-id="300ec-105">The **DeliverMeetingRequests** element defines how meeting requests are handled between the delegate and the principal.</span></span> <span data-ttu-id="300ec-106">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="300ec-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```XML
<DeliverMeetingRequests>DelegatesOnly or DelegatesAndMe or DelegatesAndSendInformationToMe or NoForward</DeliverMeetingRequests>
```

 <span data-ttu-id="300ec-107">**DeliverMeetingRequestsType**</span><span class="sxs-lookup"><span data-stu-id="300ec-107">**DeliverMeetingRequestsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="300ec-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="300ec-108">Attributes and elements</span></span>

<span data-ttu-id="300ec-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="300ec-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="300ec-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="300ec-110">Attributes</span></span>

<span data-ttu-id="300ec-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="300ec-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="300ec-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="300ec-112">Child elements</span></span>

<span data-ttu-id="300ec-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="300ec-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="300ec-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="300ec-114">Parent elements</span></span>

|<span data-ttu-id="300ec-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="300ec-115">**Element**</span></span>|<span data-ttu-id="300ec-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="300ec-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="300ec-117">AddDelegate</span><span class="sxs-lookup"><span data-stu-id="300ec-117">AddDelegate</span></span>](adddelegate.md) <br/> |<span data-ttu-id="300ec-118">Définit une demande pour ajouter des délégués à une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="300ec-118">Defines a request to add delegates to a mailbox.</span></span> <span data-ttu-id="300ec-119">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="300ec-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="300ec-120">UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="300ec-120">UpdateDelegate</span></span>](updatedelegate.md) <br/> |<span data-ttu-id="300ec-121">Définit une demande de mise à jour des délégués dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="300ec-121">Defines a request to update delegates in a mailbox.</span></span> <span data-ttu-id="300ec-122">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="300ec-122">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="300ec-123">GetDelegateResponse</span><span class="sxs-lookup"><span data-stu-id="300ec-123">GetDelegateResponse</span></span>](getdelegateresponse.md) <br/> |<span data-ttu-id="300ec-124">Contient l’état et les résultats d’une demande GetDelegate.</span><span class="sxs-lookup"><span data-stu-id="300ec-124">Contains the status and result of a GetDelegate request.</span></span> <span data-ttu-id="300ec-125">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="300ec-125">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="300ec-126">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="300ec-126">Text value</span></span>

<span data-ttu-id="300ec-127">Le tableau suivant répertorie les valeurs possibles pour l’élément **DeliverMeetingRequests** .</span><span class="sxs-lookup"><span data-stu-id="300ec-127">The following table lists the possible values for the **DeliverMeetingRequests** element.</span></span> 
  
<span data-ttu-id="300ec-128">**Valeurs des éléments DeliverMeetingRequests**</span><span class="sxs-lookup"><span data-stu-id="300ec-128">**DeliverMeetingRequests element values**</span></span>

|<span data-ttu-id="300ec-129">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="300ec-129">**Value**</span></span>|<span data-ttu-id="300ec-130">**Description**</span><span class="sxs-lookup"><span data-stu-id="300ec-130">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="300ec-131">DelegatesOnly</span><span class="sxs-lookup"><span data-stu-id="300ec-131">DelegatesOnly</span></span>  <br/> |<span data-ttu-id="300ec-132">Demandes de réunion sont transmises au délégué et déplacés vers le dossier éléments supprimés dans la boîte aux lettres de l’entité de sécurité.</span><span class="sxs-lookup"><span data-stu-id="300ec-132">Meeting requests are forwarded to the delegate and moved to the Deleted Items folder in the principal's mailbox.</span></span>  <br/> |
|<span data-ttu-id="300ec-133">DelegatesAndMe</span><span class="sxs-lookup"><span data-stu-id="300ec-133">DelegatesAndMe</span></span>  <br/> |<span data-ttu-id="300ec-134">Demandes de réunion sont transférés vers le délégué et restent dans le dossier boîte de réception dans la boîte aux lettres de l’entité de sécurité.</span><span class="sxs-lookup"><span data-stu-id="300ec-134">Meeting requests are forwarded to the delegate and remain in the Inbox folder in the principal's mailbox.</span></span>  <br/> |
|<span data-ttu-id="300ec-135">DelegatesAndSendInformationToMe</span><span class="sxs-lookup"><span data-stu-id="300ec-135">DelegatesAndSendInformationToMe</span></span>  <br/> |<span data-ttu-id="300ec-136">Demandes de réunion sont transférés vers le délégué et restent dans le dossier boîte de réception dans la boîte aux lettres de l’entité de sécurité, mais les boutons Accepter, provisoire et refuser n’apparaissent pas dans le volet de lecture de Microsoft Office Outlook.</span><span class="sxs-lookup"><span data-stu-id="300ec-136">Meeting requests are forwarded to the delegate and remain in the Inbox folder in the principal's mailbox, but the Accept, Tentative, and Decline buttons do not appear in the Microsoft Office Outlook reading pane.</span></span>  <br/> |
|<span data-ttu-id="300ec-137">NoForward</span><span class="sxs-lookup"><span data-stu-id="300ec-137">NoForward</span></span>  <br/> |<span data-ttu-id="300ec-138">Demandes de réunion ne sont pas transférés vers le délégué.</span><span class="sxs-lookup"><span data-stu-id="300ec-138">Meeting requests are not forwarded to the delegate.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="300ec-139">Remarques</span><span class="sxs-lookup"><span data-stu-id="300ec-139">Remarks</span></span>

<span data-ttu-id="300ec-140">Le paramètre **DeliverMeetingRequests** affecte tous les délégués dans la boîte aux lettres d’un utilisateur principal.</span><span class="sxs-lookup"><span data-stu-id="300ec-140">The **DeliverMeetingRequests** setting affects all delegates in a principal's mailbox.</span></span> 
  
<span data-ttu-id="300ec-141">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="300ec-141">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="300ec-142">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="300ec-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="300ec-143">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="300ec-143">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="300ec-144">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="300ec-144">Schema Name</span></span>  <br/> |<span data-ttu-id="300ec-145">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="300ec-145">Messages schema</span></span>  <br/> |
|<span data-ttu-id="300ec-146">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="300ec-146">Validation File</span></span>  <br/> |<span data-ttu-id="300ec-147">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="300ec-147">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="300ec-148">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="300ec-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="300ec-149">False</span><span class="sxs-lookup"><span data-stu-id="300ec-149">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="300ec-150">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="300ec-150">See also</span></span>

- [<span data-ttu-id="300ec-151">Opération AddDelegate</span><span class="sxs-lookup"><span data-stu-id="300ec-151">AddDelegate operation</span></span>](adddelegate-operation.md)  
- [<span data-ttu-id="300ec-152">Opération UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="300ec-152">UpdateDelegate operation</span></span>](updatedelegate-operation.md)  
- [<span data-ttu-id="300ec-153">Opération GetDelegate</span><span class="sxs-lookup"><span data-stu-id="300ec-153">GetDelegate operation</span></span>](getdelegate-operation.md)
- [<span data-ttu-id="300ec-154">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="300ec-154">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="300ec-155">Ajout de délégués</span><span class="sxs-lookup"><span data-stu-id="300ec-155">Adding Delegates</span></span>](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

