---
title: CopyItem Operation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CopyItem
api_type:
- schema
ms.assetid: bcc68f9e-d511-4c29-bba6-ed535524624a
description: L’opération CopyItem copie des éléments et place les éléments dans un autre dossier.
ms.openlocfilehash: 95d2371e9185aa25f40eaec37dda54276a54d321
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755667"
---
# <a name="copyitem-operation"></a><span data-ttu-id="fe0db-103">CopyItem Operation</span><span class="sxs-lookup"><span data-stu-id="fe0db-103">CopyItem operation</span></span>

<span data-ttu-id="fe0db-104">L’opération **CopyItem** copie des éléments et place les éléments dans un autre dossier.</span><span class="sxs-lookup"><span data-stu-id="fe0db-104">The **CopyItem** operation copies items and puts the items in a different folder.</span></span> 
  
## <a name="copyitem-request-example"></a><span data-ttu-id="fe0db-105">Exemple de requête CopyItem</span><span class="sxs-lookup"><span data-stu-id="fe0db-105">CopyItem request example</span></span>

### <a name="description"></a><span data-ttu-id="fe0db-106">Description</span><span class="sxs-lookup"><span data-stu-id="fe0db-106">Description</span></span>

<span data-ttu-id="fe0db-107">Une demande **CopyItem** l’exemple suivant montre comment créer une requête pour copier un élément dans la boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="fe0db-107">The following example of a **CopyItem** request shows how to form a request to copy an item to the Inbox.</span></span> 
  
### <a name="code"></a><span data-ttu-id="fe0db-108">Code</span><span class="sxs-lookup"><span data-stu-id="fe0db-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CopyItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ToFolderId>
        <t:DistinguishedFolderId Id="inbox"/>
      </ToFolderId>
      <ItemIds>
        <t:ItemId Id="AS4AUnV="/>
      </ItemIds>
    </CopyItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="fe0db-109">Commentaires</span><span class="sxs-lookup"><span data-stu-id="fe0db-109">Comments</span></span>

> [!NOTE]
> <span data-ttu-id="fe0db-110">L’ID de dossier et la clé de modification ont été réduits afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="fe0db-110">The folder ID and the change key have been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="fe0db-111">Éléments de la demande</span><span class="sxs-lookup"><span data-stu-id="fe0db-111">Request elements</span></span>

<span data-ttu-id="fe0db-112">Les éléments suivants sont utilisés dans la demande :</span><span class="sxs-lookup"><span data-stu-id="fe0db-112">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="fe0db-113">CopyItem</span><span class="sxs-lookup"><span data-stu-id="fe0db-113">CopyItem</span></span>](copyitem.md)
    
- [<span data-ttu-id="fe0db-114">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="fe0db-114">ToFolderId</span></span>](tofolderid.md)
    
- [<span data-ttu-id="fe0db-115">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="fe0db-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="fe0db-116">ItemId</span><span class="sxs-lookup"><span data-stu-id="fe0db-116">ItemIds</span></span>](itemids.md)
    
- [<span data-ttu-id="fe0db-117">ID d’élément</span><span class="sxs-lookup"><span data-stu-id="fe0db-117">ItemId</span></span>](itemid.md)
    
> [!NOTE]
> <span data-ttu-id="fe0db-118">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="fe0db-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span> 
  
<span data-ttu-id="fe0db-119">Pour trouver d’autres options pour le message de demande de l’opération **CopyItem** , explorez la hiérarchie de schéma.</span><span class="sxs-lookup"><span data-stu-id="fe0db-119">To find other options for the request message of the **CopyItem** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="fe0db-120">Commencer à l’élément [CopyItem](copyitem.md) .</span><span class="sxs-lookup"><span data-stu-id="fe0db-120">Start at the [CopyItem](copyitem.md) element.</span></span> 
  
## <a name="successful-copyitem-response"></a><span data-ttu-id="fe0db-121">Réponse CopyItem réussie</span><span class="sxs-lookup"><span data-stu-id="fe0db-121">Successful CopyItem Response</span></span>

### <a name="description"></a><span data-ttu-id="fe0db-122">Description</span><span class="sxs-lookup"><span data-stu-id="fe0db-122">Description</span></span>

<span data-ttu-id="fe0db-123">L’exemple suivant montre une réponse positive à la demande **CopyItem** .</span><span class="sxs-lookup"><span data-stu-id="fe0db-123">The following example shows a successful response to the **CopyItem** request.</span></span> 
  
<span data-ttu-id="fe0db-124">L’identificateur d’élément du nouvel élément est retournée dans le message de réponse.</span><span class="sxs-lookup"><span data-stu-id="fe0db-124">The item identifier of the new item is returned in the response message.</span></span> <span data-ttu-id="fe0db-125">Identificateurs d’éléments ne sont pas retournés dans les réponses pour cross-boîte aux lettres ou aux opérations **CopyItem** de dossier public.</span><span class="sxs-lookup"><span data-stu-id="fe0db-125">Item identifiers are not returned in responses for cross-mailbox or mailbox to public folder **CopyItem** operations.</span></span> 
  
### <a name="code"></a><span data-ttu-id="fe0db-126">Code</span><span class="sxs-lookup"><span data-stu-id="fe0db-126">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CopyItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CopyItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Message>
              <t:ItemID Id="AAMkAd" ChangeKey="FwAAABY" />
            </t:Message>
          </m:Items>
        </m:CopyItemResponseMessage>
      </m:ResponseMessages>
    </CopyItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a><span data-ttu-id="fe0db-127">Éléments de réponse réussie</span><span class="sxs-lookup"><span data-stu-id="fe0db-127">Successful response elements</span></span>

<span data-ttu-id="fe0db-128">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="fe0db-128">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="fe0db-129">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="fe0db-129">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="fe0db-130">CopyItemResponse</span><span class="sxs-lookup"><span data-stu-id="fe0db-130">CopyItemResponse</span></span>](copyitemresponse.md)
    
