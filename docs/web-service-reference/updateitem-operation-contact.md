---
title: Opération UpdateItem (contacts)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateItem
api_type:
- schema
ms.assetid: 298fdd71-a83d-4407-9728-4f0a8e2d857c
description: L'opération UpdateItem sert à mettre à jour les propriétés de l'élément de contact dans la banque d'informations Exchange.
ms.openlocfilehash: 66e1b91ea3154d8a501339aed7b398970e8f5392
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459825"
---
# <a name="updateitem-operation-contact"></a><span data-ttu-id="41dd9-103">Opération UpdateItem (contacts)</span><span class="sxs-lookup"><span data-stu-id="41dd9-103">UpdateItem operation (contact)</span></span>

<span data-ttu-id="41dd9-104">L'opération UpdateItem sert à mettre à jour les propriétés de l'élément de contact dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="41dd9-104">The UpdateItem operation is used to update contact item properties in the Exchange store.</span></span>
  
## <a name="updateitem-contact-request-example"></a><span data-ttu-id="41dd9-105">Exemple de requête UpdateItem (contact)</span><span class="sxs-lookup"><span data-stu-id="41dd9-105">UpdateItem (Contact) request example</span></span>

### <a name="description"></a><span data-ttu-id="41dd9-106">Description</span><span class="sxs-lookup"><span data-stu-id="41dd9-106">Description</span></span>

<span data-ttu-id="41dd9-107">L'exemple de code suivant montre comment mettre à jour l'adresse de messagerie d'un contact.</span><span class="sxs-lookup"><span data-stu-id="41dd9-107">The following code example shows how to update the e-mail address of a contact.</span></span>
  
### <a name="code"></a><span data-ttu-id="41dd9-108">Code</span><span class="sxs-lookup"><span data-stu-id="41dd9-108">Code</span></span>

