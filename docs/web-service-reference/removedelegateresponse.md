---
title: RemoveDelegateResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RemoveDelegateResponse
api_type:
- schema
ms.assetid: eef56c53-d0a7-4342-9ce6-4dbb6b1a1369
description: L’élément RemoveDelegateResponse contient l’état et les résultats d’une demande d’opération RemoveDelegate.
ms.openlocfilehash: 45d0bcfaeb4d453f50cce8449f5cb7fdb70512a6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829092"
---
# <a name="removedelegateresponse"></a><span data-ttu-id="db585-103">RemoveDelegateResponse</span><span class="sxs-lookup"><span data-stu-id="db585-103">RemoveDelegateResponse</span></span>

<span data-ttu-id="db585-104">L’élément **RemoveDelegateResponse** contient l’état et les résultats d’une demande [d’opération RemoveDelegate](removedelegate-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="db585-104">The **RemoveDelegateResponse** element contains the status and result of a [RemoveDelegate operation](removedelegate-operation.md) request.</span></span> 
  
```xml
<RemoveDelegateResponse>
   <ResponseMessages/>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</RemoveDelegateResponse>
```

 <span data-ttu-id="db585-105">**RemoveDelegateResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="db585-105">**RemoveDelegateResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="db585-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="db585-106">Attributes and elements</span></span>

<span data-ttu-id="db585-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="db585-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="db585-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="db585-108">Attributes</span></span>

<span data-ttu-id="db585-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="db585-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="db585-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="db585-110">Child elements</span></span>

|<span data-ttu-id="db585-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="db585-111">**Element**</span></span>|<span data-ttu-id="db585-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="db585-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="db585-113">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span><span class="sxs-lookup"><span data-stu-id="db585-113">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span></span>](responsemessages-arrayofdelegateuserresponsemessagetype.md) <br/> |<span data-ttu-id="db585-114">Contient les messages de réponse pour une demande de gestion des Services Web Exchange délégué.</span><span class="sxs-lookup"><span data-stu-id="db585-114">Contains the response messages for an Exchange Web Services delegate management request.</span></span>  <br/> |
|[<span data-ttu-id="db585-115">MessageText</span><span class="sxs-lookup"><span data-stu-id="db585-115">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="db585-116">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="db585-116">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="db585-117">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="db585-117">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="db585-118">Fournit un code d’erreur qui identifie l’erreur spécifique qui a rencontré la demande.</span><span class="sxs-lookup"><span data-stu-id="db585-118">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="db585-119">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="db585-119">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="db585-120">Actuellement inutilisés et est réservé à un usage ultérieur.</span><span class="sxs-lookup"><span data-stu-id="db585-120">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="db585-121">Il contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="db585-121">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="db585-122">MessageXml</span><span class="sxs-lookup"><span data-stu-id="db585-122">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="db585-123">Fournit des informations de réponse d’erreur.</span><span class="sxs-lookup"><span data-stu-id="db585-123">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="db585-124">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="db585-124">Parent elements</span></span>

<span data-ttu-id="db585-125">Aucun.</span><span class="sxs-lookup"><span data-stu-id="db585-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="db585-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="db585-126">Remarks</span></span>

<span data-ttu-id="db585-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="db585-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="db585-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="db585-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="db585-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="db585-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="db585-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="db585-130">Schema Name</span></span>  <br/> |<span data-ttu-id="db585-131">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="db585-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="db585-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="db585-132">Validation File</span></span>  <br/> |<span data-ttu-id="db585-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="db585-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="db585-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="db585-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="db585-135">False</span><span class="sxs-lookup"><span data-stu-id="db585-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="db585-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="db585-136">See also</span></span>



[<span data-ttu-id="db585-137">Opération RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="db585-137">RemoveDelegate operation</span></span>](removedelegate-operation.md)


- [<span data-ttu-id="db585-138">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="db585-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

