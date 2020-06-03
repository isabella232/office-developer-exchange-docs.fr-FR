---
title: Opération SendItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SendItem
api_type:
- schema
ms.assetid: 337b89ef-e1b7-45ed-92f3-8abe4200e4c7
description: L’opération SendItem est utilisée pour envoyer des messages électroniques situés dans la Banque d’Exchange.
ms.openlocfilehash: 9136379e50723211fe5a483c7f113da4fa125fc1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530337"
---
# <a name="senditem-operation"></a><span data-ttu-id="9bfd1-103">Opération SendItem</span><span class="sxs-lookup"><span data-stu-id="9bfd1-103">SendItem operation</span></span>

<span data-ttu-id="9bfd1-104">L’opération SendItem est utilisée pour envoyer des messages électroniques situés dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="9bfd1-104">The SendItem operation is used to send e-mail messages that are located in the Exchange store.</span></span>
  
## <a name="senditem-e-mail-message-request-example"></a><span data-ttu-id="9bfd1-105">Exemple de requête SendItem (message électronique)</span><span class="sxs-lookup"><span data-stu-id="9bfd1-105">SendItem (E-mail Message) request example</span></span>

### <a name="description"></a><span data-ttu-id="9bfd1-106">Description</span><span class="sxs-lookup"><span data-stu-id="9bfd1-106">Description</span></span>

<span data-ttu-id="9bfd1-107">L’exemple suivant montre comment envoyer un message électronique.</span><span class="sxs-lookup"><span data-stu-id="9bfd1-107">The following example shows how to send an e-mail message.</span></span>
  
### <a name="code"></a><span data-ttu-id="9bfd1-108">Code</span><span class="sxs-lookup"><span data-stu-id="9bfd1-108">Code</span></span>

```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <SendItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" 
              SaveItemToFolder="true">
      <ItemIds>
        <t:ItemId Id="AAAtAEF=" ChangeKey="CQAAABY+T" />
      </ItemIds>
    </SendItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="9bfd1-109">Commentaires</span><span class="sxs-lookup"><span data-stu-id="9bfd1-109">Comments</span></span>

<span data-ttu-id="9bfd1-110">Identificateur de l'élément a été raccourcie afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="9bfd1-110">The item identifier has been shortened to preserve readability.</span></span>
  
### <a name="request-elements"></a><span data-ttu-id="9bfd1-111">Demander des éléments</span><span class="sxs-lookup"><span data-stu-id="9bfd1-111">Request elements</span></span>

<span data-ttu-id="9bfd1-112">Les éléments suivants sont utilisés dans la demande :</span><span class="sxs-lookup"><span data-stu-id="9bfd1-112">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="9bfd1-113">SendItem</span><span class="sxs-lookup"><span data-stu-id="9bfd1-113">SendItem</span></span>](senditem.md)
    
- [<span data-ttu-id="9bfd1-114">ItemIds</span><span class="sxs-lookup"><span data-stu-id="9bfd1-114">ItemIds</span></span>](itemids.md)
    
- [<span data-ttu-id="9bfd1-115">ItemId</span><span class="sxs-lookup"><span data-stu-id="9bfd1-115">ItemId</span></span>](itemid.md)
    
## <a name="successful-senditem-e-mail-message-response"></a><span data-ttu-id="9bfd1-116">Réponse SendItem (message électronique)</span><span class="sxs-lookup"><span data-stu-id="9bfd1-116">Successful SendItem (E-mail Message) Response</span></span>

### <a name="description"></a><span data-ttu-id="9bfd1-117">Description</span><span class="sxs-lookup"><span data-stu-id="9bfd1-117">Description</span></span>

<span data-ttu-id="9bfd1-118">L’exemple suivant montre une réponse SendItem réussie.</span><span class="sxs-lookup"><span data-stu-id="9bfd1-118">The following example shows a successful SendItem response.</span></span>
  
### <a name="code"></a><span data-ttu-id="9bfd1-119">Code</span><span class="sxs-lookup"><span data-stu-id="9bfd1-119">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="602" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <SendItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:SendItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:SendItemResponseMessage>
      </m:ResponseMessages>
    </SendItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a><span data-ttu-id="9bfd1-120">Éléments de réponse réussis</span><span class="sxs-lookup"><span data-stu-id="9bfd1-120">Successful response elements</span></span>

<span data-ttu-id="9bfd1-121">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="9bfd1-121">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="9bfd1-122">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="9bfd1-122">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="9bfd1-123">SendItemResponse</span><span class="sxs-lookup"><span data-stu-id="9bfd1-123">SendItemResponse</span></span>](senditemresponse.md)
    
- [<span data-ttu-id="9bfd1-124">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="9bfd1-124">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="9bfd1-125">SendItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="9bfd1-125">SendItemResponseMessage</span></span>](senditemresponsemessage.md)
    
- [<span data-ttu-id="9bfd1-126">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="9bfd1-126">ResponseCode</span></span>](responsecode.md)
    
### <a name="comments"></a><span data-ttu-id="9bfd1-127">Commentaires</span><span class="sxs-lookup"><span data-stu-id="9bfd1-127">Comments</span></span>

<span data-ttu-id="9bfd1-128">Un délégué qui tente d’envoyer un message électronique qui se trouve dans le dossier Brouillons de l’entité avec l’option Méthodesendandsavecopy définie sur enregistrer une copie dans le dossier unique éléments envoyés ne parviendra pas à déplacer une copie de l’élément envoyé vers le dossier unique éléments envoyés.</span><span class="sxs-lookup"><span data-stu-id="9bfd1-128">A delegate who tries to send an e-mail message that is located in the principal's Drafts folder with the SendAndSaveCopy option set to save a copy in the Sent Items distinguished folder will silently fail to move a copy of the sent item to the Sent Items distinguished folder.</span></span> <span data-ttu-id="9bfd1-129">L’élément reste dans le dossier Brouillons de l’entité de sécurité.</span><span class="sxs-lookup"><span data-stu-id="9bfd1-129">The item will remain in the principal's Drafts folder.</span></span> <span data-ttu-id="9bfd1-130">Pour contourner ce problème, spécifiez la boîte aux lettres de l’entité dans l’élément [DistinguishedFolderId](distinguishedfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="9bfd1-130">The workaround for this issue is to specify the principal's mailbox in the [DistinguishedFolderId](distinguishedfolderid.md) element.</span></span> 
  
<span data-ttu-id="9bfd1-131">Un autre scénario à prendre en considération est lorsqu’un délégué crée un message électronique et l’enregistre dans le dossier Brouillons de la boîte aux lettres du délégué.</span><span class="sxs-lookup"><span data-stu-id="9bfd1-131">An additional scenario to consider is when a delegate creates an e-mail message and saves it to the Drafts folder of the delegate's mailbox.</span></span> <span data-ttu-id="9bfd1-132">Si le délégué tente d’envoyer l’élément et d’enregistrer une copie dans le dossier unique éléments envoyés du principal, le message est envoyé correctement, le brouillon du message reste dans le dossier Brouillons du délégué, le message envoyé n’apparaît pas dans le dossier éléments envoyés du délégué ou du principal, et la réponse est une réussite.</span><span class="sxs-lookup"><span data-stu-id="9bfd1-132">If the delegate tries to send the item and save a copy to the principal's Sent Items distinguished folder, the message is sent correctly, the draft message remains in the delegate's Drafts folder, the sent message does not appear in either the delegate's or principal's Sent Items folder, and the response is a success.</span></span>
  
## <a name="invalid-senditem-e-mail-message-request-example"></a><span data-ttu-id="9bfd1-133">Exemple de requête SendItem (message électronique) non valide</span><span class="sxs-lookup"><span data-stu-id="9bfd1-133">Invalid SendItem (E-mail Message) request example</span></span>

### <a name="description"></a><span data-ttu-id="9bfd1-134">Description</span><span class="sxs-lookup"><span data-stu-id="9bfd1-134">Description</span></span>

<span data-ttu-id="9bfd1-135">L’exemple de code suivant montre un exemple de requête avec un identificateur non valide.</span><span class="sxs-lookup"><span data-stu-id="9bfd1-135">The following code sample shows an example of a request with an invalid identifier.</span></span>
  
### <a name="code"></a><span data-ttu-id="9bfd1-136">Code</span><span class="sxs-lookup"><span data-stu-id="9bfd1-136">Code</span></span>

```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <SendItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" 
              SaveItemToFolder="true">
      <ItemIds>
        <t:ItemId Id="%BadItemId%" ChangeKey="CQAAABYAAA" />
      </ItemIds>
    </SendItem>
  </soap:Body>
