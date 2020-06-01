---
title: Opération UploadItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UploadItems
api_type:
- schema
ms.assetid: a88cbe99-7968-454d-a545-4f92c330909f
description: L’opération UploadItems télécharge un flux d’éléments dans une boîte aux lettres Exchange.
ms.openlocfilehash: 57e722c7775baa090736875077781cee869c3b01
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468501"
---
# <a name="uploaditems-operation"></a><span data-ttu-id="720db-103">Opération UploadItems</span><span class="sxs-lookup"><span data-stu-id="720db-103">UploadItems operation</span></span>

<span data-ttu-id="720db-104">L’opération **UploadItems** télécharge un flux d’éléments dans une boîte aux lettres Exchange.</span><span class="sxs-lookup"><span data-stu-id="720db-104">The **UploadItems** operation uploads a stream of items into an Exchange mailbox.</span></span> 
  
> [!IMPORTANT]
> <span data-ttu-id="720db-105">L’opération **UploadItems** est limitée dans MicrosoftExchange Server 2010 Service Pack 1 (SP1) à une charge utile d’importation maximale de 25 Mo de données codées en base64.</span><span class="sxs-lookup"><span data-stu-id="720db-105">The **UploadItems** operation is restricted in MicrosoftExchange Server 2010 Service Pack 1 (SP1) to a maximum import payload of 25MB of base64 encoded data.</span></span> <span data-ttu-id="720db-106">Le paramètre peut être modifié dans le fichier Web. config.</span><span class="sxs-lookup"><span data-stu-id="720db-106">The setting can be altered in the web.config file.</span></span> 
  
## <a name="uploaditems-request-example"></a><span data-ttu-id="720db-107">Exemple de requête UploadItems</span><span class="sxs-lookup"><span data-stu-id="720db-107">UploadItems request example</span></span>

### <a name="description"></a><span data-ttu-id="720db-108">Description</span><span class="sxs-lookup"><span data-stu-id="720db-108">Description</span></span>

<span data-ttu-id="720db-109">L’exemple de requête **UploadItems** suivant montre comment télécharger deux éléments dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="720db-109">The following example of an **UploadItems** request shows how to upload two items into a mailbox.</span></span> <span data-ttu-id="720db-110">Le premier élément est un nouvel élément.</span><span class="sxs-lookup"><span data-stu-id="720db-110">The first item is a new item.</span></span> <span data-ttu-id="720db-111">Le deuxième élément est une version mise à jour d’un élément existant dans la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="720db-111">The second item is an updated version of an existing item in the mailbox.</span></span> 
  
### <a name="code"></a><span data-ttu-id="720db-112">Code</span><span class="sxs-lookup"><span data-stu-id="720db-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010_SP1" />
  </soap:Header>
  <soap:Body>
    <m:UploadItems>
      <m:Items>
        <t:Item CreateAction="CreateNew">
          <t:ParentFolderId Id="AQMkADhhOGIgAAAA==" ChangeKey="AQAAAA=="/>
          <t:Data>
            AQAAAAgAAAAAAAAAAQAAAAMAAAAYAAAAAQAAAAcDAgAAAAAAwAAAAA
            AAAEYAJACABAAAAAYAAAABDqSAAAACAAAAcSMAAOSECEBbAAAAL089
            RklSU1QgT1JHQU5JWkFUSU9OL09VPUVYQ0hBTkdFIEFETUlOSVNUUk
            FUSVZFIEdST1VQIChGWURJQk9IRjIzU1BETFQpL0NOPVJFQ0lQSUVO
            VFMvQ049AAMAFwABAAAAsIQaABIAAABJAFAATQAuAE4AbwB0AGUAAA
            ALACMAAAADACYAAAAAAAsAKQAAAAMALgAAAAAAAwA2AAAAAACwhw4=
          </t:Data>
        </t:Item>
        <t:Item CreateAction="Update">
          <t:ParentFolderId Id="AQMkADhhOGIgAAAB==" ChangeKey="AQAAAA=="/>
          <t:ItemId Id="AAMkADhhOGU0MGM7AAA=" ChangeKey="CQAAAA=="/>
          <t:Data>
            AQAAAAgAAAAAAAAAAQAAAAMAAAAYAAAAAQAAAAcDAgAAAAAAwAAAAA
            AAAEYAJACABAAAAAYAAAABDqSAAAACAAAANiAAAOSECEBbAAAAL089
            RklSU1QgT1JHQU5JWkFUSU9OL09VPUVYQ0hBTkdFIEFETUlOSVNUUk
            FUSVZFIEdST1VQIChGWURJQk9IRjIzU1BETFQpL0NOPVJFQ0lQSUVO
            VFMvQ049AAMAFwABAAAAsIQaABIAAABJAFAATQAuAE4AbwB0AGUAAA
            ALACMAAAALACkAAAADADYAAAAAALCENwAyAAAASQBuAHQAZQByAGUA
            cwB0AGkAbgBnACAALQAgAGYAcgBvAG0AIABFAFcAUwBNAEEAAABAAD
            kAgJ2chyHuygECATsAZQAAAEVYOi9PPUZJUlNUIE9SR0FOSVpBVBMO
          </t:Data>
        </t:Item>
      </m:Items>
    </m:UploadItems>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="720db-113">Commentaires</span><span class="sxs-lookup"><span data-stu-id="720db-113">Comments</span></span>

