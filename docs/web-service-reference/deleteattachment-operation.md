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
description: L’opération DeleteAttachment est utilisée pour supprimer les pièces jointes d’un fichier et d’un élément d’un élément existant dans la Banque d’Exchange.
ms.openlocfilehash: 1d34ce4c5ba1d955989a35dafb8ab3c5d229d505
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457332"
---
# <a name="deleteattachment-operation"></a><span data-ttu-id="1b29b-103">Opération DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="1b29b-103">DeleteAttachment operation</span></span>

<span data-ttu-id="1b29b-104">L’opération DeleteAttachment est utilisée pour supprimer les pièces jointes d’un fichier et d’un élément d’un élément existant dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="1b29b-104">The DeleteAttachment operation is used to delete file and item attachments from an existing item in the Exchange store.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1b29b-105">Remarques</span><span class="sxs-lookup"><span data-stu-id="1b29b-105">Remarks</span></span>

<span data-ttu-id="1b29b-106">Cette opération vous permet de supprimer une ou plusieurs pièces jointes par ID.</span><span class="sxs-lookup"><span data-stu-id="1b29b-106">This operation allows you to delete one or more attachments by ID.</span></span>
  
## <a name="deleteattachment-request-example"></a><span data-ttu-id="1b29b-107">Exemple de requête DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="1b29b-107">DeleteAttachment request example</span></span>

### <a name="description"></a><span data-ttu-id="1b29b-108">Description</span><span class="sxs-lookup"><span data-stu-id="1b29b-108">Description</span></span>

<span data-ttu-id="1b29b-109">L’exemple de requête DeleteAttachment suivant montre comment supprimer une pièce jointe d’un élément.</span><span class="sxs-lookup"><span data-stu-id="1b29b-109">The following example of a DeleteAttachment request shows how to delete an item attachment.</span></span>
  
### <a name="code"></a><span data-ttu-id="1b29b-110">Code</span><span class="sxs-lookup"><span data-stu-id="1b29b-110">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <DeleteAttachment xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <AttachmentIds>
        <t:AttachmentId Id="AAAtAEFkbWluaX"/>
      </AttachmentIds>
    </DeleteAttachment>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="1b29b-111">Commentaires</span><span class="sxs-lookup"><span data-stu-id="1b29b-111">Comments</span></span>

<span data-ttu-id="1b29b-112">L’identificateur de pièce jointe a été raccourcie afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="1b29b-112">The attachment identifier has been shortened to preserve readability.</span></span>
  
### <a name="request-elements"></a><span data-ttu-id="1b29b-113">Demander des éléments</span><span class="sxs-lookup"><span data-stu-id="1b29b-113">Request elements</span></span>

<span data-ttu-id="1b29b-114">Les éléments suivants sont utilisés dans la demande :</span><span class="sxs-lookup"><span data-stu-id="1b29b-114">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="1b29b-115">DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="1b29b-115">DeleteAttachment</span></span>](deleteattachment.md)
    
- [<span data-ttu-id="1b29b-116">AttachmentIds</span><span class="sxs-lookup"><span data-stu-id="1b29b-116">AttachmentIds</span></span>](attachmentids.md)
    
- [<span data-ttu-id="1b29b-117">AttachmentId</span><span class="sxs-lookup"><span data-stu-id="1b29b-117">AttachmentId</span></span>](attachmentid.md)
    
## <a name="deleteattachment-response-example"></a><span data-ttu-id="1b29b-118">Exemple de réponse DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="1b29b-118">DeleteAttachment response example</span></span>

### <a name="description"></a><span data-ttu-id="1b29b-119">Description</span><span class="sxs-lookup"><span data-stu-id="1b29b-119">Description</span></span>

<span data-ttu-id="1b29b-120">L’exemple suivant montre une réponse réussie à une demande DeleteAttachment.</span><span class="sxs-lookup"><span data-stu-id="1b29b-120">The following example shows a successful response to a DeleteAttachment request.</span></span>
  
