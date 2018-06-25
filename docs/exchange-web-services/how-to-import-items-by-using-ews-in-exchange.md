---
title: Importer des éléments à l’aide de EWS dans Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: dd3d3221-c98e-4fa0-81f0-77f733d2f432
description: Découvrez comment importer les rendez-vous, les messages électroniques, contacts, tâches et autres éléments à l’aide de l’API managée EWS ou EWS dans Exchange.
ms.openlocfilehash: c09c96eff455b7584b084e71b937853abfde731d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754894"
---
# <a name="import-items-by-using-ews-in-exchange"></a><span data-ttu-id="8693d-103">Importer des éléments à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="8693d-103">Import items by using EWS in Exchange</span></span>

<span data-ttu-id="8693d-104">Découvrez comment importer les rendez-vous, les messages électroniques, contacts, tâches et autres éléments à l’aide de l’API managée EWS ou EWS dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="8693d-104">Learn how to import appointments, emails, contacts, tasks, and other items by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="8693d-105">De nombreux systèmes contiennent des messages électroniques, contacts, tâches et rendez-vous et vous pouvez importer ces éléments dans Exchange dans un certain nombre de différentes manières.</span><span class="sxs-lookup"><span data-stu-id="8693d-105">Many systems contain appointments, emails, contacts, and tasks, and you can import those items into Exchange in a number of different ways.</span></span> <span data-ttu-id="8693d-106">Importation d’éléments dans Exchange est simple lorsque les relations de boîte aux lettres ne sont pas conservées sur ces éléments.</span><span class="sxs-lookup"><span data-stu-id="8693d-106">Importing items into Exchange is simple when mailbox relationships aren't maintained on those items.</span></span> <span data-ttu-id="8693d-107">Vous pouvez utiliser la méthode d’API managées [Item.Save](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.item.save%28v=exchg.80%29.aspx) ou l’opération EWS [CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) pour créer les éléments dans une boîte aux lettres Exchange.</span><span class="sxs-lookup"><span data-stu-id="8693d-107">You can use the [Item.Save](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.item.save%28v=exchg.80%29.aspx) EWS Managed API method or the [CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS operation to create the items in an Exchange mailbox.</span></span> <span data-ttu-id="8693d-108">L’approche simple ne prend pas en charge tous les scénarios, par exemple :</span><span class="sxs-lookup"><span data-stu-id="8693d-108">The simple approach does not support all scenarios, however; for example:</span></span> 
  
- <span data-ttu-id="8693d-109">Vous ne pouvez pas mettre à jour la relation entre les organisateurs et les participants lors de l’importation des rendez-vous avec les participants (réunions).</span><span class="sxs-lookup"><span data-stu-id="8693d-109">You cannot maintain the relationship between organizers and attendees when importing appointments with attendees (meetings).</span></span> <span data-ttu-id="8693d-110">Cela signifie que l’organisateur de la réunion vous devrez renvoyer des invitations de réunion aux participants afin de rétablir la relation entre l’organisateur et les participants.</span><span class="sxs-lookup"><span data-stu-id="8693d-110">This means that the meeting organizer will need to resend meeting invites to attendees in order to reestablish the relationship between the organizer and attendees.</span></span> <span data-ttu-id="8693d-111">Si le rendez-vous a été importé dans le calendrier du participant, le rendez-vous ne sera pas être lié à un rendez-vous de l’organisateur de la réunion.</span><span class="sxs-lookup"><span data-stu-id="8693d-111">If the appointment was imported into an attendee's calendar, the appointment will not be related to the meeting organizer's appointment.</span></span> <span data-ttu-id="8693d-112">Les participants devez accepter l’invitation à la réunion récente de la bibliothèque multimédia afin de rétablir la relation participant à la bibliothèque multimédia.</span><span class="sxs-lookup"><span data-stu-id="8693d-112">The attendees will need to accept the resent meeting invite from the organizer in order to reestablish the organizer-attendee relationship.</span></span>
    
