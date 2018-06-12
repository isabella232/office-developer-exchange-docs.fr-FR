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
description: L’élément ReceiveCopiesOfMeetingMessages indique si un délégué reçoive des copies de messages adressés à l’entité de sécurité liées à la réunion. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: e39a5d3255268b418fa956959da5ae0ea062d831
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828967"
---
# <a name="receivecopiesofmeetingmessages"></a><span data-ttu-id="aec1d-104">ReceiveCopiesOfMeetingMessages</span><span class="sxs-lookup"><span data-stu-id="aec1d-104">ReceiveCopiesOfMeetingMessages</span></span>

<span data-ttu-id="aec1d-105">L’élément **ReceiveCopiesOfMeetingMessages** indique si un délégué reçoive des copies de messages adressés à l’entité de sécurité liées à la réunion.</span><span class="sxs-lookup"><span data-stu-id="aec1d-105">The **ReceiveCopiesOfMeetingMessages** element indicates whether a delegate receives copies of meeting-related messages that are addressed to the principal.</span></span> <span data-ttu-id="aec1d-106">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="aec1d-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<ReceiveCopiesOfMeetingMessages>true or false</ReceiveCopiesOfMeetingMessages>
```

 <span data-ttu-id="aec1d-107">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="aec1d-107">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="aec1d-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="aec1d-108">Attributes and elements</span></span>

<span data-ttu-id="aec1d-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="aec1d-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="aec1d-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="aec1d-110">Attributes</span></span>

<span data-ttu-id="aec1d-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="aec1d-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="aec1d-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="aec1d-112">Child elements</span></span>

<span data-ttu-id="aec1d-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="aec1d-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="aec1d-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="aec1d-114">Parent elements</span></span>

|<span data-ttu-id="aec1d-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="aec1d-115">**Element**</span></span>|<span data-ttu-id="aec1d-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="aec1d-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aec1d-117">Utilisateur_délégué</span><span class="sxs-lookup"><span data-stu-id="aec1d-117">DelegateUser</span></span>](delegateuser.md) <br/> |<span data-ttu-id="aec1d-118">Identifie un délégué pour ajouter ou mettre à jour dans une boîte aux lettres unique.</span><span class="sxs-lookup"><span data-stu-id="aec1d-118">Identifies a single delegate to add or update in a mailbox.</span></span> <span data-ttu-id="aec1d-119">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="aec1d-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="aec1d-120">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="aec1d-120">Text value</span></span>

<span data-ttu-id="aec1d-121">Une valeur de texte de **la valeur true** indique qu’un délégué reçoit une copie des messages de la réunion.</span><span class="sxs-lookup"><span data-stu-id="aec1d-121">A text value of **true** indicates that a delegate receives a copy of meeting messages.</span></span> <span data-ttu-id="aec1d-122">Texte la valeur **false** indique qu’un délégué ne reçoit pas d’une copie des messages de la réunion.</span><span class="sxs-lookup"><span data-stu-id="aec1d-122">A text value of **false** indicates that a delegate does not receive a copy of meeting messages.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="aec1d-123">Note</span><span class="sxs-lookup"><span data-stu-id="aec1d-123">Remarks</span></span>

<span data-ttu-id="aec1d-124">Lorsque **ReceiveCopiesOfMeetingMessages** est défini sur **false**, le délégué peut encore envoyer des messages au nom de l’entité de sécurité, mais il ne recevra pas tous les messages liés à la réunion.</span><span class="sxs-lookup"><span data-stu-id="aec1d-124">When **ReceiveCopiesOfMeetingMessages** is set to **false**, the delegate can still send message on behalf of the principal, but will not receive any meeting-related messages.</span></span>
  
<span data-ttu-id="aec1d-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="aec1d-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="aec1d-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="aec1d-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="aec1d-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="aec1d-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="aec1d-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="aec1d-128">Schema Name</span></span>  <br/> |<span data-ttu-id="aec1d-129">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="aec1d-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="aec1d-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="aec1d-130">Validation File</span></span>  <br/> |<span data-ttu-id="aec1d-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="aec1d-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="aec1d-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="aec1d-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="aec1d-133">False</span><span class="sxs-lookup"><span data-stu-id="aec1d-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="aec1d-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="aec1d-134">See also</span></span>



[<span data-ttu-id="aec1d-135">Opération AddDelegate</span><span class="sxs-lookup"><span data-stu-id="aec1d-135">AddDelegate operation</span></span>](adddelegate-operation.md)
  
[<span data-ttu-id="aec1d-136">Opération UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="aec1d-136">UpdateDelegate operation</span></span>](updatedelegate-operation.md)


- [<span data-ttu-id="aec1d-137">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="aec1d-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="aec1d-138">Ajout de délégués</span><span class="sxs-lookup"><span data-stu-id="aec1d-138">Adding Delegates</span></span>](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

