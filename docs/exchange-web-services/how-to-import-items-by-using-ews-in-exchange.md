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
# <a name="import-items-by-using-ews-in-exchange"></a>Importer des éléments à l’aide d’EWS dans Exchange

Découvrez comment importer des rendez-vous, des courriers électroniques, des contacts, des tâches et d’autres éléments à l’aide de l’API managée EWS ou d’EWS dans Exchange.
  
De nombreux systèmes contiennent des rendez-vous, des courriers électroniques, des contacts et des tâches, et vous pouvez importer ces éléments dans Exchange de différentes manières. L’importation d’éléments dans Exchange est simple lorsque les relations de boîtes aux lettres ne sont pas conservées sur ces éléments. Vous pouvez utiliser la méthode [de l’API](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) managée [EWS pour créer les éléments](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.item.save%28v=exchg.80%29.aspx) dans une boîte aux lettres Exchange. Toutefois, l’approche simple ne prend pas en charge tous les scénarios ; par exemple : 
  
- Vous ne pouvez pas maintenir la relation entre les organisateurs et les participants lors de l’importation de rendez-vous avec des participants (réunions). Cela signifie que l’organisateur de la réunion devra renvoyer les invitations aux réunions aux participants afin de rétablir la relation entre l’organisateur et les participants. Si le rendez-vous a été importé dans le calendrier d’un participant, le rendez-vous n’est pas lié au rendez-vous de l’organisateur de la réunion. Les participants doivent accepter l’invitation de réunion renvoyée à partir de l’organisateur afin de rétablir la relation organisateur-participant.
    
- Les informations sur les utilisateurs ne sont pas conservées lors de l’importation des tâches affectées.
    
Toutes les options d’importation peuvent être utilisées pour importer par lots des éléments dans Exchange.
  
## <a name="use-ews-managed-api-or-ews-item-types-to-import-an-item"></a>Utiliser l’API managée EWS ou les types d’élément EWS pour importer un élément
<a name="bk_importproperties"> </a>

Vous pouvez utiliser l’API managée EWS ou EWS pour importer des courriers électroniques, des contacts, des rendez-vous ou des tâches à partir d’autres systèmes. Il vous suffit de définir les [Propriétés](properties-and-extended-properties-in-ews-in-exchange.md) à partir de votre format source sur l’un des objets suivants, en fonction de ce que vous importez. 
  
**Tableau 1. Objets de l’API managée EWS et éléments EWS**

