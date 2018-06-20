---
title: CreateItem (AcceptSharingInvitation)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateItem
api_type:
- schema
ms.assetid: 710c893a-3037-4f04-b336-aefedd36c406
description: L’opération CreateItem sert à accepter une invitation à partager le calendrier d’un autre utilisateur ou des données de contacts.
ms.openlocfilehash: 993ef0402e624af69f632af5bdce4c02bd9d41f3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755712"
---
# <a name="createitem-acceptsharinginvitation"></a><span data-ttu-id="c819d-103">CreateItem (AcceptSharingInvitation)</span><span class="sxs-lookup"><span data-stu-id="c819d-103">CreateItem (AcceptSharingInvitation)</span></span>

<span data-ttu-id="c819d-104">L’opération **CreateItem** sert à accepter une invitation à partager le calendrier d’un autre utilisateur ou des données de contacts.</span><span class="sxs-lookup"><span data-stu-id="c819d-104">The **CreateItem** operation is used to accept an invitation to share another user's calendar or contacts data.</span></span> 
  
## <a name="accept-sharing-invitation-request-example"></a><span data-ttu-id="c819d-105">Accepter l’exemple de requête d’Invitation de partage</span><span class="sxs-lookup"><span data-stu-id="c819d-105">Accept Sharing Invitation request example</span></span>

### <a name="description"></a><span data-ttu-id="c819d-106">Description</span><span class="sxs-lookup"><span data-stu-id="c819d-106">Description</span></span>

<span data-ttu-id="c819d-107">L’exemple suivant montre comment accepter une invitation de partage.</span><span class="sxs-lookup"><span data-stu-id="c819d-107">The following example shows how to accept a sharing invitation.</span></span>
  
### <a name="code"></a><span data-ttu-id="c819d-108">Code</span><span class="sxs-lookup"><span data-stu-id="c819d-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <Items xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
        <AcceptSharingInvitation xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <ReferenceItemId Id="AAAlAFVzZ" ChangeKey="CwAAABYAA" />
        </AcceptSharingInvitation>
      </Items>
    </CreateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="c819d-109">Éléments de la demande</span><span class="sxs-lookup"><span data-stu-id="c819d-109">Request elements</span></span>

<span data-ttu-id="c819d-110">Les éléments suivants sont utilisés dans la demande :</span><span class="sxs-lookup"><span data-stu-id="c819d-110">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="c819d-111">CreateItem</span><span class="sxs-lookup"><span data-stu-id="c819d-111">CreateItem</span></span>](createitem.md)
    
- [<span data-ttu-id="c819d-112">Items</span><span class="sxs-lookup"><span data-stu-id="c819d-112">Items</span></span>](items.md)
    
- [<span data-ttu-id="c819d-113">AcceptSharingInvitation</span><span class="sxs-lookup"><span data-stu-id="c819d-113">AcceptSharingInvitation</span></span>](acceptsharinginvitation.md)
    
- [<span data-ttu-id="c819d-114">ReferenceItemId</span><span class="sxs-lookup"><span data-stu-id="c819d-114">ReferenceItemId</span></span>](referenceitemid.md)
    
### <a name="comments"></a><span data-ttu-id="c819d-115">Commentaires</span><span class="sxs-lookup"><span data-stu-id="c819d-115">Comments</span></span>

<span data-ttu-id="c819d-116">L’identificateur d’élément et modifier la clé ont été réduits afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="c819d-116">The item identifier and change key have been shortened to preserve readability.</span></span>
  
## <a name="successful-accept-sharing-invitation-response-example"></a><span data-ttu-id="c819d-117">Exemple de réponse Invitation de partage accepter réussie</span><span class="sxs-lookup"><span data-stu-id="c819d-117">Successful Accept Sharing Invitation response example</span></span>

### <a name="description"></a><span data-ttu-id="c819d-118">Description</span><span class="sxs-lookup"><span data-stu-id="c819d-118">Description</span></span>

