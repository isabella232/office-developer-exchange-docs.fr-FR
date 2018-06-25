---
title: Opération CreateItem (contacts)
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
ms.assetid: 417e994b-0a17-4c24-9527-04796b80b029
description: L'opération de la méthode CreateItem permet de créer des contacts dans la banque d'informations Exchange.
ms.openlocfilehash: 05e4715f3c6675401ae7afac852395f7459c02c9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755718"
---
# <a name="createitem-operation-contact"></a><span data-ttu-id="04d0a-103">Opération CreateItem (contacts)</span><span class="sxs-lookup"><span data-stu-id="04d0a-103">CreateItem operation (contact)</span></span>

<span data-ttu-id="04d0a-104">Ce document peut contenir des informations liées aux fonctionnalités ou produits préliminaires qui sont sujettes à modifications avant la sortie de la version définitive. Ce document est fourni "tel quel" à titre indicatif et Microsoft exclut toute garantie, expresse ou implicite, en ce qui concerne ce document. L'opération de la méthode CreateItem permet de créer des contacts dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="04d0a-104">The CreateItem operation is used to create contacts in the Exchange store.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="04d0a-105">Remarques</span><span class="sxs-lookup"><span data-stu-id="04d0a-105">Remarks</span></span>

<span data-ttu-id="04d0a-p101">La création de listes de distribution privée n'est pas pris en charge. Toutes les propriétés au sein du conteneur [CompleteName](completename.md) sont en lecture seule et ne peut pas être définies sur un élément de contact.</span><span class="sxs-lookup"><span data-stu-id="04d0a-p101">The creation of private distribution lists is not supported. All properties within the [CompleteName](completename.md) container are read-only and cannot be set on a contact item.</span></span> 
  
## <a name="createitem-request-example"></a><span data-ttu-id="04d0a-108">Exemple de requête CreateItem</span><span class="sxs-lookup"><span data-stu-id="04d0a-108">CreateItem request example</span></span>

### <a name="description"></a><span data-ttu-id="04d0a-109">Description</span><span class="sxs-lookup"><span data-stu-id="04d0a-109">Description</span></span>

<span data-ttu-id="04d0a-110">Une demande CreateItem SOAP valide l'exemple suivant montre comment créer un contact dans le dossier Contacts par défaut.</span><span class="sxs-lookup"><span data-stu-id="04d0a-110">The following example of a valid CreateItem SOAP request shows how to create a contact in the default Contacts folder.</span></span>
  
### <a name="code"></a><span data-ttu-id="04d0a-111">Code</span><span class="sxs-lookup"><span data-stu-id="04d0a-111">Code</span></span>

