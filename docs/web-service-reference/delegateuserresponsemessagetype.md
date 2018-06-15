---
title: DelegateUserResponseMessageType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DelegateUserResponseMessageType
api_type:
- schema
ms.assetid: 3dc9552c-1e2d-40ac-a137-827883c2bb88
description: L’élément DelegateUserResponseMessageType contient le message de réponse pour un utilisateur délégué unique.
ms.openlocfilehash: ac99e0ca219fc1f1e117f9288d895e27a1df4700
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/15/2018
ms.locfileid: "19755842"
---
# <a name="delegateuserresponsemessagetype"></a><span data-ttu-id="36df8-103">DelegateUserResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="36df8-103">DelegateUserResponseMessageType</span></span>

<span data-ttu-id="36df8-104">L’élément **DelegateUserResponseMessageType** contient le message de réponse pour un utilisateur délégué unique.</span><span class="sxs-lookup"><span data-stu-id="36df8-104">The **DelegateUserResponseMessageType** element contains the response message for a single delegate user.</span></span> 
  
```xml
<DelegateUserResponseMessageType>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <DelegateUser/>
</DelegateUserResponseMessageType>
```

<span data-ttu-id="36df8-105">**DelegateUserResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="36df8-105">**DelegateUserResponseMessageType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="36df8-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="36df8-106">Attributes and elements</span></span>

<span data-ttu-id="36df8-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="36df8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="36df8-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="36df8-108">Attributes</span></span>

<span data-ttu-id="36df8-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="36df8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="36df8-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="36df8-110">Child elements</span></span>

|<span data-ttu-id="36df8-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="36df8-111">**Element**</span></span>|<span data-ttu-id="36df8-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="36df8-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="36df8-113">MessageText</span><span class="sxs-lookup"><span data-stu-id="36df8-113">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="36df8-114">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="36df8-114">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="36df8-115">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="36df8-115">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="36df8-116">Fournit un code d’erreur qui identifie l’erreur spécifique qui a rencontré la demande.</span><span class="sxs-lookup"><span data-stu-id="36df8-116">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="36df8-117">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="36df8-117">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="36df8-118">Actuellement inutilisés et est réservé à un usage ultérieur.</span><span class="sxs-lookup"><span data-stu-id="36df8-118">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="36df8-119">Il contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="36df8-119">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="36df8-120">MessageXml</span><span class="sxs-lookup"><span data-stu-id="36df8-120">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="36df8-121">Fournit des informations de réponse d’erreur.</span><span class="sxs-lookup"><span data-stu-id="36df8-121">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="36df8-122">Utilisateur_délégué</span><span class="sxs-lookup"><span data-stu-id="36df8-122">DelegateUser</span></span>](delegateuser.md) <br/> |<span data-ttu-id="36df8-123">Identifie un délégué unique qui est retourné dans une réponse de gestion de délégué.</span><span class="sxs-lookup"><span data-stu-id="36df8-123">Identifies a single delegate that is returned in a delegate management response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="36df8-124">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="36df8-124">Parent elements</span></span>

|<span data-ttu-id="36df8-125">**Élément**</span><span class="sxs-lookup"><span data-stu-id="36df8-125">**Element**</span></span>|<span data-ttu-id="36df8-126">**Description**</span><span class="sxs-lookup"><span data-stu-id="36df8-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="36df8-127">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span><span class="sxs-lookup"><span data-stu-id="36df8-127">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span></span>](responsemessages-arrayofdelegateuserresponsemessagetype.md) <br/> |<span data-ttu-id="36df8-128">Contient les messages de réponse pour une demande de gestion des Services Web Exchange délégué.</span><span class="sxs-lookup"><span data-stu-id="36df8-128">Contains the response messages for an Exchange Web Services delegate management request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="36df8-129">Note</span><span class="sxs-lookup"><span data-stu-id="36df8-129">Remarks</span></span>

<span data-ttu-id="36df8-130">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Exchange Server avec le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="36df8-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="36df8-131">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="36df8-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="36df8-132">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="36df8-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="36df8-133">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="36df8-133">Schema Name</span></span>  <br/> |<span data-ttu-id="36df8-134">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="36df8-134">Messages schema</span></span>  <br/> |
|<span data-ttu-id="36df8-135">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="36df8-135">Validation File</span></span>  <br/> |<span data-ttu-id="36df8-136">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="36df8-136">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="36df8-137">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="36df8-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="36df8-138">False</span><span class="sxs-lookup"><span data-stu-id="36df8-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="36df8-139">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="36df8-139">See also</span></span>

- [<span data-ttu-id="36df8-140">Opération AddDelegate</span><span class="sxs-lookup"><span data-stu-id="36df8-140">AddDelegate operation</span></span>](adddelegate-operation.md)  
- [<span data-ttu-id="36df8-141">Opération GetDelegate</span><span class="sxs-lookup"><span data-stu-id="36df8-141">GetDelegate operation</span></span>](getdelegate-operation.md) 
- [<span data-ttu-id="36df8-142">Opération UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="36df8-142">UpdateDelegate operation</span></span>](updatedelegate-operation.md)  
- [<span data-ttu-id="36df8-143">Opération RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="36df8-143">RemoveDelegate operation</span></span>](removedelegate-operation.md)
- [<span data-ttu-id="36df8-144">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="36df8-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

