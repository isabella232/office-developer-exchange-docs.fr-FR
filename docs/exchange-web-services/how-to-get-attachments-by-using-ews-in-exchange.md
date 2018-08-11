---
title: Récupérer des pièces jointes à l’aide d’EWS dans Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 12ce3cc0-a201-42e4-93e1-1f57961ff711
description: Découvrez comment accéder aux pièces jointes à partir d’éléments EWS à l’aide de l’API managée EWS ou d’EWS dans Exchange.
ms.openlocfilehash: 2e1b3cfb346abd068695f66b01f9e34f1f5ff03f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754839"
---
# <a name="get-attachments-by-using-ews-in-exchange"></a><span data-ttu-id="eb518-103">Récupérer des pièces jointes à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="eb518-103">How to: Get attachments by using EWS in Exchange</span></span>

<span data-ttu-id="eb518-104">Découvrez comment accéder aux pièces jointes à partir d’éléments EWS à l’aide de l’API managée EWS ou d’EWS dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="eb518-104">Learn how to get attachments from EWS items by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="eb518-p101">Vous pouvez obtenir des pièces jointes à partir d'un élément à l'aide de l'API managée EWS ou d'EWS. Étant donné que l'appel initial pour obtenir un élément inclut uniquement les métadonnées de la collection de pièces jointes associée à cet élément, la récupération de pièces jointes est toujours un processus en deux étapes. Vous devez d'abord récupérer l'élément, puis sa pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="eb518-p101">You can get attachments from an item by using the EWS Managed API or EWS. Because the initial call to get an item only includes metadata about the attachment collection on the item, retrieving attachments is always a two-step process. First, retrieve the item. Next, retrieve the attachment.</span></span>
  
<span data-ttu-id="eb518-109">**Tableau 1. Méthodes de l'API managée EWS et opérations EWS pour l'ajout de pièces jointes**</span><span class="sxs-lookup"><span data-stu-id="eb518-109">**Table 1. EWS Managed API methods and EWS operations for adding attachments**</span></span>