- <span data-ttu-id="8693d-113">Plus d’informations sur les intervenants ne sont pas conservées lors de l’importation des tâches affectées.</span><span class="sxs-lookup"><span data-stu-id="8693d-113">Information about the assignees is not preserved when assigned tasks are imported.</span></span>
    
<span data-ttu-id="8693d-114">Toutes les options d’importation permet d’importer des éléments de lot dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="8693d-114">All the import options can be used to batch import items into Exchange.</span></span>
  
## <a name="use-ews-managed-api-or-ews-item-types-to-import-an-item"></a><span data-ttu-id="8693d-115">Utilisation API managées ou EWS types pour importer un élément d’éléments</span><span class="sxs-lookup"><span data-stu-id="8693d-115">Use EWS Managed API or EWS item types to import an item</span></span>
<span data-ttu-id="8693d-116"><a name="bk_importproperties"> </a></span><span class="sxs-lookup"><span data-stu-id="8693d-116"></span></span>

<span data-ttu-id="8693d-117">Vous pouvez utiliser les API managées EWS pour importer les messages électroniques, des contacts, des rendez-vous ou des tâches à partir d’autres systèmes.</span><span class="sxs-lookup"><span data-stu-id="8693d-117">You can use the EWS Managed API or EWS to import emails, contacts, appointments, or tasks from other systems.</span></span> <span data-ttu-id="8693d-118">Définissez simplement les [Propriétés](properties-and-extended-properties-in-ews-in-exchange.md) à partir de votre format source sur un des objets suivants, selon que vous importez.</span><span class="sxs-lookup"><span data-stu-id="8693d-118">Just set the [properties ](properties-and-extended-properties-in-ews-in-exchange.md) from your source format on any of the following objects, depending on what you're importing.</span></span> 
  
<span data-ttu-id="8693d-119">**Le tableau 1. Objets d’API managées et éléments EWS**</span><span class="sxs-lookup"><span data-stu-id="8693d-119">**Table 1. EWS Managed API objects and EWS elements**</span></span>

