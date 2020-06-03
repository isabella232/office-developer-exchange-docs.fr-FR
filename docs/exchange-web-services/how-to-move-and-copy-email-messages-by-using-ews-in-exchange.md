---
title: Déplacer et copier des messages électroniques à l’aide d’EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 4771668f-5623-4397-a5c0-b75a7ba01698
description: Découvrez comment déplacer et copier des messages électroniques à l’aide de l’API managée EWS ou d’EWS dans Exchange.
localization_priority: Priority
ms.openlocfilehash: d13e84648f194dd4f431cf128396daf016addb22
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527935"
---
# <a name="move-and-copy-email-messages-by-using-ews-in-exchange"></a><span data-ttu-id="a43d7-103">Déplacer et copier des messages électroniques à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="a43d7-103">Move and copy email messages by using EWS in Exchange</span></span>

<span data-ttu-id="a43d7-104">Découvrez comment déplacer et copier des messages électroniques à l’aide de l’API managée EWS ou d’EWS dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="a43d7-104">Learn how to move and copy email messages by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="a43d7-105">Vous pouvez utiliser l’API managée EWS ou EWS pour déplacer et copier des messages électroniques dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="a43d7-105">You can use the EWS Managed API or EWS to move and copy email messages in a mailbox.</span></span>
  
<span data-ttu-id="a43d7-106">**Tableau 1. Méthodes d’API managée EWS et opérations EWS pour le transfert et la copie de messages électroniques**</span><span class="sxs-lookup"><span data-stu-id="a43d7-106">**Table 1. EWS Managed API methods and EWS operations for moving and copying email messages**</span></span>

|<span data-ttu-id="a43d7-107">**Tâche**</span><span class="sxs-lookup"><span data-stu-id="a43d7-107">**Task**</span></span>|<span data-ttu-id="a43d7-108">**Méthode d'API managée EWS**</span><span class="sxs-lookup"><span data-stu-id="a43d7-108">**EWS Managed API method**</span></span>|<span data-ttu-id="a43d7-109">**Opération EWS**</span><span class="sxs-lookup"><span data-stu-id="a43d7-109">**EWS operation**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="a43d7-110">Déplacer un message électronique</span><span class="sxs-lookup"><span data-stu-id="a43d7-110">Move an email message</span></span>  <br/> |[<span data-ttu-id="a43d7-111">EmailMessage. Move</span><span class="sxs-lookup"><span data-stu-id="a43d7-111">EmailMessage.Move</span></span>](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.move%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="a43d7-112">MoveItem</span><span class="sxs-lookup"><span data-stu-id="a43d7-112">MoveItem</span></span>](https://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="a43d7-113">Copier un message électronique</span><span class="sxs-lookup"><span data-stu-id="a43d7-113">Copy an email message</span></span>  <br/> |[<span data-ttu-id="a43d7-114">EmailMessage. Copy</span><span class="sxs-lookup"><span data-stu-id="a43d7-114">EmailMessage.Copy</span></span>](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.copy%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="a43d7-115">CopyItem</span><span class="sxs-lookup"><span data-stu-id="a43d7-115">CopyItem</span></span>](https://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> |
   
<span data-ttu-id="a43d7-116">Il est important de noter que lorsque vous déplacez ou copiez un message électronique dans un autre dossier, un nouvel élément est créé dans le nouveau dossier avec un ID d’élément unique et le message d’origine est supprimé.</span><span class="sxs-lookup"><span data-stu-id="a43d7-116">It's important to note that when you move or copy an email message into a different folder, a new item is created in the new folder with a unique item ID, and the original message is deleted.</span></span> <span data-ttu-id="a43d7-117">Si vous déplacez ou copiez un message électronique entre deux dossiers dans la même boîte aux lettres, le nouvel élément est renvoyé dans la réponse, qui vous donne accès au nouvel ID d’élément.</span><span class="sxs-lookup"><span data-stu-id="a43d7-117">If you're moving or copying an email message between two folders in the same mailbox, the new item is returned in the response, which gives you access to the new item ID.</span></span> <span data-ttu-id="a43d7-118">Toutefois, si vous déplacez ou copiez un message électronique entre deux boîtes aux lettres ou entre une boîte aux lettres et un dossier public, le nouvel élément n’est pas renvoyé dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="a43d7-118">However, if you're moving or copying an email message between two mailboxes or between a mailbox and a public folder, the new item is not returned in the response.</span></span> <span data-ttu-id="a43d7-119">Pour accéder au message déplacé dans ce scénario, utilisez la méthode [FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) de l’API managée EWS ou l’opération EWS [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) , [créez une définition de propriété étendue](properties-and-extended-properties-in-ews-in-exchange.md) pour la propriété [PidTagSearchKey](https://msdn.microsoft.com/library/cc839918.aspx) (0x300B0102) ou créez et définissez une propriété étendue personnalisée, puis recherchez la propriété étendue personnalisée dans le nouveau dossier.</span><span class="sxs-lookup"><span data-stu-id="a43d7-119">To access the moved message in that scenario, use the EWS Managed API [FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) method or EWS [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) operation, [create an extended property definition](properties-and-extended-properties-in-ews-in-exchange.md) for the [PidTagSearchKey](https://msdn.microsoft.com/library/cc839918.aspx) (0x300B0102) property, or create and set a custom extended property and then search for the custom extended property in the new folder.</span></span> 
  