|<span data-ttu-id="eb518-110">**Tâche**</span><span class="sxs-lookup"><span data-stu-id="eb518-110">**Task**</span></span>|<span data-ttu-id="eb518-111">**Méthode d'API managée EWS**</span><span class="sxs-lookup"><span data-stu-id="eb518-111">**EWS Managed API method**</span></span>|<span data-ttu-id="eb518-112">**Opération EWS**</span><span class="sxs-lookup"><span data-stu-id="eb518-112">**EWS operation**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="eb518-113">Récupérer des pièces jointes (élément)</span><span class="sxs-lookup"><span data-stu-id="eb518-113">Get item attachments</span></span>  <br/> |<span data-ttu-id="eb518-114">[Item.Bind](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) suivi de [ItemAttachment.Load](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.itemattachment.load%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="eb518-114">[Item.Bind](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) followed by [ItemAttachment.Load](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.itemattachment.load%28v=exchg.80%29.aspx)</span></span> <br/> |<span data-ttu-id="eb518-115">[GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) suivi de [GetAttachment](http://msdn.microsoft.com/library/24d10a15-b942-415e-9024-a6375708f326%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="eb518-115">[GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) followed by [GetAttachment](http://msdn.microsoft.com/library/24d10a15-b942-415e-9024-a6375708f326%28Office.15%29.aspx)</span></span> <br/> |
|<span data-ttu-id="eb518-116">Récupérer des pièces jointes (fichier)</span><span class="sxs-lookup"><span data-stu-id="eb518-116">Get file attachments</span></span>  <br/> |<span data-ttu-id="eb518-117">[Item.Bind](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) suivi de [FileAttachment.Load](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.fileattachment.load%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="eb518-117">[Item.Bind](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) followed by [FileAttachment.Load](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.fileattachment.load%28v=exchg.80%29.aspx)</span></span> <br/> |<span data-ttu-id="eb518-118">[GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) suivi de [GetAttachment](http://msdn.microsoft.com/library/24d10a15-b942-415e-9024-a6375708f326%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="eb518-118">[GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) followed by [GetAttachment](http://msdn.microsoft.com/library/24d10a15-b942-415e-9024-a6375708f326%28Office.15%29.aspx)</span></span> <br/> |
   
## <a name="get-attachments-from-an-email-by-using-the-ews-managed-api"></a><span data-ttu-id="eb518-119">Récupérer des pièces jointes à partir d’un e-mail à partir de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="eb518-119">Get attachments from an email by using the EWS Managed API</span></span>
<span data-ttu-id="eb518-120"><a name="bk_getattachewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="eb518-120"></span></span>

<span data-ttu-id="eb518-p102">L'exemple de code suivant permet d'obtenir un objet [EmailMessage](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) à l'aide la méthode **Bind**, puis d'itérer la collection de pièces jointes et d'appeler la méthode **FileAttachment.Load** ou **ItemAttachment.Load** sur chaque pièce jointe, comme requis. Chaque pièce jointe est enregistrée dans le dossier C:\temp\ et chaque pièce jointe est chargée en mémoire. Pour plus d'informations sur l'enregistrement d'une pièce jointe, voir [Enregistrer un e-mail mis en pièce jointe à l'aide de l'API managée EWS](#bk_saveitemattach).</span><span class="sxs-lookup"><span data-stu-id="eb518-p102">The following code example shows how to get an [EmailMessage](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) object by using the **Bind** method, then iterate through the attachment collection and call the **FileAttachment.Load** or **ItemAttachment.Load** method on each attachment as appropriate. Each file attachment is saved to the C:\temp\ folder, and each item attachment is loaded into memory. For information about how to save an item attachment, see [Save an attached email by using the EWS Managed API](#bk_saveitemattach).</span></span>
  
<span data-ttu-id="eb518-124">L'exemple ci-dessous suppose que le **service** est un objet [ExchangeService](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide, que **itemId** correspond à la valeur [ItemId](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.itemid%28v=exchg.80%29.aspx) du message dont les pièces jointes seront extraites et que l'utilisateur a été authentifié auprès d'un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="eb518-124">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, that **itemId** is the [ItemId](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.itemid%28v=exchg.80%29.aspx) of the message from which attachments will be retrieved, and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
public static void GetAttachmentsFromEmail(ExchangeService service, ItemId itemId)
{
    // Bind to an existing message item and retrieve the attachments collection.
    // This method results in an GetItem call to EWS.
    EmailMessage message = EmailMessage.Bind(service, itemId, new PropertySet(ItemSchema.Attachments));
    // Iterate through the attachments collection and load each attachment.
    foreach (Attachment attachment in message.Attachments)
    {
        if (attachment is FileAttachment)
        {
            FileAttachment fileAttachment = attachment as FileAttachment;
            // Load the attachment into a file.
            // This call results in a GetAttachment call to EWS.
            fileAttachment.Load("C:\\temp\\" + fileAttachment.Name);
           
            Console.WriteLine("File attachment name: " + fileAttachment.Name);
        }
        else // Attachment is an item attachment.
        {
            ItemAttachment itemAttachment = attachment as ItemAttachment;
            // Load attachment into memory and write out the subject.
            // This does not save the file like it does with a file attachment.
            // This call results in a GetAttachment call to EWS.
            itemAttachment.Load();
            Console.WriteLine("Item attachment name: " + itemAttachment.Name);
        }
    }
}
```

## <a name="get-an-attachment-from-an-email-by-using-ews"></a><span data-ttu-id="eb518-125">Récupérer une pièce jointe à partir d’un e-mail à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="eb518-125">Get an attachment from an email by using EWS</span></span>
<span data-ttu-id="eb518-126"><a name="bk_getattachewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="eb518-126"></span></span>

<span data-ttu-id="eb518-p103">Pour obtenir des pièces jointes à l'aide d'EWS, vous devez tout d'abord récupérer le message et la collection de pièces jointes pour obtenir l'ID ([AttachmentId (GetAttachment et DeleteAttachment)](http://msdn.microsoft.com/library/4bea1cb5-0a0f-4e14-9b09-f91af8cf9899%28Office.15%29.aspx)) de la pièce jointe à récupérer. Une fois que vous avez une ou plusieurs valeurs **AttachmentId** à récupérer, appelez l'opération [GetAttachment](http://msdn.microsoft.com/library/24d10a15-b942-415e-9024-a6375708f326%28Office.15%29.aspx) pour charger toutes les propriétés associées à la pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="eb518-p103">To get attachments by using EWS, you first need to retrieve the message and the attachment collection to get the [AttachmentId (GetAttachment and DeleteAttachment)](http://msdn.microsoft.com/library/4bea1cb5-0a0f-4e14-9b09-f91af8cf9899%28Office.15%29.aspx) of the attachment to retrieve. After you have one or more **AttachmentId** values to retrieve, call the [GetAttachment](http://msdn.microsoft.com/library/24d10a15-b942-415e-9024-a6375708f326%28Office.15%29.aspx) operation to load all the properties for the attachment.</span></span> 
  
<span data-ttu-id="eb518-p104">L'exemple de code suivant montre comment utiliser l'opération [GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) pour récupérer un message électronique et la collection de pièces jointes associée au message. C'est également la première demande XML que l'API managée EWS envoie lorsque vous l'utilisez pour [obtenir toutes les pièces jointes d'un message électronique](#bk_getattachewsma). Les valeurs de certains attributs ont été raccourcies pour améliorer la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="eb518-p104">The following code example shows how to use the [GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) operation to get an email message and the collection of attachments on the message. This is also the first XML request that the EWS Managed API sends when you use the EWS Managed API to [get all attachments from an email](#bk_getattachewsma). The values of some attributes are shortened for readability.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange207_SP1" />
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
        <t:ItemId Id="ERu/AAA=" />
      </m:ItemIds>
    </m:GetItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="eb518-132">Le serveur répond à la demande **GetItem** par un message [GetItemResponse](http://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx) où [ResponseCode](http://msdn.microsoft.com/fr-FR/library/aa580757%28v=exchg.150%29.aspx) renvoie la valeur **NoError**, ce qui indique que le message a bien été récupéré, et où apparaissent les valeurs [AttachmentId](http://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx) des pièces jointes existantes.</span><span class="sxs-lookup"><span data-stu-id="eb518-132">The server responds to the **GetItem** request with a [GetItemResponse](http://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/fr-FR/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the email was retrieved successfully, and the [AttachmentId](http://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx) values of the existing attachments.</span></span> 
  
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
              <t:ItemId Id="ERu/AAA="
                        ChangeKey="CQAAABYAAAAFI5DJmZv+TLtyLOLIF1S5AAAYEMnd" />
              <t:Attachments>
                <t:FileAttachment>
                  <t:AttachmentId Id="5zTzlqU=" />
                  <t:Name>FileAttachment.txt</t:Name>
                  <t:Size>212</t:Size>
                  <t:LastModifiedTime>2014-05-14T17:59:30</t:LastModifiedTime>
                  <t:IsInline>false</t:IsInline>
                  <t:IsContactPhoto>false</t:IsContactPhoto>
                </t:FileAttachment>
                <t:ItemAttachment>
                  <t:AttachmentId Id="Ktum21o=" />
                  <t:Name>Attached Message Item</t:Name>
                  <t:Size>3063</t:Size>
                  <t:LastModifiedTime>2014-05-14T17:59:30</t:LastModifiedTime>
                  <t:IsInline>false</t:IsInline>
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

<span data-ttu-id="eb518-133">Maintenant que vous disposez des valeurs [AttachmentId](http://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx), appelez [GetAttachment](http://msdn.microsoft.com/library/24d10a15-b942-415e-9024-a6375708f326%28Office.15%29.aspx) pour chaque pièce jointe que vous souhaitez récupérer.</span><span class="sxs-lookup"><span data-stu-id="eb518-133">Now that you have the [AttachmentId](http://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx) values, call [GetAttachment](http://msdn.microsoft.com/library/24d10a15-b942-415e-9024-a6375708f326%28Office.15%29.aspx) on each attachment you want to retrieve.</span></span> 
  
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
    <m:GetAttachment>
      <m:AttachmentIds>
        <t:AttachmentId Id="5zTzlqU=" />
      </m:AttachmentIds>
    </m:GetAttachment>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="eb518-134">Lorsque vous récupérez une pièce jointe, le serveur répond à la demande **GetAttachment** par un message [GetAttachmentResponse](http://msdn.microsoft.com/library/cb65f449-309b-4b6e-8d22-d1967135490c%28Office.15%29.aspx) où [ResponseCode](http://msdn.microsoft.com/fr-FR/library/aa580757%28v=exchg.150%29.aspx) a la valeur **NoError**, ce qui indique que la pièce jointe a bien été récupérée, et où apparaissent tous les éléments associés à l'élément mis en pièce jointe, à savoir ici un message électronique.</span><span class="sxs-lookup"><span data-stu-id="eb518-134">When retrieving an item attachment, the server responds to the **GetAttachment** request with a [GetAttachmentResponse](http://msdn.microsoft.com/library/cb65f449-309b-4b6e-8d22-d1967135490c%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/fr-FR/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the attachment was retrieved successfully, and all the elements for the attached item, which in this case is an email message.</span></span>
  
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
    <m:GetAttachmentResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                             xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetAttachmentResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Attachments>
            <t:ItemAttachment>
              <t:AttachmentId Id="Ktum21o=" />
              <t:Name>Attached Message Item</t:Name>
              <t:Message>
                <t:ItemClass>IPM.Note</t:ItemClass>
                <t:Subject>Message Item Subject</t:Subject>
                <t:Body BodyType="HTML">&amp;lt;meta http-equiv="Content-Type" 
                    content="text/html; charset=utf-8"&amp;gt;Message Item Body</t:Body>
                <t:Size>2859</t:Size>
                <t:IsSubmitted>false</t:IsSubmitted>
                <t:IsDraft>true</t:IsDraft>
                <t:IsFromMe>false</t:IsFromMe>
                <t:IsResend>false</t:IsResend>
                <t:IsUnmodified>false</t:IsUnmodified>
                <t:DateTimeCreated>2014-05-14T17:59:37Z</t:DateTimeCreated>
                <t:ResponseObjects>
                  <t:ForwardItem />
                </t:ResponseObjects>
                <t:DisplayCc />
                <t:DisplayTo>primary; emaildelegate</t:DisplayTo>
                <t:HasAttachments>false</t:HasAttachments>
                <t:Culture>en</t:Culture>
                <t:EffectiveRights>
                  <t:CreateAssociated>false</t:CreateAssociated>
                  <t:CreateContents>false</t:CreateContents>
                  <t:CreateHierarchy>false</t:CreateHierarchy>
                  <t:Delete>true</t:Delete>
                  <t:Modify>true</t:Modify>
                  <t:Read>true</t:Read>
                </t:EffectiveRights>
                <t:LastModifiedName>primary</t:LastModifiedName>
                <t:LastModifiedTime>2014-05-14T17:59:30Z</t:LastModifiedTime>
                <t:IsAssociated>false</t:IsAssociated>
                <t:WebClientReadFormQueryString>?ItemID=AAMk3D&amp;amp;exvsurl=1&amp;amp;viewmodel=
                    ReadMessageItem</t:WebClientReadFormQueryString>
                <t:ConversationId Id="AAQkADIwM2ZlM2ZlLWMwYjctNDg2N/Rc+d0=" />
                <t:ToRecipients>
                  <t:Mailbox>
                    <t:Name>primary</t:Name>
                    <t:EmailAddress>sadie@contoso.com</t:EmailAddress>
                    <t:RoutingType>SMTP</t:RoutingType>
                    <t:MailboxType>Mailbox</t:MailboxType>
                  </t:Mailbox>
                  <t:Mailbox>
                    <t:Name>emaildelegate</t:Name>
                    <t:EmailAddress>ronnie@contoso.com</t:EmailAddress>
                    <t:RoutingType>SMTP</t:RoutingType>
                    <t:MailboxType>Mailbox</t:MailboxType>
                  </t:Mailbox>
                </t:ToRecipients>
                <t:IsReadReceiptRequested>false</t:IsReadReceiptRequested>
                <t:ConversationIndex>AQHPb55BxR5Fm0Arx0yY4xbL9Fz53Q==</t:ConversationIndex>
                <t:ConversationTopic>Message Item Subject</t:ConversationTopic>
                <t:IsRead>true</t:IsRead>
              </t:Message>
            </t:ItemAttachment>
          </m:Attachments>
        </m:GetAttachmentResponseMessage>
      </m:ResponseMessages>
    </m:GetAttachmentResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="eb518-135">Lorsque vous récupérez une pièce jointe, le serveur répond à la demande **GetAttachment** par un message [GetAttachmentResponse](http://msdn.microsoft.com/library/cb65f449-309b-4b6e-8d22-d1967135490c%28Office.15%29.aspx) où [ResponseCode](http://msdn.microsoft.com/fr-FR/library/aa580757%28v=exchg.150%29.aspx) a la valeur **NoError**, ce qui indique que la pièce jointe a bien été récupérée, et où apparaissent tous les éléments associés au fichier de la pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="eb518-135">When retrieving a file attachment, the server responds to the **GetAttachment** request with a [GetAttachmentResponse](http://msdn.microsoft.com/library/cb65f449-309b-4b6e-8d22-d1967135490c%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/fr-FR/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the attachment was retrieved successfully, and all the elements of the file attachment.</span></span>
  
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
    <m:GetAttachmentResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                             xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetAttachmentResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Attachments>
            <t:FileAttachment>
              <t:AttachmentId Id="5zTzlqU=" />
              <t:Name>FileAttachment.txt</t:Name>
              <t:Content>VGhpcyBpcyBhIGZpbGUgYXR0YWNobWVudC4=</t:Content>
            </t:FileAttachment>
          </m:Attachments>
        </m:GetAttachmentResponseMessage>
      </m:ResponseMessages>
    </m:GetAttachmentResponse>
  </s:Body>
</s:Envelope>
```

## <a name="save-an-attached-email-by-using-the-ews-managed-api"></a><span data-ttu-id="eb518-136">Enregistrer un e-mail mis en pièce jointe à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="eb518-136">Save an attached email by using the EWS Managed API</span></span>
<span data-ttu-id="eb518-137"><a name="bk_saveitemattach"> </a></span><span class="sxs-lookup"><span data-stu-id="eb518-137"></span></span>

<span data-ttu-id="eb518-138">Afin d’enregistrer le contenu d’une pièce jointe à l’aide de l’API EWS managée, vous devez enregistrer la[MimeContent](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.item.mimecontent%28v=exchg.80%29.aspx) vers un fichier.</span><span class="sxs-lookup"><span data-stu-id="eb518-138">In order to save the contents of an email attachment using the EWS Managed API, you need to save the [MimeContent](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.item.mimecontent%28v=exchg.80%29.aspx) to a file.</span></span> <span data-ttu-id="eb518-139">Notez que vous perdrez les propriétés étendues définies concernant l’élément, telles que les catégories et les indicateurs de suivi.</span><span class="sxs-lookup"><span data-stu-id="eb518-139">In doing so, you will lose any extended properties set on the item, such as follow-up flags and categories.</span></span> <span data-ttu-id="eb518-140">Cet exemple enregistre l’e-mail transmis en pièce jointe dans le dossier C:\temp\.</span><span class="sxs-lookup"><span data-stu-id="eb518-140">This example saves the email attachment to the to the C:\temp\ folder.</span></span> 
  
<span data-ttu-id="eb518-141">Vous ne pouvez pas déplacer ou copier la pièce jointe vers un autre dossier, car la pièce jointe n'est pas un élément fortement typé. Aussi, si vous essayez de déplacer une pièce jointe vers un autre dossier, utilisez l'exemple de code suivant, puis [importez le fichier](how-to-import-items-by-using-ews-in-exchange.md) dans un autre dossier.</span><span class="sxs-lookup"><span data-stu-id="eb518-141">Note that you cannot move or copy the item attachment to another folder because the item attachment is not a strongly-typed item, so if you're trying to move an attachment to a different folder, use the following code example and then [import the file](how-to-import-items-by-using-ews-in-exchange.md) into a different folder.</span></span> 
  
```cs
public static void SaveEmailAttachment(ExchangeService service, ItemId itemId)
{
    // Bind to an existing message item and retrieve the attachments collection.
    // This method results in an GetItem call to EWS.
    EmailMessage message = EmailMessage.Bind(service, itemId, new PropertySet(ItemSchema.Attachments));
    
    foreach (Attachment attachment in message.Attachments)
    {
        if (attachment is ItemAttachment)
        {
            ItemAttachment itemAttachment = attachment as ItemAttachment;
            itemAttachment.Load(ItemSchema.MimeContent);
            string fileName = "C:\\Temp\\" + itemAttachment.Item.Subject + ".eml";
            // Write the bytes of the attachment into a file.
            File.WriteAllBytes(fileName, itemAttachment.Item.MimeContent.Content);
            Console.WriteLine("Email attachment name: "+ itemAttachment.Item.Subject + ".eml");
        }
    }
}
```

## <a name="see-also"></a><span data-ttu-id="eb518-142">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="eb518-142">See also</span></span>


- [<span data-ttu-id="eb518-143">Pièces jointes et EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="eb518-143">Attachments and EWS in Exchange</span></span>](attachments-and-ews-in-exchange.md)
    
- [<span data-ttu-id="eb518-144">Récupérer des pièces jointes à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="eb518-144">How to: Add attachments by using EWS in Exchange</span></span>](how-to-add-attachments-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="eb518-145">Supprimer des pièces jointes à l'aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="eb518-145">How to: Delete attachments by using EWS in Exchange</span></span>](how-to-delete-attachments-by-using-ews-in-exchange.md)
    

