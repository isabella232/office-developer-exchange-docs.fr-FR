---
title: Opération CreateAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateAttachment
api_type:
- schema
ms.assetid: e066db95-6963-4507-a8d0-8efad287f550
description: L’opération CreateAttachment crée un élément ou une pièce jointe et l’attache à l’élément spécifié.
ms.openlocfilehash: 8028c56aa306774b54b39e5ee1ac0382b9113fa0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456569"
---
# <a name="createattachment-operation"></a><span data-ttu-id="b7525-103">Opération CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="b7525-103">CreateAttachment operation</span></span>

<span data-ttu-id="b7525-104">L’opération CreateAttachment crée un élément ou une pièce jointe et l’attache à l’élément spécifié.</span><span class="sxs-lookup"><span data-stu-id="b7525-104">The CreateAttachment operation creates either an item or file attachment and attaches it to the specified item.</span></span>
  
## <a name="file-createattachment-request-example"></a><span data-ttu-id="b7525-105">Exemple de requête CreateAttachment de fichier</span><span class="sxs-lookup"><span data-stu-id="b7525-105">File CreateAttachment request example</span></span>

### <a name="description"></a><span data-ttu-id="b7525-106">Description</span><span class="sxs-lookup"><span data-stu-id="b7525-106">Description</span></span>

<span data-ttu-id="b7525-107">L’exemple de requête CreateAttachment suivant montre comment créer une pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="b7525-107">The following example of a CreateAttachment request shows how to create a file attachment.</span></span>
  
### <a name="code"></a><span data-ttu-id="b7525-108">Code</span><span class="sxs-lookup"><span data-stu-id="b7525-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
<soap:Body>
  <CreateAttachment xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
    <ParentItemId Id="AAAtAE..." ChangeKey="CQAAABYA..."/>
    <Attachments>
      <t:FileAttachment>
        <t:Name>SomeFile</t:Name>
        <t:Content>AQIDBAU=</t:Content>
      </t:FileAttachment>
    </Attachments>
  </CreateAttachment>
