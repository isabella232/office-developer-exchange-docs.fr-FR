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
description: L’opération CreateItem permet d’accepter une invitation pour partager le calendrier ou les données de contacts d’un autre utilisateur.
ms.openlocfilehash: eda846b72f42fe886497b355d9cddade7c5f4044
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457514"
---
# <a name="createitem-acceptsharinginvitation"></a><span data-ttu-id="8113f-103">CreateItem (AcceptSharingInvitation)</span><span class="sxs-lookup"><span data-stu-id="8113f-103">CreateItem (AcceptSharingInvitation)</span></span>

<span data-ttu-id="8113f-104">L’opération **CreateItem** permet d’accepter une invitation pour partager le calendrier ou les données de contacts d’un autre utilisateur.</span><span class="sxs-lookup"><span data-stu-id="8113f-104">The **CreateItem** operation is used to accept an invitation to share another user's calendar or contacts data.</span></span> 
  
## <a name="accept-sharing-invitation-request-example"></a><span data-ttu-id="8113f-105">Exemple de demande d’acceptation de partage</span><span class="sxs-lookup"><span data-stu-id="8113f-105">Accept Sharing Invitation request example</span></span>

### <a name="description"></a><span data-ttu-id="8113f-106">Description</span><span class="sxs-lookup"><span data-stu-id="8113f-106">Description</span></span>

<span data-ttu-id="8113f-107">L’exemple suivant montre comment accepter une invitation de partage.</span><span class="sxs-lookup"><span data-stu-id="8113f-107">The following example shows how to accept a sharing invitation.</span></span>
  
### <a name="code"></a><span data-ttu-id="8113f-108">Code</span><span class="sxs-lookup"><span data-stu-id="8113f-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <Items xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
        <AcceptSharingInvitation xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <ReferenceItemId Id="AAAlAFVzZ" ChangeKey="CwAAABYAA" />
        </AcceptSharingInvitation>
      </Items>
    </CreateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="8113f-109">Demander des éléments</span><span class="sxs-lookup"><span data-stu-id="8113f-109">Request elements</span></span>

<span data-ttu-id="8113f-110">Les éléments suivants sont utilisés dans la demande :</span><span class="sxs-lookup"><span data-stu-id="8113f-110">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="8113f-111">CreateItem</span><span class="sxs-lookup"><span data-stu-id="8113f-111">CreateItem</span></span>](createitem.md)
    
- [<span data-ttu-id="8113f-112">Items</span><span class="sxs-lookup"><span data-stu-id="8113f-112">Items</span></span>](items.md)
    
- [<span data-ttu-id="8113f-113">AcceptSharingInvitation</span><span class="sxs-lookup"><span data-stu-id="8113f-113">AcceptSharingInvitation</span></span>](acceptsharinginvitation.md)
    
- [<span data-ttu-id="8113f-114">ReferenceItemId</span><span class="sxs-lookup"><span data-stu-id="8113f-114">ReferenceItemId</span></span>](referenceitemid.md)
    
### <a name="comments"></a><span data-ttu-id="8113f-115">Commentaires</span><span class="sxs-lookup"><span data-stu-id="8113f-115">Comments</span></span>

<span data-ttu-id="8113f-116">L’identificateur d’élément et la clé de modification ont été raccourcies afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="8113f-116">The item identifier and change key have been shortened to preserve readability.</span></span>
  
## <a name="successful-accept-sharing-invitation-response-example"></a><span data-ttu-id="8113f-117">Exemple de réponse d’acceptation de partage réussi</span><span class="sxs-lookup"><span data-stu-id="8113f-117">Successful Accept Sharing Invitation response example</span></span>

### <a name="description"></a><span data-ttu-id="8113f-118">Description</span><span class="sxs-lookup"><span data-stu-id="8113f-118">Description</span></span>

<span data-ttu-id="8113f-119">L’exemple suivant montre une réponse réussie à une demande **CreateItem** .</span><span class="sxs-lookup"><span data-stu-id="8113f-119">The following example shows a successful response to a **CreateItem** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="8113f-120">Code</span><span class="sxs-lookup"><span data-stu-id="8113f-120">Code</span></span>

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
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CreateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="successful-response-elements"></a><span data-ttu-id="8113f-121">Éléments de réponse réussis</span><span class="sxs-lookup"><span data-stu-id="8113f-121">Successful response elements</span></span>

<span data-ttu-id="8113f-122">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="8113f-122">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="8113f-123">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="8113f-123">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="8113f-124">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="8113f-124">CreateItemResponse</span></span>](createitemresponse.md)
    
- [<span data-ttu-id="8113f-125">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="8113f-125">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="8113f-126">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="8113f-126">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
    
- [<span data-ttu-id="8113f-127">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="8113f-127">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="8113f-128">Items</span><span class="sxs-lookup"><span data-stu-id="8113f-128">Items</span></span>](items.md)
    
## <a name="accept-sharing-invitation-error-response-example"></a><span data-ttu-id="8113f-129">Exemple de réponse d’erreur d’acceptation de partage</span><span class="sxs-lookup"><span data-stu-id="8113f-129">Accept Sharing Invitation Error response example</span></span>

### <a name="description"></a><span data-ttu-id="8113f-130">Description</span><span class="sxs-lookup"><span data-stu-id="8113f-130">Description</span></span>

<span data-ttu-id="8113f-131">L’exemple suivant montre une réponse d’erreur à une demande **CreateItem** .</span><span class="sxs-lookup"><span data-stu-id="8113f-131">The following example shows an error response to a **CreateItem** request.</span></span> <span data-ttu-id="8113f-132">L’erreur est causée par une tentative d’acceptation d’une invitation de partage introuvable dans la Banque d’aide Exchange.</span><span class="sxs-lookup"><span data-stu-id="8113f-132">The error is caused by an attempt to accept a sharing invitation that cannot be found in the Exchange store.</span></span> 
  
### <a name="code"></a><span data-ttu-id="8113f-133">Code</span><span class="sxs-lookup"><span data-stu-id="8113f-133">Code</span></span>

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
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CreateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="error-response-elements"></a><span data-ttu-id="8113f-134">Éléments de réponse d’erreur</span><span class="sxs-lookup"><span data-stu-id="8113f-134">Error response elements</span></span>

<span data-ttu-id="8113f-135">Les éléments suivants sont utilisés dans la réponse d'erreur :</span><span class="sxs-lookup"><span data-stu-id="8113f-135">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="8113f-136">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="8113f-136">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="8113f-137">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="8113f-137">CreateItemResponse</span></span>](createitemresponse.md)
    
- [<span data-ttu-id="8113f-138">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="8113f-138">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="8113f-139">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="8113f-139">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
    
- [<span data-ttu-id="8113f-140">MessageText</span><span class="sxs-lookup"><span data-stu-id="8113f-140">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="8113f-141">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="8113f-141">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="8113f-142">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="8113f-142">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="8113f-143">Items</span><span class="sxs-lookup"><span data-stu-id="8113f-143">Items</span></span>](items.md)
    
## <a name="see-also"></a><span data-ttu-id="8113f-144">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="8113f-144">See also</span></span>



[<span data-ttu-id="8113f-145">CreateItem Operation</span><span class="sxs-lookup"><span data-stu-id="8113f-145">CreateItem operation</span></span>](createitem-operation.md)

