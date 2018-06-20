---
title: ResponseMessages (ArrayOfDelegateUserResponseMessageType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResponseMessages
api_type:
- schema
ms.assetid: 14819975-ce54-4f0e-9f90-d4b275895ea0
description: L’élément ResponseMessages contient les messages de réponse pour une demande de gestion des Services Web Exchange délégué.
ms.openlocfilehash: e4b5567f3ded003e9648eb8ebebfadf8f1748d6c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829193"
---
# <a name="responsemessages-arrayofdelegateuserresponsemessagetype"></a><span data-ttu-id="50400-103">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span><span class="sxs-lookup"><span data-stu-id="50400-103">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span></span>

<span data-ttu-id="50400-104">L’élément **ResponseMessages** contient les messages de réponse pour une demande de gestion des Services Web Exchange délégué.</span><span class="sxs-lookup"><span data-stu-id="50400-104">The **ResponseMessages** element contains the response messages for an Exchange Web Services delegate management request.</span></span> 
  
```
<ResponseMessages>
   <DelegateUserResponseMessageType/>
</ResponseMessages>
```

 <span data-ttu-id="50400-105">**ArrayOfDelegateUserResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="50400-105">**ArrayOfDelegateUserResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="50400-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="50400-106">Attributes and elements</span></span>

<span data-ttu-id="50400-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="50400-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="50400-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="50400-108">Attributes</span></span>

<span data-ttu-id="50400-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="50400-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="50400-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="50400-110">Child elements</span></span>

|<span data-ttu-id="50400-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="50400-111">**Element**</span></span>|<span data-ttu-id="50400-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="50400-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="50400-113">DelegateUserResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="50400-113">DelegateUserResponseMessageType</span></span>](delegateuserresponsemessagetype.md) <br/> |<span data-ttu-id="50400-114">Contient des messages de réponse pour les opérations de gestion de délégué.</span><span class="sxs-lookup"><span data-stu-id="50400-114">Contains response messages for delegate management operations.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="50400-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="50400-115">Parent elements</span></span>

|<span data-ttu-id="50400-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="50400-116">**Element**</span></span>|<span data-ttu-id="50400-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="50400-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="50400-118">AddDelegateResponse</span><span class="sxs-lookup"><span data-stu-id="50400-118">AddDelegateResponse</span></span>](adddelegateresponse.md) <br/> |<span data-ttu-id="50400-119">Contient l’état et les résultats d’une requête [d’opération AddDelegate](adddelegate-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="50400-119">Contains the status and result of an [AddDelegate operation](adddelegate-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="50400-120">GetDelegateResponse</span><span class="sxs-lookup"><span data-stu-id="50400-120">GetDelegateResponse</span></span>](getdelegateresponse.md) <br/> |<span data-ttu-id="50400-121">Contient l’état et les résultats d’une demande [d’opération GetDelegate](getdelegate-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="50400-121">Contains the status and result of a [GetDelegate operation](getdelegate-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="50400-122">UpdateDelegateResponse</span><span class="sxs-lookup"><span data-stu-id="50400-122">UpdateDelegateResponse</span></span>](updatedelegateresponse.md) <br/> |<span data-ttu-id="50400-123">Contient l’état et les résultats d’une requête [d’opération UpdateDelegate](updatedelegate-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="50400-123">Contains the status and result of an [UpdateDelegate operation](updatedelegate-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="50400-124">RemoveDelegateResponse</span><span class="sxs-lookup"><span data-stu-id="50400-124">RemoveDelegateResponse</span></span>](removedelegateresponse.md) <br/> |<span data-ttu-id="50400-125">Contient l’état et les résultats d’une demande [d’opération RemoveDelegate](removedelegate-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="50400-125">Contains the status and result of a [RemoveDelegate operation](removedelegate-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="50400-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="50400-126">Remarks</span></span>

<span data-ttu-id="50400-127">Cet élément est utilisé dans l' [opération AddDelegate](adddelegate-operation.md), l' [opération GetDelegate](getdelegate-operation.md), l' [opération UpdateDelegate](updatedelegate-operation.md)et l' [opération RemoveDelegate](removedelegate-operation.md).</span><span class="sxs-lookup"><span data-stu-id="50400-127">This element is used in the [AddDelegate operation](adddelegate-operation.md), the [GetDelegate operation](getdelegate-operation.md), the [UpdateDelegate operation](updatedelegate-operation.md), and the [RemoveDelegate operation](removedelegate-operation.md).</span></span> <span data-ttu-id="50400-128">Les réponses d’opérations de gestion délégué sont structurées différemment des autres réponses.</span><span class="sxs-lookup"><span data-stu-id="50400-128">The delegate management operation responses are structured differently than other responses.</span></span> <span data-ttu-id="50400-129">Les messages de réponse de gestion de délégué sont fortement typées.</span><span class="sxs-lookup"><span data-stu-id="50400-129">The delegate management response messages are strongly typed.</span></span>
  
<span data-ttu-id="50400-130">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Exchange Server avec le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="50400-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="50400-131">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="50400-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="50400-132">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="50400-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="50400-133">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="50400-133">Schema Name</span></span>  <br/> |<span data-ttu-id="50400-134">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="50400-134">Messages schema</span></span>  <br/> |
|<span data-ttu-id="50400-135">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="50400-135">Validation File</span></span>  <br/> |<span data-ttu-id="50400-136">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="50400-136">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="50400-137">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="50400-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="50400-138">False</span><span class="sxs-lookup"><span data-stu-id="50400-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="50400-139">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="50400-139">See also</span></span>



[<span data-ttu-id="50400-140">Opération AddDelegate</span><span class="sxs-lookup"><span data-stu-id="50400-140">AddDelegate operation</span></span>](adddelegate-operation.md)
  
[<span data-ttu-id="50400-141">Opération GetDelegate</span><span class="sxs-lookup"><span data-stu-id="50400-141">GetDelegate operation</span></span>](getdelegate-operation.md)
  
[<span data-ttu-id="50400-142">Opération UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="50400-142">UpdateDelegate operation</span></span>](updatedelegate-operation.md)
  
[<span data-ttu-id="50400-143">Opération RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="50400-143">RemoveDelegate operation</span></span>](removedelegate-operation.md)


- [<span data-ttu-id="50400-144">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="50400-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