</soap:Body>
</soap:Envelope>
```

### <a name="comment"></a><span data-ttu-id="b7525-109">Commentaire</span><span class="sxs-lookup"><span data-stu-id="b7525-109">Comment</span></span>

<span data-ttu-id="b7525-110">Un nom pour la pièce jointe doit être fourni.</span><span class="sxs-lookup"><span data-stu-id="b7525-110">A name for the attachment must be provided.</span></span>
  
> [!NOTE]
> <span data-ttu-id="b7525-111">L’identificateur de l’élément parent et la clé de modification ont été raccourcies afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="b7525-111">The parent item identifier and change key have been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="b7525-112">Demander des éléments</span><span class="sxs-lookup"><span data-stu-id="b7525-112">Request elements</span></span>

<span data-ttu-id="b7525-113">Les éléments suivants sont utilisés dans la demande :</span><span class="sxs-lookup"><span data-stu-id="b7525-113">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="b7525-114">CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="b7525-114">CreateAttachment</span></span>](createattachment.md)
    
- [<span data-ttu-id="b7525-115">ParentItemId</span><span class="sxs-lookup"><span data-stu-id="b7525-115">ParentItemId</span></span>](parentitemid.md)
    
- [<span data-ttu-id="b7525-116">Attachments</span><span class="sxs-lookup"><span data-stu-id="b7525-116">Attachments</span></span>](attachments-ex15websvcsotherref.md)
    
- [<span data-ttu-id="b7525-117">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="b7525-117">FileAttachment</span></span>](fileattachment.md)
    
- [<span data-ttu-id="b7525-118">Nom (AttachmentType)</span><span class="sxs-lookup"><span data-stu-id="b7525-118">Name (AttachmentType)</span></span>](name-attachmenttype.md)
    
- [<span data-ttu-id="b7525-119">Content</span><span class="sxs-lookup"><span data-stu-id="b7525-119">Content</span></span>](content.md)
    
## <a name="successful-file-createattachment-response-example"></a><span data-ttu-id="b7525-120">Exemple de réponse de CreateAttachment de fichier réussi</span><span class="sxs-lookup"><span data-stu-id="b7525-120">Successful File CreateAttachment response example</span></span>

### <a name="description"></a><span data-ttu-id="b7525-121">Description</span><span class="sxs-lookup"><span data-stu-id="b7525-121">Description</span></span>

<span data-ttu-id="b7525-122">L’exemple suivant montre une réponse réussie à la demande CreateAttachment.</span><span class="sxs-lookup"><span data-stu-id="b7525-122">The following example shows a successful response to the CreateAttachment request.</span></span>
  
### <a name="code"></a><span data-ttu-id="b7525-123">Code</span><span class="sxs-lookup"><span data-stu-id="b7525-123">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="653" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateAttachmentResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                              xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                              xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateAttachmentResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Attachments>
            <t:FileAttachment>
              <t:AttachmentId Id="AAAtAE=" RootItemId="AAAtAEFk=" RootItemChangeKey="CQAAAB"/>
            </t:FileAttachment>
          </m:Attachments>
        </m:CreateAttachmentResponseMessage>
      </m:ResponseMessages>
    </CreateAttachmentResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comment"></a><span data-ttu-id="b7525-124">Commentaire</span><span class="sxs-lookup"><span data-stu-id="b7525-124">Comment</span></span>

<span data-ttu-id="b7525-125">La réponse contient l’identificateur du fichier joint.</span><span class="sxs-lookup"><span data-stu-id="b7525-125">The response contains the identifier of the attached file.</span></span> <span data-ttu-id="b7525-126">Il contient également l’identificateur et la clé de modification de l’élément racine.</span><span class="sxs-lookup"><span data-stu-id="b7525-126">It also contains the identifier and change key of the root item.</span></span> <span data-ttu-id="b7525-127">Les identificateurs d’élément et la clé de modification ont été raccourcies afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="b7525-127">The item identifiers and change key have been shortened to preserve readability.</span></span>
  
### <a name="successful-response-elements"></a><span data-ttu-id="b7525-128">Éléments de réponse réussis</span><span class="sxs-lookup"><span data-stu-id="b7525-128">Successful response elements</span></span>

<span data-ttu-id="b7525-129">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="b7525-129">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="b7525-130">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="b7525-130">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="b7525-131">CreateAttachmentResponse</span><span class="sxs-lookup"><span data-stu-id="b7525-131">CreateAttachmentResponse</span></span>](createattachmentresponse.md)
    
- [<span data-ttu-id="b7525-132">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="b7525-132">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="b7525-133">CreateAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="b7525-133">CreateAttachmentResponseMessage</span></span>](createattachmentresponsemessage.md)
    
- [<span data-ttu-id="b7525-134">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="b7525-134">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="b7525-135">Attachments</span><span class="sxs-lookup"><span data-stu-id="b7525-135">Attachments</span></span>](attachments-ex15websvcsotherref.md)
    
- [<span data-ttu-id="b7525-136">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="b7525-136">FileAttachment</span></span>](fileattachment.md)
    
- [<span data-ttu-id="b7525-137">AttachmentId</span><span class="sxs-lookup"><span data-stu-id="b7525-137">AttachmentId</span></span>](attachmentid.md)
    
## <a name="item-createattachment-request-example"></a><span data-ttu-id="b7525-138">Exemple de requête CreateAttachment Item</span><span class="sxs-lookup"><span data-stu-id="b7525-138">Item CreateAttachment request example</span></span>

### <a name="description"></a><span data-ttu-id="b7525-139">Description</span><span class="sxs-lookup"><span data-stu-id="b7525-139">Description</span></span>

<span data-ttu-id="b7525-140">L’exemple de requête CreateAttachment suivant montre comment créer une pièce jointe d’un élément.</span><span class="sxs-lookup"><span data-stu-id="b7525-140">The following example of a CreateAttachment request shows how to create an item attachment.</span></span>
  
### <a name="code"></a><span data-ttu-id="b7525-141">Code</span><span class="sxs-lookup"><span data-stu-id="b7525-141">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateAttachment xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <ParentItemId Id="AAAtAE=" ChangeKey="CQAAABYA"/>
      <Attachments>
        <t:ItemAttachment>
          <t:Name>An item attachment</t:Name>
          <t:Message>
            <t:Subject>A message to attach</t:Subject>
          </t:Message>
        </t:ItemAttachment>
      </Attachments>
    </CreateAttachment>
  </soap:Body>
</soap:Envelope>
```

### <a name="comment"></a><span data-ttu-id="b7525-142">Commentaire</span><span class="sxs-lookup"><span data-stu-id="b7525-142">Comment</span></span>

<span data-ttu-id="b7525-143">Un nom pour la pièce jointe doit être fourni.</span><span class="sxs-lookup"><span data-stu-id="b7525-143">A name for the attachment must be provided.</span></span>
  
 <span data-ttu-id="b7525-144">**Note** L’identificateur de l’élément parent et la clé de modification ont été raccourcies afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="b7525-144">**Note** The parent item identifier and change key have been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="b7525-145">Demander des éléments</span><span class="sxs-lookup"><span data-stu-id="b7525-145">Request elements</span></span>

