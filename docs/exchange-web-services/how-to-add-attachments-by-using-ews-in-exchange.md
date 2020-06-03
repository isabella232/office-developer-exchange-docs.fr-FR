---
title: Récupérer des pièces jointes à l’aide d’EWS dans Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.assetid: 0cbce436-2ae6-4fcc-bd8b-f517a0724e55
description: Découvrez comment créer des éléments avec des pièces jointes, ou ajouter des pièces jointes à des éléments existants à l’aide de l’API managée EWS ou d’EWS dans Exchange.
localization_priority: Priority
ms.openlocfilehash: fa98eb437d1289f25cfb827b6fa9b351d842bd40
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528264"
---
# <a name="add-attachments-by-using-ews-in-exchange"></a><span data-ttu-id="72eb9-103">Récupérer des pièces jointes à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="72eb9-103">Add attachments by using EWS in Exchange</span></span>

<span data-ttu-id="72eb9-104">Découvrez comment créer des éléments avec des pièces jointes, ou ajouter des pièces jointes à des éléments existants à l’aide de l’API managée EWS ou d’EWS dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="72eb9-104">Learn how to create new items with attachments, or add attachments to existing items by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="72eb9-105">Vous pouvez ajouter des pièces jointes ou des pièces jointes à des éléments nouveaux ou existants à l’aide de l’API managée EWS ou d’EWS.</span><span class="sxs-lookup"><span data-stu-id="72eb9-105">You can add file attachments or item attachments to new or existing items by using the EWS Managed API or EWS.</span></span> <span data-ttu-id="72eb9-106">Si vous utilisez l’API managée EWS, vous utilisez la même méthode pour ajouter des pièces jointes à des éléments nouveaux ou existants ; Toutefois, la méthode change si vous utilisez un fichier ou une pièce jointe d’élément.</span><span class="sxs-lookup"><span data-stu-id="72eb9-106">If you are using the EWS Managed API, you use the same method to add attachments to new or existing items; however, the method changes if you're using a file or item attachment.</span></span> <span data-ttu-id="72eb9-107">À l’inverse, si vous utilisez EWS, vous utilisez la même opération pour ajouter un fichier ou une pièce jointe à un élément, mais l’opération change si vous ajoutez la pièce jointe à un élément nouveau ou existant.</span><span class="sxs-lookup"><span data-stu-id="72eb9-107">Conversely, if you are using EWS, you use the same operation to add either a file or item attachment to an item, but the operation changes if you're adding the attachment to a new or existing item.</span></span>
  
<span data-ttu-id="72eb9-108">**Tableau 1. Méthodes de l'API managée EWS et opérations EWS pour l'ajout de pièces jointes**</span><span class="sxs-lookup"><span data-stu-id="72eb9-108">**Table 1. EWS Managed API methods and EWS operations for adding attachments**</span></span>

