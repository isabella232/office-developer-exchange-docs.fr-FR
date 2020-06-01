---
title: Opération de GetItem (contacts)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetItem
api_type:
- schema
ms.assetid: 6b96dace-1260-4b83-869a-7c31c5583daa
description: L'opération GetItem est utilisée pour obtenir des éléments de contact à partir de la banque d'informations Exchange.
ms.openlocfilehash: 93e8dbe28e130ab64d4b8d12d2befde1f77ae8fa
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460021"
---
# <a name="getitem-operation-contact"></a><span data-ttu-id="f5355-103">Opération de GetItem (contacts)</span><span class="sxs-lookup"><span data-stu-id="f5355-103">GetItem operation (contact)</span></span>

<span data-ttu-id="f5355-104">L'opération GetItem est utilisée pour obtenir des éléments de contact à partir de la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="f5355-104">The GetItem operation is used to get contact items from the Exchange store.</span></span>
  
## <a name="getitem-contact-request-example"></a><span data-ttu-id="f5355-105">Exemple de requête GetItem (contact)</span><span class="sxs-lookup"><span data-stu-id="f5355-105">GetItem (Contact) request example</span></span>

### <a name="description"></a><span data-ttu-id="f5355-106">Description</span><span class="sxs-lookup"><span data-stu-id="f5355-106">Description</span></span>

<span data-ttu-id="f5355-107">L'exemple suivant montre comment obtenir un élément à partir de la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="f5355-107">The following example shows how to get an item from the Exchange store.</span></span>
  
### <a name="code"></a><span data-ttu-id="f5355-108">Code</span><span class="sxs-lookup"><span data-stu-id="f5355-108">Code</span></span>

