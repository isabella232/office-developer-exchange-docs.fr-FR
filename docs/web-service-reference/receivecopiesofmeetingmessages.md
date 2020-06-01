---
title: ReceiveCopiesOfMeetingMessages
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ReceiveCopiesOfMeetingMessages
api_type:
- schema
ms.assetid: 65217ca8-6aea-47eb-a989-e6cce25f5f09
description: L’élément ReceiveCopiesOfMeetingMessages indique si un délégué reçoit des copies des messages relatifs à la réunion adressés au principal. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: af6e220304f88c4db00ab675077dcd9bf581ea9e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468263"
---
# <a name="receivecopiesofmeetingmessages"></a><span data-ttu-id="88b51-104">ReceiveCopiesOfMeetingMessages</span><span class="sxs-lookup"><span data-stu-id="88b51-104">ReceiveCopiesOfMeetingMessages</span></span>

<span data-ttu-id="88b51-105">L’élément **ReceiveCopiesOfMeetingMessages** indique si un délégué reçoit des copies des messages relatifs à la réunion adressés au principal.</span><span class="sxs-lookup"><span data-stu-id="88b51-105">The **ReceiveCopiesOfMeetingMessages** element indicates whether a delegate receives copies of meeting-related messages that are addressed to the principal.</span></span> <span data-ttu-id="88b51-106">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="88b51-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<ReceiveCopiesOfMeetingMessages>true or false</ReceiveCopiesOfMeetingMessages>
```

 <span data-ttu-id="88b51-107">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="88b51-107">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="88b51-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="88b51-108">Attributes and elements</span></span>

<span data-ttu-id="88b51-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="88b51-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="88b51-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="88b51-110">Attributes</span></span>

<span data-ttu-id="88b51-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="88b51-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="88b51-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="88b51-112">Child elements</span></span>

<span data-ttu-id="88b51-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="88b51-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="88b51-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="88b51-114">Parent elements</span></span>

|<span data-ttu-id="88b51-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="88b51-115">**Element**</span></span>|<span data-ttu-id="88b51-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="88b51-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="88b51-117">DelegateUser</span><span class="sxs-lookup"><span data-stu-id="88b51-117">DelegateUser</span></span>](delegateuser.md) <br/> |<span data-ttu-id="88b51-118">Identifie un seul délégué à ajouter ou mettre à jour dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="88b51-118">Identifies a single delegate to add or update in a mailbox.</span></span> <span data-ttu-id="88b51-119">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="88b51-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="88b51-120">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="88b51-120">Text value</span></span>

<span data-ttu-id="88b51-121">Une valeur de texte **true** indique qu’un délégué reçoit une copie des messages de réunion.</span><span class="sxs-lookup"><span data-stu-id="88b51-121">A text value of **true** indicates that a delegate receives a copy of meeting messages.</span></span> <span data-ttu-id="88b51-122">Une valeur de texte **false** indique qu’un délégué ne reçoit pas de copie des messages de réunion.</span><span class="sxs-lookup"><span data-stu-id="88b51-122">A text value of **false** indicates that a delegate does not receive a copy of meeting messages.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="88b51-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="88b51-123">Remarks</span></span>

<span data-ttu-id="88b51-124">Lorsque **ReceiveCopiesOfMeetingMessages** est défini sur **false**, le délégué peut toujours envoyer un message de la part du principal, mais ne reçoit pas de messages liés à la réunion.</span><span class="sxs-lookup"><span data-stu-id="88b51-124">When **ReceiveCopiesOfMeetingMessages** is set to **false**, the delegate can still send message on behalf of the principal, but will not receive any meeting-related messages.</span></span>
  
<span data-ttu-id="88b51-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="88b51-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="88b51-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="88b51-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="88b51-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="88b51-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="88b51-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="88b51-128">Schema Name</span></span>  <br/> |<span data-ttu-id="88b51-129">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="88b51-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="88b51-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="88b51-130">Validation File</span></span>  <br/> |<span data-ttu-id="88b51-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="88b51-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="88b51-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="88b51-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="88b51-133">False</span><span class="sxs-lookup"><span data-stu-id="88b51-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="88b51-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="88b51-134">See also</span></span>



[<span data-ttu-id="88b51-135">Opération AddDelegate</span><span class="sxs-lookup"><span data-stu-id="88b51-135">AddDelegate operation</span></span>](adddelegate-operation.md)
  
[<span data-ttu-id="88b51-136">Opération UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="88b51-136">UpdateDelegate operation</span></span>](updatedelegate-operation.md)


- [<span data-ttu-id="88b51-137">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="88b51-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="88b51-138">Ajout de délégués</span><span class="sxs-lookup"><span data-stu-id="88b51-138">Adding Delegates</span></span>](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