<span data-ttu-id="a43d7-120">La suppression d’un message électronique est différente de celle du transfert d’un élément dans le dossier éléments supprimés.</span><span class="sxs-lookup"><span data-stu-id="a43d7-120">Deleting an email message is different than moving an item to the Deleted Items folder.</span></span> <span data-ttu-id="a43d7-121">Si vous utilisez l’élément de l’API managée EWS [. Delete](https://msdn.microsoft.com/library/office/dd635072%28v=exchg.80%29.aspx) ou [l’opération EWS](../web-service-reference/deleteitem-operation.md) EWS, l’élément spécifié dans la demande est supprimé du dossier d’origine, et une copie est placée dans le dossier éléments supprimés avec un nouvel ID d’élément.</span><span class="sxs-lookup"><span data-stu-id="a43d7-121">If you use the EWS Managed API [Item.Delete](https://msdn.microsoft.com/library/office/dd635072%28v=exchg.80%29.aspx) method or the EWS [DeleteItem](../web-service-reference/deleteitem-operation.md) operation, the item specified in the request is removed from the original folder, and a copy is placed in the Deleted Items folder with a new item ID.</span></span> <span data-ttu-id="a43d7-122">Contrairement à ce qui se passe lorsque vous déplacez ou copiez un élément, le nouvel élément n’est pas renvoyé dans la méthode **Delete** ou la réponse de l’opération **DeleteItem** .</span><span class="sxs-lookup"><span data-stu-id="a43d7-122">Unlike when you move or copy any item, the new item is not returned in the **Delete** method or the **DeleteItem** operation response.</span></span> <span data-ttu-id="a43d7-123">La procédure de [Suppression d’un courrier électronique à l’aide de l’API managée EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteewsma) ou [EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteews) est identique à celle de la suppression d’un élément générique de la Banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="a43d7-123">The steps involved in [deleting an email by using the EWS Managed API](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteewsma) or [EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteews) are the same as those for deleting any generic item from the Exchange store.</span></span> 
  
## <a name="move-an-email-message-by-using-the-ews-managed-api"></a><span data-ttu-id="a43d7-124">Déplacer un message électronique à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="a43d7-124">Move an email message by using the EWS Managed API</span></span>
<span data-ttu-id="a43d7-125"><a name="bk_moveewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="a43d7-125"><a name="bk_moveewsma"> </a></span></span>

<span data-ttu-id="a43d7-126">L’exemple de code suivant montre comment utiliser la méthode [EmailMessage. Move](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.move%28v=exchg.80%29.aspx) pour déplacer un message électronique existant d’un dossier à un autre.</span><span class="sxs-lookup"><span data-stu-id="a43d7-126">The following code example shows how to use the [EmailMessage.Move](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.move%28v=exchg.80%29.aspx) method to move an existing email message from one folder to another.</span></span> 
  
<span data-ttu-id="a43d7-127">Cet exemple part du principe que le **service** est un objet [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’ID **ItemId** est l' [ID](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) du message électronique à déplacer ou à copier.</span><span class="sxs-lookup"><span data-stu-id="a43d7-127">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, and that **ItemId** is the [Id](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) of the email message to move or copy.</span></span> 
  
```cs
// As a best practice, limit the properties returned by the Bind method to only those that are required.
PropertySet propSet = new PropertySet(BasePropertySet.IdOnly, EmailMessageSchema.Subject, EmailMessageSchema.ParentFolderId);
// Bind to the existing item by using the ItemId.
// This method call results in a GetItem call to EWS.
EmailMessage beforeMessage = EmailMessage.Bind(service, ItemId, propSet);
// Move the specified mail to the JunkEmail folder and store the returned item.
Item item = beforeMessage.Move(WellKnownFolderName.JunkEmail);
// Check that the item was moved by binding to the moved email message 
// and retrieving the new ParentFolderId.
// This method call results in a GetItem call to EWS.
EmailMessage movedMessage = EmailMessage.Bind(service, item.Id, propSet);
Console.WriteLine("An email message with the subject '" + beforeMessage.Subject + "' has been moved from the '" + beforeMessage.ParentFolderId + "' folder to the '" + movedMessage.ParentFolderId + "' folder.");
```

## <a name="move-an-email-message-by-using-ews"></a><span data-ttu-id="a43d7-128">Déplacer un message électronique à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="a43d7-128">Move an email message by using EWS</span></span>
<span data-ttu-id="a43d7-129"><a name="bk_moveews"> </a></span><span class="sxs-lookup"><span data-stu-id="a43d7-129"><a name="bk_moveews"> </a></span></span>

<span data-ttu-id="a43d7-130">L’exemple de code suivant montre comment utiliser l’opération [MoveItem](https://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) pour déplacer un message électronique dans le dossier courrier indésirable.</span><span class="sxs-lookup"><span data-stu-id="a43d7-130">The following code example shows how to use the [MoveItem](https://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) operation to move an email message to the Junk Email folder.</span></span> 
  
<span data-ttu-id="a43d7-131">Il s’agit également de la requête XML envoyée par l’API managée EWS lors de l’appel de la méthode [Move](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.move%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="a43d7-131">This is also the XML request that is sent by the EWS Managed API when calling the [Move](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.move%28v=exchg.80%29.aspx) method.</span></span> <span data-ttu-id="a43d7-132">Les valeurs de certains attributs et éléments ont été raccourcies pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="a43d7-132">The values of some attributes and elements have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
  <soap:Body>
    <m:MoveItem>
      <m:ToFolderId>
        <t:DistinguishedFolderId Id="junkemail" />
      </m:ToFolderId>
      <m:ItemIds>
        <t:ItemId Id="AfwDoAAA="
                  ChangeKey="CQAAABYAAAApjGm7TnMWQ5TzjbhziLL0AAF25sM1" />
      </m:ItemIds>
    </m:MoveItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="a43d7-133">Le serveur répond à la demande **MoveItem** avec un message [MoveItemResponse](https://msdn.microsoft.com/library/77be5104-1e09-4d50-abec-4fadb3a230e5%28Office.15%29.aspx) qui inclut une valeur [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NOERROR**, ce qui indique que le message électronique a été déplacé avec succès.</span><span class="sxs-lookup"><span data-stu-id="a43d7-133">The server responds to the **MoveItem** request with a [MoveItemResponse](https://msdn.microsoft.com/library/77be5104-1e09-4d50-abec-4fadb3a230e5%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates that the email message was moved successfully.</span></span> <span data-ttu-id="a43d7-134">La réponse inclut également l' **ItemId** pour le message électronique dans le nouveau dossier, ce qui est important pour le stockage car l' **ItemId** est différent dans le nouveau dossier.</span><span class="sxs-lookup"><span data-stu-id="a43d7-134">The response also includes the **ItemId** for the email message in the new folder, which is important to store because the **ItemId** is different in the new folder.</span></span> 
  
## <a name="copy-an-email-message-by-using-the-ews-managed-api"></a><span data-ttu-id="a43d7-135">Copier un message électronique à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="a43d7-135">Copy an email message by using the EWS Managed API</span></span>
<span data-ttu-id="a43d7-136"><a name="bk_copyewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="a43d7-136"><a name="bk_copyewsma"> </a></span></span>

<span data-ttu-id="a43d7-137">L’exemple de code suivant montre comment utiliser la méthode [EmailMessage. Copy](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.copy%28v=exchg.80%29.aspx) pour copier un message électronique existant d’un dossier vers un autre.</span><span class="sxs-lookup"><span data-stu-id="a43d7-137">The following code example shows how to use the [EmailMessage.Copy](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.copy%28v=exchg.80%29.aspx) method to copy an existing email message from one folder to another.</span></span> 
  
<span data-ttu-id="a43d7-138">Cet exemple part du principe que le **service** est un objet [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’ID **ItemId** est l' [ID](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) du message électronique à copier.</span><span class="sxs-lookup"><span data-stu-id="a43d7-138">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, and that **ItemId** is the [Id](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) of the email message to copy.</span></span> <span data-ttu-id="a43d7-139">Les valeurs de certains paramètres ont été raccourcies pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="a43d7-139">The values of some parameters have been shortened for readability.</span></span> 
  
```cs
// As a best practice, limit the properties returned by the Bind method to only those that are required.
PropertySet propSet = new PropertySet(BasePropertySet.IdOnly, EmailMessageSchema.Subject, EmailMessageSchema.ParentFolderId);
// Bind to the existing item by using the ItemId.
// This method call results in a GetItem call to EWS.
EmailMessage originalMessage = EmailMessage.Bind(service, ItemId, propSet);
// Copy the orignal message into another folder in the mailbox and store the returned item.
Item item = originalMessage.Copy("epQ/3AAA=");
// Check that the item was copied by binding to the copied email message 
// and retrieving the new ParentFolderId.
// This method call results in a GetItem call to EWS.
EmailMessage copiedMessage = EmailMessage.Bind(service, item.Id, propSet);
Console.WriteLine("An email message with the subject '" + originalMessage.Subject + "' has been copied from the '" + originalMessage.ParentFolderId + "' folder to the '" + copiedMessage.ParentFolderId + "' folder.");
```

## <a name="copy-an-email-message-by-using-ews"></a><span data-ttu-id="a43d7-140">Copier un message électronique à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="a43d7-140">Copy an email message by using EWS</span></span>
<span data-ttu-id="a43d7-141"><a name="bk_copyews"> </a></span><span class="sxs-lookup"><span data-stu-id="a43d7-141"><a name="bk_copyews"> </a></span></span>

<span data-ttu-id="a43d7-142">L’exemple de code suivant montre comment utiliser l’opération [CopyItem](https://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) pour copier un message électronique dans un autre dossier de la même boîte aux lettres en envoyant l' [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) du message électronique à déplacer et en spécifiant le dossier de destination dans l’élément [ToFolderId](https://msdn.microsoft.com/library/bd6a4265-ad40-43f6-bcc4-0bf5df4e984c%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="a43d7-142">The following code example shows how to use the [CopyItem](https://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) operation to copy an email message to different folder in the same mailbox by sending the [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) of the email message to move, and specifying the destination folder in the [ToFolderId](https://msdn.microsoft.com/library/bd6a4265-ad40-43f6-bcc4-0bf5df4e984c%28Office.15%29.aspx) element.</span></span> 
  
<span data-ttu-id="a43d7-143">Il s’agit également de la requête XML envoyée par l’API managée EWS lors de l’appel de la méthode [Copy](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.copy%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="a43d7-143">This is also the XML request that is sent by the EWS Managed API when calling the [Copy](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.copy%28v=exchg.80%29.aspx) method.</span></span> <span data-ttu-id="a43d7-144">Les valeurs de certains attributs et éléments ont été raccourcies pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="a43d7-144">The values of some attributes and elements have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
  <soap:Body>
    <m:CopyItem>
      <m:ToFolderId>
        <t:FolderId Id="pQ/3AAA=" />
      </m:ToFolderId>
      <m:ItemIds>
        <t:ItemId Id="2TSeSAAA="
                  ChangeKey="CQAAABYAAAApjGm7TnMWQ5TzjbhziLL0AAF2d+3+" />
      </m:ItemIds>
    </m:CopyItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="a43d7-145">Le serveur répond à la demande **CopyItem** avec un message [CopyItemResponse](https://msdn.microsoft.com/library/ae402bc1-4589-45e0-a929-f368c916a7e4%28Office.15%29.aspx) qui inclut une valeur [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NOERROR**, ce qui indique que le message électronique a été correctement copié.</span><span class="sxs-lookup"><span data-stu-id="a43d7-145">The server responds to the **CopyItem** request with a [CopyItemResponse](https://msdn.microsoft.com/library/ae402bc1-4589-45e0-a929-f368c916a7e4%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates that the email message was copied successfully.</span></span> <span data-ttu-id="a43d7-146">La réponse inclut également l' **ItemId** pour le message électronique dans le nouveau dossier, ce qui est important pour le stockage car l' **ItemId** est différent dans le nouveau dossier.</span><span class="sxs-lookup"><span data-stu-id="a43d7-146">The response also includes the **ItemId** for the email message in the new folder, which is important to store because the **ItemId** is different in the new folder.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="a43d7-147">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a43d7-147">See also</span></span>


- [<span data-ttu-id="a43d7-148">Courrier électronique et les services EWS d'Exchange</span><span class="sxs-lookup"><span data-stu-id="a43d7-148">Email and EWS in Exchange</span></span>](email-and-ews-in-exchange.md)
    
- [<span data-ttu-id="a43d7-149">Envoyer des messages électroniques à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="a43d7-149">Send email messages by using EWS in Exchange</span></span>](how-to-send-email-messages-by-using-ews-in-exchange.md)
    

