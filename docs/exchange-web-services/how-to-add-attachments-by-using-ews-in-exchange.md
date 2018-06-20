---
title: Ajouter des pièces jointes à l’aide de EWS dans Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 0cbce436-2ae6-4fcc-bd8b-f517a0724e55
description: Découvrez comment créer des éléments avec les pièces jointes, ou ajouter des pièces jointes aux éléments existants à l’aide de l’API managée EWS ou EWS dans Exchange.
ms.openlocfilehash: dbfff879c92dafeec588d79cddd92e294b763c06
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19754831"
---
# <a name="add-attachments-by-using-ews-in-exchange"></a><span data-ttu-id="0b936-103">Ajouter des pièces jointes à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="0b936-103">Add attachments by using EWS in Exchange</span></span>

<span data-ttu-id="0b936-104">Découvrez comment créer des éléments avec les pièces jointes, ou ajouter des pièces jointes aux éléments existants à l’aide de l’API managée EWS ou EWS dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="0b936-104">Learn how to create new items with attachments, or add attachments to existing items by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="0b936-105">Vous pouvez ajouter des pièces jointes de fichier ou élément aux éléments de nouveau ou existants à l’aide de l’API managée EWS ou EWS.</span><span class="sxs-lookup"><span data-stu-id="0b936-105">You can add file attachments or item attachments to new or existing items by using the EWS Managed API or EWS.</span></span> <span data-ttu-id="0b936-106">Si vous utilisez l’API managée EWS, vous utilisez la même méthode pour ajouter des pièces jointes aux éléments de nouveau ou existants ; Toutefois, la méthode change si vous utilisez un fichier ou un élément des pièces jointes.</span><span class="sxs-lookup"><span data-stu-id="0b936-106">If you are using the EWS Managed API, you use the same method to add attachments to new or existing items; however, the method changes if you're using a file or item attachment.</span></span> <span data-ttu-id="0b936-107">Inversement, si vous utilisez EWS, la même opération vous permet d’ajouter un fichier ou un élément de pièce jointe à un élément, mais l’opération change si vous ajoutez la pièce jointe à un élément nouveau ou existant.</span><span class="sxs-lookup"><span data-stu-id="0b936-107">Conversely, if you are using EWS, you use the same operation to add either a file or item attachment to an item, but the operation changes if you're adding the attachment to a new or existing item.</span></span>
  
<span data-ttu-id="0b936-108">**Tableau 1. Méthodes de l'API managée EWS et opérations EWS pour l'ajout de pièces jointes**</span><span class="sxs-lookup"><span data-stu-id="0b936-108">**Table 1. EWS Managed API methods and EWS operations for adding attachments**</span></span>

