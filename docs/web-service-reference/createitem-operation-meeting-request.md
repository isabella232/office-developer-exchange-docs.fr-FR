---
title: Opération CreateItem (demande de réunion)
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
ms.assetid: fe136881-a804-456a-8552-8a1bea5eb9c8
description: L’opération CreateItem est utilisée pour répondre aux demandes de réunion.
ms.openlocfilehash: f9e6bd1742e6a30d08736ea67c0ff80b7a18e88a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457108"
---
# <a name="createitem-operation-meeting-request"></a><span data-ttu-id="3576d-103">Opération CreateItem (demande de réunion)</span><span class="sxs-lookup"><span data-stu-id="3576d-103">CreateItem operation (meeting request)</span></span>

<span data-ttu-id="3576d-104">L’opération CreateItem est utilisée pour répondre aux demandes de réunion.</span><span class="sxs-lookup"><span data-stu-id="3576d-104">The CreateItem operation is used to respond to meeting requests.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3576d-105">Remarques</span><span class="sxs-lookup"><span data-stu-id="3576d-105">Remarks</span></span>

<span data-ttu-id="3576d-106">L’opération CreateItem fournit trois options pour répondre à une demande de réunion : accepter, accepter provisoirement ou refuser.</span><span class="sxs-lookup"><span data-stu-id="3576d-106">The CreateItem operation provides three options for responding to a meeting request: accept, tentatively accept, or decline.</span></span> 
  
## <a name="accept-meeting-request-example"></a><span data-ttu-id="3576d-107">Exemple d’acceptation d’une demande de réunion</span><span class="sxs-lookup"><span data-stu-id="3576d-107">Accept Meeting request example</span></span>

### <a name="description"></a><span data-ttu-id="3576d-108">Description</span><span class="sxs-lookup"><span data-stu-id="3576d-108">Description</span></span>

<span data-ttu-id="3576d-109">L’exemple suivant montre comment accepter une invitation à une demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="3576d-109">The following example shows how to accept a meeting request invitation.</span></span>
  
### <a name="code"></a><span data-ttu-id="3576d-110">Code</span><span class="sxs-lookup"><span data-stu-id="3576d-110">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                MessageDisposition="SendAndSaveCopy">
      <Items>
        <AcceptItem xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <ReferenceItemId Id="AAAlAFVzZ"
                           ChangeKey="CwAAABYAA"/>
        </AcceptItem>
      </Items>
    </CreateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="3576d-111">Commentaires</span><span class="sxs-lookup"><span data-stu-id="3576d-111">Comments</span></span>

<span data-ttu-id="3576d-112">Pour accepter provisoirement ou refuser la demande de réunion, utilisez les éléments [TentativelyAcceptItem](tentativelyacceptitem.md) ou [DeclineItem](declineitem.md) à la place de l’élément [AcceptItem](acceptitem.md) .</span><span class="sxs-lookup"><span data-stu-id="3576d-112">To tentatively accept or to decline the meeting request, use the [TentativelyAcceptItem](tentativelyacceptitem.md) or [DeclineItem](declineitem.md) elements in place of the [AcceptItem](acceptitem.md) element.</span></span> 
  
<span data-ttu-id="3576d-113">L’identificateur d’élément et la clé de modification ont été raccourcies afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="3576d-113">The item identifier and change key have been shortened to preserve readability.</span></span>
  
### <a name="accepting-meeting-request-elements"></a><span data-ttu-id="3576d-114">Acceptation des éléments de demande de réunion</span><span class="sxs-lookup"><span data-stu-id="3576d-114">Accepting Meeting Request Elements</span></span>

<span data-ttu-id="3576d-115">Les éléments suivants sont utilisés dans la demande :</span><span class="sxs-lookup"><span data-stu-id="3576d-115">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="3576d-116">CreateItem</span><span class="sxs-lookup"><span data-stu-id="3576d-116">CreateItem</span></span>](createitem.md)
    