```XML
<soap:Envelope
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
 xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                ConflictResolution="AlwaysOverwrite">
      <ItemChanges>
        <t:ItemChange>
          <t:ItemId Id="AAAtAA=" ChangeKey="EQAAABYi" />
          <t:Updates>
            <t:SetItemField>
              <t:IndexedFieldURI FieldURI="contacts:EmailAddress" FieldIndex="EmailAddress1"/>
              <t:Contact>
                <t:EmailAddresses>
                  <t:Entry Key="EmailAddress1">changedemail@example.com</t:Entry>
                </t:EmailAddresses>
              </t:Contact>
            </t:SetItemField>
          </t:Updates>
        </t:ItemChange>
      </ItemChanges>
    </UpdateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="41dd9-109">Commentaires</span><span class="sxs-lookup"><span data-stu-id="41dd9-109">Comments</span></span>

<span data-ttu-id="41dd9-110">Identificateur de l'élément a été raccourcie afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="41dd9-110">The item identifier has been shortened to preserve readability.</span></span>
  
### <a name="request-elements"></a><span data-ttu-id="41dd9-111">Demander des éléments</span><span class="sxs-lookup"><span data-stu-id="41dd9-111">Request elements</span></span>

<span data-ttu-id="41dd9-112">Les éléments suivants sont utilisés dans la demande :</span><span class="sxs-lookup"><span data-stu-id="41dd9-112">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="41dd9-113">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="41dd9-113">UpdateItem</span></span>](updateitem.md)
    
- [<span data-ttu-id="41dd9-114">ItemChanges</span><span class="sxs-lookup"><span data-stu-id="41dd9-114">ItemChanges</span></span>](itemchanges.md)
    
- [<span data-ttu-id="41dd9-115">ItemChange</span><span class="sxs-lookup"><span data-stu-id="41dd9-115">ItemChange</span></span>](itemchange.md)
    
- [<span data-ttu-id="41dd9-116">ItemId</span><span class="sxs-lookup"><span data-stu-id="41dd9-116">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="41dd9-117">Mises à jour (élément)</span><span class="sxs-lookup"><span data-stu-id="41dd9-117">Updates (Item)</span></span>](updates-item.md)
    
- [<span data-ttu-id="41dd9-118">SetItemField</span><span class="sxs-lookup"><span data-stu-id="41dd9-118">SetItemField</span></span>](setitemfield.md)
    
- [<span data-ttu-id="41dd9-119">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="41dd9-119">IndexedFieldURI</span></span>](indexedfielduri.md)
    
- [<span data-ttu-id="41dd9-120">Contact</span><span class="sxs-lookup"><span data-stu-id="41dd9-120">Contact</span></span>](contact.md)
    
- [<span data-ttu-id="41dd9-121">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="41dd9-121">EmailAddresses</span></span>](emailaddresses.md)
    
- [<span data-ttu-id="41dd9-122">Entrée (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="41dd9-122">Entry (EmailAddress)</span></span>](entry-emailaddress.md)
    
## <a name="successful-updateitem-contact-response"></a><span data-ttu-id="41dd9-123">Réponse de réussite UpdateItem (contacts)</span><span class="sxs-lookup"><span data-stu-id="41dd9-123">Successful UpdateItem (Contact) Response</span></span>

### <a name="description"></a><span data-ttu-id="41dd9-124">Description</span><span class="sxs-lookup"><span data-stu-id="41dd9-124">Description</span></span>

<span data-ttu-id="41dd9-125">L'exemple de code suivant montre une réponse UpdateItem réussie.</span><span class="sxs-lookup"><span data-stu-id="41dd9-125">The following code example shows a successful UpdateItem response.</span></span>
  
### <a name="code"></a><span data-ttu-id="41dd9-126">Code</span><span class="sxs-lookup"><span data-stu-id="41dd9-126">Code</span></span>

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
    <UpdateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:UpdateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Contact>
              <t:ItemId Id="AAAtAE=" ChangeKey="EQAAABYx" />
            </t:Contact>
          </m:Items>
        </m:UpdateItemResponseMessage>
      </m:ResponseMessages>
    </UpdateItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="41dd9-127">Commentaires</span><span class="sxs-lookup"><span data-stu-id="41dd9-127">Comments</span></span>

<span data-ttu-id="41dd9-128">Identificateur de l'élément a été raccourcie afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="41dd9-128">The item identifier has been shortened to preserve readability.</span></span>
  
### <a name="successful-response-elements"></a><span data-ttu-id="41dd9-129">Éléments de réponse réussis</span><span class="sxs-lookup"><span data-stu-id="41dd9-129">Successful response elements</span></span>

<span data-ttu-id="41dd9-130">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="41dd9-130">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="41dd9-131">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="41dd9-131">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="41dd9-132">UpdateItemResponse</span><span class="sxs-lookup"><span data-stu-id="41dd9-132">UpdateItemResponse</span></span>](updateitemresponse.md)
    
- [<span data-ttu-id="41dd9-133">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="41dd9-133">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="41dd9-134">UpdateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="41dd9-134">UpdateItemResponseMessage</span></span>](updateitemresponsemessage.md)
    
- [<span data-ttu-id="41dd9-135">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="41dd9-135">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="41dd9-136">Éléments (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="41dd9-136">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md)
    
- [<span data-ttu-id="41dd9-137">Contact</span><span class="sxs-lookup"><span data-stu-id="41dd9-137">Contact</span></span>](contact.md)
    
- [<span data-ttu-id="41dd9-138">ItemId</span><span class="sxs-lookup"><span data-stu-id="41dd9-138">ItemId</span></span>](itemid.md)
    
## <a name="invalid-updateitem-contact-request-example"></a><span data-ttu-id="41dd9-139">Exemple de requête UpdateItem (contact) non valide</span><span class="sxs-lookup"><span data-stu-id="41dd9-139">Invalid UpdateItem (Contact) request example</span></span>

### <a name="description"></a><span data-ttu-id="41dd9-140">Description</span><span class="sxs-lookup"><span data-stu-id="41dd9-140">Description</span></span>

<span data-ttu-id="41dd9-141">L'exemple de code suivant illustre une demande non valide.</span><span class="sxs-lookup"><span data-stu-id="41dd9-141">The following code example shows an invalid request.</span></span>
  
### <a name="code"></a><span data-ttu-id="41dd9-142">Code</span><span class="sxs-lookup"><span data-stu-id="41dd9-142">Code</span></span>

```XML
<soap:Envelope
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
 xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                ConflictResolution="AlwaysOverwrite">
      <ItemChanges>
        <t:ItemChange>
          <t:ItemId Id="AAAtAEF=" ChangeKey="EQAAABYi" />
          <t:Updates>
            <t:SetItemField>
              <t:IndexedFieldURI FieldURI="contacts:EmailAddress" FieldIndex="EmailAddress4"/>
              <t:Contact>
                <t:EmailAddresses>
                  <t:Entry Key="EmailAddress4">changedemail2@example.com</t:Entry>
                </t:EmailAddresses>
              </t:Contact>
            </t:SetItemField>
          </t:Updates>
        </t:ItemChange>
      </ItemChanges>
    </UpdateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="41dd9-143">Commentaires</span><span class="sxs-lookup"><span data-stu-id="41dd9-143">Comments</span></span>