```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetItem xmlns='https://schemas.microsoft.com/exchange/services/2006/messages'>
      <ItemShape>
        <t:BaseShape>AllProperties</t:BaseShape>
      </ItemShape>
      <ItemIds>
        <t:ItemId Id="AAAtAE=" ChangeKey="EQAAABY" />
      </ItemIds>
    </GetItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="f5355-109">Commentaires</span><span class="sxs-lookup"><span data-stu-id="f5355-109">Comments</span></span>

<span data-ttu-id="f5355-p101">La demande pour obtenir un élément à partir de la banque d'informations Exchange prend la même forme pour tous les types d'élément. Les réponses aux demandes de différents éléments sera différents, car les différents éléments renvoient des informations différentes selon les formes de la réponse.</span><span class="sxs-lookup"><span data-stu-id="f5355-p101">The request to get an item from the Exchange store takes the same form for all item types. The responses to requests for different items will be different because different items return different information based on the response shapes.</span></span>
  
> [!NOTE]
> <span data-ttu-id="f5355-112">[!REMARQUE] Identificateur de l'élément a été raccourcie afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="f5355-112">The item identifier has been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="f5355-113">Demander des éléments</span><span class="sxs-lookup"><span data-stu-id="f5355-113">Request elements</span></span>

<span data-ttu-id="f5355-114">Les éléments suivants sont utilisés dans la demande :</span><span class="sxs-lookup"><span data-stu-id="f5355-114">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="f5355-115">GetItem</span><span class="sxs-lookup"><span data-stu-id="f5355-115">GetItem</span></span>](getitem.md)
    
- [<span data-ttu-id="f5355-116">ItemShape</span><span class="sxs-lookup"><span data-stu-id="f5355-116">ItemShape</span></span>](itemshape.md)
    
- [<span data-ttu-id="f5355-117">BaseShape</span><span class="sxs-lookup"><span data-stu-id="f5355-117">BaseShape</span></span>](baseshape.md)
    
- [<span data-ttu-id="f5355-118">ItemIds</span><span class="sxs-lookup"><span data-stu-id="f5355-118">ItemIds</span></span>](itemids.md)
    
- [<span data-ttu-id="f5355-119">ItemId</span><span class="sxs-lookup"><span data-stu-id="f5355-119">ItemId</span></span>](itemid.md)
    
## <a name="successful-getitem-contact-response"></a><span data-ttu-id="f5355-120">Réponse de réussite GetItem (contacts)</span><span class="sxs-lookup"><span data-stu-id="f5355-120">Successful GetItem (Contact) Response</span></span>

### <a name="description"></a><span data-ttu-id="f5355-121">Description</span><span class="sxs-lookup"><span data-stu-id="f5355-121">Description</span></span>

<span data-ttu-id="f5355-122">L'exemple de code suivant montre une réponse positive de GetItem pour l' **AllProperties**[BaseShape](baseshape.md).</span><span class="sxs-lookup"><span data-stu-id="f5355-122">The following code example shows a successful GetItem response for the **AllProperties**[BaseShape](baseshape.md).</span></span>
  
### <a name="code"></a><span data-ttu-id="f5355-123">Code</span><span class="sxs-lookup"><span data-stu-id="f5355-123">Code</span></span>

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
    <GetItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                     xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                     xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Contact>
              <t:ItemId Id="AAAtAEA=" ChangeKey="EQAAABYq" />
              <t:ParentFolderId Id="AQAtAEFk==" ChangeKey="AQAAAA==" />
              <t:ItemClass>IPM.Contact</t:ItemClass>
              <t:Sensitivity>Normal</t:Sensitivity>
              <t:Body BodyType="Text" />
              <t:DateTimeReceived>2006-08-18T17:31:18Z</t:DateTimeReceived>
              <t:Size>382</t:Size>
              <t:Importance>Normal</t:Importance>
              <t:IsSubmitted>false</t:IsSubmitted>
              <t:IsDraft>true</t:IsDraft>
              <t:IsFromMe>false</t:IsFromMe>
              <t:IsResend>false</t:IsResend>
              <t:IsUnmodified>false</t:IsUnmodified>
              <t:DateTimeSent>2006-08-18T17:31:18Z</t:DateTimeSent>
              <t:DateTimeCreated>2006-08-18T17:31:18Z</t:DateTimeCreated>
              <t:HasAttachments>false</t:HasAttachments>
              <t:Culture>en</t:Culture>
              <t:FileAs>SampleContact</t:FileAs>
              <t:FileAsMapping>None</t:FileAsMapping>
              <t:DisplayName>Tanja Plate</t:DisplayName>
              <t:GivenName>Tanja</t:GivenName>
              <t:Initials>T.P.</t:Initials>
              <t:CompleteName>
                <t:FirstName>Tanja</t:FirstName>
                <t:LastName>Plate</t:LastName>
                <t:Initials>T.P.</t:Initials>
                <t:FullName>Tanja Plate</t:FullName>
              </t:CompleteName>
              <t:CompanyName>Northwind Traders</t:CompanyName>
              <t:EmailAddresses>
                <t:Entry Key="EmailAddress1">tplate@example.com</t:Entry>
                <t:Entry Key="EmailAddress2">tplate@example.com</t:Entry>
              </t:EmailAddresses>
              <t:PhysicalAddresses>
                <t:Entry Key="Business">
                  <t:Street>12345 67th Ave</t:Street>
                  <t:City>Whittier</t:City>
                  <t:State>CA</t:State>
                  <t:Country>USA</t:Country>
                </t:Entry>
              </t:PhysicalAddresses>
              <t:PhoneNumbers>
                <t:Entry Key="BusinessPhone">5625550199</t:Entry>
              </t:PhoneNumbers>
              <t:JobTitle>Project Manager</t:JobTitle>
              <t:Surname>Plate</t:Surname>
            </t:Contact>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </GetItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="f5355-124">Commentaires</span><span class="sxs-lookup"><span data-stu-id="f5355-124">Comments</span></span>

<span data-ttu-id="f5355-125">Identificateur de l'élément a été raccourcie afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="f5355-125">The item identifier has been shortened to preserve readability.</span></span>
  
### <a name="successful-response-elements"></a><span data-ttu-id="f5355-126">Éléments de réponse réussis</span><span class="sxs-lookup"><span data-stu-id="f5355-126">Successful response elements</span></span>

<span data-ttu-id="f5355-127">Les éléments suivants sont utilisés dans la réponse à une demande de GetItem avec une forme de réponse de **AllProperties** pour un élément de contact.</span><span class="sxs-lookup"><span data-stu-id="f5355-127">The following elements are used in the response for a GetItem request with a response shape of **AllProperties** for a contact item.</span></span> 
  
- [<span data-ttu-id="f5355-128">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="f5355-128">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="f5355-129">GetItemResponse</span><span class="sxs-lookup"><span data-stu-id="f5355-129">GetItemResponse</span></span>](getitemresponse.md)
    
- [<span data-ttu-id="f5355-130">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="f5355-130">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="f5355-131">GetItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="f5355-131">GetItemResponseMessage</span></span>](getitemresponsemessage.md)
    
- [<span data-ttu-id="f5355-132">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="f5355-132">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="f5355-133">Items</span><span class="sxs-lookup"><span data-stu-id="f5355-133">Items</span></span>](items.md)
    
- [<span data-ttu-id="f5355-134">Contact</span><span class="sxs-lookup"><span data-stu-id="f5355-134">Contact</span></span>](contact.md)
    
- [<span data-ttu-id="f5355-135">ItemId</span><span class="sxs-lookup"><span data-stu-id="f5355-135">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="f5355-136">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="f5355-136">ParentFolderId</span></span>](parentfolderid.md)
    
- [<span data-ttu-id="f5355-137">ItemClass</span><span class="sxs-lookup"><span data-stu-id="f5355-137">ItemClass</span></span>](itemclass.md)
    
- [<span data-ttu-id="f5355-138">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="f5355-138">Sensitivity</span></span>](sensitivity.md)
    
- [<span data-ttu-id="f5355-139">Corps</span><span class="sxs-lookup"><span data-stu-id="f5355-139">Body</span></span>](body.md)
    
- [<span data-ttu-id="f5355-140">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="f5355-140">DateTimeReceived</span></span>](datetimereceived.md)
    
- [<span data-ttu-id="f5355-141">Taille</span><span class="sxs-lookup"><span data-stu-id="f5355-141">Size</span></span>](size.md)
    
- [<span data-ttu-id="f5355-142">Importance</span><span class="sxs-lookup"><span data-stu-id="f5355-142">Importance</span></span>](importance.md)
    
- [<span data-ttu-id="f5355-143">IsSubmitted</span><span class="sxs-lookup"><span data-stu-id="f5355-143">IsSubmitted</span></span>](issubmitted.md)
    
- [<span data-ttu-id="f5355-144">IsDraft</span><span class="sxs-lookup"><span data-stu-id="f5355-144">IsDraft</span></span>](isdraft.md)
    
- [<span data-ttu-id="f5355-145">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="f5355-145">IsFromMe</span></span>](isfromme.md)
    
- [<span data-ttu-id="f5355-146">IsResend</span><span class="sxs-lookup"><span data-stu-id="f5355-146">IsResend</span></span>](isresend.md)
    
- [<span data-ttu-id="f5355-147">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="f5355-147">IsUnmodified</span></span>](isunmodified.md)
    
- [<span data-ttu-id="f5355-148">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="f5355-148">DateTimeSent</span></span>](datetimesent.md)
    
- [<span data-ttu-id="f5355-149">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="f5355-149">DateTimeCreated</span></span>](datetimecreated.md)
    
- [<span data-ttu-id="f5355-150">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="f5355-150">HasAttachments</span></span>](hasattachments.md)
    
- [<span data-ttu-id="f5355-151">Culture</span><span class="sxs-lookup"><span data-stu-id="f5355-151">Culture</span></span>](culture.md)
    
- [<span data-ttu-id="f5355-152">FileAs</span><span class="sxs-lookup"><span data-stu-id="f5355-152">FileAs</span></span>](fileas.md)
    
- [<span data-ttu-id="f5355-153">FileAsMapping</span><span class="sxs-lookup"><span data-stu-id="f5355-153">FileAsMapping</span></span>](fileasmapping.md)
    
- [<span data-ttu-id="f5355-154">DisplayName (chaîne)</span><span class="sxs-lookup"><span data-stu-id="f5355-154">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="f5355-155">GivenName</span><span class="sxs-lookup"><span data-stu-id="f5355-155">GivenName</span></span>](givenname.md)
    
- [<span data-ttu-id="f5355-156">Initials</span><span class="sxs-lookup"><span data-stu-id="f5355-156">Initials</span></span>](initials.md)
    
- [<span data-ttu-id="f5355-157">CompleteName</span><span class="sxs-lookup"><span data-stu-id="f5355-157">CompleteName</span></span>](completename.md)
    
- [<span data-ttu-id="f5355-158">FirstName</span><span class="sxs-lookup"><span data-stu-id="f5355-158">FirstName</span></span>](firstname.md)
    
- [<span data-ttu-id="f5355-159">LastName</span><span class="sxs-lookup"><span data-stu-id="f5355-159">LastName</span></span>](lastname.md)
    
- [<span data-ttu-id="f5355-160">FullName</span><span class="sxs-lookup"><span data-stu-id="f5355-160">FullName</span></span>](fullname.md)
    
- [<span data-ttu-id="f5355-161">CompanyName</span><span class="sxs-lookup"><span data-stu-id="f5355-161">CompanyName</span></span>](companyname.md)
    
- [<span data-ttu-id="f5355-162">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="f5355-162">EmailAddresses</span></span>](emailaddresses.md)
    
- [<span data-ttu-id="f5355-163">Entrée (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="f5355-163">Entry (EmailAddress)</span></span>](entry-emailaddress.md)
    
- [<span data-ttu-id="f5355-164">PhysicalAddresses</span><span class="sxs-lookup"><span data-stu-id="f5355-164">PhysicalAddresses</span></span>](physicaladdresses.md)
    
- [<span data-ttu-id="f5355-165">Entrée (PhysicalAddress)</span><span class="sxs-lookup"><span data-stu-id="f5355-165">Entry (PhysicalAddress)</span></span>](entry-physicaladdress.md)
    
- [<span data-ttu-id="f5355-166">Street</span><span class="sxs-lookup"><span data-stu-id="f5355-166">Street</span></span>](street.md)
    
- [<span data-ttu-id="f5355-167">Ville</span><span class="sxs-lookup"><span data-stu-id="f5355-167">City</span></span>](city.md)
    
- [<span data-ttu-id="f5355-168">State</span><span class="sxs-lookup"><span data-stu-id="f5355-168">State</span></span>](state-ex15websvcsotherref.md)
    
- [<span data-ttu-id="f5355-169">CountryOrRegion</span><span class="sxs-lookup"><span data-stu-id="f5355-169">CountryOrRegion</span></span>](countryorregion.md)
    
- [<span data-ttu-id="f5355-170">PhoneNumbers</span><span class="sxs-lookup"><span data-stu-id="f5355-170">PhoneNumbers</span></span>](phonenumbers.md)
    
- [<span data-ttu-id="f5355-171">Entrée (PhoneNumber)</span><span class="sxs-lookup"><span data-stu-id="f5355-171">Entry (PhoneNumber)</span></span>](entry-phonenumber.md)
    
- [<span data-ttu-id="f5355-172">JobTitle</span><span class="sxs-lookup"><span data-stu-id="f5355-172">JobTitle</span></span>](jobtitle.md)
    
- [<span data-ttu-id="f5355-173">Surname</span><span class="sxs-lookup"><span data-stu-id="f5355-173">Surname</span></span>](surname.md)
    
## <a name="invalid-getitem-contact-request-example"></a><span data-ttu-id="f5355-174">Exemple de requête GetItem (contact) non valide</span><span class="sxs-lookup"><span data-stu-id="f5355-174">Invalid GetItem (Contact) request example</span></span>

### <a name="description"></a><span data-ttu-id="f5355-175">Description</span><span class="sxs-lookup"><span data-stu-id="f5355-175">Description</span></span>

<span data-ttu-id="f5355-176">L'exemple de code suivant illustre une demande non valide.</span><span class="sxs-lookup"><span data-stu-id="f5355-176">The following code example shows an invalid request.</span></span>
  
### <a name="code"></a><span data-ttu-id="f5355-177">Code</span><span class="sxs-lookup"><span data-stu-id="f5355-177">Code</span></span>

```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetItem xmlns='https://schemas.microsoft.com/exchange/services/2006/messages'>
      <ItemShape>
        <t:BaseShape>AllProperties</t:BaseShape>
        <t:IncludeMimeContent>true</t:IncludeMimeContent>
      </ItemShape>
      <ItemIds>
        <t:ItemId Id="AAAtAEF=" ChangeKey="EQAAABq" />
      </ItemIds>
    </GetItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="f5355-178">Commentaires</span><span class="sxs-lookup"><span data-stu-id="f5355-178">Comments</span></span>

