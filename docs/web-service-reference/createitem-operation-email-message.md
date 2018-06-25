---
title: Opération CreateItem (e-mail)
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
ms.assetid: fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1
description: L’opération CreateItem permet de créer des messages électroniques.
ms.openlocfilehash: 591209165cfbafc2d5f4036dd8fab6659523a044
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755719"
---
# <a name="createitem-operation-email-message"></a><span data-ttu-id="a8980-103">Opération CreateItem (e-mail)</span><span class="sxs-lookup"><span data-stu-id="a8980-103">CreateItem operation (email message)</span></span>

<span data-ttu-id="a8980-104">L’opération CreateItem permet de créer des messages électroniques.</span><span class="sxs-lookup"><span data-stu-id="a8980-104">The CreateItem operation is used to create e-mail messages.</span></span>
  
## <a name="createitem-request-example"></a><span data-ttu-id="a8980-105">Exemple de requête CreateItem</span><span class="sxs-lookup"><span data-stu-id="a8980-105">CreateItem request example</span></span>

### <a name="description"></a><span data-ttu-id="a8980-106">Description</span><span class="sxs-lookup"><span data-stu-id="a8980-106">Description</span></span>

<span data-ttu-id="a8980-107">Une demande CreateItem l’exemple suivant montre comment créer un nouveau message électronique, envoyer le message et enregistrer une copie dans le dossier Brouillons.</span><span class="sxs-lookup"><span data-stu-id="a8980-107">The following example of a CreateItem request shows how to create a new e-mail message, send the message, and save a copy of it in the drafts folder.</span></span>
  
### <a name="code"></a><span data-ttu-id="a8980-108">Code</span><span class="sxs-lookup"><span data-stu-id="a8980-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem MessageDisposition="SendAndSaveCopy" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <SavedItemFolderId>
        <t:DistinguishedFolderId Id="drafts" />
      </SavedItemFolderId>
      <Items>
        <t:Message>
          <t:ItemClass>IPM.Note</t:ItemClass>
          <t:Subject>Project Action</t:Subject>
          <t:Body BodyType="Text">Priority - Update specification</t:Body>
          <t:ToRecipients>
            <t:Mailbox>
              <t:EmailAddress>sschmidt@example.com</t:EmailAddress>
            </t:Mailbox>
          </t:ToRecipients>
          <t:IsRead>false</t:IsRead>
        </t:Message>
      </Items>
    </CreateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="a8980-109">Éléments de la demande</span><span class="sxs-lookup"><span data-stu-id="a8980-109">Request elements</span></span>

<span data-ttu-id="a8980-110">Les éléments suivants sont utilisés dans la demande :</span><span class="sxs-lookup"><span data-stu-id="a8980-110">The following elements are used in the request:</span></span> 
  
- [<span data-ttu-id="a8980-111">CreateItem</span><span class="sxs-lookup"><span data-stu-id="a8980-111">CreateItem</span></span>](createitem.md)
    
- [<span data-ttu-id="a8980-112">SavedItemFolderId</span><span class="sxs-lookup"><span data-stu-id="a8980-112">SavedItemFolderId</span></span>](saveditemfolderid.md)
    