|<span data-ttu-id="8693d-120">**Objet d’API managées**</span><span class="sxs-lookup"><span data-stu-id="8693d-120">**EWS Managed API object**</span></span>|<span data-ttu-id="8693d-121">**Élément EWS**</span><span class="sxs-lookup"><span data-stu-id="8693d-121">**EWS element**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8693d-122">EmailMessage</span><span class="sxs-lookup"><span data-stu-id="8693d-122">EmailMessage</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="8693d-123">Message</span><span class="sxs-lookup"><span data-stu-id="8693d-123">Message</span></span>](http://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx) <br/> |
|[<span data-ttu-id="8693d-124">Contact</span><span class="sxs-lookup"><span data-stu-id="8693d-124">Contact</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="8693d-125">Contact</span><span class="sxs-lookup"><span data-stu-id="8693d-125">Contact</span></span>](http://msdn.microsoft.com/library/66bfff50-7a91-4d81-b6a0-610b9962f677%28Office.15%29.aspx) <br/> |
|[<span data-ttu-id="8693d-126">Rendez-vous</span><span class="sxs-lookup"><span data-stu-id="8693d-126">Appointment</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="8693d-127">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="8693d-127">CalendarItem</span></span>](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) <br/> |
|[<span data-ttu-id="8693d-128">Tâche</span><span class="sxs-lookup"><span data-stu-id="8693d-128">Task</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.task%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="8693d-129">Tâche</span><span class="sxs-lookup"><span data-stu-id="8693d-129">Task</span></span>](http://msdn.microsoft.com/library/7c84927e-db28-4c5d-b0b5-cbcc2b88d869%28Office.15%29.aspx) <br/> |
   
<span data-ttu-id="8693d-130">Utilisez la méthode d’API managées [Item.Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.save%28v=exchg.80%29.aspx) ou l’opération EWS [CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) pour effectuer l’importation d’éléments.</span><span class="sxs-lookup"><span data-stu-id="8693d-130">Use the [Item.Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.save%28v=exchg.80%29.aspx) EWS Managed API method or the [CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS operation to perform the import of items.</span></span> <span data-ttu-id="8693d-131">Nous vous recommandons cette approche lorsque vous importez des éléments à partir d’autres systèmes, car vous avez le contrôle sur lequel les propriétés sont importées.</span><span class="sxs-lookup"><span data-stu-id="8693d-131">We recommend this approach when you're importing items from other systems because you have control over which properties get imported.</span></span> <span data-ttu-id="8693d-132">Pour plus d’informations sur la façon de définir les propriétés sur les éléments, puis enregistrez l’élément, voir [créer un élément à l’aide de l’API managée EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_createewsma) ou [créer un élément à l’aide de EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_createews).</span><span class="sxs-lookup"><span data-stu-id="8693d-132">For more information about how to set properties on items and then save the item, see [Create an item by using the EWS Managed API](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_createewsma) or [Create an item by using EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_createews).</span></span>
  
## <a name="import-items-with-full-fidelity"></a><span data-ttu-id="8693d-133">Importer des éléments de fidélité</span><span class="sxs-lookup"><span data-stu-id="8693d-133">Import items with full fidelity</span></span>
<span data-ttu-id="8693d-134"><a name="bk_importproperties"> </a></span><span class="sxs-lookup"><span data-stu-id="8693d-134"></span></span>

<span data-ttu-id="8693d-135">Vous pouvez utiliser l’opération EWS [UploadItems](http://msdn.microsoft.com/library/a88cbe99-7968-454d-a545-4f92c330909f%28Office.15%29.aspx) pour télécharger un élément en tant qu’un flux de données.</span><span class="sxs-lookup"><span data-stu-id="8693d-135">You can use the [UploadItems](http://msdn.microsoft.com/library/a88cbe99-7968-454d-a545-4f92c330909f%28Office.15%29.aspx) EWS operation to upload an item as a data stream.</span></span> <span data-ttu-id="8693d-136">Cette représentation du flux de données d’un élément doit provenir les résultats d’un appel d’opération [ExportItems](http://msdn.microsoft.com/library/e2846abb-0b16-4732-bbd8-038a674672f6%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="8693d-136">This data stream representation of an item has to come from the results of an [ExportItems](http://msdn.microsoft.com/library/e2846abb-0b16-4732-bbd8-038a674672f6%28Office.15%29.aspx) operation call.</span></span> <span data-ttu-id="8693d-137">Étant donné que l’API managée EWS n’implémente pas l’opération **UploadItems** , si vous utilisez l’API managée EWS, vous devrez écrire une routine pour envoyer les requêtes web.</span><span class="sxs-lookup"><span data-stu-id="8693d-137">Because the EWS Managed API does not implement the **UploadItems** operation, if you use the EWS Managed API, you'll need to write a routine to send the web requests.</span></span> 
  
<span data-ttu-id="8693d-138">C’est la plus simple pour importer des éléments qui ont été exportés à partir d’un autre serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="8693d-138">This is the easiest way to import items that have been exported from another Exchange server.</span></span>
  
<span data-ttu-id="8693d-139">Dans l’exemple suivant, les identificateurs et le contenu de l’élément de **données** sont limitent pour une meilleure lisibilité.</span><span class="sxs-lookup"><span data-stu-id="8693d-139">In the following example, the identifiers and the **Data** element content are shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
      xmlns:xsd="http://www.w3.org/2001/XMLSchema"
      xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
      xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
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

Le serveur répond à la demande **UploadItems** avec un élément [UploadItemsResponse](http://msdn.microsoft.com/library/93044d39-4489-456a-8cce-b6d69873348f%28Office.15%29.aspx) incluant la valeur [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) élément **NoError**, ce qui indique que l’élément a été téléchargé avec succès. <span data-ttu-id="8693d-141">La réponse inclut également l’ID d’élément de l’élément téléchargé.</span><span class="sxs-lookup"><span data-stu-id="8693d-141">The response also includes the item ID of the uploaded item.</span></span> 
  
## <a name="use-the-mime-stream-to-import-from-common-file-formats"></a><span data-ttu-id="8693d-142">Utilisez le flux MIME pour importer à partir de formats de fichiers communs</span><span class="sxs-lookup"><span data-stu-id="8693d-142">Use the MIME stream to import from common file formats</span></span>
<span data-ttu-id="8693d-143"><a name="bk_importproperties"> </a></span><span class="sxs-lookup"><span data-stu-id="8693d-143"></span></span>

<span data-ttu-id="8693d-144">EWS peut importer EML (.eml) et fichiers iCal (.ics).</span><span class="sxs-lookup"><span data-stu-id="8693d-144">EWS can import EML (.eml) and iCal (.ics) files.</span></span> <span data-ttu-id="8693d-145">Vous souhaiterez tester votre contenu MIME pour voir comment l’analyseur MIME Exchange gère le contenu de votre flux de données MIME.</span><span class="sxs-lookup"><span data-stu-id="8693d-145">You'll want to test your MIME content to see how the Exchange MIME parser handles the content of your MIME stream.</span></span> <span data-ttu-id="8693d-146">Bien que l’utilisation du flux MIME est pratique, il est généralement préférable [d’utiliser API managées ou EWS item types pour importer un élément](#bk_importproperties).</span><span class="sxs-lookup"><span data-stu-id="8693d-146">Although using the MIME stream is convenient, it is typically better to [Use EWS Managed API or EWS item types to import an item](#bk_importproperties).</span></span> <span data-ttu-id="8693d-147">Voici un exemple de la façon [d’Importer un fichier vCard](http://code.msdn.microsoft.com/How-to-Import-vCard-Files-ffa0ff50).</span><span class="sxs-lookup"><span data-stu-id="8693d-147">Here's an example of how to [import a vCard](http://code.msdn.microsoft.com/How-to-Import-vCard-Files-ffa0ff50).</span></span>
  
### <a name="use-the-ews-managed-api-to-import-an-email-from-an-eml-file-by-using-the-mime-stream"></a><span data-ttu-id="8693d-148">Utiliser l’API managée EWS pour importer un message électronique à partir d’un fichier EML à l’aide du flux MIME</span><span class="sxs-lookup"><span data-stu-id="8693d-148">Use the EWS Managed API to import an email from an EML file by using the MIME stream</span></span>

<span data-ttu-id="8693d-149">L’exemple suivant montre comment définir la propriété [MimeContent](http://msdn.microsoft.com/EN-US/library/microsoft.exchange.webservices.data.item.mimecontent%28v=exchg.80%29.aspx) avec le contenu d’un fichier EML, puis importer le courrier électronique dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="8693d-149">The following example shows how to set the [MimeContent](http://msdn.microsoft.com/EN-US/library/microsoft.exchange.webservices.data.item.mimecontent%28v=exchg.80%29.aspx) property with the contents of an EML file and then import the email into a mailbox.</span></span> <span data-ttu-id="8693d-150">Cet exemple montre également comment définir le [PidTagMessageFlags (0x0E07)](http://msdn.microsoft.com/en-us/library/office/cc839733%28v=office.15%29.aspx) propriété sur un message électronique importé étendue afin qu’il n’apparaît pas dans la boîte aux lettres comme un élément de brouillon.</span><span class="sxs-lookup"><span data-stu-id="8693d-150">This example also shows how to set the [PidTagMessageFlags (0x0E07)](http://msdn.microsoft.com/en-us/library/office/cc839733%28v=office.15%29.aspx) extended property on an imported email so that it doesn't appear in the mailbox as a draft item.</span></span> <span data-ttu-id="8693d-151">Cet exemple suppose que ce **service** est un objet [ExchangeService](http://msdn.microsoft.com/EN-US/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide, et que l’utilisateur peut s’authentifier à un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="8693d-151">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/EN-US/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, and that the user can authenticate to an Exchange server.</span></span> 
  
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

### <a name="use-the-ews-managed-api-to-import-an-appointment-from-an-ical-file-by-using-the-mime-stream"></a><span data-ttu-id="8693d-152">Utiliser l’API managée EWS pour importer un rendez-vous à partir d’un fichier iCal à l’aide du flux MIME</span><span class="sxs-lookup"><span data-stu-id="8693d-152">Use the EWS Managed API to import an appointment from an iCal file by using the MIME stream</span></span>

<span data-ttu-id="8693d-153">Vous pouvez importer des rendez-vous simples sous la forme de fichiers iCalendar en utilisant le flux MIME.</span><span class="sxs-lookup"><span data-stu-id="8693d-153">You can import simple appointments in the form of iCalendar files by using the MIME stream.</span></span> <span data-ttu-id="8693d-154">Vous ne pouvez pas importer de réunions, qui sont des rendez-vous avec les participants, car la relation entre les organisateurs de réunion et les participants doit être définie dans le cadre du flux de travail [du calendrier Exchange](calendars-and-ews-in-exchange.md) .</span><span class="sxs-lookup"><span data-stu-id="8693d-154">You can't import meetings, which are appointments with attendees, because the relationship between meeting organizers and attendees has to be set as part of the [Exchange calendaring](calendars-and-ews-in-exchange.md) workflow.</span></span> <span data-ttu-id="8693d-155">Participants ne peuvent pas être capturés dans le flux MIME.</span><span class="sxs-lookup"><span data-stu-id="8693d-155">Attendees cannot be captured in the MIME stream.</span></span> 
  
<span data-ttu-id="8693d-156">L’exemple de code suivant montre comment importer un fichier .ics simple dans la boîte aux lettres d’un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="8693d-156">The following code example shows you how to import a simple .ics file into a user's mailbox.</span></span>
  
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

### <a name="use-ews-to-import-an-item-by-using-the-mime-stream"></a><span data-ttu-id="8693d-157">Utiliser EWS pour importer un élément à l’aide du flux MIME</span><span class="sxs-lookup"><span data-stu-id="8693d-157">Use EWS to import an item by using the MIME stream</span></span>

<span data-ttu-id="8693d-158">Vous pouvez utiliser l’opération EWS [CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) pour importer EML et des éléments iCal à l’aide de leur flux de données MIME.</span><span class="sxs-lookup"><span data-stu-id="8693d-158">You can use the [CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS operation to import EML and iCal items by using their MIME stream.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
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

## <a name="next-steps"></a><span data-ttu-id="8693d-159">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="8693d-159">Next steps</span></span>
<span data-ttu-id="8693d-160"><a name="bk_importproperties"> </a></span><span class="sxs-lookup"><span data-stu-id="8693d-160"></span></span>

<span data-ttu-id="8693d-161">Une fois que vous importez des éléments dans une boîte aux lettres, vous souhaitez [créer un dossier personnalisé pour stocker vos éléments importés](how-to-work-with-folders-by-using-ews-in-exchange.md)ou [synchroniser vos éléments de client et boîte aux lettres](mailbox-synchronization-and-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="8693d-161">After you import items into a mailbox, you might want to [create a custom folder to store your imported items](how-to-work-with-folders-by-using-ews-in-exchange.md), or [synchronize your client and mailbox items](mailbox-synchronization-and-ews-in-exchange.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="8693d-162">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="8693d-162">See also</span></span>


- [<span data-ttu-id="8693d-163">Exporter et importer des éléments à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="8693d-163">Exporting and importing items by using EWS in Exchange</span></span>](exporting-and-importing-items-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="8693d-164">Exporter les éléments à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="8693d-164">Export items by using EWS in Exchange</span></span>](how-to-export-items-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="8693d-165">Dossiers et éléments dans EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="8693d-165">Folders and items in EWS in Exchange</span></span>](folders-and-items-in-ews-in-exchange.md)
    
- [<span data-ttu-id="8693d-166">Synchronisation de la boîte aux lettres et les services EWS d'Exchange</span><span class="sxs-lookup"><span data-stu-id="8693d-166">Mailbox synchronization and EWS in Exchange</span></span>](mailbox-synchronization-and-ews-in-exchange.md)
    

