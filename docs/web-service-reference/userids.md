---
title: ID utilisateur
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UserIds
api_type:
- schema
ms.assetid: 78a09c3a-1646-4c55-95a2-1109fb11e1c6
description: Les ID utilisateur élément contient un tableau de déléguer aux utilisateurs d’obtenir ou de supprimer la boîte aux lettres d’un utilisateur principal. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 277ae96fdbc30f1b39ef20553e10ff1de3ff7a8b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838960"
---
# <a name="userids"></a><span data-ttu-id="80a15-104">ID utilisateur</span><span class="sxs-lookup"><span data-stu-id="80a15-104">UserIds</span></span>

<span data-ttu-id="80a15-105">L’élément **UserIds** contient un tableau de déléguer aux utilisateurs d’obtenir ou de supprimer la boîte aux lettres d’un utilisateur principal.</span><span class="sxs-lookup"><span data-stu-id="80a15-105">The **UserIds** element contains an array of delegate users to get or remove from a principal's mailbox.</span></span> <span data-ttu-id="80a15-106">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="80a15-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<UserIds>
   <UserId/>
</UserIds>
```

 <span data-ttu-id="80a15-107">**ArrayOfUserIdType**</span><span class="sxs-lookup"><span data-stu-id="80a15-107">**ArrayOfUserIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="80a15-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="80a15-108">Attributes and elements</span></span>

<span data-ttu-id="80a15-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="80a15-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="80a15-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="80a15-110">Attributes</span></span>

<span data-ttu-id="80a15-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="80a15-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="80a15-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="80a15-112">Child elements</span></span>

|<span data-ttu-id="80a15-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="80a15-113">**Element**</span></span>|<span data-ttu-id="80a15-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="80a15-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="80a15-115">Nom d’utilisateur</span><span class="sxs-lookup"><span data-stu-id="80a15-115">UserId</span></span>](userid.md) <br/> |<span data-ttu-id="80a15-116">Identifie un délégué d’obtenir ou de supprimer la boîte aux lettres d’un utilisateur principal.</span><span class="sxs-lookup"><span data-stu-id="80a15-116">Identifies a delegate to get or remove from a principal's mailbox.</span></span> <span data-ttu-id="80a15-117">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="80a15-117">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="80a15-118">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="80a15-118">Parent elements</span></span>

|<span data-ttu-id="80a15-119">**Élément**</span><span class="sxs-lookup"><span data-stu-id="80a15-119">**Element**</span></span>|<span data-ttu-id="80a15-120">**Description**</span><span class="sxs-lookup"><span data-stu-id="80a15-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="80a15-121">GetDelegate</span><span class="sxs-lookup"><span data-stu-id="80a15-121">GetDelegate</span></span>](getdelegate.md) <br/> |<span data-ttu-id="80a15-122">Définit une demande pour obtenir des informations sur les délégués à une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="80a15-122">Defines a request to get information about delegates to a mailbox.</span></span> <span data-ttu-id="80a15-123">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="80a15-123">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="80a15-124">RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="80a15-124">RemoveDelegate</span></span>](removedelegate.md) <br/> |<span data-ttu-id="80a15-125">Définit une demande pour supprimer des délégués d’une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="80a15-125">Defines a request to remove delegates from a mailbox.</span></span> <span data-ttu-id="80a15-126">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="80a15-126">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="80a15-127">Remarques</span><span class="sxs-lookup"><span data-stu-id="80a15-127">Remarks</span></span>

<span data-ttu-id="80a15-128">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="80a15-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="80a15-129">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="80a15-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="80a15-130">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="80a15-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="80a15-131">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="80a15-131">Schema Name</span></span>  <br/> |<span data-ttu-id="80a15-132">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="80a15-132">Messages schema</span></span>  <br/> |
|<span data-ttu-id="80a15-133">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="80a15-133">Validation File</span></span>  <br/> |<span data-ttu-id="80a15-134">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="80a15-134">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="80a15-135">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="80a15-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="80a15-136">False</span><span class="sxs-lookup"><span data-stu-id="80a15-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="80a15-137">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="80a15-137">See also</span></span>



[<span data-ttu-id="80a15-138">Opération GetDelegate</span><span class="sxs-lookup"><span data-stu-id="80a15-138">GetDelegate operation</span></span>](getdelegate-operation.md)
  
[<span data-ttu-id="80a15-139">Opération RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="80a15-139">RemoveDelegate operation</span></span>](removedelegate-operation.md)


- [<span data-ttu-id="80a15-140">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="80a15-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

