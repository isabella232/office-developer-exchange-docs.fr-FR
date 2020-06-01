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
description: L’opération GetAttachment est utilisée pour récupérer des pièces jointes existantes sur des éléments de la Banque d’Exchange.
ms.openlocfilehash: ac7eafd61c62b077a8d20e5fd8d004924bf06cf1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461288"
---
# <a name="getattachment-operation"></a><span data-ttu-id="4d690-103">Opération GetAttachment</span><span class="sxs-lookup"><span data-stu-id="4d690-103">GetAttachment operation</span></span>

<span data-ttu-id="4d690-104">L’opération GetAttachment est utilisée pour récupérer des pièces jointes existantes sur des éléments de la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="4d690-104">The GetAttachment operation is used to retrieve existing attachments on items in the Exchange store.</span></span>
  
## <a name="getattachment-request-example"></a><span data-ttu-id="4d690-105">Exemple de requête GetAttachment</span><span class="sxs-lookup"><span data-stu-id="4d690-105">GetAttachment request example</span></span>

### <a name="description"></a><span data-ttu-id="4d690-106">Description</span><span class="sxs-lookup"><span data-stu-id="4d690-106">Description</span></span>

<span data-ttu-id="4d690-107">L’exemple de requête GetAttachment suivant montre comment obtenir une pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="4d690-107">The following example of GetAttachment request shows how to get an attachment.</span></span>
  
### <a name="code"></a><span data-ttu-id="4d690-108">Code</span><span class="sxs-lookup"><span data-stu-id="4d690-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
xmlns:xsd="http://www.w3.org/2001/XMLSchema"
xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetAttachment xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <AttachmentShape/>
      <AttachmentIds>
        <t:AttachmentId Id="AAAtAEFkbWluaX..."/>
      </AttachmentIds>
    </GetAttachment>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="4d690-109">Commentaires</span><span class="sxs-lookup"><span data-stu-id="4d690-109">Comments</span></span>

<span data-ttu-id="4d690-110">L’élément [AttachmentShape](attachmentshape.md) vous permet de spécifier les informations de pièce jointe à renvoyer.</span><span class="sxs-lookup"><span data-stu-id="4d690-110">The [AttachmentShape](attachmentshape.md) element allows you to specify which attachment information should be returned.</span></span> <span data-ttu-id="4d690-111">Un élément [AttachmentShape](attachmentshape.md) vide est valide et affiche vos pièces jointes sans contenu MIME pour les pièces jointes d’éléments, avec un type de corps de texte et sans propriétés supplémentaires.</span><span class="sxs-lookup"><span data-stu-id="4d690-111">An empty [AttachmentShape](attachmentshape.md) element is valid and will render your attachments without MIME content for item attachments, with a text body type, and without any additional properties.</span></span> 
  
<span data-ttu-id="4d690-112">La collection [AttachmentIds](attachmentids.md) vous permet de spécifier un ou plusieurs identificateurs de pièce jointe à renvoyer.</span><span class="sxs-lookup"><span data-stu-id="4d690-112">The [AttachmentIds](attachmentids.md) collection allows you to specify one or more attachment identifiers to return.</span></span> <span data-ttu-id="4d690-113">Notez que ces éléments sont de type RequestAttachmentIdType, de sorte que les AttachmentIds que vous recevez de **CreateAttachment** doivent être supprimés des attributs **RootItemId** et **RootItemChangeKey** avant de les transmettre à **GetAttachment**.</span><span class="sxs-lookup"><span data-stu-id="4d690-113">Note that these are of type RequestAttachmentIdType, so any AttachmentIds that you receive from **CreateAttachment** must have the **RootItemId** and **RootItemChangeKey** attributes removed before passing them to **GetAttachment**.</span></span>
  
> [!NOTE]
> <span data-ttu-id="4d690-114">L’identificateur de pièce jointe et la clé de modification ont été raccourcies afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="4d690-114">The attachment identifier and change key have been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="4d690-115">Demander des éléments</span><span class="sxs-lookup"><span data-stu-id="4d690-115">Request elements</span></span>

<span data-ttu-id="4d690-116">Les éléments suivants sont utilisés dans la demande :</span><span class="sxs-lookup"><span data-stu-id="4d690-116">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="4d690-117">GetAttachment</span><span class="sxs-lookup"><span data-stu-id="4d690-117">GetAttachment</span></span>](getattachment.md)
    
- [<span data-ttu-id="4d690-118">AttachmentShape</span><span class="sxs-lookup"><span data-stu-id="4d690-118">AttachmentShape</span></span>](attachmentshape.md)
    
- [<span data-ttu-id="4d690-119">AttachmentIds</span><span class="sxs-lookup"><span data-stu-id="4d690-119">AttachmentIds</span></span>](attachmentids.md)
    
- [<span data-ttu-id="4d690-120">AttachmentId (GetAttachment et DeleteAttachment)</span><span class="sxs-lookup"><span data-stu-id="4d690-120">AttachmentId (GetAttachment and DeleteAttachment)</span></span>](attachmentid-getattachment-and-deleteattachment.md)
    
## <a name="getattachment-response-example"></a><span data-ttu-id="4d690-121">Exemple de réponse GetAttachment</span><span class="sxs-lookup"><span data-stu-id="4d690-121">GetAttachment response example</span></span>

