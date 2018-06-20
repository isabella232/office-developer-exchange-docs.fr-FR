---
title: Opération DeleteItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteItem
api_type:
- schema
ms.assetid: 3e26c416-fa12-476e-bfd2-5c1f4bb7b348
description: L’opération DeleteItem supprime les éléments de la banque d’informations Exchange.
ms.openlocfilehash: 87d7853daa5db0cd87b3f6469c228a584b4d9caf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755869"
---
# <a name="deleteitem-operation"></a><span data-ttu-id="7c724-103">Opération DeleteItem</span><span class="sxs-lookup"><span data-stu-id="7c724-103">DeleteItem operation</span></span>

<span data-ttu-id="7c724-104">L’opération **DeleteItem** supprime les éléments de la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="7c724-104">The **DeleteItem** operation deletes items in the Exchange store.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="7c724-105">Une réponse d’erreur qui inclut le code d’erreur ErrorCannotDeleteObject s’afficheront pour une opération **DeleteItem** lorsqu’un délégué tente de supprimer un élément dans la boîte aux lettres de l’entité de sécurité en définissant le DisposalType à MoveToDeletedItems.</span><span class="sxs-lookup"><span data-stu-id="7c724-105">An error response that includes the ErrorCannotDeleteObject error code will be returned for a **DeleteItem** operation when a delegate tries to delete an item in the principal's mailbox by setting the DisposalType to MoveToDeletedItems.</span></span> <span data-ttu-id="7c724-106">Pour supprimer un élément en le faisant glisser vers le dossier éléments supprimés, un délégué doit utiliser l' [opération MoveItem](moveitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="7c724-106">To delete an item by moving it to the Deleted Items folder, a delegate must use the [MoveItem operation](moveitem-operation.md).</span></span> 
  
## <a name="deleteitem-request-example"></a><span data-ttu-id="7c724-107">Exemple de requête DeleteItem</span><span class="sxs-lookup"><span data-stu-id="7c724-107">DeleteItem request example</span></span>

### <a name="description"></a><span data-ttu-id="7c724-108">Description</span><span class="sxs-lookup"><span data-stu-id="7c724-108">Description</span></span>

<span data-ttu-id="7c724-109">L’exemple suivant d’une demande **DeleteItem** indique comment effectuer une suppression définitive d’un élément à partir d’une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="7c724-109">The following example of a **DeleteItem** request shows how to perform a hard delete of an item from a mailbox.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="7c724-110">L’ID d’élément a été raccourcie afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="7c724-110">The item ID has been shortened to preserve readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="7c724-111">Code</span><span class="sxs-lookup"><span data-stu-id="7c724-111">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <DeleteItem DeleteType="HardDelete" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ItemIds>
        <t:ItemId Id="AS4AUn=="/>
      </ItemIds>
    </DeleteItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="7c724-112">Éléments de la demande</span><span class="sxs-lookup"><span data-stu-id="7c724-112">Request elements</span></span>

<span data-ttu-id="7c724-113">Les éléments suivants sont utilisés dans la demande :</span><span class="sxs-lookup"><span data-stu-id="7c724-113">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="7c724-114">DeleteItem</span><span class="sxs-lookup"><span data-stu-id="7c724-114">DeleteItem</span></span>](deleteitem.md)
    
- [<span data-ttu-id="7c724-115">ItemId</span><span class="sxs-lookup"><span data-stu-id="7c724-115">ItemIds</span></span>](itemids.md)
    
- [<span data-ttu-id="7c724-116">ID d’élément</span><span class="sxs-lookup"><span data-stu-id="7c724-116">ItemId</span></span>](itemid.md)
    
<span data-ttu-id="7c724-117">Pour trouver d’autres options pour le message de demande de l’opération **DeleteItem** , explorez la hiérarchie de schéma.</span><span class="sxs-lookup"><span data-stu-id="7c724-117">To find other options for the request message of the **DeleteItem** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="7c724-118">Commencer à l’élément [DeleteItem](deleteitem.md) .</span><span class="sxs-lookup"><span data-stu-id="7c724-118">Start at the [DeleteItem](deleteitem.md) element.</span></span> 
  
## <a name="successful-deleteitem-response"></a><span data-ttu-id="7c724-119">Réponse DeleteItem réussie</span><span class="sxs-lookup"><span data-stu-id="7c724-119">Successful DeleteItem response</span></span>

### <a name="description"></a><span data-ttu-id="7c724-120">Description</span><span class="sxs-lookup"><span data-stu-id="7c724-120">Description</span></span>

<span data-ttu-id="7c724-121">L’exemple suivant montre une réponse positive à la demande **DeleteItem** .</span><span class="sxs-lookup"><span data-stu-id="7c724-121">The following example shows a successful response to the **DeleteItem** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="7c724-122">Code</span><span class="sxs-lookup"><span data-stu-id="7c724-122">Code</span></span>

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
    <DeleteItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:DeleteItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:DeleteItemResponseMessage>
      </m:ResponseMessages>
    </DeleteItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a><span data-ttu-id="7c724-123">Éléments de réponse réussie</span><span class="sxs-lookup"><span data-stu-id="7c724-123">Successful response elements</span></span>

