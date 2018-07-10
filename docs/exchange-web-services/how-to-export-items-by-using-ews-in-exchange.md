---
title: Exporter les éléments à l’aide de EWS dans Exchange
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: e93ee68c-e134-4469-9070-fba404d46cb4
description: Découvrez comment exporter les rendez-vous, les messages électroniques, contacts, tâches et autres éléments à l’aide de l’API managée EWS ou EWS dans Exchange.
ms.openlocfilehash: 65b5b2ef1eba66877d5b6f6c3d4237a26a254196
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754836"
---
# <a name="export-items-by-using-ews-in-exchange"></a><span data-ttu-id="4890f-103">Exporter les éléments à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="4890f-103">Export items by using EWS in Exchange</span></span>

<span data-ttu-id="4890f-104">Découvrez comment exporter les rendez-vous, les messages électroniques, contacts, tâches et autres éléments à l’aide de l’API managée EWS ou EWS dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="4890f-104">Learn how to export appointments, emails, contacts, tasks, and other items by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="4890f-105">Vous pouvez exporter les éléments à partir d’Exchange à l’aide de l’API managée EWS ou EWS dans un certain nombre de différentes manières.</span><span class="sxs-lookup"><span data-stu-id="4890f-105">You can export items from Exchange by using the EWS Managed API or EWS in a number of different ways.</span></span> <span data-ttu-id="4890f-106">Dépend de l’option que vous utilisez :</span><span class="sxs-lookup"><span data-stu-id="4890f-106">The option you use depends on:</span></span>
  
- <span data-ttu-id="4890f-107">Le type d’élément qui est exporté.</span><span class="sxs-lookup"><span data-stu-id="4890f-107">The item type that is exported.</span></span>
    
- <span data-ttu-id="4890f-108">Degré de fidélité que vous voulez maintenir entre l’état de l’élément dans Exchange et de l’élément exporté.</span><span class="sxs-lookup"><span data-stu-id="4890f-108">The degree of fidelity that you want maintained between the item state in Exchange and the exported item.</span></span>
    
- <span data-ttu-id="4890f-109">Le format de l’élément exporté.</span><span class="sxs-lookup"><span data-stu-id="4890f-109">The format of the exported item.</span></span>
    
- <span data-ttu-id="4890f-110">Les exigences de post-traitement.</span><span class="sxs-lookup"><span data-stu-id="4890f-110">Any post-processing requirements.</span></span>
    
- <span data-ttu-id="4890f-111">Si vous souhaitez importer l’élément précédent dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="4890f-111">Whether you want to import the item back into Exchange.</span></span>
    
<span data-ttu-id="4890f-112">Cet article explique comment utiliser chacune des options différentes pour exporter les éléments.</span><span class="sxs-lookup"><span data-stu-id="4890f-112">This article shows you how to use each of the different options to export items.</span></span> <span data-ttu-id="4890f-113">Vous pouvez utiliser n’importe quelle option pour exporter des éléments en dehors d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="4890f-113">You can use any option to batch export items out of Exchange.</span></span>
  
## <a name="export-an-item-into-a-custom-format"></a><span data-ttu-id="4890f-114">Exporter un élément dans un format personnalisé</span><span class="sxs-lookup"><span data-stu-id="4890f-114">Export an item into a custom format</span></span>
<span data-ttu-id="4890f-115"><a name="bk_exportcustom"> </a></span><span class="sxs-lookup"><span data-stu-id="4890f-115"></span></span>

