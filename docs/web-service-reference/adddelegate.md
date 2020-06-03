---
title: AddDelegate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AddDelegate
api_type:
- schema
ms.assetid: 646fb994-229e-4d90-8b95-6541191cb3ae
description: L’élément AddDelegate définit une demande d’ajout de délégués à une boîte aux lettres. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: a08b83ad6e114c194073716c82228ea20ae1d3b7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466499"
---
# <a name="adddelegate"></a><span data-ttu-id="991d3-104">AddDelegate</span><span class="sxs-lookup"><span data-stu-id="991d3-104">AddDelegate</span></span>

<span data-ttu-id="991d3-105">L’élément **AddDelegate** définit une demande d’ajout de délégués à une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="991d3-105">The **AddDelegate** element defines a request to add delegates to a mailbox.</span></span> <span data-ttu-id="991d3-106">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="991d3-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<AddDelegate>
   <DelegateUsers/>
   <DeliverMeetingRequests/>
   <Mailbox/>
</AddDelegate>
```

 <span data-ttu-id="991d3-107">**AddDelegateType**</span><span class="sxs-lookup"><span data-stu-id="991d3-107">**AddDelegateType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="991d3-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="991d3-108">Attributes and elements</span></span>

<span data-ttu-id="991d3-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="991d3-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="991d3-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="991d3-110">Attributes</span></span>

<span data-ttu-id="991d3-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="991d3-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="991d3-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="991d3-112">Child elements</span></span>

|<span data-ttu-id="991d3-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="991d3-113">**Element**</span></span>|<span data-ttu-id="991d3-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="991d3-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="991d3-115">DelegateUsers</span><span class="sxs-lookup"><span data-stu-id="991d3-115">DelegateUsers</span></span>](delegateusers.md) <br/> |<span data-ttu-id="991d3-116">Contient les identités des délégués à ajouter à ou à mettre à jour dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="991d3-116">Contains the identities of delegates to add to or update in a mailbox.</span></span> <span data-ttu-id="991d3-117">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="991d3-117">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="991d3-118">DeliverMeetingRequests</span><span class="sxs-lookup"><span data-stu-id="991d3-118">DeliverMeetingRequests</span></span>](delivermeetingrequests.md) <br/> |<span data-ttu-id="991d3-119">Définit la manière dont les demandes de réunion sont gérées entre le délégué et le principal.</span><span class="sxs-lookup"><span data-stu-id="991d3-119">Defines how meeting requests are handled between the delegate and the principal.</span></span> <span data-ttu-id="991d3-120">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="991d3-120">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="991d3-121">Boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="991d3-121">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="991d3-122">Identifie un objet de service d'annuaire à extension messagerie Active Directory.</span><span class="sxs-lookup"><span data-stu-id="991d3-122">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="991d3-123">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="991d3-123">Parent elements</span></span>

<span data-ttu-id="991d3-124">Aucun.</span><span class="sxs-lookup"><span data-stu-id="991d3-124">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="991d3-125">Remarques</span><span class="sxs-lookup"><span data-stu-id="991d3-125">Remarks</span></span>

<span data-ttu-id="991d3-126">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="991d3-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="991d3-127">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="991d3-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="991d3-128">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="991d3-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="991d3-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="991d3-129">Schema Name</span></span>  <br/> |<span data-ttu-id="991d3-130">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="991d3-130">Messages schema</span></span>  <br/> |
|<span data-ttu-id="991d3-131">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="991d3-131">Validation File</span></span>  <br/> |<span data-ttu-id="991d3-132">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="991d3-132">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="991d3-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="991d3-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="991d3-134">False</span><span class="sxs-lookup"><span data-stu-id="991d3-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="991d3-135">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="991d3-135">See also</span></span>

- [<span data-ttu-id="991d3-136">Opération AddDelegate</span><span class="sxs-lookup"><span data-stu-id="991d3-136">AddDelegate operation</span></span>](adddelegate-operation.md)
- [<span data-ttu-id="991d3-137">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="991d3-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="991d3-138">Ajout de délégués</span><span class="sxs-lookup"><span data-stu-id="991d3-138">Adding Delegates</span></span>](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