<span data-ttu-id="7c724-124">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="7c724-124">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="7c724-125">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="7c724-125">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="7c724-126">DeleteItemResponse</span><span class="sxs-lookup"><span data-stu-id="7c724-126">DeleteItemResponse</span></span>](deleteitemresponse.md)
    
- [<span data-ttu-id="7c724-127">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="7c724-127">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="7c724-128">DeleteItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="7c724-128">DeleteItemResponseMessage</span></span>](deleteitemresponsemessage.md)
    
- [<span data-ttu-id="7c724-129">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="7c724-129">ResponseCode</span></span>](responsecode.md)
    
<span data-ttu-id="7c724-130">Pour trouver d’autres options pour le message de réponse de l’opération **DeleteItem** , explorez la hiérarchie de schéma.</span><span class="sxs-lookup"><span data-stu-id="7c724-130">To find other options for the response message of the **DeleteItem** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="7c724-131">Démarrez au niveau de l’élément [DeleteItemResponse](deleteitemresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="7c724-131">Start at the [DeleteItemResponse](deleteitemresponse.md) element.</span></span> 
  
## <a name="deleteitem-error-response"></a><span data-ttu-id="7c724-132">Réponse d’erreur DeleteItem</span><span class="sxs-lookup"><span data-stu-id="7c724-132">DeleteItem error response</span></span>

### <a name="description"></a><span data-ttu-id="7c724-133">Description</span><span class="sxs-lookup"><span data-stu-id="7c724-133">Description</span></span>

<span data-ttu-id="7c724-134">L’exemple suivant montre une réponse d’erreur à une demande **DeleteItem** .</span><span class="sxs-lookup"><span data-stu-id="7c724-134">The following example shows an error response to a **DeleteItem** request.</span></span> <span data-ttu-id="7c724-135">L’erreur a été créé, car l’opération a tenté de supprimer un élément est introuvable dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="7c724-135">The error was created because the operation tried to delete an item that was not found in the Exchange store.</span></span> 
  
### <a name="code"></a><span data-ttu-id="7c724-136">Code</span><span class="sxs-lookup"><span data-stu-id="7c724-136">Code</span></span>

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
    <DeleteItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:DeleteItemResponseMessage ResponseClass="Error">
          <m:MessageText>The specified object was not found in the store.</m:MessageText>
          <m:ResponseCode>ErrorItemNotFound</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:DeleteItemResponseMessage>
      </m:ResponseMessages>
    </DeleteItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="7c724-137">Éléments de réponse d’erreur</span><span class="sxs-lookup"><span data-stu-id="7c724-137">Error response elements</span></span>

<span data-ttu-id="7c724-138">Les éléments suivants sont utilisés dans la réponse d'erreur :</span><span class="sxs-lookup"><span data-stu-id="7c724-138">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="7c724-139">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="7c724-139">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="7c724-140">DeleteItemResponse</span><span class="sxs-lookup"><span data-stu-id="7c724-140">DeleteItemResponse</span></span>](deleteitemresponse.md)
    
- [<span data-ttu-id="7c724-141">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="7c724-141">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="7c724-142">DeleteItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="7c724-142">DeleteItemResponseMessage</span></span>](deleteitemresponsemessage.md)
    
- [<span data-ttu-id="7c724-143">MessageText</span><span class="sxs-lookup"><span data-stu-id="7c724-143">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="7c724-144">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="7c724-144">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="7c724-145">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="7c724-145">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="7c724-146">Pour trouver d’autres options pour le message de réponse de l’opération **DeleteItem** , explorez la hiérarchie de schéma.</span><span class="sxs-lookup"><span data-stu-id="7c724-146">To find other options for the error response message of the **DeleteItem** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="7c724-147">Démarrez au niveau de l’élément [DeleteItemResponse](deleteitemresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="7c724-147">Start at the [DeleteItemResponse](deleteitemresponse.md) element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="7c724-148">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7c724-148">See also</span></span>

- [<span data-ttu-id="7c724-149">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="7c724-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="7c724-150">Deleting Contacts</span><span class="sxs-lookup"><span data-stu-id="7c724-150">Deleting Contacts</span></span>](http://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)  
- [<span data-ttu-id="7c724-151">Suppression de Messages électroniques</span><span class="sxs-lookup"><span data-stu-id="7c724-151">Deleting E-mail Messages</span></span>](http://msdn.microsoft.com/library/c40f2f0b-dae0-412f-b716-727e8c0949b4%28Office.15%29.aspx) 
- [<span data-ttu-id="7c724-152">Suppression de tâches</span><span class="sxs-lookup"><span data-stu-id="7c724-152">Deleting Tasks</span></span>](http://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)