<span data-ttu-id="4890f-116">Vous pouvez utiliser les résultats d’un appel de méthode d’API managées [Item.Bind](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getewsma) ou analyser les résultats d’une opération EWS [GetItem](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getews) dans un format qui fonctionne avec les exigences de votre application.</span><span class="sxs-lookup"><span data-stu-id="4890f-116">You can use the results of an [Item.Bind](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getewsma) EWS Managed API method call or parse the results of a [GetItem](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getews) EWS operation into a format that works with your application requirements.</span></span> <span data-ttu-id="4890f-117">Utilisez cette option lorsque vous exportez des éléments afin de les importer dans une base de données, fichier .csv, ou un autre format ou système.</span><span class="sxs-lookup"><span data-stu-id="4890f-117">Use this option when you are exporting items in order to import them into a database, .csv file, or another format or system.</span></span> <span data-ttu-id="4890f-118">Vous pouvez même enregistrer l’élément dans le formulaire de l’élément XML EWS, qui peut être utile car de nombreux systèmes possèdent des capacités d’analyse XML.</span><span class="sxs-lookup"><span data-stu-id="4890f-118">You can even save the item in the form of the item EWS XML, which can be useful because many systems have XML parsing capability.</span></span> <span data-ttu-id="4890f-119">Nous vous recommandons d’utiliser la méthode **Item.Bind** ou l’opération de **GetItem** (sans la propriété [Item.MimeContent](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.item.mimecontent%28v=exchg.80%29.aspx) ), car cette option vous permet de contrôler les propriétés qui est exportés.</span><span class="sxs-lookup"><span data-stu-id="4890f-119">We recommend that you use the **Item.Bind** method or the **GetItem** operation (without the [Item.MimeContent](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.item.mimecontent%28v=exchg.80%29.aspx) property) because this option gives you control over which properties are exported.</span></span> 
  
## <a name="export-items-with-full-fidelity"></a><span data-ttu-id="4890f-120">Exporter des éléments de fidélité</span><span class="sxs-lookup"><span data-stu-id="4890f-120">Export items with full fidelity</span></span>
<span data-ttu-id="4890f-121"><a name="bk_exportfullfidelity"> </a></span><span class="sxs-lookup"><span data-stu-id="4890f-121"></span></span>

