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
description: L’opération CreateAttachment crée un élément ou un fichier de pièce jointe et l’attache à l’élément spécifié.
ms.openlocfilehash: fed60275a007f2796c60d936def7a937e4982f29
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755681"
---
# <a name="createattachment-operation"></a><span data-ttu-id="7d028-103">Opération CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="7d028-103">CreateAttachment operation</span></span>

<span data-ttu-id="7d028-104">L’opération CreateAttachment crée un élément ou un fichier de pièce jointe et l’attache à l’élément spécifié.</span><span class="sxs-lookup"><span data-stu-id="7d028-104">The CreateAttachment operation creates either an item or file attachment and attaches it to the specified item.</span></span>
  
## <a name="file-createattachment-request-example"></a><span data-ttu-id="7d028-105">Exemple de fichier de demande CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="7d028-105">File CreateAttachment request example</span></span>

### <a name="description"></a><span data-ttu-id="7d028-106">Description</span><span class="sxs-lookup"><span data-stu-id="7d028-106">Description</span></span>

<span data-ttu-id="7d028-107">Une demande CreateAttachment l’exemple suivant montre comment créer un fichier joint.</span><span class="sxs-lookup"><span data-stu-id="7d028-107">The following example of a CreateAttachment request shows how to create a file attachment.</span></span>
  
### <a name="code"></a><span data-ttu-id="7d028-108">Code</span><span class="sxs-lookup"><span data-stu-id="7d028-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
<soap:Body>
  <CreateAttachment xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

### <a name="comment"></a><span data-ttu-id="7d028-109">Commentaires</span><span class="sxs-lookup"><span data-stu-id="7d028-109">Comment</span></span>

<span data-ttu-id="7d028-110">Nom de la pièce jointe doit être fourni.</span><span class="sxs-lookup"><span data-stu-id="7d028-110">A name for the attachment must be provided.</span></span>
  
> [!NOTE]
> <span data-ttu-id="7d028-111">L’identificateur de l’élément parent et modifier la clé ont été réduits afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="7d028-111">The parent item identifier and change key have been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="7d028-112">Éléments de la demande</span><span class="sxs-lookup"><span data-stu-id="7d028-112">Request elements</span></span>

<span data-ttu-id="7d028-113">Les éléments suivants sont utilisés dans la demande :</span><span class="sxs-lookup"><span data-stu-id="7d028-113">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="7d028-114">CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="7d028-114">CreateAttachment</span></span>](createattachment.md)
    
- [<span data-ttu-id="7d028-115">ParentItemId</span><span class="sxs-lookup"><span data-stu-id="7d028-115">ParentItemId</span></span>](parentitemid.md)
    
- [<span data-ttu-id="7d028-116">Pièces jointes</span><span class="sxs-lookup"><span data-stu-id="7d028-116">Attachments</span></span>](attachments-ex15websvcsotherref.md)
    
- [<span data-ttu-id="7d028-117">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="7d028-117">FileAttachment</span></span>](fileattachment.md)
    
- [<span data-ttu-id="7d028-118">Nom (AttachmentType)</span><span class="sxs-lookup"><span data-stu-id="7d028-118">Name (AttachmentType)</span></span>](name-attachmenttype.md)
    
- [<span data-ttu-id="7d028-119">Content</span><span class="sxs-lookup"><span data-stu-id="7d028-119">Content</span></span>](content.md)
    
## <a name="successful-file-createattachment-response-example"></a><span data-ttu-id="7d028-120">Exemple de réponse CreateAttachment fichier réussie</span><span class="sxs-lookup"><span data-stu-id="7d028-120">Successful File CreateAttachment response example</span></span>

### <a name="description"></a><span data-ttu-id="7d028-121">Description</span><span class="sxs-lookup"><span data-stu-id="7d028-121">Description</span></span>

<span data-ttu-id="7d028-122">L’exemple suivant montre une réponse positive à la demande CreateAttachment.</span><span class="sxs-lookup"><span data-stu-id="7d028-122">The following example shows a successful response to the CreateAttachment request.</span></span>
  
