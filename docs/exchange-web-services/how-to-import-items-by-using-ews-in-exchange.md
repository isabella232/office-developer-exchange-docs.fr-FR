---
title: Importer des éléments à l’aide d’EWS dans Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: dd3d3221-c98e-4fa0-81f0-77f733d2f432
description: Découvrez comment importer des rendez-vous, des courriers électroniques, des contacts, des tâches et d’autres éléments à l’aide de l’API managée EWS ou d’EWS dans Exchange.
ms.openlocfilehash: bc874c667c31beb4e59a305626247488cb1a1781
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527984"
---
# <a name="import-items-by-using-ews-in-exchange"></a><span data-ttu-id="2405a-103">Importer des éléments à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="2405a-103">Import items by using EWS in Exchange</span></span>

<span data-ttu-id="2405a-104">Découvrez comment importer des rendez-vous, des courriers électroniques, des contacts, des tâches et d’autres éléments à l’aide de l’API managée EWS ou d’EWS dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="2405a-104">Learn how to import appointments, emails, contacts, tasks, and other items by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="2405a-105">De nombreux systèmes contiennent des rendez-vous, des courriers électroniques, des contacts et des tâches, et vous pouvez importer ces éléments dans Exchange de différentes manières.</span><span class="sxs-lookup"><span data-stu-id="2405a-105">Many systems contain appointments, emails, contacts, and tasks, and you can import those items into Exchange in a number of different ways.</span></span> <span data-ttu-id="2405a-106">L’importation d’éléments dans Exchange est simple lorsque les relations de boîtes aux lettres ne sont pas conservées sur ces éléments.</span><span class="sxs-lookup"><span data-stu-id="2405a-106">Importing items into Exchange is simple when mailbox relationships aren't maintained on those items.</span></span> <span data-ttu-id="2405a-107">Vous pouvez utiliser la méthode [de l’API](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) managée [EWS pour créer les éléments](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.item.save%28v=exchg.80%29.aspx) dans une boîte aux lettres Exchange.</span><span class="sxs-lookup"><span data-stu-id="2405a-107">You can use the [Item.Save](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.item.save%28v=exchg.80%29.aspx) EWS Managed API method or the [CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS operation to create the items in an Exchange mailbox.</span></span> <span data-ttu-id="2405a-108">Toutefois, l’approche simple ne prend pas en charge tous les scénarios ; par exemple :</span><span class="sxs-lookup"><span data-stu-id="2405a-108">The simple approach does not support all scenarios, however; for example:</span></span> 
  
- <span data-ttu-id="2405a-109">Vous ne pouvez pas maintenir la relation entre les organisateurs et les participants lors de l’importation de rendez-vous avec des participants (réunions).</span><span class="sxs-lookup"><span data-stu-id="2405a-109">You cannot maintain the relationship between organizers and attendees when importing appointments with attendees (meetings).</span></span> <span data-ttu-id="2405a-110">Cela signifie que l’organisateur de la réunion devra renvoyer les invitations aux réunions aux participants afin de rétablir la relation entre l’organisateur et les participants.</span><span class="sxs-lookup"><span data-stu-id="2405a-110">This means that the meeting organizer will need to resend meeting invites to attendees in order to reestablish the relationship between the organizer and attendees.</span></span> <span data-ttu-id="2405a-111">Si le rendez-vous a été importé dans le calendrier d’un participant, le rendez-vous n’est pas lié au rendez-vous de l’organisateur de la réunion.</span><span class="sxs-lookup"><span data-stu-id="2405a-111">If the appointment was imported into an attendee's calendar, the appointment will not be related to the meeting organizer's appointment.</span></span> <span data-ttu-id="2405a-112">Les participants doivent accepter l’invitation de réunion renvoyée à partir de l’organisateur afin de rétablir la relation organisateur-participant.</span><span class="sxs-lookup"><span data-stu-id="2405a-112">The attendees will need to accept the resent meeting invite from the organizer in order to reestablish the organizer-attendee relationship.</span></span>
    
- <span data-ttu-id="2405a-113">Les informations sur les utilisateurs ne sont pas conservées lors de l’importation des tâches affectées.</span><span class="sxs-lookup"><span data-stu-id="2405a-113">Information about the assignees is not preserved when assigned tasks are imported.</span></span>
    
<span data-ttu-id="2405a-114">Toutes les options d’importation peuvent être utilisées pour importer par lots des éléments dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="2405a-114">All the import options can be used to batch import items into Exchange.</span></span>
  
