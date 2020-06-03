---
title: DelegateUser
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DelegateUser
api_type:
- schema
ms.assetid: aac4e74e-f69b-4c41-a0c9-489610330fbf
description: L’élément DelegateUser identifie un délégué unique à ajouter ou mettre à jour dans une boîte aux lettres ou un délégué renvoyé dans une réponse de gestion de délégué. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 40d9dacbd544436a3edf3213cf078cd33f961a74
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458802"
---
# <a name="delegateuser"></a><span data-ttu-id="2f8c0-104">DelegateUser</span><span class="sxs-lookup"><span data-stu-id="2f8c0-104">DelegateUser</span></span>

<span data-ttu-id="2f8c0-105">L’élément **DelegateUser** identifie un délégué unique à ajouter ou mettre à jour dans une boîte aux lettres ou un délégué renvoyé dans une réponse de gestion de délégué.</span><span class="sxs-lookup"><span data-stu-id="2f8c0-105">The **DelegateUser** element identifies a single delegate to add or update in a mailbox or a delegate returned in a delegate management response.</span></span> <span data-ttu-id="2f8c0-106">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="2f8c0-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<DelegateUser>
   <UserId/>
   <DelegatePermissions/>
   <ReceiveCopiesOfMeetingMessages/>
   <ViewPrivateItems/>
</DelegateUser>
```

<span data-ttu-id="2f8c0-107">**DelegateUserType**</span><span class="sxs-lookup"><span data-stu-id="2f8c0-107">**DelegateUserType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="2f8c0-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="2f8c0-108">Attributes and elements</span></span>

<span data-ttu-id="2f8c0-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="2f8c0-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2f8c0-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="2f8c0-110">Attributes</span></span>

<span data-ttu-id="2f8c0-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="2f8c0-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2f8c0-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="2f8c0-112">Child elements</span></span>

|<span data-ttu-id="2f8c0-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2f8c0-113">**Element**</span></span>|<span data-ttu-id="2f8c0-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="2f8c0-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2f8c0-115">UserId</span><span class="sxs-lookup"><span data-stu-id="2f8c0-115">UserId</span></span>](userid.md) <br/> |<span data-ttu-id="2f8c0-116">Identifie le délégué.</span><span class="sxs-lookup"><span data-stu-id="2f8c0-116">Identifies the delegate.</span></span> <span data-ttu-id="2f8c0-117">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="2f8c0-117">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="2f8c0-118">DelegatePermissions</span><span class="sxs-lookup"><span data-stu-id="2f8c0-118">DelegatePermissions</span></span>](delegatepermissions.md) <br/> |<span data-ttu-id="2f8c0-119">Contient les paramètres de niveau d’autorisation de délégué.</span><span class="sxs-lookup"><span data-stu-id="2f8c0-119">Contains the delegate permission level settings.</span></span> <span data-ttu-id="2f8c0-120">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="2f8c0-120">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="2f8c0-121">ReceiveCopiesOfMeetingMessages</span><span class="sxs-lookup"><span data-stu-id="2f8c0-121">ReceiveCopiesOfMeetingMessages</span></span>](receivecopiesofmeetingmessages.md) <br/> |<span data-ttu-id="2f8c0-122">Indique si un délégué reçoit des copies des messages relatifs à la réunion adressés au principal.</span><span class="sxs-lookup"><span data-stu-id="2f8c0-122">Indicates whether a delegate receives copies of meeting-related messages that are addressed to the principal.</span></span> <span data-ttu-id="2f8c0-123">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="2f8c0-123">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="2f8c0-124">ViewPrivateItems</span><span class="sxs-lookup"><span data-stu-id="2f8c0-124">ViewPrivateItems</span></span>](viewprivateitems.md) <br/> |<span data-ttu-id="2f8c0-125">Indique si un délégué dispose de l’autorisation d’afficher des éléments de calendrier privés dans la boîte aux lettres de l’entité de sécurité.</span><span class="sxs-lookup"><span data-stu-id="2f8c0-125">Indicates whether a delegate has permission to view private calendar items in the principal's mailbox.</span></span> <span data-ttu-id="2f8c0-126">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="2f8c0-126">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2f8c0-127">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="2f8c0-127">Parent elements</span></span>

|<span data-ttu-id="2f8c0-128">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2f8c0-128">**Element**</span></span>|<span data-ttu-id="2f8c0-129">**Description**</span><span class="sxs-lookup"><span data-stu-id="2f8c0-129">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2f8c0-130">DelegateUsers</span><span class="sxs-lookup"><span data-stu-id="2f8c0-130">DelegateUsers</span></span>](delegateusers.md) <br/> |<span data-ttu-id="2f8c0-131">Contient les identités des délégués à ajouter ou mettre à jour dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="2f8c0-131">Contains the identities of delegates to add or update in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="2f8c0-132">DelegateUserResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="2f8c0-132">DelegateUserResponseMessageType</span></span>](delegateuserresponsemessagetype.md) <br/> |<span data-ttu-id="2f8c0-133">Contient des messages de réponse pour les opérations de gestion de délégués.</span><span class="sxs-lookup"><span data-stu-id="2f8c0-133">Contains response messages for delegate management operations.</span></span> <span data-ttu-id="2f8c0-134">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="2f8c0-134">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2f8c0-135">Remarques</span><span class="sxs-lookup"><span data-stu-id="2f8c0-135">Remarks</span></span>

<span data-ttu-id="2f8c0-136">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="2f8c0-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2f8c0-137">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="2f8c0-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2f8c0-138">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="2f8c0-138">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2f8c0-139">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="2f8c0-139">Schema Name</span></span>  <br/> |<span data-ttu-id="2f8c0-140">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="2f8c0-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="2f8c0-141">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="2f8c0-141">Validation File</span></span>  <br/> |<span data-ttu-id="2f8c0-142">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2f8c0-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2f8c0-143">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="2f8c0-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="2f8c0-144">False</span><span class="sxs-lookup"><span data-stu-id="2f8c0-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2f8c0-145">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="2f8c0-145">See also</span></span>

- [<span data-ttu-id="2f8c0-146">Opération AddDelegate</span><span class="sxs-lookup"><span data-stu-id="2f8c0-146">AddDelegate operation</span></span>](adddelegate-operation.md) 
- [<span data-ttu-id="2f8c0-147">Opération UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="2f8c0-147">UpdateDelegate operation</span></span>](updatedelegate-operation.md)
- [<span data-ttu-id="2f8c0-148">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="2f8c0-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="2f8c0-149">Ajout de délégués</span><span class="sxs-lookup"><span data-stu-id="2f8c0-149">Adding Delegates</span></span>](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

