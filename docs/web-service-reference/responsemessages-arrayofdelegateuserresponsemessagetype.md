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
description: L’élément ResponseMessages contient les messages de réponse pour une demande de gestion des délégués des services Web Exchange.
ms.openlocfilehash: 6b035f4ee46af1750a275e2c61b2cddea06b37a1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465456"
---
# <a name="responsemessages-arrayofdelegateuserresponsemessagetype"></a><span data-ttu-id="1d91e-103">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span><span class="sxs-lookup"><span data-stu-id="1d91e-103">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span></span>

<span data-ttu-id="1d91e-104">L’élément **ResponseMessages** contient les messages de réponse pour une demande de gestion des délégués des services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="1d91e-104">The **ResponseMessages** element contains the response messages for an Exchange Web Services delegate management request.</span></span> 
  
```
<ResponseMessages>
   <DelegateUserResponseMessageType/>
</ResponseMessages>
```

 <span data-ttu-id="1d91e-105">**ArrayOfDelegateUserResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="1d91e-105">**ArrayOfDelegateUserResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1d91e-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="1d91e-106">Attributes and elements</span></span>

<span data-ttu-id="1d91e-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="1d91e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1d91e-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="1d91e-108">Attributes</span></span>

<span data-ttu-id="1d91e-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="1d91e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1d91e-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="1d91e-110">Child elements</span></span>

|<span data-ttu-id="1d91e-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1d91e-111">**Element**</span></span>|<span data-ttu-id="1d91e-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="1d91e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1d91e-113">DelegateUserResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="1d91e-113">DelegateUserResponseMessageType</span></span>](delegateuserresponsemessagetype.md) <br/> |<span data-ttu-id="1d91e-114">Contient des messages de réponse pour les opérations de gestion de délégués.</span><span class="sxs-lookup"><span data-stu-id="1d91e-114">Contains response messages for delegate management operations.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1d91e-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="1d91e-115">Parent elements</span></span>

|<span data-ttu-id="1d91e-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1d91e-116">**Element**</span></span>|<span data-ttu-id="1d91e-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="1d91e-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1d91e-118">AddDelegateResponse</span><span class="sxs-lookup"><span data-stu-id="1d91e-118">AddDelegateResponse</span></span>](adddelegateresponse.md) <br/> |<span data-ttu-id="1d91e-119">Contient l’État et le résultat d’une demande d' [opération AddDelegate](adddelegate-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="1d91e-119">Contains the status and result of an [AddDelegate operation](adddelegate-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="1d91e-120">GetDelegateResponse</span><span class="sxs-lookup"><span data-stu-id="1d91e-120">GetDelegateResponse</span></span>](getdelegateresponse.md) <br/> |<span data-ttu-id="1d91e-121">Contient l’État et le résultat d’une demande d' [opération GetDelegate](getdelegate-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="1d91e-121">Contains the status and result of a [GetDelegate operation](getdelegate-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="1d91e-122">UpdateDelegateResponse</span><span class="sxs-lookup"><span data-stu-id="1d91e-122">UpdateDelegateResponse</span></span>](updatedelegateresponse.md) <br/> |<span data-ttu-id="1d91e-123">Contient l’État et le résultat d’une demande d' [opération UpdateDelegate](updatedelegate-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="1d91e-123">Contains the status and result of an [UpdateDelegate operation](updatedelegate-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="1d91e-124">RemoveDelegateResponse</span><span class="sxs-lookup"><span data-stu-id="1d91e-124">RemoveDelegateResponse</span></span>](removedelegateresponse.md) <br/> |<span data-ttu-id="1d91e-125">Contient l’État et le résultat d’une demande d' [opération RemoveDelegate](removedelegate-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="1d91e-125">Contains the status and result of a [RemoveDelegate operation](removedelegate-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1d91e-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="1d91e-126">Remarks</span></span>

<span data-ttu-id="1d91e-127">Cet élément est utilisé dans l' [opération AddDelegate](adddelegate-operation.md), l’opération [GetDelegate](getdelegate-operation.md), l' [opération UpdateDelegate](updatedelegate-operation.md)et l' [opération RemoveDelegate](removedelegate-operation.md).</span><span class="sxs-lookup"><span data-stu-id="1d91e-127">This element is used in the [AddDelegate operation](adddelegate-operation.md), the [GetDelegate operation](getdelegate-operation.md), the [UpdateDelegate operation](updatedelegate-operation.md), and the [RemoveDelegate operation](removedelegate-operation.md).</span></span> <span data-ttu-id="1d91e-128">Les réponses aux opérations de gestion des délégués sont structurées différemment des autres réponses.</span><span class="sxs-lookup"><span data-stu-id="1d91e-128">The delegate management operation responses are structured differently than other responses.</span></span> <span data-ttu-id="1d91e-129">Les messages de réponse de gestion déléguée sont fortement typés.</span><span class="sxs-lookup"><span data-stu-id="1d91e-129">The delegate management response messages are strongly typed.</span></span>
  
<span data-ttu-id="1d91e-130">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Exchange Server et sur lequel le rôle serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="1d91e-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1d91e-131">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="1d91e-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1d91e-132">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="1d91e-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1d91e-133">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="1d91e-133">Schema Name</span></span>  <br/> |<span data-ttu-id="1d91e-134">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="1d91e-134">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1d91e-135">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="1d91e-135">Validation File</span></span>  <br/> |<span data-ttu-id="1d91e-136">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="1d91e-136">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1d91e-137">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="1d91e-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="1d91e-138">False</span><span class="sxs-lookup"><span data-stu-id="1d91e-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1d91e-139">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1d91e-139">See also</span></span>



[<span data-ttu-id="1d91e-140">Opération AddDelegate</span><span class="sxs-lookup"><span data-stu-id="1d91e-140">AddDelegate operation</span></span>](adddelegate-operation.md)
  
[<span data-ttu-id="1d91e-141">Opération GetDelegate</span><span class="sxs-lookup"><span data-stu-id="1d91e-141">GetDelegate operation</span></span>](getdelegate-operation.md)
  
[<span data-ttu-id="1d91e-142">Opération UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="1d91e-142">UpdateDelegate operation</span></span>](updatedelegate-operation.md)
  
[<span data-ttu-id="1d91e-143">Opération RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="1d91e-143">RemoveDelegate operation</span></span>](removedelegate-operation.md)


- [<span data-ttu-id="1d91e-144">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="1d91e-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

