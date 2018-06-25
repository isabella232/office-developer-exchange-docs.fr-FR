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
ms.openlocfilehash: 6b002d531c7011b18ae1f88adfc2923d5a51e81c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838922"
---
# <a name="uploaditems-operation"></a><span data-ttu-id="7922c-103">Opération UploadItems</span><span class="sxs-lookup"><span data-stu-id="7922c-103">UploadItems operation</span></span>

<span data-ttu-id="7922c-104">L’opération **UploadItems** télécharge un flux d’éléments dans une boîte aux lettres Exchange.</span><span class="sxs-lookup"><span data-stu-id="7922c-104">The **UploadItems** operation uploads a stream of items into an Exchange mailbox.</span></span> 
  
> [!IMPORTANT]
> <span data-ttu-id="7922c-105">L’opération **UploadItems** est limitée à une charge maximale d’importation de 25 Mo de données codées en base64 dans MicrosoftExchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="7922c-105">The **UploadItems** operation is restricted in MicrosoftExchange Server 2010 Service Pack 1 (SP1) to a maximum import payload of 25MB of base64 encoded data.</span></span> <span data-ttu-id="7922c-106">Le paramètre peut être modifié dans le fichier web.config.</span><span class="sxs-lookup"><span data-stu-id="7922c-106">The setting can be altered in the web.config file.</span></span> 
  
## <a name="uploaditems-request-example"></a><span data-ttu-id="7922c-107">Exemple de requête UploadItems</span><span class="sxs-lookup"><span data-stu-id="7922c-107">UploadItems request example</span></span>

### <a name="description"></a><span data-ttu-id="7922c-108">Description</span><span class="sxs-lookup"><span data-stu-id="7922c-108">Description</span></span>

<span data-ttu-id="7922c-109">Une demande de **UploadItems** l’exemple suivant montre comment charger des deux éléments dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="7922c-109">The following example of an **UploadItems** request shows how to upload two items into a mailbox.</span></span> <span data-ttu-id="7922c-110">Le premier élément est un nouvel élément.</span><span class="sxs-lookup"><span data-stu-id="7922c-110">The first item is a new item.</span></span> <span data-ttu-id="7922c-111">Le deuxième élément est une version mise à jour d’un élément existant dans la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="7922c-111">The second item is an updated version of an existing item in the mailbox.</span></span> 
  
### <a name="code"></a><span data-ttu-id="7922c-112">Code</span><span class="sxs-lookup"><span data-stu-id="7922c-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="7922c-113">Commentaires</span><span class="sxs-lookup"><span data-stu-id="7922c-113">Comments</span></span>

<span data-ttu-id="7922c-114">Identificateurs et les données ont été réduites afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="7922c-114">Identifiers and the item data have been shortened to preserve readability.</span></span>
  
### <a name="request-elements"></a><span data-ttu-id="7922c-115">Éléments de la demande</span><span class="sxs-lookup"><span data-stu-id="7922c-115">Request elements</span></span>

<span data-ttu-id="7922c-116">Les éléments suivants sont utilisés dans la demande :</span><span class="sxs-lookup"><span data-stu-id="7922c-116">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="7922c-117">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="7922c-117">RequestServerVersion</span></span>](requestserverversion.md)
    
- [<span data-ttu-id="7922c-118">UploadItems</span><span class="sxs-lookup"><span data-stu-id="7922c-118">UploadItems</span></span>](uploaditems.md)
    
- [<span data-ttu-id="7922c-119">Éléments (NonEmptyArrayOfUploadItemsType)</span><span class="sxs-lookup"><span data-stu-id="7922c-119">Items (NonEmptyArrayOfUploadItemsType)</span></span>](items-nonemptyarrayofuploaditemstype.md)
    
- [<span data-ttu-id="7922c-120">Élément (UploadItemType)</span><span class="sxs-lookup"><span data-stu-id="7922c-120">Item (UploadItemType)</span></span>](item-uploaditemtype.md)
    
- [<span data-ttu-id="7922c-121">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="7922c-121">ParentFolderId</span></span>](parentfolderid.md)
    
- [<span data-ttu-id="7922c-122">Données (base64Binary)</span><span class="sxs-lookup"><span data-stu-id="7922c-122">Data (base64Binary)</span></span>](data-base64binary.md)
    
- [<span data-ttu-id="7922c-123">ID d’élément</span><span class="sxs-lookup"><span data-stu-id="7922c-123">ItemId</span></span>](itemid.md)
    