### <a name="description"></a><span data-ttu-id="4d690-122">Description</span><span class="sxs-lookup"><span data-stu-id="4d690-122">Description</span></span>

<span data-ttu-id="4d690-123">L’exemple suivant montre une réponse réussie à une demande GetAttachment.</span><span class="sxs-lookup"><span data-stu-id="4d690-123">The following example shows a successful response to a GetAttachment request.</span></span> <span data-ttu-id="4d690-124">Cet exemple renvoie une pièce jointe de fichier.</span><span class="sxs-lookup"><span data-stu-id="4d690-124">This example returns a file attachment.</span></span>
  
### <a name="code"></a><span data-ttu-id="4d690-125">Code</span><span class="sxs-lookup"><span data-stu-id="4d690-125">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="662" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <GetAttachmentResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                           xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="4d690-126">Commentaires</span><span class="sxs-lookup"><span data-stu-id="4d690-126">Comments</span></span>

<span data-ttu-id="4d690-127">Les messages de réponse pour GetAttachment contiennent toujours la pièce jointe complète ; autrement dit, toutes les propriétés sont toujours incluses.</span><span class="sxs-lookup"><span data-stu-id="4d690-127">The response messages for GetAttachment will always contain the full attachment; that is, all properties will always be included.</span></span> <span data-ttu-id="4d690-128">Pour les pièces jointes, ces propriétés sont [Name (AttachmentType)](name-attachmenttype.md), [ContentType](contenttype.md), [contentid](contentid.md), [ContentLocation](contentlocation.md)et [content](content.md).</span><span class="sxs-lookup"><span data-stu-id="4d690-128">For file attachments, those properties are [Name (AttachmentType)](name-attachmenttype.md), [ContentType](contenttype.md), [ContentId](contentid.md), [ContentLocation](contentlocation.md), and [Content](content.md).</span></span> <span data-ttu-id="4d690-129">Pour les pièces jointes d’éléments, ces propriétés sont [Name (AttachmentType)](name-attachmenttype.md), [ContentType](contenttype.md), [contentid](contentid.md), [ContentLocation](contentlocation.md) et toutes les propriétés de l’élément, comme si la forme **AllProperties** avait été utilisée dans un appel de GetItem.</span><span class="sxs-lookup"><span data-stu-id="4d690-129">For item attachments, those properties are [Name (AttachmentType)](name-attachmenttype.md), [ContentType](contenttype.md), [ContentId](contentid.md), [ContentLocation](contentlocation.md) and all of the item's properties, as if the **AllProperties** shape had been used in a GetItem call.</span></span> <span data-ttu-id="4d690-130">L’élément [AttachmentShape](attachmentshape.md) , s’il est présent, permet à une application consommateur de demander des propriétés étendues supplémentaires pour les pièces jointes d’éléments.</span><span class="sxs-lookup"><span data-stu-id="4d690-130">The [AttachmentShape](attachmentshape.md) element, if present, will allow a consumer application to request additional extended properties for item attachments.</span></span> 
  
### <a name="successful-response-elements"></a><span data-ttu-id="4d690-131">Éléments de réponse réussis</span><span class="sxs-lookup"><span data-stu-id="4d690-131">Successful response elements</span></span>

<span data-ttu-id="4d690-132">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="4d690-132">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="4d690-133">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="4d690-133">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="4d690-134">GetAttachmentResponse</span><span class="sxs-lookup"><span data-stu-id="4d690-134">GetAttachmentResponse</span></span>](getattachmentresponse.md)
    
- [<span data-ttu-id="4d690-135">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="4d690-135">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="4d690-136">GetAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="4d690-136">GetAttachmentResponseMessage</span></span>](getattachmentresponsemessage.md)
    
- [<span data-ttu-id="4d690-137">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="4d690-137">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="4d690-138">Attachments</span><span class="sxs-lookup"><span data-stu-id="4d690-138">Attachments</span></span>](attachments-ex15websvcsotherref.md)
    
- [<span data-ttu-id="4d690-139">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="4d690-139">FileAttachment</span></span>](fileattachment.md)
    
- [<span data-ttu-id="4d690-140">AttachmentId (GetAttachment et DeleteAttachment)</span><span class="sxs-lookup"><span data-stu-id="4d690-140">AttachmentId (GetAttachment and DeleteAttachment)</span></span>](attachmentid-getattachment-and-deleteattachment.md)
    
- [<span data-ttu-id="4d690-141">Nom (AttachmentType)</span><span class="sxs-lookup"><span data-stu-id="4d690-141">Name (AttachmentType)</span></span>](name-attachmenttype.md)
    
- [<span data-ttu-id="4d690-142">Content</span><span class="sxs-lookup"><span data-stu-id="4d690-142">Content</span></span>](content.md)
    
## <a name="see-also"></a><span data-ttu-id="4d690-143">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4d690-143">See also</span></span>



[<span data-ttu-id="4d690-144">Opération CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="4d690-144">CreateAttachment operation</span></span>](createattachment-operation.md)
  
[<span data-ttu-id="4d690-145">Opération DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="4d690-145">DeleteAttachment operation</span></span>](deleteattachment-operation.md)

