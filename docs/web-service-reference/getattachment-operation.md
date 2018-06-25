---
title: Opération GetAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetAttachment
api_type:
- schema
ms.assetid: 24d10a15-b942-415e-9024-a6375708f326
description: L’opération GetAttachment est utilisée pour récupérer les pièces jointes existantes sur des éléments de la banque d’informations Exchange.
ms.openlocfilehash: c260033208bf49c60463c09041d8ffcc52a8f5c2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756527"
---
# <a name="getattachment-operation"></a><span data-ttu-id="014c9-103">Opération GetAttachment</span><span class="sxs-lookup"><span data-stu-id="014c9-103">GetAttachment operation</span></span>

<span data-ttu-id="014c9-104">L’opération GetAttachment est utilisée pour récupérer les pièces jointes existantes sur des éléments de la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="014c9-104">The GetAttachment operation is used to retrieve existing attachments on items in the Exchange store.</span></span>
  
## <a name="getattachment-request-example"></a><span data-ttu-id="014c9-105">Exemple de requête GetAttachment</span><span class="sxs-lookup"><span data-stu-id="014c9-105">GetAttachment request example</span></span>

### <a name="description"></a><span data-ttu-id="014c9-106">Description</span><span class="sxs-lookup"><span data-stu-id="014c9-106">Description</span></span>

<span data-ttu-id="014c9-107">L’exemple de requête GetAttachment suivant montre comment obtenir une pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="014c9-107">The following example of GetAttachment request shows how to get an attachment.</span></span>
  
### <a name="code"></a><span data-ttu-id="014c9-108">Code</span><span class="sxs-lookup"><span data-stu-id="014c9-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
xmlns:xsd="http://www.w3.org/2001/XMLSchema"
xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetAttachment xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <AttachmentShape/>
      <AttachmentIds>
        <t:AttachmentId Id="AAAtAEFkbWluaX..."/>
      </AttachmentIds>
    </GetAttachment>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="014c9-109">Commentaires</span><span class="sxs-lookup"><span data-stu-id="014c9-109">Comments</span></span>

<span data-ttu-id="014c9-110">L’élément [AttachmentShape](attachmentshape.md) vous permet de vous permet de spécifier les informations de pièce jointe doivent être retournées.</span><span class="sxs-lookup"><span data-stu-id="014c9-110">The [AttachmentShape](attachmentshape.md) element allows you to specify which attachment information should be returned.</span></span> <span data-ttu-id="014c9-111">Un élément [AttachmentShape](attachmentshape.md) vide est valide et affiche votre les pièces jointes sans contenu MIME des pièces jointes d’élément, avec un type de corps de texte et sans les propriétés supplémentaires.</span><span class="sxs-lookup"><span data-stu-id="014c9-111">An empty [AttachmentShape](attachmentshape.md) element is valid and will render your attachments without MIME content for item attachments, with a text body type, and without any additional properties.</span></span> 
  
<span data-ttu-id="014c9-112">La collection [AttachmentIds](attachmentids.md) vous permet de spécifier un ou plusieurs identificateurs de pièce jointe à renvoyer.</span><span class="sxs-lookup"><span data-stu-id="014c9-112">The [AttachmentIds](attachmentids.md) collection allows you to specify one or more attachment identifiers to return.</span></span> <span data-ttu-id="014c9-113">Notez qu’il s’agit du type RequestAttachmentIdType, n’importe quel AttachmentIds que vous recevez **CreateAttachment** doit avoir les attributs **RootItemId** et **RootItemChangeKey** supprimé avant de les transmettre à **GetAttachment**.</span><span class="sxs-lookup"><span data-stu-id="014c9-113">Note that these are of type RequestAttachmentIdType, so any AttachmentIds that you receive from **CreateAttachment** must have the **RootItemId** and **RootItemChangeKey** attributes removed before passing them to **GetAttachment**.</span></span>
  
> [!NOTE]
> <span data-ttu-id="014c9-114">L’identificateur de pièce jointe et modifier la clé ont été réduits afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="014c9-114">The attachment identifier and change key have been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="014c9-115">Éléments de la demande</span><span class="sxs-lookup"><span data-stu-id="014c9-115">Request elements</span></span>

<span data-ttu-id="014c9-116">Les éléments suivants sont utilisés dans la demande :</span><span class="sxs-lookup"><span data-stu-id="014c9-116">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="014c9-117">GetAttachment</span><span class="sxs-lookup"><span data-stu-id="014c9-117">GetAttachment</span></span>](getattachment.md)
    
- [<span data-ttu-id="014c9-118">AttachmentShape</span><span class="sxs-lookup"><span data-stu-id="014c9-118">AttachmentShape</span></span>](attachmentshape.md)
    
- [<span data-ttu-id="014c9-119">AttachmentIds</span><span class="sxs-lookup"><span data-stu-id="014c9-119">AttachmentIds</span></span>](attachmentids.md)
    
- [<span data-ttu-id="014c9-120">AttachmentId (GetAttachment et DeleteAttachment)</span><span class="sxs-lookup"><span data-stu-id="014c9-120">AttachmentId (GetAttachment and DeleteAttachment)</span></span>](attachmentid-getattachment-and-deleteattachment.md)
    
## <a name="getattachment-response-example"></a><span data-ttu-id="014c9-121">Exemple de réponse GetAttachment</span><span class="sxs-lookup"><span data-stu-id="014c9-121">GetAttachment response example</span></span>