### <a name="code"></a><span data-ttu-id="7d028-123">Code</span><span class="sxs-lookup"><span data-stu-id="7d028-123">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="653" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateAttachmentResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                              xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                              xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comment"></a><span data-ttu-id="7d028-124">Commentaires</span><span class="sxs-lookup"><span data-stu-id="7d028-124">Comment</span></span>

<span data-ttu-id="7d028-125">La réponse contient l’identificateur du fichier joint.</span><span class="sxs-lookup"><span data-stu-id="7d028-125">The response contains the identifier of the attached file.</span></span> <span data-ttu-id="7d028-126">Il contient également la clé d’identificateur et modification de l’élément racine.</span><span class="sxs-lookup"><span data-stu-id="7d028-126">It also contains the identifier and change key of the root item.</span></span> <span data-ttu-id="7d028-127">Les identificateurs d’élément et modifier la clé ont été réduits afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="7d028-127">The item identifiers and change key have been shortened to preserve readability.</span></span>
  
### <a name="successful-response-elements"></a><span data-ttu-id="7d028-128">Éléments de réponse réussie</span><span class="sxs-lookup"><span data-stu-id="7d028-128">Successful response elements</span></span>

<span data-ttu-id="7d028-129">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="7d028-129">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="7d028-130">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="7d028-130">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="7d028-131">CreateAttachmentResponse</span><span class="sxs-lookup"><span data-stu-id="7d028-131">CreateAttachmentResponse</span></span>](createattachmentresponse.md)
    
- [<span data-ttu-id="7d028-132">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="7d028-132">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="7d028-133">CreateAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="7d028-133">CreateAttachmentResponseMessage</span></span>](createattachmentresponsemessage.md)
    
- [<span data-ttu-id="7d028-134">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="7d028-134">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="7d028-135">Pièces jointes</span><span class="sxs-lookup"><span data-stu-id="7d028-135">Attachments</span></span>](attachments-ex15websvcsotherref.md)
    
- [<span data-ttu-id="7d028-136">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="7d028-136">FileAttachment</span></span>](fileattachment.md)
    
- [<span data-ttu-id="7d028-137">AttachmentId</span><span class="sxs-lookup"><span data-stu-id="7d028-137">AttachmentId</span></span>](attachmentid.md)
    
## <a name="item-createattachment-request-example"></a><span data-ttu-id="7d028-138">Exemple de requête CreateAttachment élément</span><span class="sxs-lookup"><span data-stu-id="7d028-138">Item CreateAttachment request example</span></span>

### <a name="description"></a><span data-ttu-id="7d028-139">Description</span><span class="sxs-lookup"><span data-stu-id="7d028-139">Description</span></span>

<span data-ttu-id="7d028-140">Une demande CreateAttachment l’exemple suivant montre comment créer une pièce jointe d’élément.</span><span class="sxs-lookup"><span data-stu-id="7d028-140">The following example of a CreateAttachment request shows how to create an item attachment.</span></span>
  
### <a name="code"></a><span data-ttu-id="7d028-141">Code</span><span class="sxs-lookup"><span data-stu-id="7d028-141">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateAttachment xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

### <a name="comment"></a><span data-ttu-id="7d028-142">Commentaires</span><span class="sxs-lookup"><span data-stu-id="7d028-142">Comment</span></span>

<span data-ttu-id="7d028-143">Nom de la pièce jointe doit être fourni.</span><span class="sxs-lookup"><span data-stu-id="7d028-143">A name for the attachment must be provided.</span></span>
  
 <span data-ttu-id="7d028-144">**Remarque** L’identificateur de l’élément parent et modifier la clé ont été réduits afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="7d028-144">**Note** The parent item identifier and change key have been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="7d028-145">Éléments de la demande</span><span class="sxs-lookup"><span data-stu-id="7d028-145">Request elements</span></span>

<span data-ttu-id="7d028-146">Les éléments suivants sont utilisés dans la demande :</span><span class="sxs-lookup"><span data-stu-id="7d028-146">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="7d028-147">CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="7d028-147">CreateAttachment</span></span>](createattachment.md)
    