- [<span data-ttu-id="fe0db-131">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="fe0db-131">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="fe0db-132">CopyItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="fe0db-132">CopyItemResponseMessage</span></span>](copyitemresponsemessage.md)
    
- [<span data-ttu-id="fe0db-133">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="fe0db-133">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="fe0db-134">Items</span><span class="sxs-lookup"><span data-stu-id="fe0db-134">Items</span></span>](items.md)
    
<span data-ttu-id="fe0db-135">Pour trouver d’autres options pour le message de réponse de l’opération **CopyItem** , explorez la hiérarchie de schéma.</span><span class="sxs-lookup"><span data-stu-id="fe0db-135">To find other options for the response message of the **CopyItem** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="fe0db-136">Démarrez au niveau de l’élément [CopyItemResponse](copyitemresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="fe0db-136">Start at the [CopyItemResponse](copyitemresponse.md) element.</span></span> 
  
## <a name="copyitem-error-response"></a><span data-ttu-id="fe0db-137">Réponse d’erreur CopyItem</span><span class="sxs-lookup"><span data-stu-id="fe0db-137">CopyItem error response</span></span>

### <a name="description"></a><span data-ttu-id="fe0db-138">Description</span><span class="sxs-lookup"><span data-stu-id="fe0db-138">Description</span></span>

<span data-ttu-id="fe0db-139">L’exemple suivant montre une réponse d’erreur à une demande de **CopyItem** .</span><span class="sxs-lookup"><span data-stu-id="fe0db-139">The following example shows an error response to a **CopyItem** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="fe0db-140">Code</span><span class="sxs-lookup"><span data-stu-id="fe0db-140">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CopyItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CopyItemResponseMessage ResponseClass="Error">
          <m:MessageText>Id is malformed.</m:MessageText>
          <m:ResponseCode>ErrorInvalidIdMalformed</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Items />
        </m:CopyItemResponseMessage>
      </m:ResponseMessages>
    </CopyItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="fe0db-141">Éléments de réponse d’erreur</span><span class="sxs-lookup"><span data-stu-id="fe0db-141">Error response elements</span></span>

<span data-ttu-id="fe0db-142">Les éléments suivants sont utilisés dans la réponse d'erreur :</span><span class="sxs-lookup"><span data-stu-id="fe0db-142">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="fe0db-143">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="fe0db-143">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="fe0db-144">CopyItemResponse</span><span class="sxs-lookup"><span data-stu-id="fe0db-144">CopyItemResponse</span></span>](copyitemresponse.md)
    
- [<span data-ttu-id="fe0db-145">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="fe0db-145">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="fe0db-146">CopyItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="fe0db-146">CopyItemResponseMessage</span></span>](copyitemresponsemessage.md)
    
- [<span data-ttu-id="fe0db-147">MessageText</span><span class="sxs-lookup"><span data-stu-id="fe0db-147">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="fe0db-148">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="fe0db-148">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="fe0db-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="fe0db-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="fe0db-150">Items</span><span class="sxs-lookup"><span data-stu-id="fe0db-150">Items</span></span>](items.md)
    
<span data-ttu-id="fe0db-151">Pour trouver d’autres options pour le message de réponse de l’opération **CopyItem** , explorez la hiérarchie de schéma.</span><span class="sxs-lookup"><span data-stu-id="fe0db-151">To find other options for the error response message of the **CopyItem** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="fe0db-152">Démarrez au niveau de l’élément [CopyItemResponse](copyitemresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="fe0db-152">Start at the [CopyItemResponse](copyitemresponse.md) element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="fe0db-153">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="fe0db-153">See also</span></span>



- [<span data-ttu-id="fe0db-154">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="fe0db-154">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