- [<span data-ttu-id="3576d-117">Éléments (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="3576d-117">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md)
    
- [<span data-ttu-id="3576d-118">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="3576d-118">AcceptItem</span></span>](acceptitem.md)
    
- [<span data-ttu-id="3576d-119">ReferenceItemId</span><span class="sxs-lookup"><span data-stu-id="3576d-119">ReferenceItemId</span></span>](referenceitemid.md)
    
## <a name="successful-accept-meeting-response-example"></a><span data-ttu-id="3576d-120">Exemple de réponse d’acceptation de réunion réussie</span><span class="sxs-lookup"><span data-stu-id="3576d-120">Successful Accept Meeting response example</span></span>

### <a name="description"></a><span data-ttu-id="3576d-121">Description</span><span class="sxs-lookup"><span data-stu-id="3576d-121">Description</span></span>

<span data-ttu-id="3576d-122">L’exemple suivant montre une réponse réussie à la demande CreateItem.</span><span class="sxs-lookup"><span data-stu-id="3576d-122">The following example shows a successful response to the CreateItem request.</span></span>
  
### <a name="code"></a><span data-ttu-id="3576d-123">Code</span><span class="sxs-lookup"><span data-stu-id="3576d-123">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
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

### <a name="successful-response-elements"></a><span data-ttu-id="3576d-124">Éléments de réponse réussis</span><span class="sxs-lookup"><span data-stu-id="3576d-124">Successful response elements</span></span>

<span data-ttu-id="3576d-125">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="3576d-125">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="3576d-126">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="3576d-126">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="3576d-127">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="3576d-127">CreateItemResponse</span></span>](createitemresponse.md)
    
- [<span data-ttu-id="3576d-128">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="3576d-128">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="3576d-129">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="3576d-129">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
    
- [<span data-ttu-id="3576d-130">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="3576d-130">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="3576d-131">Items</span><span class="sxs-lookup"><span data-stu-id="3576d-131">Items</span></span>](items.md)
    
## <a name="accept-meeting-error-response-example"></a><span data-ttu-id="3576d-132">Exemple de réponse d’erreur d’acceptation de réunion</span><span class="sxs-lookup"><span data-stu-id="3576d-132">Accept Meeting Error response example</span></span>

### <a name="description"></a><span data-ttu-id="3576d-133">Description</span><span class="sxs-lookup"><span data-stu-id="3576d-133">Description</span></span>

<span data-ttu-id="3576d-134">L’exemple suivant montre une réponse d’erreur à la demande CreateItem.</span><span class="sxs-lookup"><span data-stu-id="3576d-134">The following example shows an error response to CreateItem request.</span></span> <span data-ttu-id="3576d-135">L’erreur est due à une tentative d’acceptation d’une demande de réunion introuvable dans la Banque d’aide Exchange.</span><span class="sxs-lookup"><span data-stu-id="3576d-135">The error is caused by an attempt to accept a meeting request that cannot be found in the Exchange store.</span></span>
  
### <a name="code"></a><span data-ttu-id="3576d-136">Code</span><span class="sxs-lookup"><span data-stu-id="3576d-136">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
  xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
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

### <a name="error-response-elements"></a><span data-ttu-id="3576d-137">Éléments de réponse d’erreur</span><span class="sxs-lookup"><span data-stu-id="3576d-137">Error response elements</span></span>

<span data-ttu-id="3576d-138">Les éléments suivants sont utilisés dans la réponse d'erreur :</span><span class="sxs-lookup"><span data-stu-id="3576d-138">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="3576d-139">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="3576d-139">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="3576d-140">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="3576d-140">CreateItemResponse</span></span>](createitemresponse.md)
    
- [<span data-ttu-id="3576d-141">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="3576d-141">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="3576d-142">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="3576d-142">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
    
- [<span data-ttu-id="3576d-143">MessageText</span><span class="sxs-lookup"><span data-stu-id="3576d-143">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="3576d-144">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="3576d-144">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="3576d-145">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="3576d-145">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="3576d-146">Items</span><span class="sxs-lookup"><span data-stu-id="3576d-146">Items</span></span>](items.md)
    
## <a name="see-also"></a><span data-ttu-id="3576d-147">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="3576d-147">See also</span></span>



[<span data-ttu-id="3576d-148">Opération CreateItem</span><span class="sxs-lookup"><span data-stu-id="3576d-148">CreateItem operation</span></span>](createitem-operation.md)
  
[<span data-ttu-id="3576d-149">Opération CreateItem (élément de calendrier)</span><span class="sxs-lookup"><span data-stu-id="3576d-149">CreateItem operation (calendar item)</span></span>](createitem-operation-calendar-item.md)