```XML
<soap:Envelope
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
 xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" >
      <SavedItemFolderId>
        <t:DistinguishedFolderId Id="contacts"/>
      </SavedItemFolderId>
      <Items>
        <t:Contact>
          <t:FileAs>SampleContact</t:FileAs>
          <t:GivenName>Tanja</t:GivenName>
          <t:CompanyName>Blue Yonder Airlines</t:CompanyName>
          <t:EmailAddresses>
            <t:Entry Key="EmailAddress1">tplate@example.com</t:Entry>
          </t:EmailAddresses>
          <t:PhysicalAddresses>
            <t:Entry Key="Business">
              <t:Street>1234 56th Ave</t:Street>
              <t:City>La Habra</t:City>
              <t:State>CA</t:State>
              <t: CountryOrRegion>USA</t: CountryOrRegion>
            </t:Entry>
          </t:PhysicalAddresses>
          <t:PhoneNumbers>
            <t:Entry Key="BusinessPhone">4255550199</t:Entry>
          </t:PhoneNumbers>
          <t:JobTitle>Manager</t:JobTitle>
          <t:Surname>Plate</t:Surname>
        </t:Contact>
      </Items>
    </CreateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="04d0a-112">Éléments de la demande</span><span class="sxs-lookup"><span data-stu-id="04d0a-112">Request elements</span></span>

<span data-ttu-id="04d0a-113">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="04d0a-113">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="04d0a-114">CreateItem</span><span class="sxs-lookup"><span data-stu-id="04d0a-114">CreateItem</span></span>](createitem.md)
    
- [<span data-ttu-id="04d0a-115">SavedItemFolderId</span><span class="sxs-lookup"><span data-stu-id="04d0a-115">SavedItemFolderId</span></span>](saveditemfolderid.md)
    
- [<span data-ttu-id="04d0a-116">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="04d0a-116">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="04d0a-117">Éléments (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="04d0a-117">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md)
    
- [<span data-ttu-id="04d0a-118">Contact</span><span class="sxs-lookup"><span data-stu-id="04d0a-118">Contact</span></span>](contact.md)
    
- [<span data-ttu-id="04d0a-119">Classer sous</span><span class="sxs-lookup"><span data-stu-id="04d0a-119">FileAs</span></span>](fileas.md)
    
- [<span data-ttu-id="04d0a-120">Prénom</span><span class="sxs-lookup"><span data-stu-id="04d0a-120">GivenName</span></span>](givenname.md)
    
- [<span data-ttu-id="04d0a-121">CompanyName</span><span class="sxs-lookup"><span data-stu-id="04d0a-121">CompanyName</span></span>](companyname.md)
    
- [<span data-ttu-id="04d0a-122">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="04d0a-122">EmailAddresses</span></span>](emailaddresses.md)
    
- [<span data-ttu-id="04d0a-123">Entrée (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="04d0a-123">Entry (EmailAddress)</span></span>](entry-emailaddress.md)
    
- [<span data-ttu-id="04d0a-124">PhysicalAddresses</span><span class="sxs-lookup"><span data-stu-id="04d0a-124">PhysicalAddresses</span></span>](physicaladdresses.md)
    
- [<span data-ttu-id="04d0a-125">Entrée (PhysicalAddress)</span><span class="sxs-lookup"><span data-stu-id="04d0a-125">Entry (PhysicalAddress)</span></span>](entry-physicaladdress.md)
    
- [<span data-ttu-id="04d0a-126">Street</span><span class="sxs-lookup"><span data-stu-id="04d0a-126">Street</span></span>](street.md)
    
- [<span data-ttu-id="04d0a-127">Ville</span><span class="sxs-lookup"><span data-stu-id="04d0a-127">City</span></span>](city.md)
    
- [<span data-ttu-id="04d0a-128">State</span><span class="sxs-lookup"><span data-stu-id="04d0a-128">State</span></span>](state-ex15websvcsotherref.md)
    
- [<span data-ttu-id="04d0a-129">Countryorregion définit</span><span class="sxs-lookup"><span data-stu-id="04d0a-129">CountryOrRegion</span></span>](countryorregion.md)
    
- [<span data-ttu-id="04d0a-130">PhoneNumbers</span><span class="sxs-lookup"><span data-stu-id="04d0a-130">PhoneNumbers</span></span>](phonenumbers.md)
    
- [<span data-ttu-id="04d0a-131">Entrée (PhoneNumber)</span><span class="sxs-lookup"><span data-stu-id="04d0a-131">Entry (PhoneNumber)</span></span>](entry-phonenumber.md)
    
- [<span data-ttu-id="04d0a-132">JobTitle</span><span class="sxs-lookup"><span data-stu-id="04d0a-132">JobTitle</span></span>](jobtitle.md)
    
- [<span data-ttu-id="04d0a-133">Surname</span><span class="sxs-lookup"><span data-stu-id="04d0a-133">Surname</span></span>](surname.md)
    
## <a name="successful-createitem-request"></a><span data-ttu-id="04d0a-134">Demande CreateItem réussie</span><span class="sxs-lookup"><span data-stu-id="04d0a-134">Successful CreateItem Request</span></span>

### <a name="description"></a><span data-ttu-id="04d0a-135">Description</span><span class="sxs-lookup"><span data-stu-id="04d0a-135">Description</span></span>

<span data-ttu-id="04d0a-p102">L'exemple suivant montre une réponse positive à la demande CreateItem qui a créé un contact. Dans cet exemple, la réponse contient l'identificateur de l'élément nouvellement créé.</span><span class="sxs-lookup"><span data-stu-id="04d0a-p102">The following example shows a successful response to the CreateItem request that created a contact. In this example, the response contains the identifier of the newly created item.</span></span>
  
### <a name="code"></a><span data-ttu-id="04d0a-138">Code</span><span class="sxs-lookup"><span data-stu-id="04d0a-138">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="602" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CreateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Contact>
              <t:ItemId Id="AAAtA=" ChangeKey="EQAAAB" />
            </t:Contact>
          </m:Items>
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </CreateItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="04d0a-139">Commentaires</span><span class="sxs-lookup"><span data-stu-id="04d0a-139">Comments</span></span>

<span data-ttu-id="04d0a-140">Identificateur de l'élément a été raccourcie afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="04d0a-140">The item identifier has been shortened to preserve readability.</span></span>
  
### <a name="successful-response-elements"></a><span data-ttu-id="04d0a-141">Éléments de réponse réussie</span><span class="sxs-lookup"><span data-stu-id="04d0a-141">Successful response elements</span></span>

<span data-ttu-id="04d0a-142">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="04d0a-142">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="04d0a-143">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="04d0a-143">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="04d0a-144">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="04d0a-144">CreateItemResponse</span></span>](createitemresponse.md)
    
- [<span data-ttu-id="04d0a-145">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="04d0a-145">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="04d0a-146">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="04d0a-146">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
    
- [<span data-ttu-id="04d0a-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="04d0a-147">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="04d0a-148">Éléments (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="04d0a-148">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md)
    
- [<span data-ttu-id="04d0a-149">Contact</span><span class="sxs-lookup"><span data-stu-id="04d0a-149">Contact</span></span>](contact.md)
    
- [<span data-ttu-id="04d0a-150">ID d’élément</span><span class="sxs-lookup"><span data-stu-id="04d0a-150">ItemId</span></span>](itemid.md)
    
## <a name="invalid-createitem-request-example"></a><span data-ttu-id="04d0a-151">Exemple de requête CreateItem non valide</span><span class="sxs-lookup"><span data-stu-id="04d0a-151">Invalid CreateItem request example</span></span>

### <a name="description"></a><span data-ttu-id="04d0a-152">Description</span><span class="sxs-lookup"><span data-stu-id="04d0a-152">Description</span></span>

<span data-ttu-id="04d0a-p103">L'exemple suivant montre une requête qui contient le XML valides, mais les instructions incompatibles. Impossible de créer un contact dans un dossier de recherche.</span><span class="sxs-lookup"><span data-stu-id="04d0a-p103">The following example shows a request that contains valid XML but incompatible instructions. A contact cannot be created in a search folder.</span></span>
  
### <a name="code"></a><span data-ttu-id="04d0a-155">Code</span><span class="sxs-lookup"><span data-stu-id="04d0a-155">Code</span></span>

```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem xmlns='http://schemas.microsoft.com/exchange/services/2006/messages'>
      <SavedItemFolderId>
        <t:DistinguishedFolderId Id='searchfolders'/>
      </SavedItemFolderId>
      <Items>
        <t:Contact>
          <t:ItemClass>IPM.Contact</t:ItemClass>
        </t:Contact>
      </Items>
    </CreateItem>
  </soap:Body>
