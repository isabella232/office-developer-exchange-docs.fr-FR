---
title: Opération DeleteAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteAttachment
api_type:
- schema
ms.assetid: 4d48e595-b98c-48e7-bbeb-cacf91d12a78
description: L’opération DeleteAttachment est utilisée pour supprimer le fichier et élément de pièces jointes à partir d’un élément existant dans la banque d’informations Exchange.
ms.openlocfilehash: 4b94bfd8d6333c1f52be8ad7d0d111ab2a0552b3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755848"
---
# <a name="deleteattachment-operation"></a><span data-ttu-id="30e47-103">Opération DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="30e47-103">DeleteAttachment operation</span></span>

<span data-ttu-id="30e47-104">L’opération DeleteAttachment est utilisée pour supprimer le fichier et élément de pièces jointes à partir d’un élément existant dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="30e47-104">The DeleteAttachment operation is used to delete file and item attachments from an existing item in the Exchange store.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="30e47-105">Remarques</span><span class="sxs-lookup"><span data-stu-id="30e47-105">Remarks</span></span>

<span data-ttu-id="30e47-106">Cette opération vous permet de supprimer une ou plusieurs pièces jointes par ID.</span><span class="sxs-lookup"><span data-stu-id="30e47-106">This operation allows you to delete one or more attachments by ID.</span></span>
  
## <a name="deleteattachment-request-example"></a><span data-ttu-id="30e47-107">Exemple de requête DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="30e47-107">DeleteAttachment request example</span></span>

### <a name="description"></a><span data-ttu-id="30e47-108">Description</span><span class="sxs-lookup"><span data-stu-id="30e47-108">Description</span></span>

<span data-ttu-id="30e47-109">Une demande DeleteAttachment l’exemple suivant montre comment supprimer la pièce jointe d’un élément.</span><span class="sxs-lookup"><span data-stu-id="30e47-109">The following example of a DeleteAttachment request shows how to delete an item attachment.</span></span>
  
### <a name="code"></a><span data-ttu-id="30e47-110">Code</span><span class="sxs-lookup"><span data-stu-id="30e47-110">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <DeleteAttachment xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <AttachmentIds>
        <t:AttachmentId Id="AAAtAEFkbWluaX"/>
      </AttachmentIds>
    </DeleteAttachment>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="30e47-111">Commentaires</span><span class="sxs-lookup"><span data-stu-id="30e47-111">Comments</span></span>

<span data-ttu-id="30e47-112">Identificateur de pièce jointe a été raccourcie afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="30e47-112">The attachment identifier has been shortened to preserve readability.</span></span>
  
### <a name="request-elements"></a><span data-ttu-id="30e47-113">Éléments de la demande</span><span class="sxs-lookup"><span data-stu-id="30e47-113">Request elements</span></span>

<span data-ttu-id="30e47-114">Les éléments suivants sont utilisés dans la demande :</span><span class="sxs-lookup"><span data-stu-id="30e47-114">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="30e47-115">DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="30e47-115">DeleteAttachment</span></span>](deleteattachment.md)
    
- [<span data-ttu-id="30e47-116">AttachmentIds</span><span class="sxs-lookup"><span data-stu-id="30e47-116">AttachmentIds</span></span>](attachmentids.md)
    
- [<span data-ttu-id="30e47-117">AttachmentId</span><span class="sxs-lookup"><span data-stu-id="30e47-117">AttachmentId</span></span>](attachmentid.md)
    
## <a name="deleteattachment-response-example"></a><span data-ttu-id="30e47-118">Exemple de réponse DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="30e47-118">DeleteAttachment response example</span></span>

### <a name="description"></a><span data-ttu-id="30e47-119">Description</span><span class="sxs-lookup"><span data-stu-id="30e47-119">Description</span></span>

<span data-ttu-id="30e47-120">L’exemple suivant montre une réponse positive à une demande DeleteAttachment.</span><span class="sxs-lookup"><span data-stu-id="30e47-120">The following example shows a successful response to a DeleteAttachment request.</span></span>
  