<span data-ttu-id="4890f-122">Si vous souhaitez exporter les éléments avec fidélité, vous pouvez utiliser l’opération EWS [ExportItems](http://msdn.microsoft.com/library/e2846abb-0b16-4732-bbd8-038a674672f6%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="4890f-122">If you want to export items with full fidelity, you can use the [ExportItems](http://msdn.microsoft.com/library/e2846abb-0b16-4732-bbd8-038a674672f6%28Office.15%29.aspx) EWS operation.</span></span> <span data-ttu-id="4890f-123">L’opération **ExportItems** exporte chaque élément sous la forme d’un flux de données.</span><span class="sxs-lookup"><span data-stu-id="4890f-123">The **ExportItems** operation exports each item as a data stream.</span></span> <span data-ttu-id="4890f-124">Ce flux de données pour l’analyse n’est pas, mais peut être utilisé comme une sauvegarde au niveau des éléments qui peut être importée dans une boîte aux lettres Exchange.</span><span class="sxs-lookup"><span data-stu-id="4890f-124">This data stream is not for parsing, but can be used as an item-level backup that can be imported back into an Exchange mailbox.</span></span> <span data-ttu-id="4890f-125">Vous pouvez inclure le nombre d’éléments dans chaque demande **ExportItems** , bien qu’il est recommandé que vous n’incluez pas plus de 100 éléments dans chaque appel.</span><span class="sxs-lookup"><span data-stu-id="4890f-125">You can include many items in each **ExportItems** request, although we recommend that you include no more than 100 items in each call.</span></span> <span data-ttu-id="4890f-126">Étant donné que l’API managée EWS n’implémente pas l’opération **ExportItems** , si vous utilisez l’API managée EWS, vous devrez écrire une routine pour envoyer les requêtes web.</span><span class="sxs-lookup"><span data-stu-id="4890f-126">Because the EWS Managed API does not implement the **ExportItems** operation, if you use the EWS Managed API, you'll need to write a routine to send the web requests.</span></span> <span data-ttu-id="4890f-127">Vous pouvez également utiliser la méthode [Item.Bind](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) pour obtenir les métadonnées relatives à l’élément de sorte que vous pouvez indexer et de stocker des informations sur le flux de données.</span><span class="sxs-lookup"><span data-stu-id="4890f-127">You can optionally use the [Item.Bind](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) method to get metadata about the item so that you can index and store information about the data stream.</span></span> 
  
<span data-ttu-id="4890f-128">Nous vous recommandons d’utiliser l’opération **ExportItems** pour exporter les éléments que vous souhaitez importer dans une boîte aux lettres Exchange.</span><span class="sxs-lookup"><span data-stu-id="4890f-128">We recommend that you use the **ExportItems** operation to export items that you plan to import into an Exchange mailbox.</span></span> 
  
<span data-ttu-id="4890f-129">L’exemple suivant montre comment utiliser l’opération **ExportItems** .</span><span class="sxs-lookup"><span data-stu-id="4890f-129">The following example shows how to use the **ExportItems** operation.</span></span> <span data-ttu-id="4890f-130">Dans cet exemple, l’identificateur d’élément est réduite pour une meilleure lisibilité.</span><span class="sxs-lookup"><span data-stu-id="4890f-130">In this example, the item identifier is shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
      xmlns:xsd="http://www.w3.org/2001/XMLSchema"
      xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
      xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013"/>
  </soap:Header>
  <soap:Body>
    <m:ExportItems>
      <m:ItemIds>
        <t:ItemId Id="AAMkAGYzZjZmRiUsidkC+NAAAAY89GAAA="/>
      </m:ItemIds>
    </m:ExportItems>
  </soap:Body>
</soap:Envelope>
```

Le serveur répond à la demande **ExportItems** avec un élément [ExportItemsResponse](http://msdn.microsoft.com/library/ef44354b-fbdb-4f7c-b6bd-b27f56a1d018%28Office.15%29.aspx) qui contient une valeur élément [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, ce qui indique que l’élément a été correctement exporté. La réponse inclut également l’ID d’élément de l’élément exporté et le flux de données qui contient le contenu exporté. <span data-ttu-id="4890f-133">L’exemple suivant montre le corps SOAP qui contient l’élément exporté.</span><span class="sxs-lookup"><span data-stu-id="4890f-133">The following example shows the SOAP body that contains the exported item.</span></span>
  
```XML
<s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
        xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <m:ExportItemsResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
    <m:ResponseMessages>
      <m:ExportItemsResponseMessage ResponseClass="Success">
        <m:ResponseCode>NoError</m:ResponseCode>
        <m:ItemId Id="AAMkAGYzZjZmRiUsidkC+NAAAAY89GAAA=" ChangeKey="FwAAAA=="/>
        <m:Data>
          AQAAAAgAAAAAAAAALgBlAHgAdABlAHMAdAAuAG0AaQBjAHIAbwBzAG8AZgB0AC4A
          cgAyAEAAYQB1AGoAaQBuAGcALQBkAG8AbQAuAGUAeAB0AGUAcwB0AC4AbQBpAGMAcgBvAHMA
          bwBmAHQALgBjAG8AbQAAAAMAADkAAAAAAwD+DwYAAAADAARAAwACQAMADkA=
        </m:Data>
      </m:ExportItemsResponseMessage>
     </m:ResponseMessages>
  </m:ExportItemsResponse>
</s:Body>
```

## <a name="use-the-mime-stream-to-export-into-common-file-formats"></a><span data-ttu-id="4890f-134">Le flux MIME permet d’exporter dans des formats de fichiers communs</span><span class="sxs-lookup"><span data-stu-id="4890f-134">Use the MIME stream to export into common file formats</span></span>
<span data-ttu-id="4890f-135"><a name="bk_exportfullfidelity"> </a></span><span class="sxs-lookup"><span data-stu-id="4890f-135"></span></span>

<span data-ttu-id="4890f-136">Vous pouvez utiliser la méthode d’API managées [Item.Bind](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) ou l’opération EWS [GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) pour obtenir une représentation sous forme de MIME d’un élément.</span><span class="sxs-lookup"><span data-stu-id="4890f-136">You can use the [Item.Bind](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) EWS Managed API method or the [GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) EWS operation to get a MIME representation of an item.</span></span> <span data-ttu-id="4890f-137">Dans la mesure où Exchange ne stocke pas le contenu MIME de chaque élément, il doit convertir la représentation sous forme de base de données de chaque élément dans le flux MIME.</span><span class="sxs-lookup"><span data-stu-id="4890f-137">Because Exchange doesn't store the MIME content of each item, it has to convert the database representation of each item into the MIME stream.</span></span> <span data-ttu-id="4890f-138">Étant donné que la conversion est coûteuse, qu'il n’est pas recommandé que vous demandez le flux MIME pour les éléments à grande échelle.</span><span class="sxs-lookup"><span data-stu-id="4890f-138">Because this conversion is costly, we do not recommend that you request the MIME stream for items on a large scale.</span></span> <span data-ttu-id="4890f-139">Notez également que le flux MIME contient un ensemble limité de propriétés. Vous devrez peut-être envisager d’autres options si le jeu de propriétés ne contienne pas les propriétés dont vous avez besoin.</span><span class="sxs-lookup"><span data-stu-id="4890f-139">Also note that the MIME stream contains a limited set of properties; you might have to consider other options if the property set doesn't contain the properties you need.</span></span> 
  
### <a name="use-the-ews-managed-api-to-export-an-email-into-an-eml-and-mht-file-by-using-the-mime-stream"></a><span data-ttu-id="4890f-140">Utiliser l’API managée EWS pour exporter un message électronique dans un fichier .eml et .mht à l’aide du flux MIME</span><span class="sxs-lookup"><span data-stu-id="4890f-140">Use the EWS Managed API to export an email into an .eml and .mht file by using the MIME stream</span></span>
<span data-ttu-id="4890f-141"><a name="bk_exportemailmime"> </a></span><span class="sxs-lookup"><span data-stu-id="4890f-141"></span></span>

<span data-ttu-id="4890f-142">Outlook et autres applications de messagerie courantes peuvent ouvrir le format de fichier EML (.eml).</span><span class="sxs-lookup"><span data-stu-id="4890f-142">Outlook and other common email applications can open the EML (.eml) file format.</span></span> <span data-ttu-id="4890f-143">L’exemple suivant vous montre comment vous pouvez exporter un message électronique à l’aide du flux MIME et utilisez le flux MIME pour créer un EML et un fichier MIME HTML (.mht).</span><span class="sxs-lookup"><span data-stu-id="4890f-143">The following example shows you how you can export an email by using the MIME stream, and use the MIME stream to create an EML and a MIME HTML (.mht) file.</span></span> <span data-ttu-id="4890f-144">De nombreux navigateurs web prennent en charge le format de fichier HTML MIME.</span><span class="sxs-lookup"><span data-stu-id="4890f-144">Many web browsers support the MIME HTML file format.</span></span> <span data-ttu-id="4890f-145">Cet exemple suppose que ce **service** est un objet [ExchangeService](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide, et que l’utilisateur peut s’authentifier à un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="4890f-145">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, and that the user can authenticate to an Exchange server.</span></span> 
  
```cs
private static void ExportMIMEEmail(ExchangeService service)
{
    Folder inbox = Folder.Bind(service, WellKnownFolderName.Inbox);
    ItemView view = new ItemView(1);
    view.PropertySet = new PropertySet(BasePropertySet.IdOnly);
    // This results in a FindItem call to EWS.
    FindItemsResults<Item> results = inbox.FindItems(view);
    foreach (var item in results)
    { 
        PropertySet props = new PropertySet(EmailMessageSchema.MimeContent);
        // This results in a GetItem call to EWS.
        var email = EmailMessage.Bind(service, item.Id, props);
                
        string emlFileName = @"C:\export\email.eml";
        string mhtFileName = @"C:\export\email.mht";
        // Save as .eml.
        using (FileStream fs = new FileStream(emlFileName, FileMode.Create, FileAccess.Write))
        {
            fs.Write(email.MimeContent.Content, 0, email.MimeContent.Content.Length);
        }
        // Save as .mht.
        using (FileStream fs = new FileStream(mhtFileName, FileMode.Create, FileAccess.Write))
        {
            fs.Write(email.MimeContent.Content, 0, email.MimeContent.Content.Length);
        }
    }
}
```

### <a name="use-the-ews-managed-api-to-export-an-appointment-into-an-ical-file-by-using-the-mime-stream"></a><span data-ttu-id="4890f-146">Utiliser l’API managée EWS pour exporter un rendez-vous dans un fichier iCal à l’aide du flux MIME</span><span class="sxs-lookup"><span data-stu-id="4890f-146">Use the EWS Managed API to export an appointment into an iCal file by using the MIME stream</span></span>
<span data-ttu-id="4890f-147"><a name="bk_exporticalmime"> </a></span><span class="sxs-lookup"><span data-stu-id="4890f-147"></span></span>

<span data-ttu-id="4890f-148">Outlook et autres applications calendrier peuvent ouvrir le format de fichier iCal (.ics).</span><span class="sxs-lookup"><span data-stu-id="4890f-148">Outlook and other common calendar applications can open the iCal (.ics) file format.</span></span> <span data-ttu-id="4890f-149">L’exemple suivant montre comment exporter un rendez-vous à l’aide du flux MIME, utilisez le flux MIME pour créer un fichier iCal.</span><span class="sxs-lookup"><span data-stu-id="4890f-149">The following example shows you how to export an appointment by using the MIME stream, and use the MIME stream to create an iCal file.</span></span> <span data-ttu-id="4890f-150">Notez que de nombreuses propriétés ne sont pas exportées avec le flux MIME, y compris les participants et les propriétés liées à la pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="4890f-150">Note that many properties are not exported with the MIME stream, including attendees and attachment-related properties.</span></span> <span data-ttu-id="4890f-151">Vous pouvez capturer des autres propriétés de EWS par leur demandant et en les enregistrant dans le fichier iCal comme des extensions privées.</span><span class="sxs-lookup"><span data-stu-id="4890f-151">You can capture other properties from EWS by requesting them and saving them in the iCal file as private extensions.</span></span> <span data-ttu-id="4890f-152">Ces extensions privées portent le préfixe « x- ».</span><span class="sxs-lookup"><span data-stu-id="4890f-152">These private extensions are prefixed with "x-".</span></span> 
  
<span data-ttu-id="4890f-153">Cet exemple suppose que ce **service** est un objet [ExchangeService](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide, et que l’utilisateur peut s’authentifier à un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="4890f-153">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, and that the user can authenticate to an Exchange server.</span></span> <span data-ttu-id="4890f-154">Cet exemple part également du principe que vous disposez d’un rendez-vous dont l’objet est « Projections financières 2015 » dans le dossier calendrier.</span><span class="sxs-lookup"><span data-stu-id="4890f-154">This example also assumes that you have an appointment with the subject "2015 Financial Projections" in the calendar folder.</span></span> 
  
```cs
private static void ExportMIMEAppointment(ExchangeService service)
{
    Folder inbox = Folder.Bind(service, WellKnownFolderName.Calendar);
    ItemView view = new ItemView(1);
    view.PropertySet = new PropertySet(BasePropertySet.IdOnly); 
    // This results in a FindItem call to EWS.
    FindItemsResults<Item> results = inbox.FindItems("subject:'2015 Financial Projections'", view);
    foreach (var item in results)
    {
        PropertySet props = new PropertySet(AppointmentSchema.MimeContent);
        // This results in a GetItem call to EWS.
        var email = Appointment.Bind(service, item.Id, props);
        string iCalFileName = @"C:\export\appointment.ics";
        // Save as .ics.
        using (FileStream fs = new FileStream(iCalFileName, FileMode.Create, FileAccess.Write))
        {
            fs.Write(email.MimeContent.Content, 0, email.MimeContent.Content.Length);
        }
    }
}
```

### <a name="use-the-ews-managed-api-to-export-a-contact-into-a-vcard-file-by-using-the-mime-stream"></a><span data-ttu-id="4890f-155">Utiliser l’API managée EWS pour exporter un contact dans un fichier vCard à l’aide du flux MIME</span><span class="sxs-lookup"><span data-stu-id="4890f-155">Use the EWS Managed API to export a contact into a vCard file by using the MIME stream</span></span>
<span data-ttu-id="4890f-156"><a name="bk_exportvcardmime"> </a></span><span class="sxs-lookup"><span data-stu-id="4890f-156"></span></span>

<span data-ttu-id="4890f-157">Outlook et autres applications de gestion des contacts commune peuvent ouvrir le format de fichier vCard (.vcf).</span><span class="sxs-lookup"><span data-stu-id="4890f-157">Outlook and other common contact management applications can open the vCard (.vcf) file format.</span></span> <span data-ttu-id="4890f-158">L’exemple suivant montre comment exporter un contact à l’aide du flux MIME et utilisez le flux MIME pour créer une carte de visite.</span><span class="sxs-lookup"><span data-stu-id="4890f-158">The following example shows you how to export a contact by using the MIME stream, and use the MIME stream to create a vCard.</span></span> <span data-ttu-id="4890f-159">Vous pouvez capturer des autres propriétés de EWS en leur demandant et en enregistrant dans le.</span><span class="sxs-lookup"><span data-stu-id="4890f-159">You can capture other properties from EWS by requesting them and saving them in the .</span></span> <span data-ttu-id="4890f-160">carte de visite comme des extensions privées.</span><span class="sxs-lookup"><span data-stu-id="4890f-160">vCard as private extensions.</span></span> <span data-ttu-id="4890f-161">Ces extensions portent le préfixe « x- ».</span><span class="sxs-lookup"><span data-stu-id="4890f-161">These extensions are prefixed with "x-".</span></span> 
  
<span data-ttu-id="4890f-162">Cet exemple suppose que ce **service** est un objet [ExchangeService](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide, et que l’utilisateur peut s’authentifier à un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="4890f-162">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, and that the user can authenticate to an Exchange server.</span></span> 
  
```cs
private static void ExportMIMEContact(ExchangeService service)
{
    Folder inbox = Folder.Bind(service, WellKnownFolderName.Contacts);
    ItemView view = new ItemView(1);
    view.PropertySet = new PropertySet(BasePropertySet.IdOnly);
    // This results in a FindItem call to EWS.
    FindItemsResults<Item> results = inbox.FindItems(view);
    foreach (var item in results)
    {
        PropertySet props = new PropertySet(ContactSchema.MimeContent);
        // This results in a GetItem call to EWS.
        var email = Contact.Bind(service, item.Id, props);
        string vcfFileName = @"C:\export\contact.vcf";
        // Save as .vcf.
        using (FileStream fs = new FileStream(vcfFileName, FileMode.Create, FileAccess.Write))
        {
            fs.Write(email.MimeContent.Content, 0, email.MimeContent.Content.Length);
        }
    }
}
```

> [!NOTE]
> <span data-ttu-id="4890f-163">Vous ne pouvez pas importer les fichiers vCard à l’aide de la propriété **MimeContent** .</span><span class="sxs-lookup"><span data-stu-id="4890f-163">You cannot import vCard files by using the **MimeContent** property.</span></span> <span data-ttu-id="4890f-164">Vous pouvez importer des contacts à l’aide de la méthode d’API managées [Contact.Save](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.contact.save%28v=exchg.80%29.aspx) ou l’opération EWS [CreateItem](http://msdn.microsoft.com/library/417e994b-0a17-4c24-9527-04796b80b029%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="4890f-164">You can import contacts by using the [Contact.Save](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.contact.save%28v=exchg.80%29.aspx) EWS Managed API method or the [CreateItem](http://msdn.microsoft.com/library/417e994b-0a17-4c24-9527-04796b80b029%28Office.15%29.aspx) EWS operation.</span></span> 
  
### <a name="use-ews-to-export-any-item-by-using-the-mime-stream"></a><span data-ttu-id="4890f-165">Utiliser EWS pour exporter n’importe quel élément à l’aide du flux MIME</span><span class="sxs-lookup"><span data-stu-id="4890f-165">Use EWS to export any item by using the MIME stream</span></span>
<span data-ttu-id="4890f-166"><a name="bk_exportewsmime"> </a></span><span class="sxs-lookup"><span data-stu-id="4890f-166"></span></span>

<span data-ttu-id="4890f-167">Utilisez l’opération **GetItem** pour obtenir le flux MIME d’un élément.</span><span class="sxs-lookup"><span data-stu-id="4890f-167">Use the **GetItem** operation to get the MIME stream of an item.</span></span> <span data-ttu-id="4890f-168">La demande de **GetItem** suivante montre comment demander le contenu MIME d’un élément.</span><span class="sxs-lookup"><span data-stu-id="4890f-168">The following **GetItem** request shows how to request the MIME content of an item.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
  <soap:Body>
    <m:GetItem>
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:IncludeMimeContent>true</t:IncludeMimeContent>
      </m:ItemShape>
      <m:ItemIds>
        <t:ItemId Id="AAMkADEzYjJkLTYxMwB8GqYicWAAA=" ChangeKey="CQAAABzXv"/>
      </m:ItemIds>
    </m:GetItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="4890f-169">L’exemple suivant montre la réponse à une demande pour obtenir le flux MIME.</span><span class="sxs-lookup"><span data-stu-id="4890f-169">The following example shows the response to a request to get the MIME stream.</span></span> <span data-ttu-id="4890f-170">Le flux MIME a été raccourci pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="4890f-170">The MIME stream has been shortened for readability.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" 
                         MinorVersion="0" 
                         MajorBuildNumber="893" 
                         MinorBuildNumber="17" 
                         Version="V2_10" 
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
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
              <t:MimeContent CharacterSet="UTF-8">UmVjZ6IGZyb2b2suY29y5hMzgwZTA1YtDQo=</t:MimeContent>
              <t:ItemId Id="AAMkADEzYjJkLTYxMwB8GqYicWAAA=" ChangeKey="CQAAABzXv"/>
            </t:Message>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </m:GetItemResponse>
  </s:Body>
</s:Envelope>
```

## 
<span data-ttu-id="4890f-171"><a name="bk_exportfullfidelity"> </a></span><span class="sxs-lookup"><span data-stu-id="4890f-171"></span></span>

<span data-ttu-id="4890f-172">Après l’exportation d’éléments, vous souhaiterez [Importer les éléments dans Exchange](how-to-import-items-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="4890f-172">After exporting items, you might want to [import items into Exchange](how-to-import-items-by-using-ews-in-exchange.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="4890f-173">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4890f-173">See also</span></span>


- [<span data-ttu-id="4890f-174">Exporter et importer des éléments à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="4890f-174">Exporting and importing items by using EWS in Exchange</span></span>](exporting-and-importing-items-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="4890f-175">Importer des éléments à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="4890f-175">Import items by using EWS in Exchange</span></span>](how-to-import-items-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="4890f-176">Dossiers et éléments dans EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="4890f-176">Folders and items in EWS in Exchange</span></span>](folders-and-items-in-ews-in-exchange.md)
    
- [<span data-ttu-id="4890f-177">Synchronisation de la boîte aux lettres et les services EWS d'Exchange</span><span class="sxs-lookup"><span data-stu-id="4890f-177">Mailbox synchronization and EWS in Exchange</span></span>](mailbox-synchronization-and-ews-in-exchange.md)
    