<span data-ttu-id="f5355-179">Identificateurs d'éléments ont été raccourcies afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="f5355-179">Item identifiers have been shortened to preserve readability.</span></span>
  
## <a name="getitem-contact-error-response"></a><span data-ttu-id="f5355-180">Réponse d’erreur GetItem (contact)</span><span class="sxs-lookup"><span data-stu-id="f5355-180">GetItem (Contact) error response</span></span>

### <a name="description"></a><span data-ttu-id="f5355-181">Description</span><span class="sxs-lookup"><span data-stu-id="f5355-181">Description</span></span>

<span data-ttu-id="f5355-182">L'exemple de code suivant montre une réponse d'erreur à une demande de GetItem (contacts).</span><span class="sxs-lookup"><span data-stu-id="f5355-182">The following code example shows an error response to a GetItem (Contact) request.</span></span>
  
### <a name="code"></a><span data-ttu-id="f5355-183">Code</span><span class="sxs-lookup"><span data-stu-id="f5355-183">Code</span></span>

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
    <GetItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                     xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                     xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Error">
          <m:MessageText>Mime conversion is not supported for this item type.</m:MessageText>
          <m:ResponseCode>ErrorUnsupportedMimeConversion</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Items />
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </GetItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="f5355-184">Éléments de réponse d’erreur</span><span class="sxs-lookup"><span data-stu-id="f5355-184">Error response elements</span></span>