<span data-ttu-id="b7525-146">Les éléments suivants sont utilisés dans la demande :</span><span class="sxs-lookup"><span data-stu-id="b7525-146">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="b7525-147">CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="b7525-147">CreateAttachment</span></span>](createattachment.md)
    
- [<span data-ttu-id="b7525-148">ParentItemId</span><span class="sxs-lookup"><span data-stu-id="b7525-148">ParentItemId</span></span>](parentitemid.md)
    
- [<span data-ttu-id="b7525-149">Attachments</span><span class="sxs-lookup"><span data-stu-id="b7525-149">Attachments</span></span>](attachments-ex15websvcsotherref.md)
    
- [<span data-ttu-id="b7525-150">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="b7525-150">ItemAttachment</span></span>](itemattachment.md)
    
- [<span data-ttu-id="b7525-151">Nom (AttachmentType)</span><span class="sxs-lookup"><span data-stu-id="b7525-151">Name (AttachmentType)</span></span>](name-attachmenttype.md)
    
- [<span data-ttu-id="b7525-152">Message</span><span class="sxs-lookup"><span data-stu-id="b7525-152">Message</span></span>](message-ex15websvcsotherref.md)
    
- [<span data-ttu-id="b7525-153">Subject</span><span class="sxs-lookup"><span data-stu-id="b7525-153">Subject</span></span>](subject.md)
    
## <a name="successful-item-createattachment-response-example"></a><span data-ttu-id="b7525-154">Exemple de réponse de CreateAttachment d’élément réussi</span><span class="sxs-lookup"><span data-stu-id="b7525-154">Successful Item CreateAttachment response example</span></span>

### <a name="description"></a><span data-ttu-id="b7525-155">Description</span><span class="sxs-lookup"><span data-stu-id="b7525-155">Description</span></span>

<span data-ttu-id="b7525-156">L’exemple suivant montre une réponse réussie à la demande CreateAttachment.</span><span class="sxs-lookup"><span data-stu-id="b7525-156">The following example shows a successful response to the CreateAttachment request.</span></span>
  
### <a name="code"></a><span data-ttu-id="b7525-157">Code</span><span class="sxs-lookup"><span data-stu-id="b7525-157">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="653" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateAttachmentResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                              xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                              xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateAttachmentResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Attachments>
            <t:ItemAttachment>
              <t:AttachmentId Id="AAAtAEFk=" RootItemId="AAAtAEFkb=" RootItemChangeKey="CQAAABYA"/>
            </t:ItemAttachment>
          </m:Attachments>
        </m:CreateAttachmentResponseMessage>
      </m:ResponseMessages>
    </CreateAttachmentResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comment"></a><span data-ttu-id="b7525-158">Commentaire</span><span class="sxs-lookup"><span data-stu-id="b7525-158">Comment</span></span>

<span data-ttu-id="b7525-159">La réponse contient l’identificateur de la nouvelle pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="b7525-159">The response contains the identifier of the new attachment.</span></span> <span data-ttu-id="b7525-160">Il contient également l’identificateur et la clé de modification de l’élément racine.</span><span class="sxs-lookup"><span data-stu-id="b7525-160">It also contains the identifier and change key of the root item.</span></span> <span data-ttu-id="b7525-161">L’élément racine est l’élément qui contient la pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="b7525-161">The root item is the item that contains the attachment.</span></span> <span data-ttu-id="b7525-162">Les identificateurs d’élément et la clé de modification ont été raccourcies afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="b7525-162">The item identifiers and change key have been shortened to preserve readability.</span></span>
  
### <a name="successful-response-elements"></a><span data-ttu-id="b7525-163">Éléments de réponse réussis</span><span class="sxs-lookup"><span data-stu-id="b7525-163">Successful response elements</span></span>

<span data-ttu-id="b7525-164">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="b7525-164">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="b7525-165">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="b7525-165">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="b7525-166">CreateAttachmentResponse</span><span class="sxs-lookup"><span data-stu-id="b7525-166">CreateAttachmentResponse</span></span>](createattachmentresponse.md)
    
- [<span data-ttu-id="b7525-167">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="b7525-167">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="b7525-168">CreateAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="b7525-168">CreateAttachmentResponseMessage</span></span>](createattachmentresponsemessage.md)
    
- [<span data-ttu-id="b7525-169">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="b7525-169">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="b7525-170">Attachments</span><span class="sxs-lookup"><span data-stu-id="b7525-170">Attachments</span></span>](attachments-ex15websvcsotherref.md)
    
