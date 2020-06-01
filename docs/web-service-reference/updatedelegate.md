---
title: UpdateDelegate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateDelegate
api_type:
- schema
ms.assetid: c6ae99c4-18b0-4136-90ab-12cf15e15f91
description: L’élément UpdateDelegate définit une demande de mise à jour des délégués dans une boîte aux lettres. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 17d69eb8c539217d39e1dd0c2616261d02ad304d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468872"
---
# <a name="updatedelegate"></a><span data-ttu-id="63406-104">UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="63406-104">UpdateDelegate</span></span>

<span data-ttu-id="63406-105">L’élément **UpdateDelegate** définit une demande de mise à jour des délégués dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="63406-105">The **UpdateDelegate** element defines a request to update delegates in a mailbox.</span></span> <span data-ttu-id="63406-106">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="63406-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<UpdateDelegate>
      <DelegateUsers/>
   <DeliverMeetingRequests/>
      <Mailbox/>
</UpdateDelegate>
```

 <span data-ttu-id="63406-107">**UpdateDelegateType**</span><span class="sxs-lookup"><span data-stu-id="63406-107">**UpdateDelegateType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="63406-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="63406-108">Attributes and elements</span></span>

<span data-ttu-id="63406-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="63406-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="63406-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="63406-110">Attributes</span></span>

<span data-ttu-id="63406-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="63406-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="63406-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="63406-112">Child elements</span></span>

|<span data-ttu-id="63406-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="63406-113">**Element**</span></span>|<span data-ttu-id="63406-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="63406-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="63406-115">DelegateUsers</span><span class="sxs-lookup"><span data-stu-id="63406-115">DelegateUsers</span></span>](delegateusers.md) <br/> |<span data-ttu-id="63406-116">Contient un tableau d’éléments [DelegateUser](delegateuser.md) qui identifient les délégués et les mises à jour à appliquer aux délégués.</span><span class="sxs-lookup"><span data-stu-id="63406-116">Contains an array of [DelegateUser](delegateuser.md) elements that identify the delegates and the updates to apply to the delegates.</span></span> <span data-ttu-id="63406-117">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="63406-117">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="63406-118">DeliverMeetingRequests</span><span class="sxs-lookup"><span data-stu-id="63406-118">DeliverMeetingRequests</span></span>](delivermeetingrequests.md) <br/> |<span data-ttu-id="63406-119">Définit la manière dont les demandes de réunion sont gérées entre le délégué et le principal.</span><span class="sxs-lookup"><span data-stu-id="63406-119">Defines how meeting requests are handled between the delegate and the principal.</span></span> <span data-ttu-id="63406-120">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="63406-120">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="63406-121">Boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="63406-121">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="63406-122">Identifie un objet de service d'annuaire à extension messagerie Active Directory.</span><span class="sxs-lookup"><span data-stu-id="63406-122">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="63406-123">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="63406-123">Parent elements</span></span>

<span data-ttu-id="63406-124">Aucun.</span><span class="sxs-lookup"><span data-stu-id="63406-124">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="63406-125">Remarques</span><span class="sxs-lookup"><span data-stu-id="63406-125">Remarks</span></span>

<span data-ttu-id="63406-126">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="63406-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="63406-127">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="63406-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="63406-128">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="63406-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="63406-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="63406-129">Schema Name</span></span>  <br/> |<span data-ttu-id="63406-130">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="63406-130">Messages schema</span></span>  <br/> |
|<span data-ttu-id="63406-131">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="63406-131">Validation File</span></span>  <br/> |<span data-ttu-id="63406-132">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="63406-132">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="63406-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="63406-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="63406-134">False</span><span class="sxs-lookup"><span data-stu-id="63406-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="63406-135">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="63406-135">See also</span></span>



[<span data-ttu-id="63406-136">Opération UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="63406-136">UpdateDelegate operation</span></span>](updatedelegate-operation.md)


- [<span data-ttu-id="63406-137">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="63406-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