<span data-ttu-id="720db-114">Les identificateurs et les données d’élément ont été raccourcies afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="720db-114">Identifiers and the item data have been shortened to preserve readability.</span></span>
  
### <a name="request-elements"></a><span data-ttu-id="720db-115">Demander des éléments</span><span class="sxs-lookup"><span data-stu-id="720db-115">Request elements</span></span>

<span data-ttu-id="720db-116">Les éléments suivants sont utilisés dans la demande :</span><span class="sxs-lookup"><span data-stu-id="720db-116">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="720db-117">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="720db-117">RequestServerVersion</span></span>](requestserverversion.md)
    
- [<span data-ttu-id="720db-118">UploadItems</span><span class="sxs-lookup"><span data-stu-id="720db-118">UploadItems</span></span>](uploaditems.md)
    
- [<span data-ttu-id="720db-119">Items (NonEmptyArrayOfUploadItemsType)</span><span class="sxs-lookup"><span data-stu-id="720db-119">Items (NonEmptyArrayOfUploadItemsType)</span></span>](items-nonemptyarrayofuploaditemstype.md)
    
- [<span data-ttu-id="720db-120">Élément (UploadItemType)</span><span class="sxs-lookup"><span data-stu-id="720db-120">Item (UploadItemType)</span></span>](item-uploaditemtype.md)
    
- [<span data-ttu-id="720db-121">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="720db-121">ParentFolderId</span></span>](parentfolderid.md)
    
- [<span data-ttu-id="720db-122">Données (base64Binary)</span><span class="sxs-lookup"><span data-stu-id="720db-122">Data (base64Binary)</span></span>](data-base64binary.md)
    
- [<span data-ttu-id="720db-123">ItemId</span><span class="sxs-lookup"><span data-stu-id="720db-123">ItemId</span></span>](itemid.md)
    
## <a name="successful-uploaditems-response-example"></a><span data-ttu-id="720db-124">Exemple de réponse UploadItems réussi</span><span class="sxs-lookup"><span data-stu-id="720db-124">Successful UploadItems response example</span></span>

### <a name="description"></a><span data-ttu-id="720db-125">Description</span><span class="sxs-lookup"><span data-stu-id="720db-125">Description</span></span>

<span data-ttu-id="720db-126">L’exemple suivant montre une réponse réussie à la demande **UploadItems** .</span><span class="sxs-lookup"><span data-stu-id="720db-126">The following example shows a successful response to the **UploadItems** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="720db-127">Code</span><span class="sxs-lookup"><span data-stu-id="720db-127">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14"
                         MinorVersion="1"
                         MajorBuildNumber="164"
                         MinorBuildNumber="0"
                         Version="Exchange2010_SP1"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:UploadItemsResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                           xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:UploadItemsResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:ItemId Id="AAMkADhhUFZ/AAA=" ChangeKey="CQAAABYAAABsMBS3hrihS7voMf0GPIQeAAAAULQm"/>
        </m:UploadItemsResponseMessage>
        <m:UploadItemsResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:ItemId Id="AAMkADhhOGZ7AAA=" ChangeKey="CQAAABYAAABsMBS3hrihS7voMf0GPIQeAAAAULQn"/>
        </m:UploadItemsResponseMessage>
      </m:ResponseMessages>
    </m:UploadItemsResponse>
  </s:Body>