- [<span data-ttu-id="b7525-171">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="b7525-171">ItemAttachment</span></span>](itemattachment.md)
    
- [<span data-ttu-id="b7525-172">AttachmentId</span><span class="sxs-lookup"><span data-stu-id="b7525-172">AttachmentId</span></span>](attachmentid.md)
    
## <a name="createattachment-error-response-example"></a><span data-ttu-id="b7525-173">Exemple de réponse d’erreur CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="b7525-173">CreateAttachment Error response example</span></span>

### <a name="description"></a><span data-ttu-id="b7525-174">Description</span><span class="sxs-lookup"><span data-stu-id="b7525-174">Description</span></span>

<span data-ttu-id="b7525-175">L’exemple suivant montre une réponse d’erreur à la demande CreateAttachment.</span><span class="sxs-lookup"><span data-stu-id="b7525-175">The following example shows an error response to the CreateAttachment request.</span></span> <span data-ttu-id="b7525-176">L’erreur est due au fait que le nom de la pièce jointe n’a pas été spécifié.</span><span class="sxs-lookup"><span data-stu-id="b7525-176">The error is due to the fact that the name of the attachment was not specified.</span></span>
  
### <a name="code"></a><span data-ttu-id="b7525-177">Code</span><span class="sxs-lookup"><span data-stu-id="b7525-177">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="653" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateAttachmentResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                              xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                              xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateAttachmentResponseMessage ResponseClass="Error">
          <m:MessageText>Required property is missing.</m:MessageText>
          <m:ResponseCode>ErrorRequiredPropertyMissing</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:MessageXml>
            <t:ExceptionFieldURI FieldURI="attachment:Name"/>
          </m:MessageXml>
          <m:Attachments/>
        </m:CreateAttachmentResponseMessage>
      </m:ResponseMessages>
    </CreateAttachmentResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="b7525-178">Éléments de réponse d’erreur</span><span class="sxs-lookup"><span data-stu-id="b7525-178">Error response elements</span></span>

<span data-ttu-id="b7525-179">Les éléments suivants sont utilisés dans la réponse d'erreur :</span><span class="sxs-lookup"><span data-stu-id="b7525-179">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="b7525-180">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="b7525-180">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="b7525-181">CreateAttachmentResponse</span><span class="sxs-lookup"><span data-stu-id="b7525-181">CreateAttachmentResponse</span></span>](createattachmentresponse.md)
    
- [<span data-ttu-id="b7525-182">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="b7525-182">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="b7525-183">CreateAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="b7525-183">CreateAttachmentResponseMessage</span></span>](createattachmentresponsemessage.md)
    
- [<span data-ttu-id="b7525-184">MessageText</span><span class="sxs-lookup"><span data-stu-id="b7525-184">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="b7525-185">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="b7525-185">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="b7525-186">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="b7525-186">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="b7525-187">MessageXml</span><span class="sxs-lookup"><span data-stu-id="b7525-187">MessageXml</span></span>](messagexml.md)
    
- [<span data-ttu-id="b7525-188">ExceptionFieldURI</span><span class="sxs-lookup"><span data-stu-id="b7525-188">ExceptionFieldURI</span></span>](exceptionfielduri.md)
    
- [<span data-ttu-id="b7525-189">Attachments</span><span class="sxs-lookup"><span data-stu-id="b7525-189">Attachments</span></span>](attachments-ex15websvcsotherref.md)
    
## <a name="remarks"></a><span data-ttu-id="b7525-190">Remarques</span><span class="sxs-lookup"><span data-stu-id="b7525-190">Remarks</span></span>

<span data-ttu-id="b7525-191">Si plusieurs pièces jointes sont attachées à un élément en un seul aller-retour, le RootItemChangeKey dans le dernier message de réponse est celui qui représente la nouvelle clé de modification de l’élément qui contient les pièces jointes.</span><span class="sxs-lookup"><span data-stu-id="b7525-191">If multiple attachments are attached to an item in a single round trip, the RootItemChangeKey in the last response message is the one that represents the new change key of the item that has the attachments.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="b7525-192">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b7525-192">See also</span></span>



[<span data-ttu-id="b7525-193">Opération DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="b7525-193">DeleteAttachment operation</span></span>](deleteattachment-operation.md)
  
[<span data-ttu-id="b7525-194">Opération GetAttachment</span><span class="sxs-lookup"><span data-stu-id="b7525-194">GetAttachment operation</span></span>](getattachment-operation.md)