### <a name="description"></a><span data-ttu-id="014c9-122">Description</span><span class="sxs-lookup"><span data-stu-id="014c9-122">Description</span></span>

<span data-ttu-id="014c9-123">L’exemple suivant montre une réponse positive à une demande GetAttachment.</span><span class="sxs-lookup"><span data-stu-id="014c9-123">The following example shows a successful response to a GetAttachment request.</span></span> <span data-ttu-id="014c9-124">Cet exemple renvoie une pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="014c9-124">This example returns a file attachment.</span></span>
  
### <a name="code"></a><span data-ttu-id="014c9-125">Code</span><span class="sxs-lookup"><span data-stu-id="014c9-125">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="662" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <GetAttachmentResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                           xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetAttachmentResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Attachments>
            <t:FileAttachment>
              <t:AttachmentId Id="AAAtAEFkbWluaX..."/>
              <t:Name>SomeFile</t:Name>
              <t:Content>AQIDBAU=</t:Content>
            </t:FileAttachment>
          </m:Attachments>
        </m:GetAttachmentResponseMessage>
      </m:ResponseMessages>
    </GetAttachmentResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="014c9-126">Commentaires</span><span class="sxs-lookup"><span data-stu-id="014c9-126">Comments</span></span>

<span data-ttu-id="014c9-127">Les messages de réponse pour GetAttachment contient toujours la pièce jointe complet ; Autrement dit, toutes les propriétés sera toujours incluses.</span><span class="sxs-lookup"><span data-stu-id="014c9-127">The response messages for GetAttachment will always contain the full attachment; that is, all properties will always be included.</span></span> <span data-ttu-id="014c9-128">Pour les pièces jointes, ces propriétés sont [nom (AttachmentType)](name-attachmenttype.md), [ContentType](contenttype.md), [ContentId](contentid.md), [ContentLocation](contentlocation.md)et [contenu](content.md).</span><span class="sxs-lookup"><span data-stu-id="014c9-128">For file attachments, those properties are [Name (AttachmentType)](name-attachmenttype.md), [ContentType](contenttype.md), [ContentId](contentid.md), [ContentLocation](contentlocation.md), and [Content](content.md).</span></span> <span data-ttu-id="014c9-129">Les pièces jointes d’élément, ces propriétés sont [nom (AttachmentType)](name-attachmenttype.md), [ContentType](contenttype.md), [ContentId](contentid.md), [ContentLocation](contentlocation.md) et toutes les propriétés de l’élément, comme si la forme **AllProperties** a été utilisée dans un appel GetItem.</span><span class="sxs-lookup"><span data-stu-id="014c9-129">For item attachments, those properties are [Name (AttachmentType)](name-attachmenttype.md), [ContentType](contenttype.md), [ContentId](contentid.md), [ContentLocation](contentlocation.md) and all of the item's properties, as if the **AllProperties** shape had been used in a GetItem call.</span></span> <span data-ttu-id="014c9-130">L’élément [AttachmentShape](attachmentshape.md) , le cas échéant, permettra une application consommateur demander les propriétés étendues supplémentaires pour les pièces jointes de l’élément.</span><span class="sxs-lookup"><span data-stu-id="014c9-130">The [AttachmentShape](attachmentshape.md) element, if present, will allow a consumer application to request additional extended properties for item attachments.</span></span> 
  
### <a name="successful-response-elements"></a><span data-ttu-id="014c9-131">Éléments de réponse réussie</span><span class="sxs-lookup"><span data-stu-id="014c9-131">Successful response elements</span></span>

<span data-ttu-id="014c9-132">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="014c9-132">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="014c9-133">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="014c9-133">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="014c9-134">GetAttachmentResponse</span><span class="sxs-lookup"><span data-stu-id="014c9-134">GetAttachmentResponse</span></span>](getattachmentresponse.md)
    
- [<span data-ttu-id="014c9-135">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="014c9-135">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="014c9-136">GetAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="014c9-136">GetAttachmentResponseMessage</span></span>](getattachmentresponsemessage.md)
    
- [<span data-ttu-id="014c9-137">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="014c9-137">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="014c9-138">Pièces jointes</span><span class="sxs-lookup"><span data-stu-id="014c9-138">Attachments</span></span>](attachments-ex15websvcsotherref.md)
    
- [<span data-ttu-id="014c9-139">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="014c9-139">FileAttachment</span></span>](fileattachment.md)
    
- [<span data-ttu-id="014c9-140">AttachmentId (GetAttachment et DeleteAttachment)</span><span class="sxs-lookup"><span data-stu-id="014c9-140">AttachmentId (GetAttachment and DeleteAttachment)</span></span>](attachmentid-getattachment-and-deleteattachment.md)
    
- [<span data-ttu-id="014c9-141">Nom (AttachmentType)</span><span class="sxs-lookup"><span data-stu-id="014c9-141">Name (AttachmentType)</span></span>](name-attachmenttype.md)
    
- [<span data-ttu-id="014c9-142">Content</span><span class="sxs-lookup"><span data-stu-id="014c9-142">Content</span></span>](content.md)
    
## <a name="see-also"></a><span data-ttu-id="014c9-143">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="014c9-143">See also</span></span>



[<span data-ttu-id="014c9-144">Opération CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="014c9-144">CreateAttachment operation</span></span>](createattachment-operation.md)
  
[<span data-ttu-id="014c9-145">Opération DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="014c9-145">DeleteAttachment operation</span></span>](deleteattachment-operation.md)

