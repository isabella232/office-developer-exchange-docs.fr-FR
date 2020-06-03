---
title: Exporter des éléments à l’aide d’EWS dans Exchange
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.assetid: e93ee68c-e134-4469-9070-fba404d46cb4
description: Découvrez comment exporter des rendez-vous, des courriers électroniques, des contacts, des tâches et d’autres éléments à l’aide de l’API managée EWS ou d’EWS dans Exchange.
localization_priority: Priority
ms.openlocfilehash: a01c9487821958b06ec162f2aee27e2d2804eaaf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455883"
---
# <a name="export-items-by-using-ews-in-exchange"></a><span data-ttu-id="a440a-103">Exporter des éléments à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="a440a-103">Export items by using EWS in Exchange</span></span>

<span data-ttu-id="a440a-104">Découvrez comment exporter des rendez-vous, des courriers électroniques, des contacts, des tâches et d’autres éléments à l’aide de l’API managée EWS ou d’EWS dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="a440a-104">Learn how to export appointments, emails, contacts, tasks, and other items by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="a440a-105">Vous pouvez exporter des éléments à partir d’Exchange à l’aide de l’API managée EWS ou d’EWS de différentes manières.</span><span class="sxs-lookup"><span data-stu-id="a440a-105">You can export items from Exchange by using the EWS Managed API or EWS in a number of different ways.</span></span> <span data-ttu-id="a440a-106">L’option que vous utilisez dépend des éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="a440a-106">The option you use depends on:</span></span>
  
- <span data-ttu-id="a440a-107">Type d’élément exporté.</span><span class="sxs-lookup"><span data-stu-id="a440a-107">The item type that is exported.</span></span>
    
- <span data-ttu-id="a440a-108">Degré de fidélité que vous souhaitez conserver entre l’état de l’élément dans Exchange et l’élément exporté.</span><span class="sxs-lookup"><span data-stu-id="a440a-108">The degree of fidelity that you want maintained between the item state in Exchange and the exported item.</span></span>
    
- <span data-ttu-id="a440a-109">Format de l’élément exporté.</span><span class="sxs-lookup"><span data-stu-id="a440a-109">The format of the exported item.</span></span>
    
- <span data-ttu-id="a440a-110">Toutes les exigences de post-traitement.</span><span class="sxs-lookup"><span data-stu-id="a440a-110">Any post-processing requirements.</span></span>
    
- <span data-ttu-id="a440a-111">Si vous souhaitez réimporter l’élément dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="a440a-111">Whether you want to import the item back into Exchange.</span></span>
    
<span data-ttu-id="a440a-112">Cet article explique comment utiliser chacune des différentes options pour exporter des éléments.</span><span class="sxs-lookup"><span data-stu-id="a440a-112">This article shows you how to use each of the different options to export items.</span></span> <span data-ttu-id="a440a-113">Vous pouvez utiliser n’importe quelle option pour exporter des éléments en dehors d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="a440a-113">You can use any option to batch export items out of Exchange.</span></span>
  
## <a name="export-an-item-into-a-custom-format"></a><span data-ttu-id="a440a-114">Exporter un élément dans un format personnalisé</span><span class="sxs-lookup"><span data-stu-id="a440a-114">Export an item into a custom format</span></span>
<span data-ttu-id="a440a-115"><a name="bk_exportcustom"> </a></span><span class="sxs-lookup"><span data-stu-id="a440a-115"><a name="bk_exportcustom"> </a></span></span>

<span data-ttu-id="a440a-116">Vous pouvez utiliser les résultats d’un [élément. lier](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getewsma) l’appel de la méthode d’API managée EWS ou analyser les résultats d’une opération EWS de [GetItem](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getews) dans un format qui fonctionne avec les exigences de votre application.</span><span class="sxs-lookup"><span data-stu-id="a440a-116">You can use the results of an [Item.Bind](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getewsma) EWS Managed API method call or parse the results of a [GetItem](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getews) EWS operation into a format that works with your application requirements.</span></span> <span data-ttu-id="a440a-117">Utilisez cette option lorsque vous exportez des éléments afin de les importer dans une base de données, un fichier. csv ou un autre format ou système.</span><span class="sxs-lookup"><span data-stu-id="a440a-117">Use this option when you are exporting items in order to import them into a database, .csv file, or another format or system.</span></span> <span data-ttu-id="a440a-118">Vous pouvez même enregistrer l’élément sous la forme du XML EWS de l’élément, ce qui peut être utile, car de nombreux systèmes disposent d’une fonctionnalité d’analyse XML.</span><span class="sxs-lookup"><span data-stu-id="a440a-118">You can even save the item in the form of the item EWS XML, which can be useful because many systems have XML parsing capability.</span></span> <span data-ttu-id="a440a-119">Nous vous recommandons d’utiliser la méthode **Item. bind** ou l’opération **GetItem** (sans la propriété [Item. lamimecontent](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.mimecontent%28v=exchg.80%29.aspx) ) car cette option vous permet de contrôler les propriétés exportées.</span><span class="sxs-lookup"><span data-stu-id="a440a-119">We recommend that you use the **Item.Bind** method or the **GetItem** operation (without the [Item.MimeContent](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.mimecontent%28v=exchg.80%29.aspx) property) because this option gives you control over which properties are exported.</span></span> 
  
