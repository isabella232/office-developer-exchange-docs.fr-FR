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
description: L’élément GetDelegateResponse contient l’État et le résultat d’une demande d’opération GetDelegate.
ms.openlocfilehash: 81c5033cd67b79baa131d71ea0b866c788ae5e82
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462023"
---
# <a name="getdelegateresponse"></a><span data-ttu-id="d6266-103">GetDelegateResponse</span><span class="sxs-lookup"><span data-stu-id="d6266-103">GetDelegateResponse</span></span>

<span data-ttu-id="d6266-104">L’élément **GetDelegateResponse** contient l’État et le résultat d’une demande d' [opération GetDelegate](getdelegate-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="d6266-104">The **GetDelegateResponse** element contains the status and result of a [GetDelegate operation](getdelegate-operation.md) request.</span></span> 
  
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

 <span data-ttu-id="d6266-105">**GetDelegateResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="d6266-105">**GetDelegateResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d6266-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d6266-106">Attributes and elements</span></span>

<span data-ttu-id="d6266-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d6266-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d6266-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="d6266-108">Attributes</span></span>

<span data-ttu-id="d6266-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="d6266-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d6266-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d6266-110">Child elements</span></span>

|<span data-ttu-id="d6266-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d6266-111">**Element**</span></span>|<span data-ttu-id="d6266-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="d6266-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d6266-113">DeliverMeetingRequests</span><span class="sxs-lookup"><span data-stu-id="d6266-113">DeliverMeetingRequests</span></span>](delivermeetingrequests.md) <br/> |<span data-ttu-id="d6266-114">Définit la manière dont les demandes de réunion sont gérées entre le délégué et le principal.</span><span class="sxs-lookup"><span data-stu-id="d6266-114">Defines how meeting requests are handled between the delegate and the principal.</span></span>  <br/> |
|[<span data-ttu-id="d6266-115">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span><span class="sxs-lookup"><span data-stu-id="d6266-115">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span></span>](responsemessages-arrayofdelegateuserresponsemessagetype.md) <br/> |<span data-ttu-id="d6266-116">Contient les messages de réponse pour une demande de gestion des délégués des services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="d6266-116">Contains the response messages for an Exchange Web Services delegate management request.</span></span>  <br/> |
|[<span data-ttu-id="d6266-117">MessageText</span><span class="sxs-lookup"><span data-stu-id="d6266-117">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="d6266-118">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="d6266-118">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="d6266-119">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="d6266-119">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="d6266-120">Fournit un code d’erreur qui identifie l’erreur spécifique rencontrée par la demande.</span><span class="sxs-lookup"><span data-stu-id="d6266-120">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="d6266-121">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="d6266-121">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="d6266-122">Actuellement inutilisé et est réservé à une utilisation ultérieure.</span><span class="sxs-lookup"><span data-stu-id="d6266-122">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="d6266-123">Il contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="d6266-123">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="d6266-124">MessageXml</span><span class="sxs-lookup"><span data-stu-id="d6266-124">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="d6266-125">Fournit des informations supplémentaires sur la réponse aux erreurs.</span><span class="sxs-lookup"><span data-stu-id="d6266-125">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d6266-126">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d6266-126">Parent elements</span></span>

<span data-ttu-id="d6266-127">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d6266-127">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d6266-128">Remarques</span><span class="sxs-lookup"><span data-stu-id="d6266-128">Remarks</span></span>

<span data-ttu-id="d6266-129">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="d6266-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d6266-130">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d6266-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d6266-131">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d6266-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d6266-132">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d6266-132">Schema Name</span></span>  <br/> |<span data-ttu-id="d6266-133">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="d6266-133">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d6266-134">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d6266-134">Validation File</span></span>  <br/> |<span data-ttu-id="d6266-135">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="d6266-135">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d6266-136">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d6266-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="d6266-137">False</span><span class="sxs-lookup"><span data-stu-id="d6266-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d6266-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d6266-138">See also</span></span>



[<span data-ttu-id="d6266-139">Opération GetDelegate</span><span class="sxs-lookup"><span data-stu-id="d6266-139">GetDelegate operation</span></span>](getdelegate-operation.md)


- [<span data-ttu-id="d6266-140">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="d6266-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