- [<span data-ttu-id="7d028-148">ParentItemId</span><span class="sxs-lookup"><span data-stu-id="7d028-148">ParentItemId</span></span>](parentitemid.md)
    
- [<span data-ttu-id="7d028-149">Pièces jointes</span><span class="sxs-lookup"><span data-stu-id="7d028-149">Attachments</span></span>](attachments-ex15websvcsotherref.md)
    
- [<span data-ttu-id="7d028-150">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="7d028-150">ItemAttachment</span></span>](itemattachment.md)
    
- [<span data-ttu-id="7d028-151">Nom (AttachmentType)</span><span class="sxs-lookup"><span data-stu-id="7d028-151">Name (AttachmentType)</span></span>](name-attachmenttype.md)
    
- [<span data-ttu-id="7d028-152">Message</span><span class="sxs-lookup"><span data-stu-id="7d028-152">Message</span></span>](message-ex15websvcsotherref.md)
    
- [<span data-ttu-id="7d028-153">Objet</span><span class="sxs-lookup"><span data-stu-id="7d028-153">Subject</span></span>](subject.md)
    
## <a name="successful-item-createattachment-response-example"></a><span data-ttu-id="7d028-154">Exemple de réponse élément CreateAttachment réussie</span><span class="sxs-lookup"><span data-stu-id="7d028-154">Successful Item CreateAttachment response example</span></span>

### <a name="description"></a><span data-ttu-id="7d028-155">Description</span><span class="sxs-lookup"><span data-stu-id="7d028-155">Description</span></span>

<span data-ttu-id="7d028-156">L’exemple suivant montre une réponse positive à la demande CreateAttachment.</span><span class="sxs-lookup"><span data-stu-id="7d028-156">The following example shows a successful response to the CreateAttachment request.</span></span>
  
### <a name="code"></a><span data-ttu-id="7d028-157">Code</span><span class="sxs-lookup"><span data-stu-id="7d028-157">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="653" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateAttachmentResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                              xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                              xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comment"></a><span data-ttu-id="7d028-158">Commentaires</span><span class="sxs-lookup"><span data-stu-id="7d028-158">Comment</span></span>

<span data-ttu-id="7d028-159">La réponse contient l’identificateur de la nouvelle pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="7d028-159">The response contains the identifier of the new attachment.</span></span> <span data-ttu-id="7d028-160">Il contient également la clé d’identificateur et modification de l’élément racine.</span><span class="sxs-lookup"><span data-stu-id="7d028-160">It also contains the identifier and change key of the root item.</span></span> <span data-ttu-id="7d028-161">L’élément racine est l’élément qui contient la pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="7d028-161">The root item is the item that contains the attachment.</span></span> <span data-ttu-id="7d028-162">Les identificateurs d’élément et modifier la clé ont été réduits afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="7d028-162">The item identifiers and change key have been shortened to preserve readability.</span></span>
  
### <a name="successful-response-elements"></a><span data-ttu-id="7d028-163">Éléments de réponse réussie</span><span class="sxs-lookup"><span data-stu-id="7d028-163">Successful response elements</span></span>

<span data-ttu-id="7d028-164">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="7d028-164">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="7d028-165">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="7d028-165">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="7d028-166">CreateAttachmentResponse</span><span class="sxs-lookup"><span data-stu-id="7d028-166">CreateAttachmentResponse</span></span>](createattachmentresponse.md)
    
- [<span data-ttu-id="7d028-167">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="7d028-167">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="7d028-168">CreateAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="7d028-168">CreateAttachmentResponseMessage</span></span>](createattachmentresponsemessage.md)
    
- [<span data-ttu-id="7d028-169">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="7d028-169">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="7d028-170">Pièces jointes</span><span class="sxs-lookup"><span data-stu-id="7d028-170">Attachments</span></span>](attachments-ex15websvcsotherref.md)
    