## <a name="use-ews-managed-api-or-ews-item-types-to-import-an-item"></a><span data-ttu-id="2405a-115">Utiliser l’API managée EWS ou les types d’élément EWS pour importer un élément</span><span class="sxs-lookup"><span data-stu-id="2405a-115">Use EWS Managed API or EWS item types to import an item</span></span>
<span data-ttu-id="2405a-116"><a name="bk_importproperties"> </a></span><span class="sxs-lookup"><span data-stu-id="2405a-116"><a name="bk_importproperties"> </a></span></span>

<span data-ttu-id="2405a-117">Vous pouvez utiliser l’API managée EWS ou EWS pour importer des courriers électroniques, des contacts, des rendez-vous ou des tâches à partir d’autres systèmes.</span><span class="sxs-lookup"><span data-stu-id="2405a-117">You can use the EWS Managed API or EWS to import emails, contacts, appointments, or tasks from other systems.</span></span> <span data-ttu-id="2405a-118">Il vous suffit de définir les [Propriétés](properties-and-extended-properties-in-ews-in-exchange.md) à partir de votre format source sur l’un des objets suivants, en fonction de ce que vous importez.</span><span class="sxs-lookup"><span data-stu-id="2405a-118">Just set the [properties ](properties-and-extended-properties-in-ews-in-exchange.md) from your source format on any of the following objects, depending on what you're importing.</span></span> 
  
<span data-ttu-id="2405a-119">**Tableau 1. Objets de l’API managée EWS et éléments EWS**</span><span class="sxs-lookup"><span data-stu-id="2405a-119">**Table 1. EWS Managed API objects and EWS elements**</span></span>

