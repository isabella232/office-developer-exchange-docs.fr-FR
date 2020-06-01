---
title: Opération MoveItem
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
description: L’opération MoveItem est utilisée pour déplacer un ou plusieurs éléments dans un seul dossier de destination.
ms.openlocfilehash: 6a455e483ad2e5c84b91cfaa7562f4f1ec46a112
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465680"
---
# <a name="moveitem-operation"></a><span data-ttu-id="a03c3-103">Opération MoveItem</span><span class="sxs-lookup"><span data-stu-id="a03c3-103">MoveItem operation</span></span>

<span data-ttu-id="a03c3-104">L’opération **MoveItem** est utilisée pour déplacer un ou plusieurs éléments dans un seul dossier de destination.</span><span class="sxs-lookup"><span data-stu-id="a03c3-104">The **MoveItem** operation is used to move one or more items to a single destination folder.</span></span> 
  
## <a name="moveitem-request-example"></a><span data-ttu-id="a03c3-105">Exemple de requête MoveItem</span><span class="sxs-lookup"><span data-stu-id="a03c3-105">MoveItem request example</span></span>

### <a name="description"></a><span data-ttu-id="a03c3-106">Description</span><span class="sxs-lookup"><span data-stu-id="a03c3-106">Description</span></span>

<span data-ttu-id="a03c3-107">L’exemple de requête **MoveItem** suivant montre comment déplacer un élément vers le dossier Brouillons.</span><span class="sxs-lookup"><span data-stu-id="a03c3-107">The following example of a **MoveItem** request shows how to move an item to the Drafts folder.</span></span> 
  
### <a name="code"></a><span data-ttu-id="a03c3-108">Code</span><span class="sxs-lookup"><span data-stu-id="a03c3-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
xmlns:xsd="http://www.w3.org/2001/XMLSchema"
xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <MoveItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

### <a name="comments"></a><span data-ttu-id="a03c3-109">Commentaires</span><span class="sxs-lookup"><span data-stu-id="a03c3-109">Comments</span></span>

<span data-ttu-id="a03c3-110">L’élément [ToFolderId](tofolderid.md) spécifie le dossier vers lequel les éléments seront déplacés.</span><span class="sxs-lookup"><span data-stu-id="a03c3-110">The [ToFolderId](tofolderid.md) element specifies the folder to which the items will be moved.</span></span> <span data-ttu-id="a03c3-111">Notez que tous les éléments figurant dans la collection [ItemIds](itemids.md) finissent dans le dossier de destination.</span><span class="sxs-lookup"><span data-stu-id="a03c3-111">Note that all items listed in the [ItemIds](itemids.md) collection will end up in the destination folder.</span></span> <span data-ttu-id="a03c3-112">Vous devez effectuer des appels **MoveItem** distincts pour placer des éléments dans différents dossiers de destination.</span><span class="sxs-lookup"><span data-stu-id="a03c3-112">You must make separate **MoveItem** calls to place items in different destination folders.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="a03c3-113">L’identificateur d’élément et la clé de modification ont été raccourcies afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="a03c3-113">The item identifier and change key have been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="a03c3-114">Demander des éléments</span><span class="sxs-lookup"><span data-stu-id="a03c3-114">Request elements</span></span>

<span data-ttu-id="a03c3-115">Les éléments suivants sont utilisés dans la demande :</span><span class="sxs-lookup"><span data-stu-id="a03c3-115">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="a03c3-116">MoveItem</span><span class="sxs-lookup"><span data-stu-id="a03c3-116">MoveItem</span></span>](moveitem.md)
    
- [<span data-ttu-id="a03c3-117">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="a03c3-117">ToFolderId</span></span>](tofolderid.md)
    
- [<span data-ttu-id="a03c3-118">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="a03c3-118">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="a03c3-119">ItemIds</span><span class="sxs-lookup"><span data-stu-id="a03c3-119">ItemIds</span></span>](itemids.md)
    
- [<span data-ttu-id="a03c3-120">ItemId</span><span class="sxs-lookup"><span data-stu-id="a03c3-120">ItemId</span></span>](itemid.md)
    
## <a name="moveitem-response-example"></a><span data-ttu-id="a03c3-121">Exemple de réponse MoveItem</span><span class="sxs-lookup"><span data-stu-id="a03c3-121">MoveItem response example</span></span>

### <a name="description"></a><span data-ttu-id="a03c3-122">Description</span><span class="sxs-lookup"><span data-stu-id="a03c3-122">Description</span></span>

<span data-ttu-id="a03c3-123">L’exemple suivant montre une réponse réussie à une demande **MoveItem** .</span><span class="sxs-lookup"><span data-stu-id="a03c3-123">The following example shows a successful response to a **MoveItem** request.</span></span> 
  
<span data-ttu-id="a03c3-124">L’identificateur d’élément du nouvel élément est renvoyé dans le message de réponse.</span><span class="sxs-lookup"><span data-stu-id="a03c3-124">The item identifier of the new item is returned in the response message.</span></span> <span data-ttu-id="a03c3-125">Les identificateurs d’élément ne sont pas renvoyés dans les réponses pour les opérations entre boîtes aux lettres ou boîtes aux lettres dans les **MoveItem** de dossiers publics.</span><span class="sxs-lookup"><span data-stu-id="a03c3-125">Item identifiers are not returned in responses for cross-mailbox or mailbox to public folder **MoveItem** operations.</span></span> 
  
### <a name="code"></a><span data-ttu-id="a03c3-126">Code</span><span class="sxs-lookup"><span data-stu-id="a03c3-126">Code</span></span>

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
    <MoveItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="a03c3-127">Commentaires</span><span class="sxs-lookup"><span data-stu-id="a03c3-127">Comments</span></span>

<span data-ttu-id="a03c3-128">L’opération **MoveItem** indique la réussite si le déplacement a réussi.</span><span class="sxs-lookup"><span data-stu-id="a03c3-128">The **MoveItem** operation will indicate success if the move was successful.</span></span> 
  
### <a name="successful-response-elements"></a><span data-ttu-id="a03c3-129">Éléments de réponse réussis</span><span class="sxs-lookup"><span data-stu-id="a03c3-129">Successful response elements</span></span>

<span data-ttu-id="a03c3-130">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="a03c3-130">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="a03c3-131">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="a03c3-131">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="a03c3-132">MoveItemResponse</span><span class="sxs-lookup"><span data-stu-id="a03c3-132">MoveItemResponse</span></span>](moveitemresponse.md)
    
- [<span data-ttu-id="a03c3-133">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="a03c3-133">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="a03c3-134">MoveItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="a03c3-134">MoveItemResponseMessage</span></span>](moveitemresponsemessage.md)
    
- [<span data-ttu-id="a03c3-135">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="a03c3-135">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="a03c3-136">Items</span><span class="sxs-lookup"><span data-stu-id="a03c3-136">Items</span></span>](items.md)
    
## <a name="see-also"></a><span data-ttu-id="a03c3-137">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a03c3-137">See also</span></span>



- [<span data-ttu-id="a03c3-138">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="a03c3-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