- [<span data-ttu-id="7d028-171">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="7d028-171">ItemAttachment</span></span>](itemattachment.md)
    
- [<span data-ttu-id="7d028-172">AttachmentId</span><span class="sxs-lookup"><span data-stu-id="7d028-172">AttachmentId</span></span>](attachmentid.md)
    
## <a name="createattachment-error-response-example"></a><span data-ttu-id="7d028-173">Exemple de réponse d’erreur CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="7d028-173">CreateAttachment Error response example</span></span>

### <a name="description"></a><span data-ttu-id="7d028-174">Description</span><span class="sxs-lookup"><span data-stu-id="7d028-174">Description</span></span>

<span data-ttu-id="7d028-175">L’exemple suivant montre une réponse d’erreur à la demande CreateAttachment.</span><span class="sxs-lookup"><span data-stu-id="7d028-175">The following example shows an error response to the CreateAttachment request.</span></span> <span data-ttu-id="7d028-176">L’erreur est due au fait que le nom de la pièce jointe n’a pas été spécifié.</span><span class="sxs-lookup"><span data-stu-id="7d028-176">The error is due to the fact that the name of the attachment was not specified.</span></span>
  
### <a name="code"></a><span data-ttu-id="7d028-177">Code</span><span class="sxs-lookup"><span data-stu-id="7d028-177">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="653" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateAttachmentResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                              xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                              xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="error-response-elements"></a><span data-ttu-id="7d028-178">Éléments de réponse d’erreur</span><span class="sxs-lookup"><span data-stu-id="7d028-178">Error response elements</span></span>

<span data-ttu-id="7d028-179">Les éléments suivants sont utilisés dans la réponse d'erreur :</span><span class="sxs-lookup"><span data-stu-id="7d028-179">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="7d028-180">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="7d028-180">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="7d028-181">CreateAttachmentResponse</span><span class="sxs-lookup"><span data-stu-id="7d028-181">CreateAttachmentResponse</span></span>](createattachmentresponse.md)
    
- [<span data-ttu-id="7d028-182">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="7d028-182">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="7d028-183">CreateAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="7d028-183">CreateAttachmentResponseMessage</span></span>](createattachmentresponsemessage.md)
    
- [<span data-ttu-id="7d028-184">MessageText</span><span class="sxs-lookup"><span data-stu-id="7d028-184">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="7d028-185">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="7d028-185">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="7d028-186">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="7d028-186">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="7d028-187">MessageXml</span><span class="sxs-lookup"><span data-stu-id="7d028-187">MessageXml</span></span>](messagexml.md)
    
- [<span data-ttu-id="7d028-188">ExceptionFieldURI</span><span class="sxs-lookup"><span data-stu-id="7d028-188">ExceptionFieldURI</span></span>](exceptionfielduri.md)
    
- [<span data-ttu-id="7d028-189">Pièces jointes</span><span class="sxs-lookup"><span data-stu-id="7d028-189">Attachments</span></span>](attachments-ex15websvcsotherref.md)
    
## <a name="remarks"></a><span data-ttu-id="7d028-190">Remarques</span><span class="sxs-lookup"><span data-stu-id="7d028-190">Remarks</span></span>

<span data-ttu-id="7d028-191">Si plusieurs pièces jointes sont associés à un élément dans une seule boucle, le RootItemChangeKey du dernier message de réponse est celui qui représente la nouvelle clé de modification de l’élément qui a les pièces jointes.</span><span class="sxs-lookup"><span data-stu-id="7d028-191">If multiple attachments are attached to an item in a single round trip, the RootItemChangeKey in the last response message is the one that represents the new change key of the item that has the attachments.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="7d028-192">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7d028-192">See also</span></span>



[<span data-ttu-id="7d028-193">Opération DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="7d028-193">DeleteAttachment operation</span></span>](deleteattachment-operation.md)
  
[<span data-ttu-id="7d028-194">Opération GetAttachment</span><span class="sxs-lookup"><span data-stu-id="7d028-194">GetAttachment operation</span></span>](getattachment-operation.md)

