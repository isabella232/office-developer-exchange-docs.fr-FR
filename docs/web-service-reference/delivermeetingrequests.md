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
description: L’élément DeliverMeetingRequests définit la manière dont les demandes de réunion sont gérées entre le délégué et le principal. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 3998443613437bca2267678f7bc2c5584b779135
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463677"
---
# <a name="delivermeetingrequests"></a><span data-ttu-id="40de5-104">DeliverMeetingRequests</span><span class="sxs-lookup"><span data-stu-id="40de5-104">DeliverMeetingRequests</span></span>

<span data-ttu-id="40de5-105">L’élément **DeliverMeetingRequests** définit la manière dont les demandes de réunion sont gérées entre le délégué et le principal.</span><span class="sxs-lookup"><span data-stu-id="40de5-105">The **DeliverMeetingRequests** element defines how meeting requests are handled between the delegate and the principal.</span></span> <span data-ttu-id="40de5-106">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="40de5-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```XML
<DeliverMeetingRequests>DelegatesOnly or DelegatesAndMe or DelegatesAndSendInformationToMe or NoForward</DeliverMeetingRequests>
```

 <span data-ttu-id="40de5-107">**DeliverMeetingRequestsType**</span><span class="sxs-lookup"><span data-stu-id="40de5-107">**DeliverMeetingRequestsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="40de5-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="40de5-108">Attributes and elements</span></span>

<span data-ttu-id="40de5-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="40de5-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="40de5-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="40de5-110">Attributes</span></span>

<span data-ttu-id="40de5-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="40de5-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="40de5-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="40de5-112">Child elements</span></span>

<span data-ttu-id="40de5-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="40de5-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="40de5-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="40de5-114">Parent elements</span></span>

|<span data-ttu-id="40de5-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="40de5-115">**Element**</span></span>|<span data-ttu-id="40de5-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="40de5-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="40de5-117">AddDelegate</span><span class="sxs-lookup"><span data-stu-id="40de5-117">AddDelegate</span></span>](adddelegate.md) <br/> |<span data-ttu-id="40de5-118">Définit une demande d’ajout de délégués à une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="40de5-118">Defines a request to add delegates to a mailbox.</span></span> <span data-ttu-id="40de5-119">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="40de5-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="40de5-120">UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="40de5-120">UpdateDelegate</span></span>](updatedelegate.md) <br/> |<span data-ttu-id="40de5-121">Définit une demande de mise à jour des délégués dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="40de5-121">Defines a request to update delegates in a mailbox.</span></span> <span data-ttu-id="40de5-122">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="40de5-122">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="40de5-123">GetDelegateResponse</span><span class="sxs-lookup"><span data-stu-id="40de5-123">GetDelegateResponse</span></span>](getdelegateresponse.md) <br/> |<span data-ttu-id="40de5-124">Contient l’État et le résultat d’une demande GetDelegate.</span><span class="sxs-lookup"><span data-stu-id="40de5-124">Contains the status and result of a GetDelegate request.</span></span> <span data-ttu-id="40de5-125">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="40de5-125">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="40de5-126">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="40de5-126">Text value</span></span>

<span data-ttu-id="40de5-127">Le tableau suivant répertorie les valeurs possibles pour l’élément **DeliverMeetingRequests** .</span><span class="sxs-lookup"><span data-stu-id="40de5-127">The following table lists the possible values for the **DeliverMeetingRequests** element.</span></span> 
  
<span data-ttu-id="40de5-128">**Valeurs de l’élément DeliverMeetingRequests**</span><span class="sxs-lookup"><span data-stu-id="40de5-128">**DeliverMeetingRequests element values**</span></span>

|<span data-ttu-id="40de5-129">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="40de5-129">**Value**</span></span>|<span data-ttu-id="40de5-130">**Description**</span><span class="sxs-lookup"><span data-stu-id="40de5-130">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="40de5-131">DelegatesOnly</span><span class="sxs-lookup"><span data-stu-id="40de5-131">DelegatesOnly</span></span>  <br/> |<span data-ttu-id="40de5-132">Les demandes de réunion sont transférées au délégué et déplacées vers le dossier éléments supprimés dans la boîte aux lettres du principal.</span><span class="sxs-lookup"><span data-stu-id="40de5-132">Meeting requests are forwarded to the delegate and moved to the Deleted Items folder in the principal's mailbox.</span></span>  <br/> |
|<span data-ttu-id="40de5-133">DelegatesAndMe</span><span class="sxs-lookup"><span data-stu-id="40de5-133">DelegatesAndMe</span></span>  <br/> |<span data-ttu-id="40de5-134">Les demandes de réunion sont transmises au délégué et restent dans le dossier boîte de réception dans la boîte aux lettres principale.</span><span class="sxs-lookup"><span data-stu-id="40de5-134">Meeting requests are forwarded to the delegate and remain in the Inbox folder in the principal's mailbox.</span></span>  <br/> |
|<span data-ttu-id="40de5-135">DelegatesAndSendInformationToMe</span><span class="sxs-lookup"><span data-stu-id="40de5-135">DelegatesAndSendInformationToMe</span></span>  <br/> |<span data-ttu-id="40de5-136">Les demandes de réunion sont transmises au délégué et restent dans le dossier boîte de réception dans la boîte aux lettres du principal, mais les boutons accepter, provisoire et refuser n’apparaissent pas dans le volet de lecture de Microsoft Office Outlook.</span><span class="sxs-lookup"><span data-stu-id="40de5-136">Meeting requests are forwarded to the delegate and remain in the Inbox folder in the principal's mailbox, but the Accept, Tentative, and Decline buttons do not appear in the Microsoft Office Outlook reading pane.</span></span>  <br/> |
|<span data-ttu-id="40de5-137">Noforward</span><span class="sxs-lookup"><span data-stu-id="40de5-137">NoForward</span></span>  <br/> |<span data-ttu-id="40de5-138">Les demandes de réunion ne sont pas transférées au délégué.</span><span class="sxs-lookup"><span data-stu-id="40de5-138">Meeting requests are not forwarded to the delegate.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="40de5-139">Remarques</span><span class="sxs-lookup"><span data-stu-id="40de5-139">Remarks</span></span>

<span data-ttu-id="40de5-140">Le paramètre **DeliverMeetingRequests** affecte tous les délégués dans la boîte aux lettres d’un principal.</span><span class="sxs-lookup"><span data-stu-id="40de5-140">The **DeliverMeetingRequests** setting affects all delegates in a principal's mailbox.</span></span> 
  
<span data-ttu-id="40de5-141">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="40de5-141">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="40de5-142">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="40de5-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="40de5-143">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="40de5-143">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="40de5-144">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="40de5-144">Schema Name</span></span>  <br/> |<span data-ttu-id="40de5-145">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="40de5-145">Messages schema</span></span>  <br/> |
|<span data-ttu-id="40de5-146">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="40de5-146">Validation File</span></span>  <br/> |<span data-ttu-id="40de5-147">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="40de5-147">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="40de5-148">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="40de5-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="40de5-149">False</span><span class="sxs-lookup"><span data-stu-id="40de5-149">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="40de5-150">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="40de5-150">See also</span></span>

- [<span data-ttu-id="40de5-151">Opération AddDelegate</span><span class="sxs-lookup"><span data-stu-id="40de5-151">AddDelegate operation</span></span>](adddelegate-operation.md)  
- [<span data-ttu-id="40de5-152">Opération UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="40de5-152">UpdateDelegate operation</span></span>](updatedelegate-operation.md)  
- [<span data-ttu-id="40de5-153">Opération GetDelegate</span><span class="sxs-lookup"><span data-stu-id="40de5-153">GetDelegate operation</span></span>](getdelegate-operation.md)
- [<span data-ttu-id="40de5-154">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="40de5-154">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="40de5-155">Ajout de délégués</span><span class="sxs-lookup"><span data-stu-id="40de5-155">Adding Delegates</span></span>](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