<span data-ttu-id="c819d-119">L’exemple suivant montre une réponse positive à une demande **CreateItem** .</span><span class="sxs-lookup"><span data-stu-id="c819d-119">The following example shows a successful response to a **CreateItem** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="c819d-120">Code</span><span class="sxs-lookup"><span data-stu-id="c819d-120">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="0" 
                         MajorBuildNumber="639" 
                         MinorBuildNumber="11" 
                         Version="Exchange2010" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CreateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items />
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </CreateItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a><span data-ttu-id="c819d-121">Éléments de réponse réussie</span><span class="sxs-lookup"><span data-stu-id="c819d-121">Successful response elements</span></span>

<span data-ttu-id="c819d-122">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="c819d-122">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="c819d-123">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="c819d-123">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="c819d-124">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="c819d-124">CreateItemResponse</span></span>](createitemresponse.md)
    
- [<span data-ttu-id="c819d-125">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="c819d-125">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="c819d-126">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="c819d-126">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
    
- [<span data-ttu-id="c819d-127">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="c819d-127">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="c819d-128">Items</span><span class="sxs-lookup"><span data-stu-id="c819d-128">Items</span></span>](items.md)
    
## <a name="accept-sharing-invitation-error-response-example"></a><span data-ttu-id="c819d-129">Accepter l’exemple de réponse d’erreur dans l’Invitation de partage</span><span class="sxs-lookup"><span data-stu-id="c819d-129">Accept Sharing Invitation Error response example</span></span>

### <a name="description"></a><span data-ttu-id="c819d-130">Description</span><span class="sxs-lookup"><span data-stu-id="c819d-130">Description</span></span>

<span data-ttu-id="c819d-131">L’exemple suivant montre une réponse d’erreur à une demande **CreateItem** .</span><span class="sxs-lookup"><span data-stu-id="c819d-131">The following example shows an error response to a **CreateItem** request.</span></span> <span data-ttu-id="c819d-132">L’erreur est provoquée par une tentative d’accepter une invitation de partage qui ne figurent pas dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="c819d-132">The error is caused by an attempt to accept a sharing invitation that cannot be found in the Exchange store.</span></span> 
  
### <a name="code"></a><span data-ttu-id="c819d-133">Code</span><span class="sxs-lookup"><span data-stu-id="c819d-133">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="0" 
                         MajorBuildNumber="639" 
                         MinorBuildNumber="11" 
                         Version="Exchange2010" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CreateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Error">
          <m:MessageText>The specified object was not found in the store.</m:MessageText>
          <m:ResponseCode>ErrorItemNotFound</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Items />
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </CreateItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="c819d-134">Éléments de réponse d’erreur</span><span class="sxs-lookup"><span data-stu-id="c819d-134">Error response elements</span></span>

<span data-ttu-id="c819d-135">Les éléments suivants sont utilisés dans la réponse d'erreur :</span><span class="sxs-lookup"><span data-stu-id="c819d-135">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="c819d-136">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="c819d-136">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="c819d-137">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="c819d-137">CreateItemResponse</span></span>](createitemresponse.md)
    
- [<span data-ttu-id="c819d-138">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="c819d-138">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="c819d-139">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="c819d-139">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
    
- [<span data-ttu-id="c819d-140">MessageText</span><span class="sxs-lookup"><span data-stu-id="c819d-140">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="c819d-141">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="c819d-141">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="c819d-142">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="c819d-142">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="c819d-143">Items</span><span class="sxs-lookup"><span data-stu-id="c819d-143">Items</span></span>](items.md)
    
## <a name="see-also"></a><span data-ttu-id="c819d-144">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c819d-144">See also</span></span>



[<span data-ttu-id="c819d-145">CreateItem Operation</span><span class="sxs-lookup"><span data-stu-id="c819d-145">CreateItem operation</span></span>](createitem-operation.md)