</soap:Envelope>
```

## <a name="senditem-e-mail-message-error-response"></a><span data-ttu-id="9bfd1-137">Réponse d’erreur SendItem (message électronique)</span><span class="sxs-lookup"><span data-stu-id="9bfd1-137">SendItem (E-mail Message) error response</span></span>

### <a name="description"></a><span data-ttu-id="9bfd1-138">Description</span><span class="sxs-lookup"><span data-stu-id="9bfd1-138">Description</span></span>

<span data-ttu-id="9bfd1-139">L’exemple suivant montre une réponse d’erreur à une requête SendItem qui contient un identificateur non valide.</span><span class="sxs-lookup"><span data-stu-id="9bfd1-139">The following example shows an error response to a SendItem request that contains an invalid identifier.</span></span>
  
### <a name="code"></a><span data-ttu-id="9bfd1-140">Code</span><span class="sxs-lookup"><span data-stu-id="9bfd1-140">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="602" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <SendItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:SendItemResponseMessage ResponseClass="Error">
          <m:MessageText>Id is malformed.</m:MessageText>
          <m:ResponseCode>ErrorInvalidIdMalformed</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:SendItemResponseMessage>
      </m:ResponseMessages>
    </SendItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="9bfd1-141">Éléments de réponse d’erreur</span><span class="sxs-lookup"><span data-stu-id="9bfd1-141">Error response elements</span></span>

<span data-ttu-id="9bfd1-142">Les éléments suivants sont utilisés dans la réponse d'erreur :</span><span class="sxs-lookup"><span data-stu-id="9bfd1-142">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="9bfd1-143">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="9bfd1-143">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="9bfd1-144">SendItemResponse</span><span class="sxs-lookup"><span data-stu-id="9bfd1-144">SendItemResponse</span></span>](senditemresponse.md)
    
- [<span data-ttu-id="9bfd1-145">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="9bfd1-145">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="9bfd1-146">SendItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="9bfd1-146">SendItemResponseMessage</span></span>](senditemresponsemessage.md)
    
- [<span data-ttu-id="9bfd1-147">MessageText</span><span class="sxs-lookup"><span data-stu-id="9bfd1-147">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="9bfd1-148">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="9bfd1-148">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="9bfd1-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="9bfd1-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="9bfd1-150">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="9bfd1-150">See also</span></span>



[<span data-ttu-id="9bfd1-151">Opération SendItem</span><span class="sxs-lookup"><span data-stu-id="9bfd1-151">SendItem operation</span></span>](senditem-operation.md)
  
 <span data-ttu-id="9bfd1-152">**SendItemType**</span><span class="sxs-lookup"><span data-stu-id="9bfd1-152">**SendItemType**</span></span>


- [<span data-ttu-id="9bfd1-153">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="9bfd1-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