</s:Envelope>
```

### <a name="comments"></a><span data-ttu-id="720db-128">Commentaires</span><span class="sxs-lookup"><span data-stu-id="720db-128">Comments</span></span>

<span data-ttu-id="720db-129">Identificateurs d'éléments ont été raccourcies afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="720db-129">Item identifiers have been shortened to preserve readability.</span></span>
  
### <a name="response-elements"></a><span data-ttu-id="720db-130">Éléments Response</span><span class="sxs-lookup"><span data-stu-id="720db-130">Response elements</span></span>

<span data-ttu-id="720db-131">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="720db-131">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="720db-132">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="720db-132">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="720db-133">UploadItemsResponse</span><span class="sxs-lookup"><span data-stu-id="720db-133">UploadItemsResponse</span></span>](uploaditemsresponse.md)
    
- [<span data-ttu-id="720db-134">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="720db-134">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="720db-135">UploadItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="720db-135">UploadItemsResponseMessage</span></span>](uploaditemsresponsemessage.md)
    
- [<span data-ttu-id="720db-136">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="720db-136">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="720db-137">ItemId</span><span class="sxs-lookup"><span data-stu-id="720db-137">ItemId</span></span>](itemid.md)
    
## <a name="uploaditems-error-response-example"></a><span data-ttu-id="720db-138">Exemple de réponse d’erreur UploadItems</span><span class="sxs-lookup"><span data-stu-id="720db-138">UploadItems Error response example</span></span>

### <a name="description"></a><span data-ttu-id="720db-139">Description</span><span class="sxs-lookup"><span data-stu-id="720db-139">Description</span></span>

<span data-ttu-id="720db-140">L’exemple suivant montre une réponse à la demande **UploadItems** qui contient une erreur causée par une tentative de mise à jour d’un élément introuvable dans la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="720db-140">The following example shows a response to the **UploadItems** request that contains an error caused by an attempt to update an item that cannot be found in the mailbox.</span></span> 
  
### <a name="code"></a><span data-ttu-id="720db-141">Code</span><span class="sxs-lookup"><span data-stu-id="720db-141">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="1" 
                         MajorBuildNumber="164" 
                         MinorBuildNumber="0" 
                         Version="Exchange2010_SP1" 
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:UploadItemsResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                           xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:UploadItemsResponseMessage ResponseClass="Error">
          <m:MessageText>The specified object was not found in the store.</m:MessageText>
          <m:ResponseCode>ErrorItemNotFound</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:UploadItemsResponseMessage>
      </m:ResponseMessages>
    </m:UploadItemsResponse>
  </s:Body>
</s:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="720db-142">Éléments de réponse d’erreur</span><span class="sxs-lookup"><span data-stu-id="720db-142">Error response elements</span></span>

<span data-ttu-id="720db-143">Les éléments suivants sont utilisés dans la réponse d'erreur :</span><span class="sxs-lookup"><span data-stu-id="720db-143">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="720db-144">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="720db-144">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="720db-145">UploadItemsResponse</span><span class="sxs-lookup"><span data-stu-id="720db-145">UploadItemsResponse</span></span>](uploaditemsresponse.md)
    
- [<span data-ttu-id="720db-146">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="720db-146">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="720db-147">UploadItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="720db-147">UploadItemsResponseMessage</span></span>](uploaditemsresponsemessage.md)
    
- [<span data-ttu-id="720db-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="720db-148">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="720db-149">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="720db-149">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="720db-150">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="720db-150">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="720db-151">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="720db-151">See also</span></span>



[<span data-ttu-id="720db-152">Opération ExportItems</span><span class="sxs-lookup"><span data-stu-id="720db-152">ExportItems operation</span></span>](exportitems-operation.md)


[<span data-ttu-id="720db-153">Opérations EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="720db-153">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
  
- [<span data-ttu-id="720db-154">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="720db-154">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