<span data-ttu-id="f5355-185">Les éléments suivants sont utilisés dans la réponse d'erreur :</span><span class="sxs-lookup"><span data-stu-id="f5355-185">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="f5355-186">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="f5355-186">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="f5355-187">GetItemResponse</span><span class="sxs-lookup"><span data-stu-id="f5355-187">GetItemResponse</span></span>](getitemresponse.md)
    
- [<span data-ttu-id="f5355-188">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="f5355-188">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="f5355-189">GetItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="f5355-189">GetItemResponseMessage</span></span>](getitemresponsemessage.md)
    
- [<span data-ttu-id="f5355-190">MessageText</span><span class="sxs-lookup"><span data-stu-id="f5355-190">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="f5355-191">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="f5355-191">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="f5355-192">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="f5355-192">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="f5355-193">Items</span><span class="sxs-lookup"><span data-stu-id="f5355-193">Items</span></span>](items.md)
    
## <a name="see-also"></a><span data-ttu-id="f5355-194">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f5355-194">See also</span></span>



[<span data-ttu-id="f5355-195">Opération GetItem</span><span class="sxs-lookup"><span data-stu-id="f5355-195">GetItem operation</span></span>](getitem-operation.md)


- [<span data-ttu-id="f5355-196">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="f5355-196">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