<span data-ttu-id="41dd9-144">Identificateur de l'élément a été raccourcie afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="41dd9-144">The item identifier has been shortened to preserve readability.</span></span>
  
## <a name="updateitem-contact-error-response"></a><span data-ttu-id="41dd9-145">Réponse d’erreur UpdateItem (contact)</span><span class="sxs-lookup"><span data-stu-id="41dd9-145">UpdateItem (Contact) error response</span></span>

### <a name="description"></a><span data-ttu-id="41dd9-146">Description</span><span class="sxs-lookup"><span data-stu-id="41dd9-146">Description</span></span>

<span data-ttu-id="41dd9-147">L'exemple de code suivant montre une réponse d'erreur à une demande de UpdateItem (contacts).</span><span class="sxs-lookup"><span data-stu-id="41dd9-147">The following code example shows an error response to an UpdateItem (Contact) request.</span></span>
  
### <a name="code"></a><span data-ttu-id="41dd9-148">Code</span><span class="sxs-lookup"><span data-stu-id="41dd9-148">Code</span></span>

```XML
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="602" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <soap:Fault>
      <soap:faultcode>Client</soap:faultcode>
      <soap:faultstring>The request failed schema validation.</soap:faultstring>
      <detail>
        <e:ResponseCode xmlns:e="https://schemas.microsoft.com/exchange/services/2006/errors">ErrorSchemaValidation</e:ResponseCode>
        <e:Message xmlns:e="https://schemas.microsoft.com/exchange/services/2006/errors">The 'Key' attribute is invalid - The value 'EmailAddress4' is invalid according to its data type 'https://schemas.microsoft.com/exchange/services/2006/types:EmailAddressKeyType' - The Enumeration constraint failed.</e:Message>
        <e:Line xmlns:e="https://schemas.microsoft.com/exchange/services/2006/errors">17</e:Line>
        <e:Position xmlns:e="https://schemas.microsoft.com/exchange/services/2006/errors">19</e:Position>
      </detail>
    </soap:Fault>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="41dd9-149">Commentaires</span><span class="sxs-lookup"><span data-stu-id="41dd9-149">Comments</span></span>

<span data-ttu-id="41dd9-p101">Certains éléments qui sont utilisés dans le corps SOAP d'une réponse d'erreur est dû à une erreur de validation de schéma ne sont pas définis dans les schémas de types ou de messages. L'élément **detail** contient des informations sur l'erreur. L'élément [ResponseCode](responsecode.md) contient le code d'erreur. L'élément [Message](message-ex15websvcsotherref.md) contient une explication de l'erreur, si elle est disponible. L'élément **Line** décrit le numéro de ligne où l'erreur de validation de schéma s'est produite. L'élément **Position** décrit la position à partir du caractère à l'extrême gauche du document XML.</span><span class="sxs-lookup"><span data-stu-id="41dd9-p101">Some elements that are used in the SOAP body of an error response that is caused by a schema validation error are not defined in the messages or types schemas. The **detail** element contains information about the error. The [ResponseCode](responsecode.md) element contains the error code. The [Message](message-ex15websvcsotherref.md) element contains an explanation for the error, if one is available. The **Line** element describes the line number where the schema validation error occurred. The **Position** element describes the position from the leftmost character of the XML document.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="41dd9-156">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="41dd9-156">See also</span></span>



[<span data-ttu-id="41dd9-157">UpdateItem Operation</span><span class="sxs-lookup"><span data-stu-id="41dd9-157">UpdateItem operation</span></span>](updateitem-operation.md)