|<span data-ttu-id="0b936-109">**Tâche**</span><span class="sxs-lookup"><span data-stu-id="0b936-109">**Task**</span></span>|<span data-ttu-id="0b936-110">**Méthode d'API managée EWS**</span><span class="sxs-lookup"><span data-stu-id="0b936-110">**EWS Managed API method**</span></span>|<span data-ttu-id="0b936-111">**Opération EWS**</span><span class="sxs-lookup"><span data-stu-id="0b936-111">**EWS operation**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="0b936-112">Ajouter une pièce jointe à un message électronique nouveau ou existant</span><span class="sxs-lookup"><span data-stu-id="0b936-112">Add a file attachment to a new or existing email</span></span>  <br/> |[<span data-ttu-id="0b936-113">AttachmentCollection.AddFileAttachment</span><span class="sxs-lookup"><span data-stu-id="0b936-113">AttachmentCollection.AddFileAttachment</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.attachmentcollection.addfileattachment%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="0b936-114">[CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) pour un nouveau courrier électronique</span><span class="sxs-lookup"><span data-stu-id="0b936-114">[CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) for a new email</span></span>  <br/> <span data-ttu-id="0b936-115">[CreateAttachment](http://msdn.microsoft.com/library/e066db95-6963-4507-a8d0-8efad287f550%28Office.15%29.aspx) à ajouter à un message électronique existant</span><span class="sxs-lookup"><span data-stu-id="0b936-115">[CreateAttachment](http://msdn.microsoft.com/library/e066db95-6963-4507-a8d0-8efad287f550%28Office.15%29.aspx) to add to an existing email</span></span>  <br/> |
|<span data-ttu-id="0b936-116">Ajouter une pièce jointe d’élément à un message électronique nouveau ou existant</span><span class="sxs-lookup"><span data-stu-id="0b936-116">Add an item attachment to a new or existing email</span></span>  <br/> |[<span data-ttu-id="0b936-117">AttachmentCollection.AddItemAttachment</span><span class="sxs-lookup"><span data-stu-id="0b936-117">AttachmentCollection.AddItemAttachment</span></span>](http://msdn.microsoft.com/en-us/library/dd634986%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="0b936-118">[CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) pour un nouveau courrier électronique</span><span class="sxs-lookup"><span data-stu-id="0b936-118">[CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) for a new email</span></span>  <br/> <span data-ttu-id="0b936-119">[CreateAttachment](http://msdn.microsoft.com/library/e066db95-6963-4507-a8d0-8efad287f550%28Office.15%29.aspx) à ajouter à un message électronique existant</span><span class="sxs-lookup"><span data-stu-id="0b936-119">[CreateAttachment](http://msdn.microsoft.com/library/e066db95-6963-4507-a8d0-8efad287f550%28Office.15%29.aspx) to add to an existing email</span></span>  <br/> |
   
## <a name="create-an-email-with-file-and-item-attachments-by-using-the-ews-managed-api"></a><span data-ttu-id="0b936-120">Créer un message électronique contenant des pièces jointes de fichier et l’élément à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="0b936-120">Create an email with file and item attachments by using the EWS Managed API</span></span>
<span data-ttu-id="0b936-121"><a name="bk_createattachewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="0b936-121"></span></span>

<span data-ttu-id="0b936-122">L’exemple de code suivant montre comment créer un message électronique avec plusieurs pièces jointes et la pièce jointe d’un élément par :</span><span class="sxs-lookup"><span data-stu-id="0b936-122">The following code example shows how to create an email with multiple file attachments and an item attachment by:</span></span> 
  
1. <span data-ttu-id="0b936-123">Utilisation de l’objet [EmailMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) pour créer un message électronique.</span><span class="sxs-lookup"><span data-stu-id="0b936-123">Using the [EmailMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) object to create an email message.</span></span> 
    
2. <span data-ttu-id="0b936-124">Utiliser les méthodes [AttachmentCollection.AddFileAttachment](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.attachmentcollection.addfileattachment%28v=exchg.80%29.aspx) et [AttachmentCollection.AddItemAttachment](http://msdn.microsoft.com/en-us/library/dd634986%28v=exchg.80%29.aspx) pour ajouter des pièces jointes au message.</span><span class="sxs-lookup"><span data-stu-id="0b936-124">Using the [AttachmentCollection.AddFileAttachment](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.attachmentcollection.addfileattachment%28v=exchg.80%29.aspx) and [AttachmentCollection.AddItemAttachment](http://msdn.microsoft.com/en-us/library/dd634986%28v=exchg.80%29.aspx) methods to add attachments to the message.</span></span> 
    
3. <span data-ttu-id="0b936-125">Utilisation de la méthode [EmailMessage.SendAndSaveCopy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) pour envoyer le message aux destinataires et enregistrer le message dans le dossier éléments envoyés.</span><span class="sxs-lookup"><span data-stu-id="0b936-125">Using the [EmailMessage.SendAndSaveCopy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) method to send the message to the recipients and save the message in the Sent Items folder.</span></span> 
    
<span data-ttu-id="0b936-126">Cet exemple de code montre les quatre manières dans lequel une pièce jointe peut être ajoutée à un élément à l’aide de l’API managée EWS :</span><span class="sxs-lookup"><span data-stu-id="0b936-126">This code example shows the four ways in which a file attachment can be added to an item by using the EWS Managed API:</span></span>
  
- <span data-ttu-id="0b936-127">En utilisant un emplacement de fichier complet.</span><span class="sxs-lookup"><span data-stu-id="0b936-127">By using a fully qualified file location.</span></span>
    
- <span data-ttu-id="0b936-128">En utilisant un emplacement de fichier complet et un nouveau nom de la pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="0b936-128">By using a fully qualified file location and a new attachment name.</span></span>
    
- <span data-ttu-id="0b936-129">En utilisant un tableau d’octets.</span><span class="sxs-lookup"><span data-stu-id="0b936-129">By using a byte array.</span></span>
    
- <span data-ttu-id="0b936-130">En utilisant un flux de données.</span><span class="sxs-lookup"><span data-stu-id="0b936-130">By using a stream.</span></span>
    
<span data-ttu-id="0b936-131">Notez que la pièce jointe d’élément dans cet exemple est créée en même temps que le message électronique.</span><span class="sxs-lookup"><span data-stu-id="0b936-131">Note that the item attachment in this example is created at the same time as the email message.</span></span> <span data-ttu-id="0b936-132">Pour ajouter un e-mail existant en tant que pièce jointe d’un élément, voir [Ajouter un élément existant à un nouveau message électronique à l’aide de la MimeContent et l’API managée EWS](#bk_addexistingemailewsma).</span><span class="sxs-lookup"><span data-stu-id="0b936-132">To add an existing email message as an item attachment, see [Add an existing item to a new email by using the MimeContent and the EWS Managed API](#bk_addexistingemailewsma).</span></span>
  
<span data-ttu-id="0b936-133">Cet exemple suppose que ce **service** est un objet [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur a été authentifié sur un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="0b936-133">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
public static void CreateEmailWithAttachments(ExchangeService service)
{
    // Create an email message and set properties on the message.
    EmailMessage message = new EmailMessage(service);
    // Set properties on the email message.
    message.Subject = "Message with Attachments";
    message.Body = "This message contains four file attachments 
        and one message item attachment.";
    message.ToRecipients.Add("sadie@contoso.com");
    message.ToRecipients.Add("ronnie@contoso.com");
    // Add a file attachment by using the fully qualified location of the file. 
    message.Attachments.AddFileAttachment("C:\\temp\\FileAttachment.txt");
    // Add a file attachment by using the fully qualified string name, 
    // and specify the name of the attachment as it will appear in the email.
    // The new name of the file attachment is SecondAttachment.txt.
    message.Attachments.AddFileAttachment("SecondAttachment.txt", "C:\\temp\\FileAttachment2.txt");
    // Add a file attachment by using a byte array.
    // In this example, theBytes is the byte array that represents the content of the image file to attach.
    byte[] theBytes = File.ReadAllBytes("C:\\Temp\\Tulips.jpg");
    // The byte array file attachment is named ThirdAttachment.jpg.
    message.Attachments.AddFileAttachment("ThirdAttachment.jpg", theBytes);
    // Add a file attachment by using a stream.
    FileStream theStream = new FileStream("C:\\temp\\FileAttachment4.txt", FileMode.OpenOrCreate);
    // The streamed file attachment is named FourthAttachment.txt.
    message.Attachments.AddFileAttachment("FourthAttachment.txt", theStream);
    // Add an email message as an item attachment and set properties on the item.
    ItemAttachment<EmailMessage> itemAttachment = message.Attachments.AddItemAttachment<EmailMessage>();
    itemAttachment.Name = "Attached Message Item";
    itemAttachment.Item.Subject = "Message Item Subject";
    itemAttachment.Item.Body = "Message Item Body";
    itemAttachment.Item.ToRecipients.Add("sadie@contoso.com");
    itemAttachment.Item.ToRecipients.Add("ronnie@contoso.com");
    // Send the mail and save a copy in the Sent Items folder.
    // This method results in a CreateItem and SendItem call to EWS.
    message.SendAndSaveCopy();
}
```

## <a name="create-an-email-with-file-and-item-attachments-by-using-ews"></a><span data-ttu-id="0b936-134">Créer un message électronique contenant des pièces jointes de fichier et l’élément à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="0b936-134">Create an email with file and item attachments by using EWS</span></span>
<span data-ttu-id="0b936-135"><a name="bk_createattachews"> </a></span><span class="sxs-lookup"><span data-stu-id="0b936-135"></span></span>

<span data-ttu-id="0b936-136">L’exemple de code suivant montre comment utiliser l’opération [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) pour créer un message électronique avec quatre pièces jointes et la pièce jointe d’un élément.</span><span class="sxs-lookup"><span data-stu-id="0b936-136">The following code example shows how to use the [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) operation to create an email message with four file attachments and one item attachment.</span></span> <span data-ttu-id="0b936-137">C’est également l’une des demandes XML qui envoie de l’API managée EWS lorsque vous [créez un message électronique contenant des pièces jointes de fichier et l’élément](#bk_createattachewsma).</span><span class="sxs-lookup"><span data-stu-id="0b936-137">This is also one of the XML requests that the EWS Managed API sends when you [create an email with file and item attachments](#bk_createattachewsma).</span></span>
  
<span data-ttu-id="0b936-138">Notez que la pièce jointe d’élément dans cet exemple est créée en même temps que le message électronique.</span><span class="sxs-lookup"><span data-stu-id="0b936-138">Note that the item attachment in this example is created at the same time as the email message.</span></span> <span data-ttu-id="0b936-139">Pour ajouter un e-mail existant en tant que pièce jointe d’un élément, voir [Ajouter un élément existant à un nouveau message électronique à l’aide de la MimeContent et l’API managée EWS](#bk_addexistingemailewsma).</span><span class="sxs-lookup"><span data-stu-id="0b936-139">To add an existing email message as an item attachment, see [Add an existing item to a new email by using the MimeContent and the EWS Managed API](#bk_addexistingemailewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:CreateItem MessageDisposition="SaveOnly">
      <m:Items>
        <t:Message>
          <t:Subject>Message with Attachments</t:Subject>
          <t:Body BodyType="HTML">This message contains four file attachments 
              and one message item attachment.</t:Body>
          <t:Attachments>
            <t:FileAttachment>
              <t:Name>FileAttachment.txt</t:Name>
              <t:IsInline>false</t:IsInline>
              <t:IsContactPhoto>false</t:IsContactPhoto>
              <t:Content>VGhpcyBpcyBhIGZpbGUgYXR0YWNobWVudC4=</t:Content>
            </t:FileAttachment>
            <t:FileAttachment>
              <t:Name>SecondAttachment.txt</t:Name>
              <t:IsInline>false</t:IsInline>
              <t:IsContactPhoto>false</t:IsContactPhoto>
              <t:Content>VGhpcyBpcyB0aGUgc2Vjb25kIGZpbGUgYXR0YWNobWVudC4=</t:Content>
            </t:FileAttachment>
            <t:FileAttachment>
              <t:Name>ThirdAttachment.jpg</t:Name>
              <t:IsInline>false</t:IsInline>
              <t:IsContactPhoto>false</t:IsContactPhoto>
              <t:Content>nAoAXNIZMVEZs5GKhdzRcLH/9k=</t:Content>
            </t:FileAttachment>
            <t:FileAttachment>
              <t:Name>FourthAttachment.txt</t:Name>
              <t:IsInline>false</t:IsInline>
              <t:IsContactPhoto>false</t:IsContactPhoto>
              <t:Content>obWVudC4=…</t:Content>
            </t:FileAttachment>
            <t:ItemAttachment>
              <t:Name>Attached Message Item</t:Name>
              <t:IsInline>false</t:IsInline>
              <t:Message>
                <t:Subject>Message Item Subject</t:Subject>
                <t:Body BodyType="HTML">Message Item Body</t:Body>
                <t:ToRecipients>
                  <t:Mailbox>
                    <t:EmailAddress>sadie@contoso.com</t:EmailAddress>
                  </t:Mailbox>
                  <t:Mailbox>
                    <t:EmailAddress>mack@contoso.com</t:EmailAddress>
                  </t:Mailbox>
                </t:ToRecipients>
              </t:Message>
            </t:ItemAttachment>
          </t:Attachments>
          <t:ToRecipients>
            <t:Mailbox>
              <t:EmailAddress>sadie@contoso.com</t:EmailAddress>
            </t:Mailbox>
            <t:Mailbox>
              <t:EmailAddress>ronnie@contoso.com</t:EmailAddress>
            </t:Mailbox>
          </t:ToRecipients>
        </t:Message>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="0b936-140">Le serveur répond à la demande **CreateItem** avec un message [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) qui contient une valeur [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) **NoError**, ce qui indique que le courrier électronique et les pièces jointes ont été correctement créées.</span><span class="sxs-lookup"><span data-stu-id="0b936-140">The server responds to the **CreateItem** request with a [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the email and the attachments were created successfully.</span></span> <span data-ttu-id="0b936-141">L' [ID d’élément](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) du message nouvellement créé et les valeurs [AttachmentId](http://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx) pour chacune des pièces jointes est également inclus dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="0b936-141">The [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) of the newly created message and the [AttachmentId](http://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx) values for each of the attachments is also included in the response.</span></span> <span data-ttu-id="0b936-142">Les valeurs de certains attributs ont été raccourcies pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="0b936-142">The values of some attributes have been shortened for readability.</span></span> 
  
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
    <m:CreateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Message>
              <t:ItemId Id="upV4AAA="
                        ChangeKey="CQAAABYAAAAFI5DJmZv+TLtyLOLIF1S5AAAXuktU" />
              <t:Attachments>
                <t:FileAttachment>
                  <t:AttachmentId Id="6ts3NuI=" />
                </t:FileAttachment>
                <t:FileAttachment>
                  <t:AttachmentId Id="gOIZx1I=" />
                </t:FileAttachment>
                <t:FileAttachment>
                  <t:AttachmentId Id="esRan5I=" />
                </t:FileAttachment>
                <t:FileAttachment>
                  <t:AttachmentId Id="t7sU6s=" />
                </t:FileAttachment>
                <t:ItemAttachment>
                  <t:AttachmentId Id="XgDCggM=" />
                </t:ItemAttachment>
              </t:Attachments>
            </t:Message>
          </m:Items>
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </m:CreateItemResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="0b936-143">Pour [Envoyer ce message nouvellement créé](how-to-send-email-messages-by-using-ews-in-exchange.md), appelez l’opération [SendItem](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="0b936-143">To [send this newly created message](how-to-send-email-messages-by-using-ews-in-exchange.md), call the [SendItem](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) operation.</span></span> 
  
## <a name="add-an-existing-item-to-a-new-email-by-using-the-mimecontent-and-the-ews-managed-api"></a><span data-ttu-id="0b936-144">Ajouter un élément existant à un nouveau courrier électronique à l’aide de la MimeContent et l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="0b936-144">Add an existing item to a new email by using the MimeContent and the EWS Managed API</span></span>
<span data-ttu-id="0b936-145"><a name="bk_addexistingemailewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="0b936-145"></span></span>

<span data-ttu-id="0b936-146">Pour ajouter un élément existant en tant que pièce jointe d’un élément à un autre élément, vous devez créer une nouvelle pièce jointe d’élément et copiez le contenu de l’élément existant dans le nouvel élément.</span><span class="sxs-lookup"><span data-stu-id="0b936-146">To add an existing item as an item attachment to another item, you need to create a new item attachment and copy the content of the existing item to the new item.</span></span> <span data-ttu-id="0b936-147">Il existe deux façons de procéder :</span><span class="sxs-lookup"><span data-stu-id="0b936-147">There are two ways to do this:</span></span> 
  
1. <span data-ttu-id="0b936-148">Si vous travaillez avec des messages électroniques en particulier, vous pouvez copier la valeur de la propriété [MimeContent](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.mimecontent%28v=exchg.80%29.aspx) à partir du message électronique dans l’élément nouvellement créé des pièces jointes.</span><span class="sxs-lookup"><span data-stu-id="0b936-148">If you're working with email messages specifically, you can copy the value of the [MimeContent](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.mimecontent%28v=exchg.80%29.aspx) property from the email into the newly created item attachment.</span></span> <span data-ttu-id="0b936-149">Vous allez perdre certaines propriétés pendant ce processus, tels que suivi des indicateurs et des catégories, mais il fonctionne parfaitement pour les messages électroniques standard.</span><span class="sxs-lookup"><span data-stu-id="0b936-149">You will lose some properties during this process, such as follow up flags and categories, but it works great for standard email messages.</span></span> 
    
2. <span data-ttu-id="0b936-150">Si vous avez besoin de fidélité pour tous les types d’éléments, vous pouvez lier à un élément existant et copier toutes les propriétés et les propriétés étendues dans la nouvelle pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="0b936-150">If you need full fidelity for all item types, you can bind to an existing item and copy all the properties and extended properties into the new attachment.</span></span>
    
<span data-ttu-id="0b936-151">L’exemple de code suivant affiche la première approche, en copiant le **MimeContent** dans la nouvelle pièce jointe d’élément.</span><span class="sxs-lookup"><span data-stu-id="0b936-151">The following code example shows the first approach, copying the **MimeContent** into the new item attachment.</span></span> <span data-ttu-id="0b936-152">Cet exemple suivant est une procédure qui montre comment vous pouvez modifier le code pour utiliser la seconde approche.</span><span class="sxs-lookup"><span data-stu-id="0b936-152">Following this example is a procedure that shows how you can modify the code to use the second approach.</span></span> 
  
<span data-ttu-id="0b936-153">Cet exemple suppose que ce **service** est un objet [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur a été authentifié sur un serveur Exchange, et l' **ID d’élément** est [ItemId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemid%28v=exchg.80%29.aspx) de l’élément à joindre.</span><span class="sxs-lookup"><span data-stu-id="0b936-153">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server, and that the **itemId** is the [ItemId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemid%28v=exchg.80%29.aspx) of the item to attach.</span></span> 
  
```cs
public static void CreateEmailExistingItem(ExchangeService service, ItemId itemId)
{        
    // This method results in a GetItem call to EWS.
    EmailMessage msgToAttach = EmailMessage.Bind(service,itemId, 
        new PropertySet(ItemSchema.MimeContent, ItemSchema.Subject));
    // Create an email message and set properties on the message.
    EmailMessage message = new EmailMessage(service);
    message.Subject = "Message with Item Attachment (MimeContent)";
    message.Body = "The attachment to this message was created by copying
        the MimeContent from the original message and adding it to a new item attachment.";
    message.ToRecipients.Add("sadie@contoso.com");
    // Add an email message item attachment and set properties on the item.
    ItemAttachment<EmailMessage> itemAttachment = message.Attachments.AddItemAttachment<EmailMessage>();
    itemAttachment.Item.MimeContent = msgToAttach.MimeContent;
    itemAttachment.Name = msgToAttach.Subject;
    // Send the mail and save a copy in the Sent Items folder.
    // This method results in a CreateItem and SendItem call to EWS.
    message.SendAndSaveCopy();
}
```

<span data-ttu-id="0b936-154">Pour modifier cet exemple montre comment copier chacune des propriétés de l’élément existant dans la nouvelle pièce jointe d’élément, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="0b936-154">To modify this example to copy each of the properties on the existing item into the new item attachment, do the following:</span></span> 
  
1. <span data-ttu-id="0b936-155">Modifiez la propriété définie pour inclure **PropertySet.FirstClassProperties** et des propriétés supplémentaires ou les propriétés étendues, que vous avez besoin.</span><span class="sxs-lookup"><span data-stu-id="0b936-155">Change the property set to include **PropertySet.FirstClassProperties** and any additional properties or extended properties you need.</span></span> 
    
  ```cs
  // Add additional properties to the PropertySet.
  EmailMessage msgToAttach = EmailMessage.Bind(service, itemId, new PropertySet(PropertySet.FirstClassProperties));
  ```

2. <span data-ttu-id="0b936-156">Supprimer la ligne suivante, car vous n’avez pas besoin de la propriété **MimeContent** .</span><span class="sxs-lookup"><span data-stu-id="0b936-156">Remove the following line, because you do not need the **MimeContent** property.</span></span> 
    
  ```cs
  itemAttachment.Item.MimeContent = msgToAttach.MimeContent;
  ```

3. <span data-ttu-id="0b936-157">Répétez cette ligne pour chaque propriété copier à partir de l’élément existant dans la nouvelle pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="0b936-157">Repeat this line for each property to copy from the existing item to the new attachment.</span></span> <span data-ttu-id="0b936-158">Ne copiez pas l' **ID d’élément** dans la nouvelle pièce jointe d’élément car c’est une propriété en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="0b936-158">Do not copy the **ItemId** into the new item attachment because that's a read-only property.</span></span> 
    
  ```cs
  itemAttachment.Item.Subject = msgToAttach.Subject;
  ```

4. <span data-ttu-id="0b936-159">Définir la propriété [PidTagMessageFlags](http://msdn.microsoft.com/en-us/library/cc839733.aspx) (0x0E070003) sur la pièce jointe sur **envoyé**.</span><span class="sxs-lookup"><span data-stu-id="0b936-159">Set the [PidTagMessageFlags](http://msdn.microsoft.com/en-us/library/cc839733.aspx) (0x0E070003) property on the attachment to **Sent**.</span></span>
    
  ```cs
  ExtendedPropertyDefinition sent = new ExtendedPropertyDefinition(3591, MapiPropertyType.Integer);
  msgToAttach.Item.SetExtendedProperty(sent, "1");
  ```

## <a name="add-an-existing-item-to-a-new-email-by-using-the-mimecontent-and-ews"></a><span data-ttu-id="0b936-160">Ajouter un élément existant à un nouveau courrier électronique à l’aide de la MimeContent et EWS</span><span class="sxs-lookup"><span data-stu-id="0b936-160">Add an existing item to a new email by using the MimeContent and EWS</span></span>
<span data-ttu-id="0b936-161"><a name="bk_addexistingemailews"> </a></span><span class="sxs-lookup"><span data-stu-id="0b936-161"></span></span>

<span data-ttu-id="0b936-162">Il existe deux façons d’ajouter un élément existant à un nouvel article :</span><span class="sxs-lookup"><span data-stu-id="0b936-162">There are two ways to add an existing item to a new item:</span></span> 
  
1. <span data-ttu-id="0b936-163">Si vous travaillez avec des messages électroniques en particulier, vous pouvez copier la valeur de l’élément [MimeContent](http://msdn.microsoft.com/library/4f472a08-5653-4c54-ba65-831dfe32f20f%28Office.15%29.aspx) à partir du message électronique dans l’élément nouvellement créé des pièces jointes.</span><span class="sxs-lookup"><span data-stu-id="0b936-163">If you're working with email messages specifically, you can copy the value of the [MimeContent](http://msdn.microsoft.com/library/4f472a08-5653-4c54-ba65-831dfe32f20f%28Office.15%29.aspx) element from the email into the newly created item attachment.</span></span> <span data-ttu-id="0b936-164">Vous allez perdre certaines propriétés pendant ce processus, tels que suivi des indicateurs et des catégories, mais il fonctionne parfaitement pour les messages électroniques standard.</span><span class="sxs-lookup"><span data-stu-id="0b936-164">You will lose some properties during this process, such as follow up flags and categories, but it works great for standard email messages.</span></span> 
    
2. <span data-ttu-id="0b936-165">Si vous avez besoin de fidélité pour tous les types d’éléments, vous pouvez lier à un élément existant et copier toutes les propriétés et les propriétés étendues dans la nouvelle pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="0b936-165">If you need full fidelity for all item types, you can bind to an existing item and copy all the properties and extended properties into the new attachment.</span></span>
    
<span data-ttu-id="0b936-166">L’exemple de code suivant montre comment utiliser l’élément **MimeContent** pour copier le contenu de l’élément d’origine dans la valeur **MimeContent** de la nouvelle pièce jointe d’élément.</span><span class="sxs-lookup"><span data-stu-id="0b936-166">The following code example shows how to use the **MimeContent** element to copy the content of the original item into the **MimeContent** value of the new item attachment.</span></span> <span data-ttu-id="0b936-167">L’exemple utilise les opérations suivantes :</span><span class="sxs-lookup"><span data-stu-id="0b936-167">The example uses the following operations:</span></span> 
  
1. <span data-ttu-id="0b936-168">[GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) — pour obtenir le **MimeContent** et l' [objet](http://msdn.microsoft.com/library/c140d6c2-deb1-4f67-a908-9397197c4ae7%28Office.15%29.aspx) du message qui deviendra la pièce jointe d’élément dans le nouveau message.</span><span class="sxs-lookup"><span data-stu-id="0b936-168">[GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) — To get the **MimeContent** and [Subject](http://msdn.microsoft.com/library/c140d6c2-deb1-4f67-a908-9397197c4ae7%28Office.15%29.aspx) of the message that will become the item attachment on the new message.</span></span> 
    
2. <span data-ttu-id="0b936-169">[CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) , pour créer le nouveau message électronique.</span><span class="sxs-lookup"><span data-stu-id="0b936-169">[CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) — To create the new email message.</span></span> 
    
3. <span data-ttu-id="0b936-170">[CreateAttachment](http://msdn.microsoft.com/library/e066db95-6963-4507-a8d0-8efad287f550%28Office.15%29.aspx)— pour créer la nouvelle pièce jointe, à l’aide de le **MimeContent** et **l’objet** récupéré par l’opération **GetItem** .</span><span class="sxs-lookup"><span data-stu-id="0b936-170">[CreateAttachment](http://msdn.microsoft.com/library/e066db95-6963-4507-a8d0-8efad287f550%28Office.15%29.aspx)— To create the new attachment, using the **MimeContent** and **Subject** retrieved by the **GetItem** operation.</span></span> 
    
4. <span data-ttu-id="0b936-171">[SendItem](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) — et enregistrez le message.</span><span class="sxs-lookup"><span data-stu-id="0b936-171">[SendItem](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) — To send and save the message.</span></span> 
    
<span data-ttu-id="0b936-172">L’exemple commence par récupérer l' **MimeContent** et l' **objet** de l’élément existant.</span><span class="sxs-lookup"><span data-stu-id="0b936-172">The example starts by retrieving the **MimeContent** and the **Subject** of the existing item.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <m:GetItem>
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:MimeContent" />
          <t:FieldURI FieldURI="item:Subject" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:ItemIds>
        <t:ItemId Id="jCrTAAA=" />
      </m:ItemIds>
    </m:GetItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="0b936-173">Le serveur répond à la demande de **GetItem** avec un message [GetItemResponse](http://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx) qui contient une valeur [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) **NoError**, ce qui indique que le courrier électronique a été récupéré avec succès et **MimeContent** et ** Objet** du courrier électronique.</span><span class="sxs-lookup"><span data-stu-id="0b936-173">The server responds to the **GetItem** request with a [GetItemResponse](http://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the email was retrieved successfully, and the **MimeContent** and **Subject** of the email.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="944"
                         MinorBuildNumber="11"
                         Version="V2_12"
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
              <t:MimeContent CharacterSet="UTF-8">tDQe/Eo=…</t:MimeContent>
              <t:ItemId Id="jCrTAAA="
                        ChangeKey="CQAAABYAAAAFI5DJmZv+TLtyLOLIF1S5AAAZi+7u" />
              <t:Subject>Play tennis?</t:Subject>
            </t:Message>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </m:GetItemResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="0b936-174">Ensuite, appeler l’opération **CreateItem** pour créer le nouveau courrier électronique.</span><span class="sxs-lookup"><span data-stu-id="0b936-174">Next, call the **CreateItem** operation to create the new email.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010" />
  </soap:Header>
  <soap:Body>
    <m:CreateItem MessageDisposition="SaveOnly">
      <m:Items>
        <t:Message>
          <t:Subject>Message with Item Attachment (MimeContent)</t:Subject>
          <t:Body BodyType="HTML">The attachment to this message was created by copying the MimeContent from the original message and adding it to a new item attachment.</t:Body>
          <t:ToRecipients>
            <t:Mailbox>
              <t:EmailAddress>primary@contoso1000.onmicrosoft.com</t:EmailAddress>
            </t:Mailbox>
          </t:ToRecipients>
        </t:Message>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="0b936-175">Le serveur répond à la demande **CreateItem** avec un message [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) qui contient une valeur [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) **NoError**, ce qui indique que le courrier électronique a été créé avec succès.</span><span class="sxs-lookup"><span data-stu-id="0b936-175">The server responds to the **CreateItem** request with a [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the email was created successfully.</span></span>
  
<span data-ttu-id="0b936-176">Ensuite, créez la nouvelle pièce jointe d’élément à l’aide de le **MimeContent** et l' **objet** récupéré par l’opération **GetItem** .</span><span class="sxs-lookup"><span data-stu-id="0b936-176">Next, create the new item attachment by using the **MimeContent** and **Subject** retrieved by the **GetItem** operation.</span></span> <span data-ttu-id="0b936-177">La valeur de l’élément [ParentItemId](http://msdn.microsoft.com/library/72dc4391-72db-44d2-85d9-4718d59886a7%28Office.15%29.aspx) est renseignée à l’aide de la valeur **ItemId** renvoyée dans la réponse **CreateItem** .</span><span class="sxs-lookup"><span data-stu-id="0b936-177">The value of the [ParentItemId](http://msdn.microsoft.com/library/72dc4391-72db-44d2-85d9-4718d59886a7%28Office.15%29.aspx) element is populated by using the **ItemId** value returned in the **CreateItem** response.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010" />
  </soap:Header>
  <soap:Body>
    <m:CreateAttachment>
      <m:ParentItemId Id="jDKsAAA=" />
      <m:Attachments>
        <t:ItemAttachment>
          <t:Name>Play tennis?</t:Name>
          <t:IsInline>false</t:IsInline>
          <t:Message>
            <t:MimeContent CharacterSet="UTF-8">tDQe/Eo=…</t:MimeContent>
          </t:Message>
        </t:ItemAttachment>
      </m:Attachments>
    </m:CreateAttachment>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="0b936-178">Le serveur répond à la demande **CreateAttachment** avec un message [CreateAttachmentResponse](http://msdn.microsoft.com/library/cf6bd8bb-5317-4a03-bd75-297dd359b5da%28Office.15%29.aspx) qui contient une valeur [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) **NoError**, ce qui indique que la pièce jointe a été créée avec succès et le [ AttachmentId](http://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx) de la pièce jointe nouvellement créée.</span><span class="sxs-lookup"><span data-stu-id="0b936-178">The server responds to the **CreateAttachment** request with a [CreateAttachmentResponse](http://msdn.microsoft.com/library/cf6bd8bb-5317-4a03-bd75-297dd359b5da%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the attachment was created successfully, and the [AttachmentId](http://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx) of the newly created attachment.</span></span> 
  
<span data-ttu-id="0b936-179">Maintenant que le nouveau message a été créé et l’élément a été associée, vous pouvez [Envoyer ce message nouvellement créé](how-to-send-email-messages-by-using-ews-in-exchange.md) en appelant l’opération [SendItem](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="0b936-179">Now that the new message has been created, and the item was attached, you can [send this newly created message](how-to-send-email-messages-by-using-ews-in-exchange.md) by calling the [SendItem](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) operation.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010" />
  </soap:Header>
  <soap:Body>
    <m:SendItem SaveItemToFolder="true">
      <m:ItemIds>
        <t:ItemId Id="jDKsAAA="
                  ChangeKey="CQAAABYAAAAFI5DJmZv+TLtyLOLIF1S5AAAZi/q/" />
      </m:ItemIds>
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="sentitems" />
      </m:SavedItemFolderId>
    </m:SendItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="0b936-180">Le serveur répond à la demande **SendItem** avec un message [SendItemResponse](http://msdn.microsoft.com/library/26ac41c7-57d9-473e-ab7a-bae93e1d2aba%28Office.15%29.aspx) qui contient une valeur [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, ce qui indique que le courrier électronique a été envoyé correctement.</span><span class="sxs-lookup"><span data-stu-id="0b936-180">The server responds to the **SendItem** request with a [SendItemResponse](http://msdn.microsoft.com/library/26ac41c7-57d9-473e-ab7a-bae93e1d2aba%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates that the email was sent successfully.</span></span>
  
## <a name="create-an-email-with-an-inline-attachment-by-using-the-ews-managed-api"></a><span data-ttu-id="0b936-181">Créer un message électronique avec une pièce jointe incorporée à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="0b936-181">Create an email with an inline attachment by using the EWS Managed API</span></span>
<span data-ttu-id="0b936-182"><a name="bk_createinlineattachewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="0b936-182"></span></span>

<span data-ttu-id="0b936-183">L’exemple de code suivant montre comment créer un message électronique comportant une pièce jointe insérée par :</span><span class="sxs-lookup"><span data-stu-id="0b936-183">The following code example shows how to create an email with an inline attachment by:</span></span>
  
1. <span data-ttu-id="0b936-184">Utilisation de l’objet [EmailMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) pour créer un message électronique.</span><span class="sxs-lookup"><span data-stu-id="0b936-184">Using the [EmailMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) object to create an email message.</span></span> 
    
2. <span data-ttu-id="0b936-185">Définition de la propriété [EmailMessage.Body](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.body%28v=exchg.80%29.aspx) à un corps HTML contenant une pièce jointe incorporée.</span><span class="sxs-lookup"><span data-stu-id="0b936-185">Setting the [EmailMessage.Body](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.body%28v=exchg.80%29.aspx) property to an HTML body that includes an inline attachment.</span></span> 
    
3. <span data-ttu-id="0b936-186">Utilisation de la méthode [AttachmentCollection.AddFileAttachment](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.attachmentcollection.addfileattachment%28v=exchg.80%29.aspx) pour ajouter la pièce jointe du message.</span><span class="sxs-lookup"><span data-stu-id="0b936-186">Using the [AttachmentCollection.AddFileAttachment](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.attachmentcollection.addfileattachment%28v=exchg.80%29.aspx) method to add the attachment to the message.</span></span> 
    
4. <span data-ttu-id="0b936-187">Utilisation de la méthode [EmailMessage.SendAndSaveCopy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) pour envoyer le message au destinataire et enregistrer le message dans le dossier éléments envoyés.</span><span class="sxs-lookup"><span data-stu-id="0b936-187">Using the [EmailMessage.SendAndSaveCopy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) method to send the message to the recipient and save the message in the Sent Items folder.</span></span> 
    
<span data-ttu-id="0b936-188">Cet exemple suppose que ce **service** est un objet [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur a été authentifié sur un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="0b936-188">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
public static void CreateEmailWithInlineAttachment(ExchangeService service)
{
    // Create the HTML body with the content identifier of the attachment.
    string html = @"<html>
                        <head>
                        </head>
                        <body>
                        <img width=100 height=100 id=""1"" src=""cid:Party.jpg"">
                        </body>
                        </html>";
         
    // Create the email message.
    EmailMessage message = new EmailMessage(service);
    message.Subject = "Inline Attachment";
    message.Body = new MessageBody(BodyType.HTML, html);
    message.ToRecipients.Add("sadie@contoso.com");
    // Add the attachment to the local copy of the email message.
    string file = @"C:\Temp\Party.jpg";
    message.Attachments.AddFileAttachment("Party.jpg", file);
    message.Attachments[0].IsInline = true;
    message.Attachments[0].ContentId = "Party.jpg";
         
    // Send the mail and save a copy in the Sent Items folder.
    // This method results in a CreateItem and SendItem call to EWS.
    message.SendAndSaveCopy();
}
```

## <a name="create-an-email-with-an-inline-attachment-by-using-ews"></a><span data-ttu-id="0b936-189">Créer un message électronique avec une pièce jointe incorporée à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="0b936-189">Create an email with an inline attachment by using EWS</span></span>
<span data-ttu-id="0b936-190"><a name="bk_createinlineattachewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="0b936-190"></span></span>

<span data-ttu-id="0b936-191">L’exemple de code suivant montre comment utiliser l’opération [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) pour créer un message électronique avec une pièce jointe incorporée.</span><span class="sxs-lookup"><span data-stu-id="0b936-191">The following code example shows how to use the [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) operation to create an email message with an inline file attachment.</span></span> <span data-ttu-id="0b936-192">L’attribut **BodyType** de l’élément [Body](http://msdn.microsoft.com/library/7851ea9b-9f87-4adc-a26f-7a27df4a9bca%28Office.15%29.aspx) indique que le contenu est au format HTML et inclut la source d’image.</span><span class="sxs-lookup"><span data-stu-id="0b936-192">The **BodyType** attribute of the [Body](http://msdn.microsoft.com/library/7851ea9b-9f87-4adc-a26f-7a27df4a9bca%28Office.15%29.aspx) element indicates that the content is in HTML format and includes the image source.</span></span> <span data-ttu-id="0b936-193">C’est également une des demandes XML qui envoie de l’API managée EWS lorsque vous utilisez l’API managée EWS pour [créer un message électronique avec une pièce jointe incorporée](#bk_createinlineattachewsma).</span><span class="sxs-lookup"><span data-stu-id="0b936-193">This is also one of the XML requests that the EWS Managed API sends when you use the EWS Managed API to [create an email with an inline attachment](#bk_createinlineattachewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010" />
  </soap:Header>
  <soap:Body>
    <m:CreateItem MessageDisposition="SaveOnly">
      <m:Items>
        <t:Message>
          <t:Subject>Inline Attachment</t:Subject>
          <t:Body BodyType="HTML">
            &amp;lt;html&amp;gt;
            &amp;lt;head&amp;gt;
            &amp;lt;/head&amp;gt;
            &amp;lt;body&amp;gt;
            &amp;lt;img width=100 height=100 id="1" src="cid:Party.jpg"&amp;gt;
            &amp;lt;/body&amp;gt;
            &amp;lt;/html&amp;gt;
          </t:Body>
          <t:ToRecipients>
            <t:Mailbox>
              <t:EmailAddress>sadie@contoso.com</t:EmailAddress>
            </t:Mailbox>
          </t:ToRecipients>
        </t:Message>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="0b936-194">Le serveur répond à la demande **CreateItem** avec un message [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) qui contient une valeur [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) **NoError**, ce qui indique que le courrier électronique a été créé avec succès et l' [ID d’élément](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) de la nouvelle message créé.</span><span class="sxs-lookup"><span data-stu-id="0b936-194">The server responds to the **CreateItem** request with a [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the email was created successfully, and the [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) of the newly created message.</span></span> 
  
<span data-ttu-id="0b936-195">Pour [Envoyer ce message nouvellement créé](how-to-send-email-messages-by-using-ews-in-exchange.md), appelez l’opération [SendItem](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="0b936-195">To [send this newly created message](how-to-send-email-messages-by-using-ews-in-exchange.md), call the [SendItem](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) operation.</span></span> 
  
## <a name="add-an-attachment-to-an-existing-email-by-using-the-ews-managed-api"></a><span data-ttu-id="0b936-196">Ajouter une pièce jointe à un message électronique existant à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="0b936-196">Add an attachment to an existing email by using the EWS Managed API</span></span>
<span data-ttu-id="0b936-197"><a name="bk_createinlineattachewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="0b936-197"></span></span>

<span data-ttu-id="0b936-198">L’exemple de code suivant montre comment ajouter une pièce jointe à un message électronique existant par :</span><span class="sxs-lookup"><span data-stu-id="0b936-198">The following code example shows how to add an attachment to an existing email by:</span></span> 
  
1. <span data-ttu-id="0b936-199">À l’aide de la méthode [EmailMessage.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) pour lier à un message électronique existant.</span><span class="sxs-lookup"><span data-stu-id="0b936-199">Using the [EmailMessage.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) method to bind to an existing email message.</span></span> 
    
2. <span data-ttu-id="0b936-200">Ajout d’un fichier joint au message à l’aide de la méthode **AddFileAttachment** .</span><span class="sxs-lookup"><span data-stu-id="0b936-200">Adding a file attachment to the message by using the **AddFileAttachment** method.</span></span> 
    
3. <span data-ttu-id="0b936-201">Enregistrer les mises à jour en appelant la méthode [EmailMessage.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="0b936-201">Saving the updates by calling the [EmailMessage.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx) method.</span></span> 
    
<span data-ttu-id="0b936-202">Cet exemple suppose que ce **service** est un objet [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur a été authentifié sur un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="0b936-202">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```XML
public static void AddAttachmentToExisting(ExchangeService service, ItemId itemId)
{
    // This method results in a GetItem call to EWS.
    EmailMessage message = EmailMessage.Bind(service, itemId);
    message.Attachments.AddFileAttachment("C:\\temp\\FileAttachment.txt");
    // This method results in a CreateAttachment call to EWS.
    message.Update(ConflictResolutionMode.AlwaysOverwrite);
}
```

## <a name="add-an-attachment-to-an-existing-email-by-using-ews"></a><span data-ttu-id="0b936-203">Ajouter une pièce jointe à un message électronique existant à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="0b936-203">Add an attachment to an existing email by using EWS</span></span>
<span data-ttu-id="0b936-204"><a name="bk_createinlineattachewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="0b936-204"></span></span>

<span data-ttu-id="0b936-205">L’exemple de code suivant montre comment utiliser l’opération [CreateAttachment](http://msdn.microsoft.com/library/e066db95-6963-4507-a8d0-8efad287f550%28Office.15%29.aspx) pour ajouter une pièce jointe à un message électronique existant.</span><span class="sxs-lookup"><span data-stu-id="0b936-205">The following code example shows how to use the [CreateAttachment](http://msdn.microsoft.com/library/e066db95-6963-4507-a8d0-8efad287f550%28Office.15%29.aspx) operation to add a file attachment to an existing email message.</span></span> <span data-ttu-id="0b936-206">C’est également une des demandes XML qui envoie de l’API managée EWS lorsque vous utilisez l’API managée EWS pour [Ajouter une pièce jointe à un message électronique existant](#bk_createinlineattachewsma).</span><span class="sxs-lookup"><span data-stu-id="0b936-206">This is also one of the XML requests that the EWS Managed API sends when you use the EWS Managed API to [add an attachment to an existing email](#bk_createinlineattachewsma).</span></span>
  
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
    <m:CreateAttachment>
      <m:ParentItemId Id="uqE2AAA=" />
      <m:Attachments>
        <t:FileAttachment>
          <t:Name>FileAttachment.txt</t:Name>
          <t:Content>VGhpcyBpcyBhIGZpbGUgYXR0YWNobWVudC4=</t:Content>
        </t:FileAttachment>
      </m:Attachments>
    </m:CreateAttachment>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="0b936-207">Le serveur répond à la demande **CreateAttachment** avec un message [CreateAttachmentResponse](http://msdn.microsoft.com/library/cf6bd8bb-5317-4a03-bd75-297dd359b5da%28Office.15%29.aspx) qui contient une valeur [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) **NoError**, ce qui indique que la pièce jointe a été créée avec succès et le [ AttachmentId](http://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx) de la pièce jointe nouvellement créée.</span><span class="sxs-lookup"><span data-stu-id="0b936-207">The server responds to the **CreateAttachment** request with a [CreateAttachmentResponse](http://msdn.microsoft.com/library/cf6bd8bb-5317-4a03-bd75-297dd359b5da%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the attachment was created successfully, and the [AttachmentId](http://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx) of the newly created attachment.</span></span> 
  
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
    <m:CreateAttachmentResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                                xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:CreateAttachmentResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Attachments>
            <t:FileAttachment>
              <t:AttachmentId Id="yRLhCh8="
                              RootItemId="uqE2AAA="
                              RootItemChangeKey="CQAAABYAAAAFI5DJmZv+TLtyLOLIF1S5AAAXulcf" />
            </t:FileAttachment>
          </m:Attachments>
        </m:CreateAttachmentResponseMessage>
      </m:ResponseMessages>
    </m:CreateAttachmentResponse>
  </s:Body>
</s:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="0b936-208">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="0b936-208">See also</span></span>


- [<span data-ttu-id="0b936-209">Pièces jointes et EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="0b936-209">Attachments and EWS in Exchange</span></span>](attachments-and-ews-in-exchange.md)
    
- [<span data-ttu-id="0b936-210">Ajouter des pièces jointes à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="0b936-210">Add attachments by using EWS in Exchange</span></span>](how-to-add-attachments-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="0b936-211">Supprimez les pièces jointes à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="0b936-211">Delete attachments by using EWS in Exchange</span></span>](how-to-delete-attachments-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="0b936-212">Obtenir des pièces jointes à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="0b936-212">Get attachments by using EWS in Exchange</span></span>](how-to-get-attachments-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="0b936-213">Envoyer des messages électroniques à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="0b936-213">Send email messages by using EWS in Exchange</span></span>](how-to-send-email-messages-by-using-ews-in-exchange.md)
    