</soap:Envelope>
```

## <a name="createitem-contact-error-response"></a><span data-ttu-id="04d0a-156">Réponse d’erreur CreateItem (contacts)</span><span class="sxs-lookup"><span data-stu-id="04d0a-156">CreateItem (Contact) error response</span></span>

### <a name="description"></a><span data-ttu-id="04d0a-157">Description</span><span class="sxs-lookup"><span data-stu-id="04d0a-157">Description</span></span>

<span data-ttu-id="04d0a-158">L'exemple suivant montre une réponse d'erreur à une demande CreateItem (contacts).</span><span class="sxs-lookup"><span data-stu-id="04d0a-158">The following example shows an error response to a CreateItem (Contact) request.</span></span>
  
### <a name="code"></a><span data-ttu-id="04d0a-159">Code</span><span class="sxs-lookup"><span data-stu-id="04d0a-159">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="602" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CreateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Error">
          <m:MessageText>Cannot create a contact in a non-contact Folder.</m:MessageText>
          <m:ResponseCode>ErrorCannotCreateContactInNonContactFolder</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Items />
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </CreateItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="04d0a-160">Éléments de réponse d’erreur</span><span class="sxs-lookup"><span data-stu-id="04d0a-160">Error response elements</span></span>

<span data-ttu-id="04d0a-161">Les éléments suivants sont utilisés dans la réponse d'erreur :</span><span class="sxs-lookup"><span data-stu-id="04d0a-161">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="04d0a-162">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="04d0a-162">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="04d0a-163">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="04d0a-163">CreateItemResponse</span></span>](createitemresponse.md)
    
- [<span data-ttu-id="04d0a-164">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="04d0a-164">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="04d0a-165">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="04d0a-165">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
    
- [<span data-ttu-id="04d0a-166">MessageText</span><span class="sxs-lookup"><span data-stu-id="04d0a-166">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="04d0a-167">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="04d0a-167">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="04d0a-168">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="04d0a-168">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="04d0a-169">Éléments (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="04d0a-169">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md)
    
## <a name="see-also"></a><span data-ttu-id="04d0a-170">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="04d0a-170">See also</span></span>



[<span data-ttu-id="04d0a-171">CreateItem Operation</span><span class="sxs-lookup"><span data-stu-id="04d0a-171">CreateItem operation</span></span>](createitem-operation.md)