|<span data-ttu-id="2405a-120">**Objet de l’API managée EWS**</span><span class="sxs-lookup"><span data-stu-id="2405a-120">**EWS Managed API object**</span></span>|<span data-ttu-id="2405a-121">**Élément EWS**</span><span class="sxs-lookup"><span data-stu-id="2405a-121">**EWS element**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2405a-122">EmailMessage</span><span class="sxs-lookup"><span data-stu-id="2405a-122">EmailMessage</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="2405a-123">Message</span><span class="sxs-lookup"><span data-stu-id="2405a-123">Message</span></span>](https://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx) <br/> |
|[<span data-ttu-id="2405a-124">Contact</span><span class="sxs-lookup"><span data-stu-id="2405a-124">Contact</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="2405a-125">Contact</span><span class="sxs-lookup"><span data-stu-id="2405a-125">Contact</span></span>](https://msdn.microsoft.com/library/66bfff50-7a91-4d81-b6a0-610b9962f677%28Office.15%29.aspx) <br/> |
|[<span data-ttu-id="2405a-126">Rendez-vous</span><span class="sxs-lookup"><span data-stu-id="2405a-126">Appointment</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="2405a-127">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="2405a-127">CalendarItem</span></span>](https://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) <br/> |
|[<span data-ttu-id="2405a-128">Task</span><span class="sxs-lookup"><span data-stu-id="2405a-128">Task</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.task%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="2405a-129">Task</span><span class="sxs-lookup"><span data-stu-id="2405a-129">Task</span></span>](https://msdn.microsoft.com/library/7c84927e-db28-4c5d-b0b5-cbcc2b88d869%28Office.15%29.aspx) <br/> |
   
<span data-ttu-id="2405a-130">Utilisez la méthode d’API managée [Item. Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.save%28v=exchg.80%29.aspx) ou l' [opération EWS EWS](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) pour effectuer l’importation des éléments.</span><span class="sxs-lookup"><span data-stu-id="2405a-130">Use the [Item.Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.save%28v=exchg.80%29.aspx) EWS Managed API method or the [CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS operation to perform the import of items.</span></span> <span data-ttu-id="2405a-131">Cette approche est recommandée lorsque vous importez des éléments à partir d’autres systèmes car vous contrôlez les propriétés qui sont importées.</span><span class="sxs-lookup"><span data-stu-id="2405a-131">We recommend this approach when you're importing items from other systems because you have control over which properties get imported.</span></span> <span data-ttu-id="2405a-132">Pour plus d’informations sur la façon de définir des propriétés sur des éléments, puis de l’enregistrer, voir [créer un élément à l’aide de l’API managée EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_createewsma) ou [créer un élément à l’aide d’EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_createews).</span><span class="sxs-lookup"><span data-stu-id="2405a-132">For more information about how to set properties on items and then save the item, see [Create an item by using the EWS Managed API](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_createewsma) or [Create an item by using EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_createews).</span></span>
  
## <a name="import-items-with-full-fidelity"></a><span data-ttu-id="2405a-133">Importer des éléments avec une fidélité totale</span><span class="sxs-lookup"><span data-stu-id="2405a-133">Import items with full fidelity</span></span>
<span data-ttu-id="2405a-134"><a name="bk_importproperties"> </a></span><span class="sxs-lookup"><span data-stu-id="2405a-134"><a name="bk_importproperties"> </a></span></span>

<span data-ttu-id="2405a-135">Vous pouvez utiliser l’opération EWS [UploadItems](https://msdn.microsoft.com/library/a88cbe99-7968-454d-a545-4f92c330909f%28Office.15%29.aspx) pour télécharger un élément en tant que flux de données.</span><span class="sxs-lookup"><span data-stu-id="2405a-135">You can use the [UploadItems](https://msdn.microsoft.com/library/a88cbe99-7968-454d-a545-4f92c330909f%28Office.15%29.aspx) EWS operation to upload an item as a data stream.</span></span> <span data-ttu-id="2405a-136">Cette représentation de flux de données d’un élément doit provenir des résultats d’un appel d’opération [ExportItems](https://msdn.microsoft.com/library/e2846abb-0b16-4732-bbd8-038a674672f6%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="2405a-136">This data stream representation of an item has to come from the results of an [ExportItems](https://msdn.microsoft.com/library/e2846abb-0b16-4732-bbd8-038a674672f6%28Office.15%29.aspx) operation call.</span></span> <span data-ttu-id="2405a-137">Étant donné que l’API managée EWS n’implémente pas l’opération **UploadItems** , si vous utilisez l’API managée EWS, vous devez écrire une routine pour envoyer les requêtes Web.</span><span class="sxs-lookup"><span data-stu-id="2405a-137">Because the EWS Managed API does not implement the **UploadItems** operation, if you use the EWS Managed API, you'll need to write a routine to send the web requests.</span></span> 
  
<span data-ttu-id="2405a-138">Il s’agit de la méthode la plus simple pour importer des éléments qui ont été exportés à partir d’un autre serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="2405a-138">This is the easiest way to import items that have been exported from another Exchange server.</span></span>
  
<span data-ttu-id="2405a-139">Dans l’exemple suivant, les identificateurs et le contenu des éléments de **données** sont réduits pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="2405a-139">In the following example, the identifiers and the **Data** element content are shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
      xmlns:xsd="http://www.w3.org/2001/XMLSchema"
      xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/"
      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
      xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013_SP1"/>
  </soap:Header>
  <soap:Body>
    <m:UploadItems>
      <m:Items>
        <t:Item CreateAction="CreateNew">
          <t:ParentFolderId  Id="AAMkADEzOTE7kV0AAA=" ChangeKey="AQAAAA=="/>
          <t:Data>AQAAAAgAAAAAAQAAAAADABZADQASDkANABMO</t:Data>
        </t:Item>
      </m:Items>
    </m:UploadItems>
  </soap:Body>
</soap:Envelope>
```

Le serveur répond à la demande **UploadItems** avec un élément [UploadItemsResponse](https://msdn.microsoft.com/library/93044d39-4489-456a-8cce-b6d69873348f%28Office.15%29.aspx) qui inclut une valeur d’élément [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NOERROR**, ce qui indique que l’élément a été téléchargé avec succès. <span data-ttu-id="2405a-141">La réponse inclut également l’ID de l’élément téléchargé.</span><span class="sxs-lookup"><span data-stu-id="2405a-141">The response also includes the item ID of the uploaded item.</span></span> 
  
## <a name="use-the-mime-stream-to-import-from-common-file-formats"></a><span data-ttu-id="2405a-142">Utiliser le flux MIME pour importer à partir de formats de fichiers communs</span><span class="sxs-lookup"><span data-stu-id="2405a-142">Use the MIME stream to import from common file formats</span></span>
<span data-ttu-id="2405a-143"><a name="bk_importproperties"> </a></span><span class="sxs-lookup"><span data-stu-id="2405a-143"><a name="bk_importproperties"> </a></span></span>

<span data-ttu-id="2405a-144">EWS peut importer des fichiers EML (. eml) et iCal (. ICS).</span><span class="sxs-lookup"><span data-stu-id="2405a-144">EWS can import EML (.eml) and iCal (.ics) files.</span></span> <span data-ttu-id="2405a-145">Vous pouvez tester votre contenu MIME pour voir comment l’analyseur MIME Exchange gère le contenu de votre flux MIME.</span><span class="sxs-lookup"><span data-stu-id="2405a-145">You'll want to test your MIME content to see how the Exchange MIME parser handles the content of your MIME stream.</span></span> <span data-ttu-id="2405a-146">Bien que l’utilisation du flux MIME soit pratique, il est généralement préférable d' [utiliser l’API managée EWS ou les types d’élément EWS pour importer un élément](#bk_importproperties).</span><span class="sxs-lookup"><span data-stu-id="2405a-146">Although using the MIME stream is convenient, it is typically better to [Use EWS Managed API or EWS item types to import an item](#bk_importproperties).</span></span> <span data-ttu-id="2405a-147">Voici un exemple d' [importation d’une vCard](https://code.msdn.microsoft.com/How-to-Import-vCard-Files-ffa0ff50).</span><span class="sxs-lookup"><span data-stu-id="2405a-147">Here's an example of how to [import a vCard](https://code.msdn.microsoft.com/How-to-Import-vCard-Files-ffa0ff50).</span></span>
  
### <a name="use-the-ews-managed-api-to-import-an-email-from-an-eml-file-by-using-the-mime-stream"></a><span data-ttu-id="2405a-148">Utiliser l’API managée EWS pour importer un message électronique à partir d’un fichier EML à l’aide du flux MIME</span><span class="sxs-lookup"><span data-stu-id="2405a-148">Use the EWS Managed API to import an email from an EML file by using the MIME stream</span></span>

<span data-ttu-id="2405a-149">L’exemple suivant montre comment définir la propriété [lamimecontent](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.mimecontent%28v=exchg.80%29.aspx) avec le contenu d’un fichier EML, puis importer le courrier électronique dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="2405a-149">The following example shows how to set the [MimeContent](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.mimecontent%28v=exchg.80%29.aspx) property with the contents of an EML file and then import the email into a mailbox.</span></span> <span data-ttu-id="2405a-150">Cet exemple montre également comment définir la propriété étendue [PidTagMessageFlags (0x0E07)](https://msdn.microsoft.com/library/office/cc839733%28v=office.15%29.aspx) sur un message électronique importé de sorte qu’elle n’apparaisse pas dans la boîte aux lettres en tant qu’élément de brouillon.</span><span class="sxs-lookup"><span data-stu-id="2405a-150">This example also shows how to set the [PidTagMessageFlags (0x0E07)](https://msdn.microsoft.com/library/office/cc839733%28v=office.15%29.aspx) extended property on an imported email so that it doesn't appear in the mailbox as a draft item.</span></span> <span data-ttu-id="2405a-151">Cet exemple suppose que le **service** est un objet [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur puisse s’authentifier auprès d’un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="2405a-151">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, and that the user can authenticate to an Exchange server.</span></span> 
  
```cs
private static void UploadMIMEEmail(ExchangeService service)
{
    EmailMessage email = new EmailMessage(service);
    
    string emlFileName = @"C:\import\email.eml";
    using (FileStream fs = new FileStream(emlFileName, FileMode.Open, FileAccess.Read))
    {
        byte[] bytes = new byte[fs.Length];
        int numBytesToRead = (int)fs.Length;
        int numBytesRead = 0;
        while (numBytesToRead > 0)
        {
            int n = fs.Read(bytes, numBytesRead, numBytesToRead);
            if (n == 0)
                break;
            numBytesRead += n;
            numBytesToRead -= n;
        }
        // Set the contents of the .eml file to the MimeContent property.
        email.MimeContent = new MimeContent("UTF-8", bytes);
    }
    
    // Indicate that this email is not a draft. Otherwise, the email will appear as a 
    // draft to clients.
    ExtendedPropertyDefinition PR_MESSAGE_FLAGS_msgflag_read = new ExtendedPropertyDefinition(3591, MapiPropertyType.Integer);
    email.SetExtendedProperty(PR_MESSAGE_FLAGS_msgflag_read, 1);
    // This results in a CreateItem call to EWS. The email will be saved in the Inbox folder.
    email.Save(WellKnownFolderName.Inbox);
}
```

### <a name="use-the-ews-managed-api-to-import-an-appointment-from-an-ical-file-by-using-the-mime-stream"></a><span data-ttu-id="2405a-152">Utiliser l’API managée EWS pour importer un rendez-vous à partir d’un fichier iCal à l’aide du flux MIME</span><span class="sxs-lookup"><span data-stu-id="2405a-152">Use the EWS Managed API to import an appointment from an iCal file by using the MIME stream</span></span>

<span data-ttu-id="2405a-153">Vous pouvez importer des rendez-vous simples sous la forme de fichiers iCalendar à l’aide du flux MIME.</span><span class="sxs-lookup"><span data-stu-id="2405a-153">You can import simple appointments in the form of iCalendar files by using the MIME stream.</span></span> <span data-ttu-id="2405a-154">Vous ne pouvez pas importer de réunions, qui sont des rendez-vous avec des participants, car la relation entre les organisateurs de réunion et les participants doit être définie dans le flux de travail de [calendrier Exchange](calendars-and-ews-in-exchange.md) .</span><span class="sxs-lookup"><span data-stu-id="2405a-154">You can't import meetings, which are appointments with attendees, because the relationship between meeting organizers and attendees has to be set as part of the [Exchange calendaring](calendars-and-ews-in-exchange.md) workflow.</span></span> <span data-ttu-id="2405a-155">Les participants ne peuvent pas être capturés dans le flux MIME.</span><span class="sxs-lookup"><span data-stu-id="2405a-155">Attendees cannot be captured in the MIME stream.</span></span> 
  
<span data-ttu-id="2405a-156">L’exemple de code suivant montre comment importer un fichier. ICS simple dans la boîte aux lettres d’un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="2405a-156">The following code example shows you how to import a simple .ics file into a user's mailbox.</span></span>
  
```cs
private static void UploadMIMEAppointment(ExchangeService service)
{
    Appointment appointment = new Appointment(service);
    string iCalFileName = @"C:\import\appointment.ics";
    using (FileStream fs = new FileStream(iCalFileName, FileMode.Open, FileAccess.Read))
    {
        byte[] bytes = new byte[fs.Length];
        int numBytesToRead = (int)fs.Length;
        int numBytesRead = 0;
        while (numBytesToRead > 0)
        {
            int n = fs.Read(bytes, numBytesRead, numBytesToRead);
            if (n == 0)
                break;
            numBytesRead += n;
            numBytesToRead -= n;
        }
        // Set the contents of the .ics file to the MimeContent property.
        appointment.MimeContent = new MimeContent("UTF-8", bytes);
    }
    // This results in a CreateItem call to EWS. 
    appointment.Save(WellKnownFolderName.Calendar);
}
```

### <a name="use-ews-to-import-an-item-by-using-the-mime-stream"></a><span data-ttu-id="2405a-157">Utiliser EWS pour importer un élément à l’aide du flux MIME</span><span class="sxs-lookup"><span data-stu-id="2405a-157">Use EWS to import an item by using the MIME stream</span></span>

<span data-ttu-id="2405a-158">Vous pouvez utiliser l’opération EWS EWS pour importer des éléments EML et iCal à l' [aide de leur](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) flux MIME.</span><span class="sxs-lookup"><span data-stu-id="2405a-158">You can use the [CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS operation to import EML and iCal items by using their MIME stream.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013_SP1" />
    <t:MailboxCulture>en-US</t:MailboxCulture>
  </soap:Header>
  <soap:Body >
    <m:CreateItem>
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="inbox"/>
      </m:SavedItemFolderId> 
        <m:Items>
        <t:Message>
          <t:MimeContent CharacterSet="UTF-8">
            <!-- Insert MIME content here-->
          </t:MimeContent>
        </t:Message>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

## <a name="next-steps"></a><span data-ttu-id="2405a-159">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="2405a-159">Next steps</span></span>
<span data-ttu-id="2405a-160"><a name="bk_importproperties"> </a></span><span class="sxs-lookup"><span data-stu-id="2405a-160"><a name="bk_importproperties"> </a></span></span>

<span data-ttu-id="2405a-161">Après avoir importé des éléments dans une boîte aux lettres, vous pouvez [créer un dossier personnalisé pour stocker vos éléments importés](how-to-work-with-folders-by-using-ews-in-exchange.md), ou [synchroniser vos éléments de client et de boîte aux lettres](mailbox-synchronization-and-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="2405a-161">After you import items into a mailbox, you might want to [create a custom folder to store your imported items](how-to-work-with-folders-by-using-ews-in-exchange.md), or [synchronize your client and mailbox items](mailbox-synchronization-and-ews-in-exchange.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="2405a-162">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="2405a-162">See also</span></span>


- [<span data-ttu-id="2405a-163">Exportation et importation d’éléments à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="2405a-163">Exporting and importing items by using EWS in Exchange</span></span>](exporting-and-importing-items-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="2405a-164">Exporter des éléments à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="2405a-164">Export items by using EWS in Exchange</span></span>](how-to-export-items-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="2405a-165">Dossiers et éléments dans EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="2405a-165">Folders and items in EWS in Exchange</span></span>](folders-and-items-in-ews-in-exchange.md)
    
- [<span data-ttu-id="2405a-166">Synchronisation de la boîte aux lettres et les services EWS d'Exchange</span><span class="sxs-lookup"><span data-stu-id="2405a-166">Mailbox synchronization and EWS in Exchange</span></span>](mailbox-synchronization-and-ews-in-exchange.md)
    