## <a name="successful-uploaditems-response-example"></a><span data-ttu-id="7922c-124">Exemple de réponse UploadItems réussie</span><span class="sxs-lookup"><span data-stu-id="7922c-124">Successful UploadItems response example</span></span>

### <a name="description"></a><span data-ttu-id="7922c-125">Description</span><span class="sxs-lookup"><span data-stu-id="7922c-125">Description</span></span>

<span data-ttu-id="7922c-126">L’exemple suivant montre une réponse positive à la demande **UploadItems** .</span><span class="sxs-lookup"><span data-stu-id="7922c-126">The following example shows a successful response to the **UploadItems** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="7922c-127">Code</span><span class="sxs-lookup"><span data-stu-id="7922c-127">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14"
                         MinorVersion="1"
                         MajorBuildNumber="164"
                         MinorBuildNumber="0"
                         Version="Exchange2010_SP1"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:UploadItemsResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                           xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

### <a name="comments"></a><span data-ttu-id="7922c-128">Commentaires</span><span class="sxs-lookup"><span data-stu-id="7922c-128">Comments</span></span>

<span data-ttu-id="7922c-129">Identificateurs d'éléments ont été raccourcies afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="7922c-129">Item identifiers have been shortened to preserve readability.</span></span>
  
### <a name="response-elements"></a><span data-ttu-id="7922c-130">Éléments de réponse</span><span class="sxs-lookup"><span data-stu-id="7922c-130">Response elements</span></span>

<span data-ttu-id="7922c-131">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="7922c-131">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="7922c-132">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="7922c-132">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="7922c-133">UploadItemsResponse</span><span class="sxs-lookup"><span data-stu-id="7922c-133">UploadItemsResponse</span></span>](uploaditemsresponse.md)
    
- [<span data-ttu-id="7922c-134">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="7922c-134">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="7922c-135">UploadItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="7922c-135">UploadItemsResponseMessage</span></span>](uploaditemsresponsemessage.md)
    
- [<span data-ttu-id="7922c-136">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="7922c-136">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="7922c-137">ID d’élément</span><span class="sxs-lookup"><span data-stu-id="7922c-137">ItemId</span></span>](itemid.md)
    
## <a name="uploaditems-error-response-example"></a><span data-ttu-id="7922c-138">Exemple de réponse d’erreur UploadItems</span><span class="sxs-lookup"><span data-stu-id="7922c-138">UploadItems Error response example</span></span>

### <a name="description"></a><span data-ttu-id="7922c-139">Description</span><span class="sxs-lookup"><span data-stu-id="7922c-139">Description</span></span>

<span data-ttu-id="7922c-140">L’exemple suivant montre une réponse à la demande **UploadItems** qui contient une erreur due à une tentative de mise à jour d’un élément qui ne figurent pas dans la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="7922c-140">The following example shows a response to the **UploadItems** request that contains an error caused by an attempt to update an item that cannot be found in the mailbox.</span></span> 
  
### <a name="code"></a><span data-ttu-id="7922c-141">Code</span><span class="sxs-lookup"><span data-stu-id="7922c-141">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="1" 
                         MajorBuildNumber="164" 
                         MinorBuildNumber="0" 
                         Version="Exchange2010_SP1" 
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:UploadItemsResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                           xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

### <a name="error-response-elements"></a><span data-ttu-id="7922c-142">Éléments de réponse d’erreur</span><span class="sxs-lookup"><span data-stu-id="7922c-142">Error response elements</span></span>

<span data-ttu-id="7922c-143">Les éléments suivants sont utilisés dans la réponse d'erreur :</span><span class="sxs-lookup"><span data-stu-id="7922c-143">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="7922c-144">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="7922c-144">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="7922c-145">UploadItemsResponse</span><span class="sxs-lookup"><span data-stu-id="7922c-145">UploadItemsResponse</span></span>](uploaditemsresponse.md)
    
- [<span data-ttu-id="7922c-146">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="7922c-146">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="7922c-147">UploadItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="7922c-147">UploadItemsResponseMessage</span></span>](uploaditemsresponsemessage.md)
    
- [<span data-ttu-id="7922c-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="7922c-148">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="7922c-149">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="7922c-149">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="7922c-150">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="7922c-150">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="7922c-151">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7922c-151">See also</span></span>



[<span data-ttu-id="7922c-152">Opération ExportItems</span><span class="sxs-lookup"><span data-stu-id="7922c-152">ExportItems operation</span></span>](exportitems-operation.md)


[<span data-ttu-id="7922c-153">Opérations EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="7922c-153">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
  
- [<span data-ttu-id="7922c-154">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="7922c-154">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

