---
title: Supprimez les pièces jointes à l’aide de EWS dans Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 71871ac7-ee1a-4f93-9e81-77f312d432f4
description: Découvrez comment supprimer les pièces jointes à partir des éléments à l’aide de l’API managée EWS ou EWS dans Exchange.
ms.openlocfilehash: 458331f81493283efc20d24c7e2bebe0e74bbdbd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754830"
---
# <a name="delete-attachments-by-using-ews-in-exchange"></a><span data-ttu-id="3f0f9-103">Supprimez les pièces jointes à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="3f0f9-103">Delete attachments by using EWS in Exchange</span></span>

<span data-ttu-id="3f0f9-104">Découvrez comment supprimer les pièces jointes à partir des éléments à l’aide de l’API managée EWS ou EWS dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="3f0f9-104">Learn how to delete attachments from items by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="3f0f9-105">Vous avez un certain nombre d’options en matière de suppression du fichier et les pièces jointes d’éléments à partir des éléments à l’aide de l’API managée EWS.</span><span class="sxs-lookup"><span data-stu-id="3f0f9-105">You have a number of options when it comes to deleting file and item attachments from items by using the EWS Managed API.</span></span> <span data-ttu-id="3f0f9-106">Vous pouvez supprimer toutes les pièces jointes à partir du message, supprimez par un nom de fichier ou supprimer par sa position dans la collection.</span><span class="sxs-lookup"><span data-stu-id="3f0f9-106">You can delete all the attachments from the message, delete by a file name, or delete by position in the collection.</span></span> <span data-ttu-id="3f0f9-107">Pour chacune de ces options, il existe une méthode [AttachmentCollection](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.attachmentcollection%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="3f0f9-107">For each of these options, there is an [AttachmentCollection](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.attachmentcollection%28v=exchg.80%29.aspx) method.</span></span> 
  
<span data-ttu-id="3f0f9-108">À l’inverse, avec EWS, quel que soit le si vous souhaitez supprimer toutes les pièces jointes à partir d’un élément ou un seul, la séquence d’opérations est identique.</span><span class="sxs-lookup"><span data-stu-id="3f0f9-108">Conversely, with EWS, no matter whether you're deleting all attachments from an item or just one, the sequence of operations is same.</span></span> <span data-ttu-id="3f0f9-109">Contrairement à l’API managée EWS, EWS n’inclut pas les opérations distinctes pour supprimer basé sur le nom ou la position dans le tableau pièces jointes.</span><span class="sxs-lookup"><span data-stu-id="3f0f9-109">Unlike the EWS Managed API, EWS does not include separate operations to delete based on name or position in the attachments array.</span></span>
  
<span data-ttu-id="3f0f9-110">**Le tableau 1. Méthodes d’API managées et opérations EWS pour supprimer les pièces jointes**</span><span class="sxs-lookup"><span data-stu-id="3f0f9-110">**Table 1. EWS Managed API methods and EWS operations for deleting attachments**</span></span>

|<span data-ttu-id="3f0f9-111">**Tâche**</span><span class="sxs-lookup"><span data-stu-id="3f0f9-111">**Task**</span></span>|<span data-ttu-id="3f0f9-112">**Méthode d'API managée EWS**</span><span class="sxs-lookup"><span data-stu-id="3f0f9-112">**EWS Managed API method**</span></span>|<span data-ttu-id="3f0f9-113">**Opération EWS**</span><span class="sxs-lookup"><span data-stu-id="3f0f9-113">**EWS operation**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="3f0f9-114">Supprimer toutes les pièces jointes d’un élément.</span><span class="sxs-lookup"><span data-stu-id="3f0f9-114">Delete all attachments from an item.</span></span>  <br/> |<span data-ttu-id="3f0f9-115">[Item.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx), suivi [AttachmentCollection.Clear](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.attachmentcollection.clear%28v=exchg.80%29.aspx), suivi de [EmailMessage.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="3f0f9-115">[Item.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx), followed by [AttachmentCollection.Clear](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.attachmentcollection.clear%28v=exchg.80%29.aspx), followed by [EmailMessage.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx)</span></span> <br/> |<span data-ttu-id="3f0f9-116">[GetItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) suivi [DeleteAttachment](http://msdn.microsoft.com/library/43d0c1cb-92ca-4399-9b3a-acb2b5c22624%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="3f0f9-116">[GetItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) followed by [DeleteAttachment](http://msdn.microsoft.com/library/43d0c1cb-92ca-4399-9b3a-acb2b5c22624%28Office.15%29.aspx)</span></span> <br/> |
|<span data-ttu-id="3f0f9-117">Supprimer une pièce jointe d’un élément par nom.</span><span class="sxs-lookup"><span data-stu-id="3f0f9-117">Delete an attachment from an item by name.</span></span>  <br/> |<span data-ttu-id="3f0f9-118">[Item.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx), suivi [AttachmentCollection.Remove](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.attachmentcollection.remove%28v=exchg.80%29.aspx), suivi de [EmailMessage.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="3f0f9-118">[Item.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx), followed by [AttachmentCollection.Remove](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.attachmentcollection.remove%28v=exchg.80%29.aspx), followed by [EmailMessage.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx)</span></span> <br/> |<span data-ttu-id="3f0f9-119">[GetItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) suivi [DeleteAttachment](http://msdn.microsoft.com/library/43d0c1cb-92ca-4399-9b3a-acb2b5c22624%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="3f0f9-119">[GetItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) followed by [DeleteAttachment](http://msdn.microsoft.com/library/43d0c1cb-92ca-4399-9b3a-acb2b5c22624%28Office.15%29.aspx)</span></span> <br/> |
|<span data-ttu-id="3f0f9-120">Supprimer une pièce jointe d’un élément par sa position dans la collection.</span><span class="sxs-lookup"><span data-stu-id="3f0f9-120">Delete an attachment from an item by position in the collection.</span></span>  <br/> |<span data-ttu-id="3f0f9-121">[Item.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx), suivi [AttachmentCollection.RemoveAt](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.attachmentcollection.removeat%28v=exchg.80%29.aspx), suivi de [EmailMessage.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="3f0f9-121">[Item.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx), followed by [AttachmentCollection.RemoveAt](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.attachmentcollection.removeat%28v=exchg.80%29.aspx), followed by [EmailMessage.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx)</span></span> <br/> |<span data-ttu-id="3f0f9-122">[GetItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) suivi [DeleteAttachment](http://msdn.microsoft.com/library/43d0c1cb-92ca-4399-9b3a-acb2b5c22624%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="3f0f9-122">[GetItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) followed by [DeleteAttachment](http://msdn.microsoft.com/library/43d0c1cb-92ca-4399-9b3a-acb2b5c22624%28Office.15%29.aspx)</span></span> <br/> |
   
## <a name="delete-all-attachments-from-an-email-by-using-the-ews-managed-api"></a><span data-ttu-id="3f0f9-123">Supprimer toutes les pièces jointes à partir d’un message électronique à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="3f0f9-123">Delete all attachments from an email by using the EWS Managed API</span></span>
<span data-ttu-id="3f0f9-124"><a name="bk_deleteattachewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="3f0f9-124"></span></span>

<span data-ttu-id="3f0f9-125">L’exemple de code suivant montre comment supprimer toutes les pièces jointes dans un message électronique à :</span><span class="sxs-lookup"><span data-stu-id="3f0f9-125">The following code example shows how to delete all attachments from an email by:</span></span>
  
1. <span data-ttu-id="3f0f9-126">À l’aide de la méthode [EmailMessage.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) pour récupérer la collection de [pièces jointes](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.attachments%28v=exchg.80%29.aspx)et les lier à un message électronique existant.</span><span class="sxs-lookup"><span data-stu-id="3f0f9-126">Using the [EmailMessage.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) method to bind to an existing email message and retrieve the collection of [Attachments](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.attachments%28v=exchg.80%29.aspx).</span></span>
    
2. <span data-ttu-id="3f0f9-127">À l’aide de la méthode [AttachmentCollection.Clear](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.attachmentcollection.clear%28v=exchg.80%29.aspx) pour supprimer toutes les pièces jointes à partir du message électronique.</span><span class="sxs-lookup"><span data-stu-id="3f0f9-127">Using the [AttachmentCollection.Clear](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.attachmentcollection.clear%28v=exchg.80%29.aspx) method to delete all the attachments from the email.</span></span> 
    
3. <span data-ttu-id="3f0f9-128">À l’aide de la méthode [EmailMessage.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx) pour enregistrer les modifications.</span><span class="sxs-lookup"><span data-stu-id="3f0f9-128">Using the [EmailMessage.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx) method to save the changes.</span></span> 
    
<span data-ttu-id="3f0f9-129">Cet exemple suppose que le **service** est un objet [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide, **itemId** est l' [ID d’élément](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemid%28v=exchg.80%29.aspx) du message à partir de laquelle les pièces jointes seront supprimés, et que l’utilisateur a été authentifié sur un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="3f0f9-129">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, **itemId** is the [ItemId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemid%28v=exchg.80%29.aspx) of the message from which attachments will be deleted, and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
public static void DeleteAllAttachments(ExchangeService service, ItemId itemId)
{
    // Bind to an existing message by using its item ID and requesting its attachments collection.
    // This method results in a GetItem call to EWS.
    EmailMessage message = EmailMessage.Bind(service, itemId, new PropertySet(ItemSchema.Attachments));
    // Delete all attachments from the message.
    message.Attachments.Clear();
    // Save the updated message.
    // This method results in an DeleteAttachment call to EWS.
    message.Update(ConflictResolutionMode.AlwaysOverwrite);
}
```

## <a name="delete-an-attachment-by-name-from-an-email-by-using-the-ews-managed-api"></a><span data-ttu-id="3f0f9-130">Supprimer une pièce jointe par un nom à partir d’un message électronique à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="3f0f9-130">Delete an attachment by name from an email by using the EWS Managed API</span></span>
<span data-ttu-id="3f0f9-131"><a name="bk_deleteattachewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="3f0f9-131"></span></span>

<span data-ttu-id="3f0f9-132">L’exemple de code suivant montre comment supprimer une pièce jointe par un nom à :</span><span class="sxs-lookup"><span data-stu-id="3f0f9-132">The following code example shows how delete an attachment by name by:</span></span>
  
1. <span data-ttu-id="3f0f9-133">À l’aide de la méthode [EmailMessage.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) pour récupérer la collection de [pièces jointes](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.attachments%28v=exchg.80%29.aspx)et les lier à un message électronique existant.</span><span class="sxs-lookup"><span data-stu-id="3f0f9-133">Using the [EmailMessage.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) method to bind to an existing email message and retrieve the collection of [Attachments](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.attachments%28v=exchg.80%29.aspx).</span></span>
    
2. <span data-ttu-id="3f0f9-134">À l’aide de la méthode [AttachmentCollection.Remove](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.attachmentcollection.remove%28v=exchg.80%29.aspx) pour supprimer une pièce jointe nommée FileAttachment.txt.</span><span class="sxs-lookup"><span data-stu-id="3f0f9-134">Using the [AttachmentCollection.Remove](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.attachmentcollection.remove%28v=exchg.80%29.aspx) method to delete an attachment named FileAttachment.txt.</span></span> 
    
3. <span data-ttu-id="3f0f9-135">À l’aide de la méthode [EmailMessage.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx) pour enregistrer les modifications.</span><span class="sxs-lookup"><span data-stu-id="3f0f9-135">Using the [EmailMessage.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx) method to save the changes.</span></span> 
    
<span data-ttu-id="3f0f9-136">Cet exemple suppose que le **service** est un objet [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide, **itemId** est l' [ID d’élément](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemid%28v=exchg.80%29.aspx) du message à partir de laquelle la pièce jointe sera supprimée, et que l’utilisateur a été authentifié sur un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="3f0f9-136">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, **itemId** is the [ItemId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemid%28v=exchg.80%29.aspx) of the message from which the attachment will be deleted, and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
public static void DeleteNamedAttachments(ExchangeService service, ItemId itemId)
{
    // Bind to an existing message by using its item ID and requesting its attachments collection.
    // This method results in a GetItem call to EWS.
    EmailMessage message = EmailMessage.Bind(service, itemId, new PropertySet(ItemSchema.Attachments));
    // Iterate through the attachments collection and delete the attachment named "FileAttachment.txt," if it exists.
    foreach (Attachment attachment in message.Attachments)
    {
        if (attachment.Name == "FileAttachment.txt")
        {
            message.Attachments.Remove(attachment);
            break;
        }
    }
    // Save the updated message.
    // This method results in an DeleteAttachment call to EWS.
    message.Update(ConflictResolutionMode.AlwaysOverwrite);
}
```

## <a name="delete-attachments-by-position-by-using-the-ews-managed-api"></a><span data-ttu-id="3f0f9-137">Supprimez les pièces jointes par sa position à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="3f0f9-137">Delete attachments by position by using the EWS Managed API</span></span>
<span data-ttu-id="3f0f9-138"><a name="bk_deleteattachewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="3f0f9-138"></span></span>

<span data-ttu-id="3f0f9-139">L’exemple de code suivant montre comment supprimer une pièce jointe par sa position par :</span><span class="sxs-lookup"><span data-stu-id="3f0f9-139">The following code example shows how to delete an attachment by position by:</span></span>
  
1. <span data-ttu-id="3f0f9-140">À l’aide de la méthode [EmailMessage.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) à lier à un message électronique existant et récupérer la collection de [pièces jointes](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.attachments%28v=exchg.80%29.aspx) et la propriété [EmailMessage.HasAttachments](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.hasattachments%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="3f0f9-140">Using the [EmailMessage.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) method to bind to an existing email message and retrieve the collection of [Attachments](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.attachments%28v=exchg.80%29.aspx) and the [EmailMessage.HasAttachments](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.hasattachments%28v=exchg.80%29.aspx) property.</span></span> 
    
2. <span data-ttu-id="3f0f9-141">À l’aide de la méthode [AttachmentCollection.Remove](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.attachmentcollection.remove%28v=exchg.80%29.aspx) pour supprimer la première pièce jointe dans la collection.</span><span class="sxs-lookup"><span data-stu-id="3f0f9-141">Using the [AttachmentCollection.Remove](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.attachmentcollection.remove%28v=exchg.80%29.aspx) method to delete the first attachment in the collection.</span></span> 
    
3. <span data-ttu-id="3f0f9-142">À l’aide de la méthode [EmailMessage.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx) pour enregistrer les modifications.</span><span class="sxs-lookup"><span data-stu-id="3f0f9-142">Using the [EmailMessage.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx) method to save the changes.</span></span> 
    
<span data-ttu-id="3f0f9-143">Cet exemple suppose que le **service** est un objet [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide, **itemId** est l' [ID d’élément](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemid%28v=exchg.80%29.aspx) du message à partir de laquelle la pièce jointe sera supprimée, et que l’utilisateur a été authentifié sur un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="3f0f9-143">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, **itemId** is the [ItemId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemid%28v=exchg.80%29.aspx) of the message from which the attachment will be deleted, and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
public static void DeleteAttachmentByPosition(ExchangeService service, ItemId itemId)
{
    // Bind to an existing message by using its item ID and requesting the HasAttachments property and the attachments collection.
    // This method results in a GetItem call to EWS.
    EmailMessage message = EmailMessage.Bind(service, itemId, new PropertySet(EmailMessageSchema.HasAttachments, ItemSchema.Attachments));
    // Remove attachments using the zero-based index position of the attachment in the attachments collection.
    if (message.HasAttachments)
    {
        message.Attachments.RemoveAt(0);
    }
    // Save the updated message.
    // This method results in an DeleteAttachment call to EWS.
    message.Update(ConflictResolutionMode.AlwaysOverwrite);
}
```

## <a name="delete-attachments-from-an-item-by-using-ews"></a><span data-ttu-id="3f0f9-144">Supprimez les pièces jointes d’un élément à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="3f0f9-144">Delete attachments from an item by using EWS</span></span>
<span data-ttu-id="3f0f9-145"><a name="bk_deleteattachewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="3f0f9-145"></span></span>

<span data-ttu-id="3f0f9-146">Pour supprimer les pièces jointes à l’aide de EWS, vous devez d’abord récupérer le message et la collection de pièces jointes pour déterminer [AttachmentId (GetAttachment et DeleteAttachment)](http://msdn.microsoft.com/library/4bea1cb5-0a0f-4e14-9b09-f91af8cf9899%28Office.15%29.aspx) de la pièce jointe à supprimer.</span><span class="sxs-lookup"><span data-stu-id="3f0f9-146">To delete attachments by using EWS, you first need to retrieve the message and the attachment collection to determine the [AttachmentId (GetAttachment and DeleteAttachment)](http://msdn.microsoft.com/library/4bea1cb5-0a0f-4e14-9b09-f91af8cf9899%28Office.15%29.aspx) of the attachment to delete.</span></span> <span data-ttu-id="3f0f9-147">Une fois que vous avez un ou plusieurs valeurs **AttachmentId** à supprimer, appelez l’opération [DeleteAttachment](http://msdn.microsoft.com/library/4d48e595-b98c-48e7-bbeb-cacf91d12a78%28Office.15%29.aspx) pour supprimer les pièces jointes spécifiés à partir du message.</span><span class="sxs-lookup"><span data-stu-id="3f0f9-147">After you have one or more **AttachmentId** values to delete, call the [DeleteAttachment](http://msdn.microsoft.com/library/4d48e595-b98c-48e7-bbeb-cacf91d12a78%28Office.15%29.aspx) operation to remove the specified attachments from the message.</span></span> 
  
<span data-ttu-id="3f0f9-148">L'exemple de code suivant montre comment utiliser l'opération [GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) pour récupérer un message électronique et la collection de pièces jointes associée au message.</span><span class="sxs-lookup"><span data-stu-id="3f0f9-148">The following code example shows how to use the [GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) operation to get an email message and the collection of attachments on the message.</span></span> <span data-ttu-id="3f0f9-149">C’est également la première requête XML qui envoie de l’API managée EWS lorsque vous utilisez l’API managée EWS pour [Supprimer toutes les pièces jointes à partir d’un message électronique](#bk_deleteattachewsma).</span><span class="sxs-lookup"><span data-stu-id="3f0f9-149">This is also the first XML request that the EWS Managed API sends when you use the EWS Managed API to [delete all attachments from an email](#bk_deleteattachewsma).</span></span> <span data-ttu-id="3f0f9-150">Les valeurs de certains attributs ont été raccourcies pour améliorer la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="3f0f9-150">The values of some attributes are shortened for readability.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Central Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:GetItem>
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Attachments" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:ItemIds>
        <t:ItemId Id="uqE1AAA=" />
      </m:ItemIds>
    </m:GetItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="3f0f9-151">Le serveur répond à la demande **GetItem** par un message [GetItemResponse](http://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx) où [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) renvoie la valeur **NoError**, ce qui indique que le message a bien été récupéré, et où apparaissent les valeurs [AttachmentId](http://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx) des pièces jointes existantes.</span><span class="sxs-lookup"><span data-stu-id="3f0f9-151">The server responds to the **GetItem** request with a [GetItemResponse](http://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the email was retrieved successfully, and the [AttachmentId](http://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx) values of the existing attachments.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="939"
                         MinorBuildNumber="12"
                         Version="V2_11"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Message>
              <t:ItemId Id="uqE1AAA="
                        ChangeKey="CQAAABYAAAAFI5DJmZv+TLtyLOLIF1S5AAAXulcd" />
              <t:Attachments>
                <t:FileAttachment>
                  <t:AttachmentId Id="IpHLObE=" />
                  <t:Name>FileAttachment.txt</t:Name>
                </t:FileAttachment>
                <t:FileAttachment>
                  <t:AttachmentId Id="QuHSSmY=" />
                  <t:Name>SecondAttachment.txt</t:Name>
                </t:FileAttachment>
                <t:FileAttachment>
                  <t:AttachmentId Id="qf2KoPo=" />
                  <t:Name>ThirdAttachment.jpg</t:Name>
                </t:FileAttachment>
                <t:FileAttachment>
                  <t:AttachmentId Id="NFQMnMc=" />
                  <t:Name>FourthAttachment.txt</t:Name>
                </t:FileAttachment>
                <t:ItemAttachment>
                  <t:AttachmentId Id="jJvbLXQ=" />
                  <t:Name>Attached Message Item</t:Name>
                </t:ItemAttachment>
              </t:Attachments>
            </t:Message>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </m:GetItemResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="3f0f9-152">Après vous déterminez les pièces jointes à supprimer, appelez l’opération [DeleteAttachment](http://msdn.microsoft.com/library/4d48e595-b98c-48e7-bbeb-cacf91d12a78%28Office.15%29.aspx) et inclure les valeurs **AttachmentId** des pièces jointes à supprimer.</span><span class="sxs-lookup"><span data-stu-id="3f0f9-152">After you determine which attachment to delete, call the [DeleteAttachment](http://msdn.microsoft.com/library/4d48e595-b98c-48e7-bbeb-cacf91d12a78%28Office.15%29.aspx) operation and include the **AttachmentId** values of the attachments to delete.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Central Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:DeleteAttachment>
      <m:AttachmentIds>
        <t:AttachmentId Id="IpHLObE=" />
        <t:AttachmentId Id="QuHSSmY=" />
        <t:AttachmentId Id="qf2KoPo=" />
        <t:AttachmentId Id="NFQMnMc=" />
        <t:AttachmentId Id="jJvbLXQ=" />
      </m:AttachmentIds>
    </m:DeleteAttachment>
  </soap:Body>
</soap:Envelope>
```

Le serveur répond à la demande **DeleteAttachment** avec un message [DeleteAttachmentResponse](http://msdn.microsoft.com/library/24099a88-4ab6-4bf3-8ed5-efec8e07b9b9%28Office.15%29.aspx) qui contient une valeur [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) **NoError** pour chaque [DeleteAttachmentResponseMessage](http://msdn.microsoft.com/library/1edb085f-1674-48e5-8ec3-42351adeac7d%28Office.15%29.aspx), qui indique que chaque pièce jointe a été supprimée. <span data-ttu-id="3f0f9-154">Les valeurs de certains attributs ont été raccourcies pour améliorer la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="3f0f9-154">The values of some attributes are shortened for readability.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="939"
                         MinorBuildNumber="12"
                         Version="V2_11"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:DeleteAttachmentResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                                xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:DeleteAttachmentResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootItemId RootItemId="uqE1AAA=" RootItemChangeKey="AAAXulck" />
        </m:DeleteAttachmentResponseMessage>
        <m:DeleteAttachmentResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootItemId RootItemId="uqE1AAA=" RootItemChangeKey="AAAXulck" />
        </m:DeleteAttachmentResponseMessage>
        <m:DeleteAttachmentResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootItemId RootItemId="uqE1AAA=" RootItemChangeKey="AAAXulck" />
        </m:DeleteAttachmentResponseMessage>
        <m:DeleteAttachmentResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootItemId RootItemId="uqE1AAA=" RootItemChangeKey="AAAXulck" />
        </m:DeleteAttachmentResponseMessage>
        <m:DeleteAttachmentResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootItemId RootItemId="uqE1AAA=" RootItemChangeKey="AAAXulck" />
        </m:DeleteAttachmentResponseMessage>
      </m:ResponseMessages>
    </m:DeleteAttachmentResponse>
  </s:Body>
</s:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="3f0f9-155">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="3f0f9-155">See also</span></span>


- [<span data-ttu-id="3f0f9-156">Pièces jointes et EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="3f0f9-156">Attachments and EWS in Exchange</span></span>](attachments-and-ews-in-exchange.md)
    
- [<span data-ttu-id="3f0f9-157">Ajouter des pièces jointes à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="3f0f9-157">Add attachments by using EWS in Exchange</span></span>](how-to-add-attachments-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="3f0f9-158">Obtenir des pièces jointes à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="3f0f9-158">Get attachments by using EWS in Exchange</span></span>](how-to-get-attachments-by-using-ews-in-exchange.md)
    

