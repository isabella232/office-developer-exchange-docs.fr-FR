---
title: GetDelegateResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetDelegateResponse
api_type:
- schema
ms.assetid: 71a418a5-5652-40e1-8f84-fe4f7c9f86af
description: L’élément GetDelegateResponse contient l’état et les résultats d’une demande d’opération GetDelegate.
ms.openlocfilehash: 52731ea66420c21cf3fb8d19082aef65551c2af2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756570"
---
# <a name="getdelegateresponse"></a><span data-ttu-id="54f29-103">GetDelegateResponse</span><span class="sxs-lookup"><span data-stu-id="54f29-103">GetDelegateResponse</span></span>

<span data-ttu-id="54f29-104">L’élément **GetDelegateResponse** contient l’état et les résultats d’une demande [d’opération GetDelegate](getdelegate-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="54f29-104">The **GetDelegateResponse** element contains the status and result of a [GetDelegate operation](getdelegate-operation.md) request.</span></span> 
  
```xml
<GetDelegateResponse>
   <DeliverMeetingRequests/>
   <ResponseMessages/>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</GetDelegateResponse>
```

 <span data-ttu-id="54f29-105">**GetDelegateResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="54f29-105">**GetDelegateResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="54f29-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="54f29-106">Attributes and elements</span></span>

<span data-ttu-id="54f29-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="54f29-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="54f29-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="54f29-108">Attributes</span></span>

<span data-ttu-id="54f29-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="54f29-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="54f29-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="54f29-110">Child elements</span></span>

|<span data-ttu-id="54f29-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="54f29-111">**Element**</span></span>|<span data-ttu-id="54f29-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="54f29-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="54f29-113">DeliverMeetingRequests</span><span class="sxs-lookup"><span data-stu-id="54f29-113">DeliverMeetingRequests</span></span>](delivermeetingrequests.md) <br/> |<span data-ttu-id="54f29-114">Définit la gestion des demandes de réunion entre le délégué et l’entité de sécurité.</span><span class="sxs-lookup"><span data-stu-id="54f29-114">Defines how meeting requests are handled between the delegate and the principal.</span></span>  <br/> |
|[<span data-ttu-id="54f29-115">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span><span class="sxs-lookup"><span data-stu-id="54f29-115">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span></span>](responsemessages-arrayofdelegateuserresponsemessagetype.md) <br/> |<span data-ttu-id="54f29-116">Contient les messages de réponse pour une demande de gestion des Services Web Exchange délégué.</span><span class="sxs-lookup"><span data-stu-id="54f29-116">Contains the response messages for an Exchange Web Services delegate management request.</span></span>  <br/> |
|[<span data-ttu-id="54f29-117">MessageText</span><span class="sxs-lookup"><span data-stu-id="54f29-117">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="54f29-118">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="54f29-118">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="54f29-119">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="54f29-119">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="54f29-120">Fournit un code d’erreur qui identifie l’erreur spécifique qui a rencontré la demande.</span><span class="sxs-lookup"><span data-stu-id="54f29-120">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="54f29-121">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="54f29-121">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="54f29-122">Actuellement inutilisés et est réservé à un usage ultérieur.</span><span class="sxs-lookup"><span data-stu-id="54f29-122">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="54f29-123">Il contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="54f29-123">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="54f29-124">MessageXml</span><span class="sxs-lookup"><span data-stu-id="54f29-124">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="54f29-125">Fournit des informations de réponse d’erreur.</span><span class="sxs-lookup"><span data-stu-id="54f29-125">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="54f29-126">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="54f29-126">Parent elements</span></span>

<span data-ttu-id="54f29-127">Aucun.</span><span class="sxs-lookup"><span data-stu-id="54f29-127">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="54f29-128">Remarques</span><span class="sxs-lookup"><span data-stu-id="54f29-128">Remarks</span></span>

<span data-ttu-id="54f29-129">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="54f29-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="54f29-130">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="54f29-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="54f29-131">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="54f29-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="54f29-132">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="54f29-132">Schema Name</span></span>  <br/> |<span data-ttu-id="54f29-133">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="54f29-133">Messages schema</span></span>  <br/> |
|<span data-ttu-id="54f29-134">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="54f29-134">Validation File</span></span>  <br/> |<span data-ttu-id="54f29-135">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="54f29-135">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="54f29-136">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="54f29-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="54f29-137">False</span><span class="sxs-lookup"><span data-stu-id="54f29-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="54f29-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="54f29-138">See also</span></span>



[<span data-ttu-id="54f29-139">Opération GetDelegate</span><span class="sxs-lookup"><span data-stu-id="54f29-139">GetDelegate operation</span></span>](getdelegate-operation.md)


- [<span data-ttu-id="54f29-140">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="54f29-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

