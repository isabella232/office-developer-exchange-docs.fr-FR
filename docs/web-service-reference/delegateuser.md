---
title: Utilisateur_délégué
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
description: L’élément Utilisateur_délégué identifie un seul délégué pour ajouter ou mettre à jour dans une boîte aux lettres ou un délégué renvoyés dans une réponse de gestion de délégué. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 72ddc313a5a76cd0345918cad63b7775ff85026b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755838"
---
# <a name="delegateuser"></a><span data-ttu-id="30726-104">Utilisateur_délégué</span><span class="sxs-lookup"><span data-stu-id="30726-104">DelegateUser</span></span>

<span data-ttu-id="30726-105">L’élément **Utilisateur_délégué** identifie un seul délégué pour ajouter ou mettre à jour dans une boîte aux lettres ou un délégué renvoyés dans une réponse de gestion de délégué.</span><span class="sxs-lookup"><span data-stu-id="30726-105">The **DelegateUser** element identifies a single delegate to add or update in a mailbox or a delegate returned in a delegate management response.</span></span> <span data-ttu-id="30726-106">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="30726-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<DelegateUser>
   <UserId/>
   <DelegatePermissions/>
   <ReceiveCopiesOfMeetingMessages/>
   <ViewPrivateItems/>
</DelegateUser>
```

<span data-ttu-id="30726-107">**DelegateUserType**</span><span class="sxs-lookup"><span data-stu-id="30726-107">**DelegateUserType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="30726-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="30726-108">Attributes and elements</span></span>

<span data-ttu-id="30726-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="30726-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="30726-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="30726-110">Attributes</span></span>

<span data-ttu-id="30726-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="30726-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="30726-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="30726-112">Child elements</span></span>

|<span data-ttu-id="30726-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="30726-113">**Element**</span></span>|<span data-ttu-id="30726-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="30726-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="30726-115">Nom d’utilisateur</span><span class="sxs-lookup"><span data-stu-id="30726-115">UserId</span></span>](userid.md) <br/> |<span data-ttu-id="30726-116">Identifie le délégué.</span><span class="sxs-lookup"><span data-stu-id="30726-116">Identifies the delegate.</span></span> <span data-ttu-id="30726-117">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="30726-117">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="30726-118">DelegatePermissions</span><span class="sxs-lookup"><span data-stu-id="30726-118">DelegatePermissions</span></span>](delegatepermissions.md) <br/> |<span data-ttu-id="30726-119">Contient les paramètres de niveau d’autorisation délégué.</span><span class="sxs-lookup"><span data-stu-id="30726-119">Contains the delegate permission level settings.</span></span> <span data-ttu-id="30726-120">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="30726-120">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="30726-121">ReceiveCopiesOfMeetingMessages</span><span class="sxs-lookup"><span data-stu-id="30726-121">ReceiveCopiesOfMeetingMessages</span></span>](receivecopiesofmeetingmessages.md) <br/> |<span data-ttu-id="30726-122">Indique si un délégué reçoive des copies de messages adressés à l’entité de sécurité liées à la réunion.</span><span class="sxs-lookup"><span data-stu-id="30726-122">Indicates whether a delegate receives copies of meeting-related messages that are addressed to the principal.</span></span> <span data-ttu-id="30726-123">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="30726-123">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="30726-124">ViewPrivateItems</span><span class="sxs-lookup"><span data-stu-id="30726-124">ViewPrivateItems</span></span>](viewprivateitems.md) <br/> |<span data-ttu-id="30726-125">Indique si un délégué a l’autorisation d’afficher des éléments de calendrier privés de boîte aux lettres de l’entité de sécurité.</span><span class="sxs-lookup"><span data-stu-id="30726-125">Indicates whether a delegate has permission to view private calendar items in the principal's mailbox.</span></span> <span data-ttu-id="30726-126">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="30726-126">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="30726-127">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="30726-127">Parent elements</span></span>

|<span data-ttu-id="30726-128">**Élément**</span><span class="sxs-lookup"><span data-stu-id="30726-128">**Element**</span></span>|<span data-ttu-id="30726-129">**Description**</span><span class="sxs-lookup"><span data-stu-id="30726-129">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="30726-130">DelegateUsers</span><span class="sxs-lookup"><span data-stu-id="30726-130">DelegateUsers</span></span>](delegateusers.md) <br/> |<span data-ttu-id="30726-131">Contient les identités des délégués pour ajouter ou mettre à jour dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="30726-131">Contains the identities of delegates to add or update in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="30726-132">DelegateUserResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="30726-132">DelegateUserResponseMessageType</span></span>](delegateuserresponsemessagetype.md) <br/> |<span data-ttu-id="30726-133">Contient des messages de réponse pour les opérations de gestion de délégué.</span><span class="sxs-lookup"><span data-stu-id="30726-133">Contains response messages for delegate management operations.</span></span> <span data-ttu-id="30726-134">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="30726-134">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="30726-135">Remarques</span><span class="sxs-lookup"><span data-stu-id="30726-135">Remarks</span></span>

<span data-ttu-id="30726-136">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="30726-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="30726-137">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="30726-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="30726-138">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="30726-138">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="30726-139">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="30726-139">Schema Name</span></span>  <br/> |<span data-ttu-id="30726-140">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="30726-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="30726-141">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="30726-141">Validation File</span></span>  <br/> |<span data-ttu-id="30726-142">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="30726-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="30726-143">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="30726-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="30726-144">False</span><span class="sxs-lookup"><span data-stu-id="30726-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="30726-145">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="30726-145">See also</span></span>

- [<span data-ttu-id="30726-146">Opération AddDelegate</span><span class="sxs-lookup"><span data-stu-id="30726-146">AddDelegate operation</span></span>](adddelegate-operation.md) 
- [<span data-ttu-id="30726-147">Opération UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="30726-147">UpdateDelegate operation</span></span>](updatedelegate-operation.md)
- [<span data-ttu-id="30726-148">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="30726-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="30726-149">Ajout de délégués</span><span class="sxs-lookup"><span data-stu-id="30726-149">Adding Delegates</span></span>](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