|**Objet de l’API managée EWS**|**Élément EWS**|
|:-----|:-----|
|[EmailMessage](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) <br/> |[Message](https://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx) <br/> |
|[Contact](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx) <br/> |[Contact](https://msdn.microsoft.com/library/66bfff50-7a91-4d81-b6a0-610b9962f677%28Office.15%29.aspx) <br/> |
|[Rendez-vous](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) <br/> |[CalendarItem](https://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) <br/> |
|[Task](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.task%28v=exchg.80%29.aspx) <br/> |[Task](https://msdn.microsoft.com/library/7c84927e-db28-4c5d-b0b5-cbcc2b88d869%28Office.15%29.aspx) <br/> |
   
Utilisez la méthode d’API managée [Item. Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.save%28v=exchg.80%29.aspx) ou l' [opération EWS EWS](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) pour effectuer l’importation des éléments. Cette approche est recommandée lorsque vous importez des éléments à partir d’autres systèmes car vous contrôlez les propriétés qui sont importées. Pour plus d’informations sur la façon de définir des propriétés sur des éléments, puis de l’enregistrer, voir [créer un élément à l’aide de l’API managée EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_createewsma) ou [créer un élément à l’aide d’EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_createews).
  
## <a name="import-items-with-full-fidelity"></a>Importer des éléments avec une fidélité totale
<a name="bk_importproperties"> </a>

Vous pouvez utiliser l’opération EWS [UploadItems](https://msdn.microsoft.com/library/a88cbe99-7968-454d-a545-4f92c330909f%28Office.15%29.aspx) pour télécharger un élément en tant que flux de données. Cette représentation de flux de données d’un élément doit provenir des résultats d’un appel d’opération [ExportItems](https://msdn.microsoft.com/library/e2846abb-0b16-4732-bbd8-038a674672f6%28Office.15%29.aspx) . Étant donné que l’API managée EWS n’implémente pas l’opération **UploadItems** , si vous utilisez l’API managée EWS, vous devez écrire une routine pour envoyer les requêtes Web. 
  
Il s’agit de la méthode la plus simple pour importer des éléments qui ont été exportés à partir d’un autre serveur Exchange.
  
Dans l’exemple suivant, les identificateurs et le contenu des éléments de **données** sont réduits pour des raisons de lisibilité. 
  
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

Le serveur répond à la demande **UploadItems** avec un élément [UploadItemsResponse](https://msdn.microsoft.com/library/93044d39-4489-456a-8cce-b6d69873348f%28Office.15%29.aspx) qui inclut une valeur d’élément [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NOERROR**, ce qui indique que l’élément a été téléchargé avec succès. La réponse inclut également l’ID de l’élément téléchargé. 
  
## <a name="use-the-mime-stream-to-import-from-common-file-formats"></a>Utiliser le flux MIME pour importer à partir de formats de fichiers communs
<a name="bk_importproperties"> </a>

EWS peut importer des fichiers EML (. eml) et iCal (. ICS). Vous pouvez tester votre contenu MIME pour voir comment l’analyseur MIME Exchange gère le contenu de votre flux MIME. Bien que l’utilisation du flux MIME soit pratique, il est généralement préférable d' [utiliser l’API managée EWS ou les types d’élément EWS pour importer un élément](#bk_importproperties). Voici un exemple d' [importation d’une vCard](https://code.msdn.microsoft.com/How-to-Import-vCard-Files-ffa0ff50).
  
### <a name="use-the-ews-managed-api-to-import-an-email-from-an-eml-file-by-using-the-mime-stream"></a>Utiliser l’API managée EWS pour importer un message électronique à partir d’un fichier EML à l’aide du flux MIME

L’exemple suivant montre comment définir la propriété [lamimecontent](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.mimecontent%28v=exchg.80%29.aspx) avec le contenu d’un fichier EML, puis importer le courrier électronique dans une boîte aux lettres. Cet exemple montre également comment définir la propriété étendue [PidTagMessageFlags (0x0E07)](https://msdn.microsoft.com/library/office/cc839733%28v=office.15%29.aspx) sur un message électronique importé de sorte qu’elle n’apparaisse pas dans la boîte aux lettres en tant qu’élément de brouillon. Cet exemple suppose que le **service** est un objet [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur puisse s’authentifier auprès d’un serveur Exchange. 
  
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

### <a name="use-the-ews-managed-api-to-import-an-appointment-from-an-ical-file-by-using-the-mime-stream"></a>Utiliser l’API managée EWS pour importer un rendez-vous à partir d’un fichier iCal à l’aide du flux MIME

Vous pouvez importer des rendez-vous simples sous la forme de fichiers iCalendar à l’aide du flux MIME. Vous ne pouvez pas importer de réunions, qui sont des rendez-vous avec des participants, car la relation entre les organisateurs de réunion et les participants doit être définie dans le flux de travail de [calendrier Exchange](calendars-and-ews-in-exchange.md) . Les participants ne peuvent pas être capturés dans le flux MIME. 
  
L’exemple de code suivant montre comment importer un fichier. ICS simple dans la boîte aux lettres d’un utilisateur.
  
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

### <a name="use-ews-to-import-an-item-by-using-the-mime-stream"></a>Utiliser EWS pour importer un élément à l’aide du flux MIME

Vous pouvez utiliser l’opération EWS EWS pour importer des éléments EML et iCal à l' [aide de leur](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) flux MIME. 
  
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

## <a name="next-steps"></a>Étapes suivantes
<a name="bk_importproperties"> </a>

Après avoir importé des éléments dans une boîte aux lettres, vous pouvez [créer un dossier personnalisé pour stocker vos éléments importés](how-to-work-with-folders-by-using-ews-in-exchange.md), ou [synchroniser vos éléments de client et de boîte aux lettres](mailbox-synchronization-and-ews-in-exchange.md).
  
## <a name="see-also"></a>Voir aussi


- [Exportation et importation d’éléments à l’aide d’EWS dans Exchange](exporting-and-importing-items-by-using-ews-in-exchange.md)
    
- [Exporter des éléments à l’aide d’EWS dans Exchange](how-to-export-items-by-using-ews-in-exchange.md)
    
- [Dossiers et éléments dans EWS dans Exchange](folders-and-items-in-ews-in-exchange.md)
    
- [Synchronisation de la boîte aux lettres et les services EWS d'Exchange](mailbox-synchronization-and-ews-in-exchange.md)
    