- [<span data-ttu-id="a8980-113">Éléments (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="a8980-113">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md)
    
- [<span data-ttu-id="a8980-114">Message</span><span class="sxs-lookup"><span data-stu-id="a8980-114">Message</span></span>](message-ex15websvcsotherref.md)
    
- [<span data-ttu-id="a8980-115">ItemClass</span><span class="sxs-lookup"><span data-stu-id="a8980-115">ItemClass</span></span>](itemclass.md)
    
- [<span data-ttu-id="a8980-116">Objet</span><span class="sxs-lookup"><span data-stu-id="a8980-116">Subject</span></span>](subject.md)
    
- [<span data-ttu-id="a8980-117">Corps</span><span class="sxs-lookup"><span data-stu-id="a8980-117">Body</span></span>](body.md)
    
- [<span data-ttu-id="a8980-118">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="a8980-118">ToRecipients</span></span>](torecipients.md)
    
- [<span data-ttu-id="a8980-119">Boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="a8980-119">Mailbox</span></span>](mailbox.md)
    
- [<span data-ttu-id="a8980-120">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="a8980-120">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md)
    
- [<span data-ttu-id="a8980-121">Estlu</span><span class="sxs-lookup"><span data-stu-id="a8980-121">IsRead</span></span>](isread.md)
    
<span data-ttu-id="a8980-122">Pour trouver d’autres options pour le message de demande de l’opération CreateItem, explorez la hiérarchie de schéma.</span><span class="sxs-lookup"><span data-stu-id="a8980-122">To find other options for the request message of the CreateItem operation, explore the schema hierarchy.</span></span> <span data-ttu-id="a8980-123">Commencer à l’élément [CreateItem](createitem.md) .</span><span class="sxs-lookup"><span data-stu-id="a8980-123">Start at the [CreateItem](createitem.md) element.</span></span> 
  
## <a name="successful-createitem-response"></a><span data-ttu-id="a8980-124">Réponse CreateItem réussie</span><span class="sxs-lookup"><span data-stu-id="a8980-124">Successful CreateItem Response</span></span>

### <a name="description"></a><span data-ttu-id="a8980-125">Description</span><span class="sxs-lookup"><span data-stu-id="a8980-125">Description</span></span>

<span data-ttu-id="a8980-126">L’exemple suivant montre une réponse positive à la demande CreateItem.</span><span class="sxs-lookup"><span data-stu-id="a8980-126">The following example shows a successful response to the CreateItem request.</span></span>
  
### <a name="code"></a><span data-ttu-id="a8980-127">Code</span><span class="sxs-lookup"><span data-stu-id="a8980-127">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
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

### <a name="successful-response-elements"></a><span data-ttu-id="a8980-128">Éléments de réponse réussie</span><span class="sxs-lookup"><span data-stu-id="a8980-128">Successful response elements</span></span>

<span data-ttu-id="a8980-129">Les éléments suivants sont inclus dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="a8980-129">The following elements are included in the response:</span></span> 
  
- [<span data-ttu-id="a8980-130">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="a8980-130">CreateItemResponse</span></span>](createitemresponse.md)
    
- [<span data-ttu-id="a8980-131">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="a8980-131">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="a8980-132">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="a8980-132">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
    
- [<span data-ttu-id="a8980-133">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="a8980-133">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="a8980-134">Items</span><span class="sxs-lookup"><span data-stu-id="a8980-134">Items</span></span>](items.md)
    
<span data-ttu-id="a8980-135">Pour trouver d’autres options pour le message de réponse de l’opération CreateItem, explorez la hiérarchie de schéma.</span><span class="sxs-lookup"><span data-stu-id="a8980-135">To find other options for the response message of the CreateItem operation, explore the schema hierarchy.</span></span> <span data-ttu-id="a8980-136">Démarrez au niveau de l’élément [CreateItemResponse](createitemresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="a8980-136">Start at the [CreateItemResponse](createitemresponse.md) element.</span></span> 
  
## <a name="error-createitem-response"></a><span data-ttu-id="a8980-137">Réponse d’erreur CreateItem</span><span class="sxs-lookup"><span data-stu-id="a8980-137">Error CreateItem Response</span></span>

### <a name="description"></a><span data-ttu-id="a8980-138">Description</span><span class="sxs-lookup"><span data-stu-id="a8980-138">Description</span></span>

<span data-ttu-id="a8980-139">L’exemple suivant montre une réponse d’erreur à une demande CreateItem.</span><span class="sxs-lookup"><span data-stu-id="a8980-139">The following example shows an error response to a CreateItem request.</span></span>
  
### <a name="code"></a><span data-ttu-id="a8980-140">Code</span><span class="sxs-lookup"><span data-stu-id="a8980-140">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CreateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Error">
          <m:MessageText>The user account which was used to submit this request does not have the right to send mail on behalf of the specified sending account.</m:MessageText>
          <m:ResponseCode>ErrorSendAsDenied</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Items />
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </CreateItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="a8980-141">Éléments de réponse d’erreur</span><span class="sxs-lookup"><span data-stu-id="a8980-141">Error response elements</span></span>

<span data-ttu-id="a8980-142">Les éléments suivants sont utilisés dans la réponse d'erreur :</span><span class="sxs-lookup"><span data-stu-id="a8980-142">The following elements are used in the error response:</span></span> 
  
- [<span data-ttu-id="a8980-143">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="a8980-143">CreateItemResponse</span></span>](createitemresponse.md)
    
- [<span data-ttu-id="a8980-144">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="a8980-144">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="a8980-145">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="a8980-145">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
    
- [<span data-ttu-id="a8980-146">MessageText</span><span class="sxs-lookup"><span data-stu-id="a8980-146">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="a8980-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="a8980-147">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="a8980-148">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="a8980-148">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="a8980-149">Items</span><span class="sxs-lookup"><span data-stu-id="a8980-149">Items</span></span>](items.md)
    
<span data-ttu-id="a8980-150">Pour trouver d’autres options pour le message de réponse de l’opération CreateItem, explorez la hiérarchie de schéma.</span><span class="sxs-lookup"><span data-stu-id="a8980-150">To find other options for the error response message of the CreateItem operation, explore the schema hierarchy.</span></span> <span data-ttu-id="a8980-151">Démarrez au niveau de l’élément [CreateItemResponse](createitemresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="a8980-151">Start at the [CreateItemResponse](createitemresponse.md) element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="a8980-152">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a8980-152">See also</span></span>



[<span data-ttu-id="a8980-153">CreateItem Operation</span><span class="sxs-lookup"><span data-stu-id="a8980-153">CreateItem operation</span></span>](createitem-operation.md)