### <a name="code"></a><span data-ttu-id="30e47-121">Code</span><span class="sxs-lookup"><span data-stu-id="30e47-121">Code</span></span>

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
    <DeleteAttachmentResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                              xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                              xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:DeleteAttachmentResponseMessage xsi:type="m:DeleteAttachmentResponseMessageType" ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootItemId RootItemId="AAAtAEFkbWluaXN..." RootItemChangeKey="CQAAABYAA..."/>
        </m:DeleteAttachmentResponseMessage>
      </m:ResponseMessages>
    </DeleteAttachmentResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="30e47-122">Commentaires</span><span class="sxs-lookup"><span data-stu-id="30e47-122">Comments</span></span>

<span data-ttu-id="30e47-123">L’opération CreateAttachment renvoie un élément de type AttachmentIdType qui inclut un **RootItemId** et le **RootItemChangeKey**.</span><span class="sxs-lookup"><span data-stu-id="30e47-123">The CreateAttachment operation returns an element of AttachmentIdType type that includes a **RootItemId** and **RootItemChangeKey**.</span></span> <span data-ttu-id="30e47-124">Ces attributs ne sont pas autorisés pour les identificateurs dans une demande DeleteAttachment.</span><span class="sxs-lookup"><span data-stu-id="30e47-124">These attributes are not permitted for identifiers within a DeleteAttachment request.</span></span> <span data-ttu-id="30e47-125">DeleteAttachment utilise des éléments de type RequestAttachmentIdType, qui n’inclut pas ces attributs.</span><span class="sxs-lookup"><span data-stu-id="30e47-125">DeleteAttachment uses elements of type RequestAttachmentIdType, which does not include these attributes.</span></span>
  
<span data-ttu-id="30e47-126">La réponse DeleteAttachment inclut l’ID de l’élément parent.</span><span class="sxs-lookup"><span data-stu-id="30e47-126">The DeleteAttachment response includes the ID of the parent item.</span></span> <span data-ttu-id="30e47-127">Lorsque les pièces jointes sont supprimés d’un élément, modifier la clé de l’élément est modifiée.</span><span class="sxs-lookup"><span data-stu-id="30e47-127">When attachments are removed from an item, the item's change key is modified.</span></span> <span data-ttu-id="30e47-128">La nouvelle clé de modification d’élément peut être obtenue à partir de la réponse DeleteAttachment.</span><span class="sxs-lookup"><span data-stu-id="30e47-128">The new item change key can be obtained from the DeleteAttachment response.</span></span>
  
> [!NOTE]
> <span data-ttu-id="30e47-129">L’identificateur [RootItemId](rootitemid.md) et ChangeKey ont été réduite afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="30e47-129">The [RootItemId](rootitemid.md) identifier and ChangeKey have been shortened to preserve readability.</span></span> 
  
### <a name="successful-response-elements"></a><span data-ttu-id="30e47-130">Éléments de réponse réussie</span><span class="sxs-lookup"><span data-stu-id="30e47-130">Successful response elements</span></span>

<span data-ttu-id="30e47-131">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="30e47-131">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="30e47-132">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="30e47-132">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="30e47-133">DeleteAttachmentResponse</span><span class="sxs-lookup"><span data-stu-id="30e47-133">DeleteAttachmentResponse</span></span>](deleteattachmentresponse.md)
    
- [<span data-ttu-id="30e47-134">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="30e47-134">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="30e47-135">DeleteAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="30e47-135">DeleteAttachmentResponseMessage</span></span>](deleteattachmentresponsemessage.md)
    
- [<span data-ttu-id="30e47-136">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="30e47-136">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="30e47-137">RootItemId</span><span class="sxs-lookup"><span data-stu-id="30e47-137">RootItemId</span></span>](rootitemid.md)
    
## <a name="see-also"></a><span data-ttu-id="30e47-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="30e47-138">See also</span></span>

- [<span data-ttu-id="30e47-139">Opération CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="30e47-139">CreateAttachment operation</span></span>](createattachment-operation.md) 
- [<span data-ttu-id="30e47-140">Opération GetAttachment</span><span class="sxs-lookup"><span data-stu-id="30e47-140">GetAttachment operation</span></span>](getattachment-operation.md)