## <a name="export-items-with-full-fidelity"></a><span data-ttu-id="a440a-120">Exporter des éléments avec une fidélité totale</span><span class="sxs-lookup"><span data-stu-id="a440a-120">Export items with full fidelity</span></span>
<span data-ttu-id="a440a-121"><a name="bk_exportfullfidelity"> </a></span><span class="sxs-lookup"><span data-stu-id="a440a-121"><a name="bk_exportfullfidelity"> </a></span></span>

<span data-ttu-id="a440a-122">Si vous souhaitez exporter les éléments avec une fidélité totale, vous pouvez utiliser l’opération EWS [ExportItems](https://msdn.microsoft.com/library/e2846abb-0b16-4732-bbd8-038a674672f6%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="a440a-122">If you want to export items with full fidelity, you can use the [ExportItems](https://msdn.microsoft.com/library/e2846abb-0b16-4732-bbd8-038a674672f6%28Office.15%29.aspx) EWS operation.</span></span> <span data-ttu-id="a440a-123">L’opération **ExportItems** exporte chaque élément en tant que flux de données.</span><span class="sxs-lookup"><span data-stu-id="a440a-123">The **ExportItems** operation exports each item as a data stream.</span></span> <span data-ttu-id="a440a-124">Ce flux de données n’est pas destiné à l’analyse, mais peut être utilisé comme une sauvegarde au niveau des éléments qui peut être réimportée dans une boîte aux lettres Exchange.</span><span class="sxs-lookup"><span data-stu-id="a440a-124">This data stream is not for parsing, but can be used as an item-level backup that can be imported back into an Exchange mailbox.</span></span> <span data-ttu-id="a440a-125">Vous pouvez inclure de nombreux éléments dans chaque demande **ExportItems** , bien que nous vous recommandons de ne pas inclure plus de 100 éléments dans chaque appel.</span><span class="sxs-lookup"><span data-stu-id="a440a-125">You can include many items in each **ExportItems** request, although we recommend that you include no more than 100 items in each call.</span></span> <span data-ttu-id="a440a-126">Étant donné que l’API managée EWS n’implémente pas l’opération **ExportItems** , si vous utilisez l’API managée EWS, vous devez écrire une routine pour envoyer les requêtes Web.</span><span class="sxs-lookup"><span data-stu-id="a440a-126">Because the EWS Managed API does not implement the **ExportItems** operation, if you use the EWS Managed API, you'll need to write a routine to send the web requests.</span></span> <span data-ttu-id="a440a-127">Vous pouvez éventuellement utiliser la méthode [Item. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) pour obtenir des métadonnées sur l’élément de sorte que vous puissiez indexer et stocker des informations sur le flux de données.</span><span class="sxs-lookup"><span data-stu-id="a440a-127">You can optionally use the [Item.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) method to get metadata about the item so that you can index and store information about the data stream.</span></span> 
  
<span data-ttu-id="a440a-128">Nous vous recommandons d’utiliser l’opération **ExportItems** pour exporter les éléments que vous envisagez d’importer dans une boîte aux lettres Exchange.</span><span class="sxs-lookup"><span data-stu-id="a440a-128">We recommend that you use the **ExportItems** operation to export items that you plan to import into an Exchange mailbox.</span></span> 
  
<span data-ttu-id="a440a-129">L’exemple suivant montre comment utiliser l’opération **ExportItems** .</span><span class="sxs-lookup"><span data-stu-id="a440a-129">The following example shows how to use the **ExportItems** operation.</span></span> <span data-ttu-id="a440a-130">Dans cet exemple, l’identificateur de l’élément est raccourci pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="a440a-130">In this example, the item identifier is shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
      xmlns:xsd="http://www.w3.org/2001/XMLSchema"
      xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/"
      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
      xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

Le serveur répond à la demande **ExportItems** avec un élément [ExportItemsResponse](https://msdn.microsoft.com/library/ef44354b-fbdb-4f7c-b6bd-b27f56a1d018%28Office.15%29.aspx) qui inclut une valeur d’élément [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NOERROR**, ce qui indique que l’élément a été correctement exporté. La réponse inclut également l’ID de l’élément exporté et le flux de données qui contient le contenu exporté. <span data-ttu-id="a440a-133">L’exemple suivant montre le corps SOAP qui contient l’élément exporté.</span><span class="sxs-lookup"><span data-stu-id="a440a-133">The following example shows the SOAP body that contains the exported item.</span></span>
  
```XML
<s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
        xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <m:ExportItemsResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="use-the-mime-stream-to-export-into-common-file-formats"></a><span data-ttu-id="a440a-134">Utiliser le flux MIME pour exporter dans des formats de fichiers communs</span><span class="sxs-lookup"><span data-stu-id="a440a-134">Use the MIME stream to export into common file formats</span></span>
<span data-ttu-id="a440a-135"><a name="bk_exportfullfidelity"> </a></span><span class="sxs-lookup"><span data-stu-id="a440a-135"><a name="bk_exportfullfidelity"> </a></span></span>

<span data-ttu-id="a440a-136">Vous pouvez utiliser la méthode de l’API managée EWS de l' [élément. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) ou l’opération EWS de [GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) pour obtenir une représentation MIME d’un élément.</span><span class="sxs-lookup"><span data-stu-id="a440a-136">You can use the [Item.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) EWS Managed API method or the [GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) EWS operation to get a MIME representation of an item.</span></span> <span data-ttu-id="a440a-137">Étant donné qu’Exchange ne stocke pas le contenu MIME de chaque élément, il doit convertir la représentation de la base de données de chaque élément dans le flux MIME.</span><span class="sxs-lookup"><span data-stu-id="a440a-137">Because Exchange doesn't store the MIME content of each item, it has to convert the database representation of each item into the MIME stream.</span></span> <span data-ttu-id="a440a-138">Étant donné que cette conversion est coûteuse, nous vous déconseillons de demander le flux MIME pour les éléments à grande échelle.</span><span class="sxs-lookup"><span data-stu-id="a440a-138">Because this conversion is costly, we do not recommend that you request the MIME stream for items on a large scale.</span></span> <span data-ttu-id="a440a-139">Notez également que le flux MIME contient un ensemble limité de propriétés ; vous devrez peut-être prendre en compte d’autres options si le jeu de propriétés ne contient pas les propriétés dont vous avez besoin.</span><span class="sxs-lookup"><span data-stu-id="a440a-139">Also note that the MIME stream contains a limited set of properties; you might have to consider other options if the property set doesn't contain the properties you need.</span></span> 
  
### <a name="use-the-ews-managed-api-to-export-an-email-into-an-eml-and-mht-file-by-using-the-mime-stream"></a><span data-ttu-id="a440a-140">Utiliser l’API managée EWS pour exporter un courrier électronique dans un fichier. eml et. mht à l’aide du flux MIME</span><span class="sxs-lookup"><span data-stu-id="a440a-140">Use the EWS Managed API to export an email into an .eml and .mht file by using the MIME stream</span></span>
<span data-ttu-id="a440a-141"><a name="bk_exportemailmime"> </a></span><span class="sxs-lookup"><span data-stu-id="a440a-141"><a name="bk_exportemailmime"> </a></span></span>

<span data-ttu-id="a440a-142">Outlook et d’autres applications de messagerie courantes peuvent ouvrir le format de fichier EML (. eml).</span><span class="sxs-lookup"><span data-stu-id="a440a-142">Outlook and other common email applications can open the EML (.eml) file format.</span></span> <span data-ttu-id="a440a-143">L’exemple suivant montre comment vous pouvez exporter un courrier électronique à l’aide du flux MIME et utiliser le flux MIME pour créer un fichier EML et un fichier MIME HTML (. mht).</span><span class="sxs-lookup"><span data-stu-id="a440a-143">The following example shows you how you can export an email by using the MIME stream, and use the MIME stream to create an EML and a MIME HTML (.mht) file.</span></span> <span data-ttu-id="a440a-144">De nombreux navigateurs Web prennent en charge le format de fichier HTML MIME.</span><span class="sxs-lookup"><span data-stu-id="a440a-144">Many web browsers support the MIME HTML file format.</span></span> <span data-ttu-id="a440a-145">Cet exemple suppose que le **service** est un objet [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur puisse s’authentifier auprès d’un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="a440a-145">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, and that the user can authenticate to an Exchange server.</span></span> 
  
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

### <a name="use-the-ews-managed-api-to-export-an-appointment-into-an-ical-file-by-using-the-mime-stream"></a><span data-ttu-id="a440a-146">Utiliser l’API managée EWS pour exporter un rendez-vous dans un fichier iCal à l’aide du flux MIME</span><span class="sxs-lookup"><span data-stu-id="a440a-146">Use the EWS Managed API to export an appointment into an iCal file by using the MIME stream</span></span>
<span data-ttu-id="a440a-147"><a name="bk_exporticalmime"> </a></span><span class="sxs-lookup"><span data-stu-id="a440a-147"><a name="bk_exporticalmime"> </a></span></span>

<span data-ttu-id="a440a-148">Outlook et d’autres applications de calendrier courantes peuvent ouvrir le format de fichier iCal (. ICS).</span><span class="sxs-lookup"><span data-stu-id="a440a-148">Outlook and other common calendar applications can open the iCal (.ics) file format.</span></span> <span data-ttu-id="a440a-149">L’exemple suivant montre comment exporter un rendez-vous à l’aide du flux MIME et utiliser le flux MIME pour créer un fichier iCal.</span><span class="sxs-lookup"><span data-stu-id="a440a-149">The following example shows you how to export an appointment by using the MIME stream, and use the MIME stream to create an iCal file.</span></span> <span data-ttu-id="a440a-150">Notez que de nombreuses propriétés ne sont pas exportées avec le flux MIME, y compris les participants et les propriétés associées aux pièces jointes.</span><span class="sxs-lookup"><span data-stu-id="a440a-150">Note that many properties are not exported with the MIME stream, including attendees and attachment-related properties.</span></span> <span data-ttu-id="a440a-151">Vous pouvez capturer d’autres propriétés à partir d’EWS en les demandant et en les enregistrant dans le fichier iCal en tant qu’extensions privées.</span><span class="sxs-lookup"><span data-stu-id="a440a-151">You can capture other properties from EWS by requesting them and saving them in the iCal file as private extensions.</span></span> <span data-ttu-id="a440a-152">Ces extensions privées sont précédées du préfixe « x- ».</span><span class="sxs-lookup"><span data-stu-id="a440a-152">These private extensions are prefixed with "x-".</span></span> 
  
<span data-ttu-id="a440a-153">Cet exemple suppose que le **service** est un objet [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur puisse s’authentifier auprès d’un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="a440a-153">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, and that the user can authenticate to an Exchange server.</span></span> <span data-ttu-id="a440a-154">Cet exemple suppose également que vous avez un rendez-vous avec l’objet « 2015 projections financières » dans le dossier calendrier.</span><span class="sxs-lookup"><span data-stu-id="a440a-154">This example also assumes that you have an appointment with the subject "2015 Financial Projections" in the calendar folder.</span></span> 
  
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

### <a name="use-the-ews-managed-api-to-export-a-contact-into-a-vcard-file-by-using-the-mime-stream"></a><span data-ttu-id="a440a-155">Utiliser l’API managée EWS pour exporter un contact dans un fichier vCard à l’aide du flux MIME</span><span class="sxs-lookup"><span data-stu-id="a440a-155">Use the EWS Managed API to export a contact into a vCard file by using the MIME stream</span></span>
<span data-ttu-id="a440a-156"><a name="bk_exportvcardmime"> </a></span><span class="sxs-lookup"><span data-stu-id="a440a-156"><a name="bk_exportvcardmime"> </a></span></span>

<span data-ttu-id="a440a-157">Outlook et d’autres applications de gestion des contacts courantes peuvent ouvrir le format de fichier vCard (. vcf).</span><span class="sxs-lookup"><span data-stu-id="a440a-157">Outlook and other common contact management applications can open the vCard (.vcf) file format.</span></span> <span data-ttu-id="a440a-158">L’exemple suivant montre comment exporter un contact à l’aide du flux MIME et comment utiliser le flux MIME pour créer une vCard.</span><span class="sxs-lookup"><span data-stu-id="a440a-158">The following example shows you how to export a contact by using the MIME stream, and use the MIME stream to create a vCard.</span></span> <span data-ttu-id="a440a-159">Vous pouvez capturer d’autres propriétés à partir d’EWS en les demandant et en les enregistrant dans le.</span><span class="sxs-lookup"><span data-stu-id="a440a-159">You can capture other properties from EWS by requesting them and saving them in the .</span></span> <span data-ttu-id="a440a-160">vCard en tant qu’extensions privées.</span><span class="sxs-lookup"><span data-stu-id="a440a-160">vCard as private extensions.</span></span> <span data-ttu-id="a440a-161">Ces extensions sont précédées du préfixe « x- ».</span><span class="sxs-lookup"><span data-stu-id="a440a-161">These extensions are prefixed with "x-".</span></span> 
  
<span data-ttu-id="a440a-162">Cet exemple suppose que le **service** est un objet [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur puisse s’authentifier auprès d’un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="a440a-162">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, and that the user can authenticate to an Exchange server.</span></span> 
  
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
> <span data-ttu-id="a440a-163">Vous ne pouvez pas importer de fichiers vCard à l’aide de la propriété **lamimecontent** .</span><span class="sxs-lookup"><span data-stu-id="a440a-163">You cannot import vCard files by using the **MimeContent** property.</span></span> <span data-ttu-id="a440a-164">Vous pouvez importer des contacts à l’aide de la méthode [contact. Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contact.save%28v=exchg.80%29.aspx) de l’API managée EWS ou de la commande [CreateItem](https://msdn.microsoft.com/library/417e994b-0a17-4c24-9527-04796b80b029%28Office.15%29.aspx) EWS.</span><span class="sxs-lookup"><span data-stu-id="a440a-164">You can import contacts by using the [Contact.Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contact.save%28v=exchg.80%29.aspx) EWS Managed API method or the [CreateItem](https://msdn.microsoft.com/library/417e994b-0a17-4c24-9527-04796b80b029%28Office.15%29.aspx) EWS operation.</span></span> 
  
### <a name="use-ews-to-export-any-item-by-using-the-mime-stream"></a><span data-ttu-id="a440a-165">Utiliser EWS pour exporter un élément à l’aide du flux MIME</span><span class="sxs-lookup"><span data-stu-id="a440a-165">Use EWS to export any item by using the MIME stream</span></span>
<span data-ttu-id="a440a-166"><a name="bk_exportewsmime"> </a></span><span class="sxs-lookup"><span data-stu-id="a440a-166"><a name="bk_exportewsmime"> </a></span></span>

<span data-ttu-id="a440a-167">Utilisez l’opération **GetItem** pour obtenir le flux MIME d’un élément.</span><span class="sxs-lookup"><span data-stu-id="a440a-167">Use the **GetItem** operation to get the MIME stream of an item.</span></span> <span data-ttu-id="a440a-168">La demande **GetItem** suivante montre comment demander le contenu MIME d’un élément.</span><span class="sxs-lookup"><span data-stu-id="a440a-168">The following **GetItem** request shows how to request the MIME content of an item.</span></span> 
  
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

<span data-ttu-id="a440a-169">L’exemple suivant montre la réponse à une demande pour obtenir le flux MIME.</span><span class="sxs-lookup"><span data-stu-id="a440a-169">The following example shows the response to a request to get the MIME stream.</span></span> <span data-ttu-id="a440a-170">Le flux MIME a été raccourci pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="a440a-170">The MIME stream has been shortened for readability.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" 
                         MinorVersion="0" 
                         MajorBuildNumber="893" 
                         MinorBuildNumber="17" 
                         Version="V2_10" 
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
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
<span data-ttu-id="a440a-171"><a name="bk_exportfullfidelity"> </a></span><span class="sxs-lookup"><span data-stu-id="a440a-171"><a name="bk_exportfullfidelity"> </a></span></span>

<span data-ttu-id="a440a-172">Après avoir exporté des éléments, vous souhaiterez peut-être [importer des éléments dans Exchange](how-to-import-items-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="a440a-172">After exporting items, you might want to [import items into Exchange](how-to-import-items-by-using-ews-in-exchange.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="a440a-173">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a440a-173">See also</span></span>


- [<span data-ttu-id="a440a-174">Exportation et importation d’éléments à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="a440a-174">Exporting and importing items by using EWS in Exchange</span></span>](exporting-and-importing-items-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="a440a-175">Importer des éléments à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="a440a-175">Import items by using EWS in Exchange</span></span>](how-to-import-items-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="a440a-176">Dossiers et éléments dans EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="a440a-176">Folders and items in EWS in Exchange</span></span>](folders-and-items-in-ews-in-exchange.md)
    
- [<span data-ttu-id="a440a-177">Synchronisation de la boîte aux lettres et les services EWS d'Exchange</span><span class="sxs-lookup"><span data-stu-id="a440a-177">Mailbox synchronization and EWS in Exchange</span></span>](mailbox-synchronization-and-ews-in-exchange.md)
    