### <a name="code"></a><span data-ttu-id="1b29b-121">Code</span><span class="sxs-lookup"><span data-stu-id="1b29b-121">Code</span></span>

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
    <DeleteAttachmentResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                              xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                              xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="1b29b-122">Commentaires</span><span class="sxs-lookup"><span data-stu-id="1b29b-122">Comments</span></span>

<span data-ttu-id="1b29b-123">L’opération CreateAttachment renvoie un élément de type AttachmentIdType qui inclut un **RootItemId** et **RootItemChangeKey**.</span><span class="sxs-lookup"><span data-stu-id="1b29b-123">The CreateAttachment operation returns an element of AttachmentIdType type that includes a **RootItemId** and **RootItemChangeKey**.</span></span> <span data-ttu-id="1b29b-124">Ces attributs ne sont pas autorisés pour les identificateurs dans une demande DeleteAttachment.</span><span class="sxs-lookup"><span data-stu-id="1b29b-124">These attributes are not permitted for identifiers within a DeleteAttachment request.</span></span> <span data-ttu-id="1b29b-125">DeleteAttachment utilise des éléments de type RequestAttachmentIdType, qui n’incluent pas ces attributs.</span><span class="sxs-lookup"><span data-stu-id="1b29b-125">DeleteAttachment uses elements of type RequestAttachmentIdType, which does not include these attributes.</span></span>
  
<span data-ttu-id="1b29b-126">La réponse DeleteAttachment inclut l’ID de l’élément parent.</span><span class="sxs-lookup"><span data-stu-id="1b29b-126">The DeleteAttachment response includes the ID of the parent item.</span></span> <span data-ttu-id="1b29b-127">Lorsque des pièces jointes sont supprimées d’un élément, la clé de modification de l’élément est modifiée.</span><span class="sxs-lookup"><span data-stu-id="1b29b-127">When attachments are removed from an item, the item's change key is modified.</span></span> <span data-ttu-id="1b29b-128">La nouvelle clé de modification d’élément peut être obtenue à partir de la réponse DeleteAttachment.</span><span class="sxs-lookup"><span data-stu-id="1b29b-128">The new item change key can be obtained from the DeleteAttachment response.</span></span>
  
> [!NOTE]
> <span data-ttu-id="1b29b-129">L’identificateur [RootItemId](rootitemid.md) et ChangeKey ont été raccourcies afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="1b29b-129">The [RootItemId](rootitemid.md) identifier and ChangeKey have been shortened to preserve readability.</span></span> 
  
### <a name="successful-response-elements"></a><span data-ttu-id="1b29b-130">Éléments de réponse réussis</span><span class="sxs-lookup"><span data-stu-id="1b29b-130">Successful response elements</span></span>

<span data-ttu-id="1b29b-131">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="1b29b-131">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="1b29b-132">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="1b29b-132">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="1b29b-133">DeleteAttachmentResponse</span><span class="sxs-lookup"><span data-stu-id="1b29b-133">DeleteAttachmentResponse</span></span>](deleteattachmentresponse.md)
    
- [<span data-ttu-id="1b29b-134">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="1b29b-134">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="1b29b-135">DeleteAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="1b29b-135">DeleteAttachmentResponseMessage</span></span>](deleteattachmentresponsemessage.md)
    
- [<span data-ttu-id="1b29b-136">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="1b29b-136">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="1b29b-137">RootItemId</span><span class="sxs-lookup"><span data-stu-id="1b29b-137">RootItemId</span></span>](rootitemid.md)
    
## <a name="see-also"></a><span data-ttu-id="1b29b-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1b29b-138">See also</span></span>

- [<span data-ttu-id="1b29b-139">Opération CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="1b29b-139">CreateAttachment operation</span></span>](createattachment-operation.md) 
- [<span data-ttu-id="1b29b-140">Opération GetAttachment</span><span class="sxs-lookup"><span data-stu-id="1b29b-140">GetAttachment operation</span></span>](getattachment-operation.md)