|<span data-ttu-id="72eb9-109">**Tâche**</span><span class="sxs-lookup"><span data-stu-id="72eb9-109">**Task**</span></span>|<span data-ttu-id="72eb9-110">**Méthode d'API managée EWS**</span><span class="sxs-lookup"><span data-stu-id="72eb9-110">**EWS Managed API method**</span></span>|<span data-ttu-id="72eb9-111">**Opération EWS**</span><span class="sxs-lookup"><span data-stu-id="72eb9-111">**EWS operation**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="72eb9-112">Ajouter un fichier en pièce jointe à un message électronique nouveau ou existant</span><span class="sxs-lookup"><span data-stu-id="72eb9-112">Add a file attachment to a new or existing email</span></span>  <br/> |[<span data-ttu-id="72eb9-113">AttachmentCollection.AddFileAttachment</span><span class="sxs-lookup"><span data-stu-id="72eb9-113">AttachmentCollection.AddFileAttachment</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.attachmentcollection.addfileattachment%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="72eb9-114">[CreateItem](https://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) pour un nouveau message électronique</span><span class="sxs-lookup"><span data-stu-id="72eb9-114">[CreateItem](https://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) for a new email</span></span>  <br/> <span data-ttu-id="72eb9-115">[CreateAttachment](https://msdn.microsoft.com/library/e066db95-6963-4507-a8d0-8efad287f550%28Office.15%29.aspx) à ajouter à un message électronique existant</span><span class="sxs-lookup"><span data-stu-id="72eb9-115">[CreateAttachment](https://msdn.microsoft.com/library/e066db95-6963-4507-a8d0-8efad287f550%28Office.15%29.aspx) to add to an existing email</span></span>  <br/> |
|<span data-ttu-id="72eb9-116">Ajouter une pièce jointe à un message électronique nouveau ou existant</span><span class="sxs-lookup"><span data-stu-id="72eb9-116">Add an item attachment to a new or existing email</span></span>  <br/> |[<span data-ttu-id="72eb9-117">AttachmentCollection.AddItemAttachment</span><span class="sxs-lookup"><span data-stu-id="72eb9-117">AttachmentCollection.AddItemAttachment</span></span>](https://msdn.microsoft.com/library/dd634986%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="72eb9-118">[CreateItem](https://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) pour un nouveau message électronique</span><span class="sxs-lookup"><span data-stu-id="72eb9-118">[CreateItem](https://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) for a new email</span></span>  <br/> <span data-ttu-id="72eb9-119">[CreateAttachment](https://msdn.microsoft.com/library/e066db95-6963-4507-a8d0-8efad287f550%28Office.15%29.aspx) à ajouter à un message électronique existant</span><span class="sxs-lookup"><span data-stu-id="72eb9-119">[CreateAttachment](https://msdn.microsoft.com/library/e066db95-6963-4507-a8d0-8efad287f550%28Office.15%29.aspx) to add to an existing email</span></span>  <br/> |
   
## <a name="create-an-email-with-file-and-item-attachments-by-using-the-ews-managed-api"></a><span data-ttu-id="72eb9-120">Créer un message électronique avec des pièces jointes de fichier et d’élément à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="72eb9-120">Create an email with file and item attachments by using the EWS Managed API</span></span>
<span data-ttu-id="72eb9-121"><a name="bk_createattachewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="72eb9-121"><a name="bk_createattachewsma"> </a></span></span>

<span data-ttu-id="72eb9-122">L’exemple de code suivant montre comment créer un message électronique avec plusieurs pièces jointes et une pièce jointe à un élément en procédant comme suit :</span><span class="sxs-lookup"><span data-stu-id="72eb9-122">The following code example shows how to create an email with multiple file attachments and an item attachment by:</span></span> 
  
1. <span data-ttu-id="72eb9-123">Utilisation de l’objet [EmailMessage](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) pour créer un message électronique.</span><span class="sxs-lookup"><span data-stu-id="72eb9-123">Using the [EmailMessage](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) object to create an email message.</span></span> 
    
2. <span data-ttu-id="72eb9-124">Utilisation des méthodes [AttachmentCollection. AddFileAttachment](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.attachmentcollection.addfileattachment%28v=exchg.80%29.aspx) et [AttachmentCollection. AddItemAttachment](https://msdn.microsoft.com/library/dd634986%28v=exchg.80%29.aspx) pour ajouter des pièces jointes au message.</span><span class="sxs-lookup"><span data-stu-id="72eb9-124">Using the [AttachmentCollection.AddFileAttachment](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.attachmentcollection.addfileattachment%28v=exchg.80%29.aspx) and [AttachmentCollection.AddItemAttachment](https://msdn.microsoft.com/library/dd634986%28v=exchg.80%29.aspx) methods to add attachments to the message.</span></span> 
    
3. <span data-ttu-id="72eb9-125">Utilisation de la méthode [EmailMessage. méthodesendandsavecopy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) pour envoyer le message aux destinataires et enregistrer le message dans le dossier éléments envoyés.</span><span class="sxs-lookup"><span data-stu-id="72eb9-125">Using the [EmailMessage.SendAndSaveCopy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) method to send the message to the recipients and save the message in the Sent Items folder.</span></span> 
    
<span data-ttu-id="72eb9-126">Cet exemple de code montre les quatre façons d’ajouter une pièce jointe à un élément à l’aide de l’API managée EWS :</span><span class="sxs-lookup"><span data-stu-id="72eb9-126">This code example shows the four ways in which a file attachment can be added to an item by using the EWS Managed API:</span></span>
  
- <span data-ttu-id="72eb9-127">À l’aide d’un emplacement de fichier complet.</span><span class="sxs-lookup"><span data-stu-id="72eb9-127">By using a fully qualified file location.</span></span>
    
- <span data-ttu-id="72eb9-128">À l’aide d’un emplacement de fichier qualifié complet et d’un nouveau nom de pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="72eb9-128">By using a fully qualified file location and a new attachment name.</span></span>
    
- <span data-ttu-id="72eb9-129">À l’aide d’un tableau d’octets.</span><span class="sxs-lookup"><span data-stu-id="72eb9-129">By using a byte array.</span></span>
    
- <span data-ttu-id="72eb9-130">À l’aide d’un objet Stream.</span><span class="sxs-lookup"><span data-stu-id="72eb9-130">By using a stream.</span></span>
    
<span data-ttu-id="72eb9-131">Notez que la pièce jointe de l’élément dans cet exemple est créée en même temps que le message électronique.</span><span class="sxs-lookup"><span data-stu-id="72eb9-131">Note that the item attachment in this example is created at the same time as the email message.</span></span> <span data-ttu-id="72eb9-132">Pour ajouter un message électronique existant en tant que pièce jointe d’un élément, consultez [la rubrique ajouter un élément existant à un nouveau courrier électronique à l’aide du lamimecontent et de l’API managée EWS](#bk_addexistingemailewsma).</span><span class="sxs-lookup"><span data-stu-id="72eb9-132">To add an existing email message as an item attachment, see [Add an existing item to a new email by using the MimeContent and the EWS Managed API](#bk_addexistingemailewsma).</span></span>
  
<span data-ttu-id="72eb9-133">Cet exemple suppose que le **service** est un objet[ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur a bien été authentifié pour un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="72eb9-133">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
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

## <a name="create-an-email-with-file-and-item-attachments-by-using-ews"></a><span data-ttu-id="72eb9-134">Créer un message électronique avec des pièces jointes de fichier et d’élément à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="72eb9-134">Create an email with file and item attachments by using EWS</span></span>
<span data-ttu-id="72eb9-135"><a name="bk_createattachews"> </a></span><span class="sxs-lookup"><span data-stu-id="72eb9-135"><a name="bk_createattachews"> </a></span></span>

<span data-ttu-id="72eb9-136">L’exemple de code suivant montre comment utiliser l’opération [CreateItem](https://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) pour créer un message électronique avec quatre pièces jointes et une pièce jointe d’un élément.</span><span class="sxs-lookup"><span data-stu-id="72eb9-136">The following code example shows how to use the [CreateItem](https://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) operation to create an email message with four file attachments and one item attachment.</span></span> <span data-ttu-id="72eb9-137">Il s’agit également de l’une des requêtes XML que l’API managée EWS envoie lorsque vous [créez un message électronique avec des pièces jointes de fichier et d’élément](#bk_createattachewsma).</span><span class="sxs-lookup"><span data-stu-id="72eb9-137">This is also one of the XML requests that the EWS Managed API sends when you [create an email with file and item attachments](#bk_createattachewsma).</span></span>
  
<span data-ttu-id="72eb9-138">Notez que la pièce jointe de l’élément dans cet exemple est créée en même temps que le message électronique.</span><span class="sxs-lookup"><span data-stu-id="72eb9-138">Note that the item attachment in this example is created at the same time as the email message.</span></span> <span data-ttu-id="72eb9-139">Pour ajouter un message électronique existant en tant que pièce jointe d’un élément, consultez [la rubrique ajouter un élément existant à un nouveau courrier électronique à l’aide du lamimecontent et de l’API managée EWS](#bk_addexistingemailewsma).</span><span class="sxs-lookup"><span data-stu-id="72eb9-139">To add an existing email message as an item attachment, see [Add an existing item to a new email by using the MimeContent and the EWS Managed API](#bk_addexistingemailewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="72eb9-140">Le serveur répond à la demande **CreateItem** avec un message [CreateItemResponse](https://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) qui inclut une valeur [ResponseCode](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) **NOERROR**, ce qui indique que le courrier électronique et les pièces jointes ont été créés avec succès.</span><span class="sxs-lookup"><span data-stu-id="72eb9-140">The server responds to the **CreateItem** request with a [CreateItemResponse](https://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the email and the attachments were created successfully.</span></span> <span data-ttu-id="72eb9-141">L' [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) du message nouvellement créé et les valeurs [attachmentid](https://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx) de chacune des pièces jointes sont également inclus dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="72eb9-141">The [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) of the newly created message and the [AttachmentId](https://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx) values for each of the attachments is also included in the response.</span></span> <span data-ttu-id="72eb9-142">Les valeurs de certains attributs ont été raccourcies pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="72eb9-142">The values of some attributes have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="939"
                         MinorBuildNumber="12"
                         Version="V2_11"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:CreateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="72eb9-143">Pour [Envoyer ce message nouvellement créé](how-to-send-email-messages-by-using-ews-in-exchange.md), appelez l’opération [SendItem](https://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="72eb9-143">To [send this newly created message](how-to-send-email-messages-by-using-ews-in-exchange.md), call the [SendItem](https://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) operation.</span></span> 
  
## <a name="add-an-existing-item-to-a-new-email-by-using-the-mimecontent-and-the-ews-managed-api"></a><span data-ttu-id="72eb9-144">Ajouter un élément existant à un nouveau courrier électronique à l’aide du Lamimecontent et de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="72eb9-144">Add an existing item to a new email by using the MimeContent and the EWS Managed API</span></span>
<span data-ttu-id="72eb9-145"><a name="bk_addexistingemailewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="72eb9-145"><a name="bk_addexistingemailewsma"> </a></span></span>

<span data-ttu-id="72eb9-146">Pour ajouter un élément existant en tant que pièce jointe d’un élément à un autre élément, vous devez créer une nouvelle pièce jointe d’élément et copier le contenu de l’élément existant dans le nouvel élément.</span><span class="sxs-lookup"><span data-stu-id="72eb9-146">To add an existing item as an item attachment to another item, you need to create a new item attachment and copy the content of the existing item to the new item.</span></span> <span data-ttu-id="72eb9-147">Vous pouvez procéder de deux manières :</span><span class="sxs-lookup"><span data-stu-id="72eb9-147">There are two ways to do this:</span></span> 
  
1. <span data-ttu-id="72eb9-148">Si vous utilisez des messages électroniques en particulier, vous pouvez copier la valeur de la propriété [lamimecontent](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.mimecontent%28v=exchg.80%29.aspx) à partir du message électronique dans la pièce jointe de l’élément nouvellement créé.</span><span class="sxs-lookup"><span data-stu-id="72eb9-148">If you're working with email messages specifically, you can copy the value of the [MimeContent](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.mimecontent%28v=exchg.80%29.aspx) property from the email into the newly created item attachment.</span></span> <span data-ttu-id="72eb9-149">Vous perdrez certaines propriétés pendant ce processus, telles que les indicateurs de suivi et les catégories, mais elle fonctionne parfaitement pour les messages électroniques standard.</span><span class="sxs-lookup"><span data-stu-id="72eb9-149">You will lose some properties during this process, such as follow up flags and categories, but it works great for standard email messages.</span></span> 
    
2. <span data-ttu-id="72eb9-150">Si vous avez besoin d’une fidélité complète pour tous les types d’éléments, vous pouvez créer une liaison avec un élément existant et copier toutes les propriétés et propriétés étendues dans la nouvelle pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="72eb9-150">If you need full fidelity for all item types, you can bind to an existing item and copy all the properties and extended properties into the new attachment.</span></span>
    
<span data-ttu-id="72eb9-151">L’exemple de code suivant illustre la première approche, en copiant le **lamimecontent** dans la nouvelle pièce jointe d’élément.</span><span class="sxs-lookup"><span data-stu-id="72eb9-151">The following code example shows the first approach, copying the **MimeContent** into the new item attachment.</span></span> <span data-ttu-id="72eb9-152">Le suivi de cet exemple est une procédure qui montre comment vous pouvez modifier le code afin d’utiliser la deuxième approche.</span><span class="sxs-lookup"><span data-stu-id="72eb9-152">Following this example is a procedure that shows how you can modify the code to use the second approach.</span></span> 
  
<span data-ttu-id="72eb9-153">Cet exemple part du principe que le **service** est un objet [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur a été authentifié auprès d’un serveur Exchange, et que l' **ID ItemId** est l' [ID ItemId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemid%28v=exchg.80%29.aspx) de l’élément à joindre.</span><span class="sxs-lookup"><span data-stu-id="72eb9-153">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server, and that the **itemId** is the [ItemId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemid%28v=exchg.80%29.aspx) of the item to attach.</span></span> 
  
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

<span data-ttu-id="72eb9-154">Pour modifier cet exemple afin de copier chacune des propriétés de l’élément existant dans la pièce jointe d’un nouvel élément, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="72eb9-154">To modify this example to copy each of the properties on the existing item into the new item attachment, do the following:</span></span> 
  
1. <span data-ttu-id="72eb9-155">Modifiez le jeu de propriétés pour inclure **PropertySet. FirstClassProperties** et toutes les propriétés supplémentaires ou propriétés étendues dont vous avez besoin.</span><span class="sxs-lookup"><span data-stu-id="72eb9-155">Change the property set to include **PropertySet.FirstClassProperties** and any additional properties or extended properties you need.</span></span> 
    
  ```cs
  // Add additional properties to the PropertySet.
  EmailMessage msgToAttach = EmailMessage.Bind(service, itemId, new PropertySet(PropertySet.FirstClassProperties));
  ```

2. <span data-ttu-id="72eb9-156">Supprimez la ligne suivante, car vous n’avez pas besoin de la propriété **lamimecontent** .</span><span class="sxs-lookup"><span data-stu-id="72eb9-156">Remove the following line, because you do not need the **MimeContent** property.</span></span> 
    
  ```cs
  itemAttachment.Item.MimeContent = msgToAttach.MimeContent;
  ```

3. <span data-ttu-id="72eb9-157">Répétez cette ligne pour chaque propriété à copier à partir de l’élément existant vers la nouvelle pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="72eb9-157">Repeat this line for each property to copy from the existing item to the new attachment.</span></span> <span data-ttu-id="72eb9-158">Ne copiez pas l’objet **ItemId** dans la nouvelle pièce jointe d’élément, car il s’agit d’une propriété en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="72eb9-158">Do not copy the **ItemId** into the new item attachment because that's a read-only property.</span></span> 
    
  ```cs
  itemAttachment.Item.Subject = msgToAttach.Subject;
  ```

4. <span data-ttu-id="72eb9-159">Définissez la propriété [PidTagMessageFlags](https://msdn.microsoft.com/library/cc839733.aspx) (0x0E070003) sur **envoyé**dans la pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="72eb9-159">Set the [PidTagMessageFlags](https://msdn.microsoft.com/library/cc839733.aspx) (0x0E070003) property on the attachment to **Sent**.</span></span>
    
  ```cs
  ExtendedPropertyDefinition sent = new ExtendedPropertyDefinition(3591, MapiPropertyType.Integer);
  msgToAttach.Item.SetExtendedProperty(sent, "1");
  ```

## <a name="add-an-existing-item-to-a-new-email-by-using-the-mimecontent-and-ews"></a><span data-ttu-id="72eb9-160">Ajouter un élément existant à un nouveau courrier électronique à l’aide de Lamimecontent et EWS</span><span class="sxs-lookup"><span data-stu-id="72eb9-160">Add an existing item to a new email by using the MimeContent and EWS</span></span>
<span data-ttu-id="72eb9-161"><a name="bk_addexistingemailews"> </a></span><span class="sxs-lookup"><span data-stu-id="72eb9-161"><a name="bk_addexistingemailews"> </a></span></span>

<span data-ttu-id="72eb9-162">Il existe deux façons d’ajouter un élément existant à un nouvel élément :</span><span class="sxs-lookup"><span data-stu-id="72eb9-162">There are two ways to add an existing item to a new item:</span></span> 
  
1. <span data-ttu-id="72eb9-163">Si vous utilisez des messages électroniques en particulier, vous pouvez copier la valeur de l’élément [lamimecontent](https://msdn.microsoft.com/library/4f472a08-5653-4c54-ba65-831dfe32f20f%28Office.15%29.aspx) à partir du message électronique dans la pièce jointe de l’élément nouvellement créé.</span><span class="sxs-lookup"><span data-stu-id="72eb9-163">If you're working with email messages specifically, you can copy the value of the [MimeContent](https://msdn.microsoft.com/library/4f472a08-5653-4c54-ba65-831dfe32f20f%28Office.15%29.aspx) element from the email into the newly created item attachment.</span></span> <span data-ttu-id="72eb9-164">Vous perdrez certaines propriétés pendant ce processus, telles que les indicateurs de suivi et les catégories, mais elle fonctionne parfaitement pour les messages électroniques standard.</span><span class="sxs-lookup"><span data-stu-id="72eb9-164">You will lose some properties during this process, such as follow up flags and categories, but it works great for standard email messages.</span></span> 
    
2. <span data-ttu-id="72eb9-165">Si vous avez besoin d’une fidélité complète pour tous les types d’éléments, vous pouvez créer une liaison avec un élément existant et copier toutes les propriétés et propriétés étendues dans la nouvelle pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="72eb9-165">If you need full fidelity for all item types, you can bind to an existing item and copy all the properties and extended properties into the new attachment.</span></span>
    
<span data-ttu-id="72eb9-166">L’exemple de code suivant montre comment utiliser l’élément **lamimecontent** pour copier le contenu de l’élément d’origine dans la valeur **lamimecontent** de la nouvelle pièce jointe d’élément.</span><span class="sxs-lookup"><span data-stu-id="72eb9-166">The following code example shows how to use the **MimeContent** element to copy the content of the original item into the **MimeContent** value of the new item attachment.</span></span> <span data-ttu-id="72eb9-167">L’exemple utilise les opérations suivantes :</span><span class="sxs-lookup"><span data-stu-id="72eb9-167">The example uses the following operations:</span></span> 
  
1. <span data-ttu-id="72eb9-168">[GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) : pour obtenir le **Lamimecontent** et l' [objet](https://msdn.microsoft.com/library/c140d6c2-deb1-4f67-a908-9397197c4ae7%28Office.15%29.aspx) du message qui deviendra la pièce jointe de l’élément sur le nouveau message.</span><span class="sxs-lookup"><span data-stu-id="72eb9-168">[GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) — To get the **MimeContent** and [Subject](https://msdn.microsoft.com/library/c140d6c2-deb1-4f67-a908-9397197c4ae7%28Office.15%29.aspx) of the message that will become the item attachment on the new message.</span></span> 
    
2. <span data-ttu-id="72eb9-169">[CreateItem](https://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) : pour créer le nouveau message électronique.</span><span class="sxs-lookup"><span data-stu-id="72eb9-169">[CreateItem](https://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) — To create the new email message.</span></span> 
    
3. <span data-ttu-id="72eb9-170">[CreateAttachment](https://msdn.microsoft.com/library/e066db95-6963-4507-a8d0-8efad287f550%28Office.15%29.aspx): pour créer la nouvelle pièce jointe à l’aide du **lamimecontent** et de l' **objet** récupérés par l’opération **GetItem** .</span><span class="sxs-lookup"><span data-stu-id="72eb9-170">[CreateAttachment](https://msdn.microsoft.com/library/e066db95-6963-4507-a8d0-8efad287f550%28Office.15%29.aspx)— To create the new attachment, using the **MimeContent** and **Subject** retrieved by the **GetItem** operation.</span></span> 
    
4. <span data-ttu-id="72eb9-171">[SendItem](https://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) : pour envoyer et enregistrer le message.</span><span class="sxs-lookup"><span data-stu-id="72eb9-171">[SendItem](https://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) — To send and save the message.</span></span> 
    
<span data-ttu-id="72eb9-172">L’exemple commence par récupérer le **lamimecontent** et l' **objet** de l’élément existant.</span><span class="sxs-lookup"><span data-stu-id="72eb9-172">The example starts by retrieving the **MimeContent** and the **Subject** of the existing item.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="72eb9-173">Le serveur répond à la **demande GetItem** avec un [message GetItemResponse](https://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx) qui inclut une valeur [ResponseCode](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) de **NOERROR**, ce qui indique que le message a été récupéré correctement, ainsi que le **lamimecontent** et l' **objet** du message.</span><span class="sxs-lookup"><span data-stu-id="72eb9-173">The server responds to the **GetItem** request with a [GetItemResponse](https://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the email was retrieved successfully, and the **MimeContent** and **Subject** of the email.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="944"
                         MinorBuildNumber="11"
                         Version="V2_12"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="72eb9-174">Ensuite, appelez l’opération **CreateItem** pour créer le nouveau message électronique.</span><span class="sxs-lookup"><span data-stu-id="72eb9-174">Next, call the **CreateItem** operation to create the new email.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="72eb9-175">Le serveur répond à la demande **CreateItem** avec un message [CreateItemResponse](https://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) qui inclut une valeur [ResponseCode](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) **NOERROR**, ce qui indique que le courrier électronique a été créé avec succès.</span><span class="sxs-lookup"><span data-stu-id="72eb9-175">The server responds to the **CreateItem** request with a [CreateItemResponse](https://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the email was created successfully.</span></span>
  
<span data-ttu-id="72eb9-176">Créez ensuite la pièce jointe de l’élément à l’aide de l' **lamimecontent** et de l' **objet** récupérés par l’opération **GetItem** .</span><span class="sxs-lookup"><span data-stu-id="72eb9-176">Next, create the new item attachment by using the **MimeContent** and **Subject** retrieved by the **GetItem** operation.</span></span> <span data-ttu-id="72eb9-177">La valeur de l’élément [parentItemId](https://msdn.microsoft.com/library/72dc4391-72db-44d2-85d9-4718d59886a7%28Office.15%29.aspx) est remplie à l’aide de la valeur **ItemId** renvoyée dans la réponse **CreateItem** .</span><span class="sxs-lookup"><span data-stu-id="72eb9-177">The value of the [ParentItemId](https://msdn.microsoft.com/library/72dc4391-72db-44d2-85d9-4718d59886a7%28Office.15%29.aspx) element is populated by using the **ItemId** value returned in the **CreateItem** response.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="72eb9-178">Le serveur répond à la demande **CreateAttachment** avec un message [CreateAttachmentResponse](https://msdn.microsoft.com/library/cf6bd8bb-5317-4a03-bd75-297dd359b5da%28Office.15%29.aspx) qui inclut une valeur [ResponseCode](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) de **NOERROR**, ce qui indique que la pièce jointe a été créée avec succès, et le [attachmentid](https://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx) de la pièce jointe nouvellement créée.</span><span class="sxs-lookup"><span data-stu-id="72eb9-178">The server responds to the **CreateAttachment** request with a [CreateAttachmentResponse](https://msdn.microsoft.com/library/cf6bd8bb-5317-4a03-bd75-297dd359b5da%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the attachment was created successfully, and the [AttachmentId](https://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx) of the newly created attachment.</span></span> 
  
<span data-ttu-id="72eb9-179">À présent que le nouveau message a été créé et que l’élément a été joint, vous pouvez [Envoyer ce message nouvellement créé](how-to-send-email-messages-by-using-ews-in-exchange.md) en appelant l’opération [SendItem](https://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="72eb9-179">Now that the new message has been created, and the item was attached, you can [send this newly created message](how-to-send-email-messages-by-using-ews-in-exchange.md) by calling the [SendItem](https://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) operation.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="72eb9-180">Le serveur répond à la demande **SendItem** avec un message [SendItemResponse](https://msdn.microsoft.com/library/26ac41c7-57d9-473e-ab7a-bae93e1d2aba%28Office.15%29.aspx) qui inclut une valeur [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NOERROR**, ce qui indique que le courrier électronique a été envoyé avec succès.</span><span class="sxs-lookup"><span data-stu-id="72eb9-180">The server responds to the **SendItem** request with a [SendItemResponse](https://msdn.microsoft.com/library/26ac41c7-57d9-473e-ab7a-bae93e1d2aba%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates that the email was sent successfully.</span></span>
  
## <a name="create-an-email-with-an-inline-attachment-by-using-the-ews-managed-api"></a><span data-ttu-id="72eb9-181">Créer un message électronique avec une pièce jointe incorporée à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="72eb9-181">Create an email with an inline attachment by using the EWS Managed API</span></span>
<span data-ttu-id="72eb9-182"><a name="bk_createinlineattachewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="72eb9-182"><a name="bk_createinlineattachewsma"> </a></span></span>

<span data-ttu-id="72eb9-183">L’exemple de code suivant montre comment créer un message électronique avec une pièce jointe incorporée en procédant comme suit :</span><span class="sxs-lookup"><span data-stu-id="72eb9-183">The following code example shows how to create an email with an inline attachment by:</span></span>
  
1. <span data-ttu-id="72eb9-184">Utilisation de l’objet [EmailMessage](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) pour créer un message électronique.</span><span class="sxs-lookup"><span data-stu-id="72eb9-184">Using the [EmailMessage](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) object to create an email message.</span></span> 
    
2. <span data-ttu-id="72eb9-185">Définition de la propriété [EmailMessage. Body](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.body%28v=exchg.80%29.aspx) sur un corps HTML qui contient une pièce jointe incorporée.</span><span class="sxs-lookup"><span data-stu-id="72eb9-185">Setting the [EmailMessage.Body](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.body%28v=exchg.80%29.aspx) property to an HTML body that includes an inline attachment.</span></span> 
    
3. <span data-ttu-id="72eb9-186">Utilisation de la méthode [AttachmentCollection. AddFileAttachment](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.attachmentcollection.addfileattachment%28v=exchg.80%29.aspx) pour ajouter la pièce jointe au message.</span><span class="sxs-lookup"><span data-stu-id="72eb9-186">Using the [AttachmentCollection.AddFileAttachment](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.attachmentcollection.addfileattachment%28v=exchg.80%29.aspx) method to add the attachment to the message.</span></span> 
    
4. <span data-ttu-id="72eb9-187">Utilisation de la méthode [EmailMessage. méthodesendandsavecopy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) pour envoyer le message au destinataire et enregistrer le message dans le dossier éléments envoyés.</span><span class="sxs-lookup"><span data-stu-id="72eb9-187">Using the [EmailMessage.SendAndSaveCopy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) method to send the message to the recipient and save the message in the Sent Items folder.</span></span> 
    
<span data-ttu-id="72eb9-188">Cet exemple suppose que le **service** est un objet[ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur a bien été authentifié pour un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="72eb9-188">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
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

## <a name="create-an-email-with-an-inline-attachment-by-using-ews"></a><span data-ttu-id="72eb9-189">Créer un message électronique avec une pièce jointe incorporée à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="72eb9-189">Create an email with an inline attachment by using EWS</span></span>
<span data-ttu-id="72eb9-190"><a name="bk_createinlineattachewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="72eb9-190"><a name="bk_createinlineattachewsma"> </a></span></span>

<span data-ttu-id="72eb9-191">L’exemple de code suivant montre comment utiliser l’opération [CreateItem](https://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) pour créer un message électronique avec une pièce jointe de fichier en ligne.</span><span class="sxs-lookup"><span data-stu-id="72eb9-191">The following code example shows how to use the [CreateItem](https://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) operation to create an email message with an inline file attachment.</span></span> <span data-ttu-id="72eb9-192">L’attribut **BodyType** de l’élément [Body](https://msdn.microsoft.com/library/7851ea9b-9f87-4adc-a26f-7a27df4a9bca%28Office.15%29.aspx) indique que le contenu est au format HTML et inclut la source de l’image.</span><span class="sxs-lookup"><span data-stu-id="72eb9-192">The **BodyType** attribute of the [Body](https://msdn.microsoft.com/library/7851ea9b-9f87-4adc-a26f-7a27df4a9bca%28Office.15%29.aspx) element indicates that the content is in HTML format and includes the image source.</span></span> <span data-ttu-id="72eb9-193">Il s’agit également de l’une des requêtes XML que l’API managée EWS envoie lorsque vous utilisez l’API managée EWS pour [créer un message électronique avec une pièce jointe incorporée](#bk_createinlineattachewsma).</span><span class="sxs-lookup"><span data-stu-id="72eb9-193">This is also one of the XML requests that the EWS Managed API sends when you use the EWS Managed API to [create an email with an inline attachment](#bk_createinlineattachewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="72eb9-194">Le serveur répond à la demande**CreateItem** par un message [GetItemResponse](https://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx), qui inclut [ResponseCode](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) renvoyant la valeur **NoError**, indiquant que le message a bien été créé, et où apparaît l’élément [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) du nouveau message.</span><span class="sxs-lookup"><span data-stu-id="72eb9-194">The server responds to the **CreateItem** request with a [CreateItemResponse](https://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the email was created successfully, and the [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) of the newly created message.</span></span> 
  
<span data-ttu-id="72eb9-195">Pour [Envoyer ce message nouvellement créé](how-to-send-email-messages-by-using-ews-in-exchange.md), appelez l’opération [SendItem](https://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="72eb9-195">To [send this newly created message](how-to-send-email-messages-by-using-ews-in-exchange.md), call the [SendItem](https://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) operation.</span></span> 
  
## <a name="add-an-attachment-to-an-existing-email-by-using-the-ews-managed-api"></a><span data-ttu-id="72eb9-196">Ajouter une pièce jointe à un message électronique existant à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="72eb9-196">Add an attachment to an existing email by using the EWS Managed API</span></span>
<span data-ttu-id="72eb9-197"><a name="bk_createinlineattachewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="72eb9-197"><a name="bk_createinlineattachewsma"> </a></span></span>

<span data-ttu-id="72eb9-198">L’exemple de code suivant montre comment ajouter une pièce jointe à un message électronique existant en procédant comme suit :</span><span class="sxs-lookup"><span data-stu-id="72eb9-198">The following code example shows how to add an attachment to an existing email by:</span></span> 
  
1. <span data-ttu-id="72eb9-199">Utilisation de la méthode [EmailMessage. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) pour établir une liaison avec un message électronique existant.</span><span class="sxs-lookup"><span data-stu-id="72eb9-199">Using the [EmailMessage.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) method to bind to an existing email message.</span></span> 
    
2. <span data-ttu-id="72eb9-200">Ajout d’une pièce jointe à un message à l’aide de la méthode **AddFileAttachment** .</span><span class="sxs-lookup"><span data-stu-id="72eb9-200">Adding a file attachment to the message by using the **AddFileAttachment** method.</span></span> 
    
3. <span data-ttu-id="72eb9-201">Enregistrement des mises à jour en appelant la méthode [EmailMessage. Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="72eb9-201">Saving the updates by calling the [EmailMessage.Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx) method.</span></span> 
    
<span data-ttu-id="72eb9-202">Cet exemple suppose que le **service** est un objet[ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur a bien été authentifié pour un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="72eb9-202">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
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

## <a name="add-an-attachment-to-an-existing-email-by-using-ews"></a><span data-ttu-id="72eb9-203">Ajouter une pièce jointe à un message électronique existant à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="72eb9-203">Add an attachment to an existing email by using EWS</span></span>
<span data-ttu-id="72eb9-204"><a name="bk_createinlineattachewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="72eb9-204"><a name="bk_createinlineattachewsma"> </a></span></span>

<span data-ttu-id="72eb9-205">L’exemple de code suivant montre comment utiliser l’opération [CreateAttachment](https://msdn.microsoft.com/library/e066db95-6963-4507-a8d0-8efad287f550%28Office.15%29.aspx) pour ajouter une pièce jointe à un message électronique existant.</span><span class="sxs-lookup"><span data-stu-id="72eb9-205">The following code example shows how to use the [CreateAttachment](https://msdn.microsoft.com/library/e066db95-6963-4507-a8d0-8efad287f550%28Office.15%29.aspx) operation to add a file attachment to an existing email message.</span></span> <span data-ttu-id="72eb9-206">Il s’agit également de l’une des requêtes XML que l’API managée EWS envoie lorsque vous utilisez l’API managée EWS pour [Ajouter une pièce jointe à un message électronique existant](#bk_createinlineattachewsma).</span><span class="sxs-lookup"><span data-stu-id="72eb9-206">This is also one of the XML requests that the EWS Managed API sends when you use the EWS Managed API to [add an attachment to an existing email](#bk_createinlineattachewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="72eb9-207">Le serveur répond à la demande **CreateAttachment** avec un message [CreateAttachmentResponse](https://msdn.microsoft.com/library/cf6bd8bb-5317-4a03-bd75-297dd359b5da%28Office.15%29.aspx) qui inclut une valeur [ResponseCode](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) de **NOERROR**, ce qui indique que la pièce jointe a été créée avec succès, et le [attachmentid](https://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx) de la pièce jointe nouvellement créée.</span><span class="sxs-lookup"><span data-stu-id="72eb9-207">The server responds to the **CreateAttachment** request with a [CreateAttachmentResponse](https://msdn.microsoft.com/library/cf6bd8bb-5317-4a03-bd75-297dd359b5da%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the attachment was created successfully, and the [AttachmentId](https://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx) of the newly created attachment.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="939"
                         MinorBuildNumber="12"
                         Version="V2_11"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:CreateAttachmentResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                                xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="see-also"></a><span data-ttu-id="72eb9-208">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="72eb9-208">See also</span></span>


- [<span data-ttu-id="72eb9-209">Pièces jointes et EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="72eb9-209">Attachments and EWS in Exchange</span></span>](attachments-and-ews-in-exchange.md)
    
- [<span data-ttu-id="72eb9-210">Récupérer des pièces jointes à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="72eb9-210">Add attachments by using EWS in Exchange</span></span>](how-to-add-attachments-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="72eb9-211">Supprimer des pièces jointes à l'aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="72eb9-211">Delete attachments by using EWS in Exchange</span></span>](how-to-delete-attachments-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="72eb9-212">Récupérer des pièces jointes à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="72eb9-212">Get attachments by using EWS in Exchange</span></span>](how-to-get-attachments-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="72eb9-213">Envoyer des messages électroniques à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="72eb9-213">Send email messages by using EWS in Exchange</span></span>](how-to-send-email-messages-by-using-ews-in-exchange.md)
    

