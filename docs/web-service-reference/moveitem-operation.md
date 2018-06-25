---
title: MoveItem Operation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MoveItem
api_type:
- schema
ms.assetid: dcf40fa7-7796-4a5c-bf5b-7a509a18d208
description: L’opération MoveItem est utilisée pour déplacer un ou plusieurs éléments dans un dossier de destination unique.
ms.openlocfilehash: c5619befb02ec20ef0911992484dcc00cc2c5e92
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828492"
---
# <a name="moveitem-operation"></a><span data-ttu-id="736c6-103">MoveItem Operation</span><span class="sxs-lookup"><span data-stu-id="736c6-103">MoveItem operation</span></span>

<span data-ttu-id="736c6-104">L’opération **MoveItem** est utilisée pour déplacer un ou plusieurs éléments dans un dossier de destination unique.</span><span class="sxs-lookup"><span data-stu-id="736c6-104">The **MoveItem** operation is used to move one or more items to a single destination folder.</span></span> 
  
## <a name="moveitem-request-example"></a><span data-ttu-id="736c6-105">Exemple de requête MoveItem</span><span class="sxs-lookup"><span data-stu-id="736c6-105">MoveItem request example</span></span>

### <a name="description"></a><span data-ttu-id="736c6-106">Description</span><span class="sxs-lookup"><span data-stu-id="736c6-106">Description</span></span>

<span data-ttu-id="736c6-107">L’exemple suivant d’une demande **MoveItem** montre comment déplacer un élément vers le dossier Brouillons.</span><span class="sxs-lookup"><span data-stu-id="736c6-107">The following example of a **MoveItem** request shows how to move an item to the Drafts folder.</span></span> 
  
### <a name="code"></a><span data-ttu-id="736c6-108">Code</span><span class="sxs-lookup"><span data-stu-id="736c6-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
xmlns:xsd="http://www.w3.org/2001/XMLSchema"
xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <MoveItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <ToFolderId>
        <t:DistinguishedFolderId Id="drafts"/>
      </ToFolderId>
      <ItemIds>
        <t:ItemId Id="AAAtAEF/swbAAA=" ChangeKey="EwAAABYA/s4b"/>
      </ItemIds>
    </MoveItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="736c6-109">Commentaires</span><span class="sxs-lookup"><span data-stu-id="736c6-109">Comments</span></span>

<span data-ttu-id="736c6-110">L’élément [ToFolderId](tofolderid.md) Spécifie le dossier vers lequel les éléments doivent être déplacées.</span><span class="sxs-lookup"><span data-stu-id="736c6-110">The [ToFolderId](tofolderid.md) element specifies the folder to which the items will be moved.</span></span> <span data-ttu-id="736c6-111">Notez que tous les éléments répertoriés dans la collection [ItemId](itemids.md) seront retrouvent dans le dossier de destination.</span><span class="sxs-lookup"><span data-stu-id="736c6-111">Note that all items listed in the [ItemIds](itemids.md) collection will end up in the destination folder.</span></span> <span data-ttu-id="736c6-112">Vous devez effectuer des appels **MoveItem** séparés pour placer les éléments dans les dossiers de destination différents.</span><span class="sxs-lookup"><span data-stu-id="736c6-112">You must make separate **MoveItem** calls to place items in different destination folders.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="736c6-113">L’identificateur d’élément et modifier la clé ont été réduits afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="736c6-113">The item identifier and change key have been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="736c6-114">Éléments de la demande</span><span class="sxs-lookup"><span data-stu-id="736c6-114">Request elements</span></span>

<span data-ttu-id="736c6-115">Les éléments suivants sont utilisés dans la demande :</span><span class="sxs-lookup"><span data-stu-id="736c6-115">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="736c6-116">MoveItem</span><span class="sxs-lookup"><span data-stu-id="736c6-116">MoveItem</span></span>](moveitem.md)
    
- [<span data-ttu-id="736c6-117">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="736c6-117">ToFolderId</span></span>](tofolderid.md)
    
- [<span data-ttu-id="736c6-118">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="736c6-118">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="736c6-119">ItemId</span><span class="sxs-lookup"><span data-stu-id="736c6-119">ItemIds</span></span>](itemids.md)
    
- [<span data-ttu-id="736c6-120">ID d’élément</span><span class="sxs-lookup"><span data-stu-id="736c6-120">ItemId</span></span>](itemid.md)
    
## <a name="moveitem-response-example"></a><span data-ttu-id="736c6-121">Exemple de réponse MoveItem</span><span class="sxs-lookup"><span data-stu-id="736c6-121">MoveItem response example</span></span>

### <a name="description"></a><span data-ttu-id="736c6-122">Description</span><span class="sxs-lookup"><span data-stu-id="736c6-122">Description</span></span>

<span data-ttu-id="736c6-123">L’exemple suivant montre une réponse positive à une demande **MoveItem** .</span><span class="sxs-lookup"><span data-stu-id="736c6-123">The following example shows a successful response to a **MoveItem** request.</span></span> 
  
<span data-ttu-id="736c6-124">L’identificateur d’élément du nouvel élément est retournée dans le message de réponse.</span><span class="sxs-lookup"><span data-stu-id="736c6-124">The item identifier of the new item is returned in the response message.</span></span> <span data-ttu-id="736c6-125">Identificateurs d’éléments ne sont pas retournés dans les réponses pour cross-boîte aux lettres ou aux opérations **MoveItem** de dossier public.</span><span class="sxs-lookup"><span data-stu-id="736c6-125">Item identifiers are not returned in responses for cross-mailbox or mailbox to public folder **MoveItem** operations.</span></span> 
  
### <a name="code"></a><span data-ttu-id="736c6-126">Code</span><span class="sxs-lookup"><span data-stu-id="736c6-126">Code</span></span>

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
    <MoveItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:MoveItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Message>
              <t:ItemID Id="AAMkAd" ChangeKey="FwAAABY" />
            </t:Message>
          </m:Items>
        </m:MoveItemResponseMessage>
      </m:ResponseMessages>
    </MoveItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="736c6-127">Commentaires</span><span class="sxs-lookup"><span data-stu-id="736c6-127">Comments</span></span>

<span data-ttu-id="736c6-128">L’opération **MoveItem** indique réussite si le déplacement a réussi.</span><span class="sxs-lookup"><span data-stu-id="736c6-128">The **MoveItem** operation will indicate success if the move was successful.</span></span> 
  
### <a name="successful-response-elements"></a><span data-ttu-id="736c6-129">Éléments de réponse réussie</span><span class="sxs-lookup"><span data-stu-id="736c6-129">Successful response elements</span></span>

<span data-ttu-id="736c6-130">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="736c6-130">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="736c6-131">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="736c6-131">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="736c6-132">MoveItemResponse</span><span class="sxs-lookup"><span data-stu-id="736c6-132">MoveItemResponse</span></span>](moveitemresponse.md)
    
- [<span data-ttu-id="736c6-133">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="736c6-133">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="736c6-134">MoveItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="736c6-134">MoveItemResponseMessage</span></span>](moveitemresponsemessage.md)
    
- [<span data-ttu-id="736c6-135">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="736c6-135">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="736c6-136">Items</span><span class="sxs-lookup"><span data-stu-id="736c6-136">Items</span></span>](items.md)
    
## <a name="see-also"></a><span data-ttu-id="736c6-137">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="736c6-137">See also</span></span>



- [<span data-ttu-id="736c6-138">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="736c6-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

