---
title: Importer des éléments à l’aide d’EWS dans Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: dd3d3221-c98e-4fa0-81f0-77f733d2f432
description: Découvrez comment importer des rendez-vous, des e-mails, des contacts, des tâches et d’autres éléments à l’aide de l’API gérée EWS ou d’EWS dans Exchange.
ms.openlocfilehash: 1e111a03f43c7c6ea30ab0dedf5cc0bb5c6a41f8
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513163"
---
# <a name="import-items-by-using-ews-in-exchange"></a>Importer des éléments à l’aide d’EWS dans Exchange

Découvrez comment importer des rendez-vous, des e-mails, des contacts, des tâches et d’autres éléments à l’aide de l’API gérée EWS ou d’EWS dans Exchange.
  
De nombreux systèmes contiennent des rendez-vous, des e-mails, des contacts et des tâches, et vous pouvez importer ces éléments dans Exchange de différentes manières. L’importation d’éléments Exchange est simple lorsque les relations de boîte aux lettres ne sont pas conservées sur ces éléments. Vous pouvez utiliser la méthode [Item.Save](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.item.save%28v=exchg.80%29.aspx) EWS Managed API ou l’opération [CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS pour créer les éléments dans une boîte aux lettres Exchange.. Toutefois, l’approche simple ne prend pas en charge tous les scénarios . par exemple : 
  
- Vous ne pouvez pas maintenir la relation entre les organisateurs et les participants lors de l’importation de rendez-vous avec des participants (réunions). Cela signifie que l’organisateur de la réunion devra renvoyer les invitations aux réunions aux participants afin de rétablir la relation entre l’organisateur et les participants. Si le rendez-vous a été importé dans le calendrier d’un participant, il n’est pas lié au rendez-vous de l’organisateur de la réunion. Les participants doivent accepter l’invitation à la réunion de l’organisateur pour rétablir la relation organisateur-participant.
    
- Les informations sur les personnes affectées ne sont pas conservées lors de l’importation des tâches affectées.
    
Toutes les options d’importation peuvent être utilisées pour l’importation par lots d’éléments Exchange.
  
## <a name="use-ews-managed-api-or-ews-item-types-to-import-an-item"></a>Utiliser l’API gérée EWS ou les types d’éléments EWS pour importer un élément
<a name="bk_importproperties"> </a>

Vous pouvez utiliser l’API gérée EWS ou EWS pour importer des courriers électroniques, des contacts, des rendez-vous ou des tâches à partir d’autres systèmes. Définissez simplement [les propriétés ](properties-and-extended-properties-in-ews-in-exchange.md) à partir de votre format source sur l’un des objets suivants, en fonction de ce que vous importez. 
  
**Tableau 1. Objets d’API gérée EWS et éléments EWS**

|**Objet API gérée EWS**|**Élément EWS**|
|:-----|:-----|
|[EmailMessage](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) <br/> |[Message](https://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx) <br/> |
|[Contact](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx) <br/> |[Contact](https://msdn.microsoft.com/library/66bfff50-7a91-4d81-b6a0-610b9962f677%28Office.15%29.aspx) <br/> |
|[Rendez-vous](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) <br/> |[CalendarItem](https://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) <br/> |
|[Tâche](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.task%28v=exchg.80%29.aspx) <br/> |[Tâche](https://msdn.microsoft.com/library/7c84927e-db28-4c5d-b0b5-cbcc2b88d869%28Office.15%29.aspx) <br/> |
   
Utilisez la [méthode d’API](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.save%28v=exchg.80%29.aspx) gérée EWS Item.Save ou l’opération [CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS pour importer des éléments. Nous vous recommandons cette approche lorsque vous importez des éléments à partir d’autres systèmes, car vous contrôlez les propriétés importées. Pour plus d’informations sur la façon de définir des propriétés sur des éléments, puis d’enregistrer l’élément, voir Créer un élément à l’aide de l’API gérée [EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_createewsma) ou Créer un élément à l’aide [d’EWS.](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_createews)
  
## <a name="import-items-with-full-fidelity"></a>Importer des éléments avec une fidélité totale
<a name="bk_importproperties"> </a>

Vous pouvez utiliser [l’opération UploadItems](https://msdn.microsoft.com/library/a88cbe99-7968-454d-a545-4f92c330909f%28Office.15%29.aspx) EWS pour télécharger un élément en tant que flux de données. Cette représentation de flux de données d’un élément doit être le résultat d’un appel d’opération [ExportItems.](https://msdn.microsoft.com/library/e2846abb-0b16-4732-bbd8-038a674672f6%28Office.15%29.aspx) Étant donné que l’API gérée EWS n’implémente pas l’opération **UploadItems,** si vous utilisez l’API gérée EWS, vous devez écrire une routine pour envoyer les demandes web. 
  
Il s’agit du moyen le plus simple d’importer des éléments qui ont été exportés à partir d’Exchange serveur.
  
Dans l’exemple suivant, les identificateurs et le contenu de l’élément **Data** sont raccourcis pour des raisons de lisibilité. 
  
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

Le serveur répond à la demande **UploadItems** avec un élément [UploadItemsResponse](https://msdn.microsoft.com/library/93044d39-4489-456a-8cce-b6d69873348f%28Office.15%29.aspx) qui inclut une valeur d’élément [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NoError**, ce qui indique que l’élément a été téléchargé avec succès. La réponse inclut également l’ID d’élément de l’élément téléchargé. 
  
## <a name="use-the-mime-stream-to-import-from-common-file-formats"></a>Utiliser le flux MIME pour importer à partir de formats de fichiers courants
<a name="bk_importproperties"> </a>

EWS peut importer des fichiers EML (.eml) et iCal (.ics). Vous pouvez tester votre contenu MIME pour voir comment l’analyseur MIME Exchange le contenu de votre flux MIME. Bien que l’utilisation du flux MIME soit pratique, il est généralement préférable d’utiliser l’API gérée EWS ou les types d’éléments [EWS](#bk_importproperties)pour importer un élément. Voici un exemple de la façon [d’importer une vCard](https://code.msdn.microsoft.com/How-to-Import-vCard-Files-ffa0ff50).
  
### <a name="use-the-ews-managed-api-to-import-an-email-from-an-eml-file-by-using-the-mime-stream"></a>Utiliser l’API gérée EWS pour importer un courrier électronique à partir d’un fichier EML à l’aide du flux MIME

L’exemple suivant montre comment définir la [propriété MimeContent](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.mimecontent%28v=exchg.80%29.aspx) avec le contenu d’un fichier EML, puis importer le courrier électronique dans une boîte aux lettres. Cet exemple montre également comment définir la propriété étendue [PidTagMessageFlags (0x0E07)](https://msdn.microsoft.com/library/office/cc839733%28v=office.15%29.aspx) sur un message électronique importé afin qu’il n’apparaisse pas dans la boîte aux lettres en tant qu’élément de brouillon. Cet exemple suppose que **le service** est un objet [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur peut s’authentifier sur Exchange serveur. 
  
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

### <a name="use-the-ews-managed-api-to-import-an-appointment-from-an-ical-file-by-using-the-mime-stream"></a>Utiliser l’API gérée EWS pour importer un rendez-vous à partir d’un fichier iCal à l’aide du flux MIME

Vous pouvez importer des rendez-vous simples sous la forme de fichiers iCalendar à l’aide du flux MIME. Vous ne pouvez pas importer de réunions, qui sont des rendez-vous avec des participants, car la relation entre les organisateurs de la réunion et les participants doit être définie dans le cadre du flux de travail de calendrier [Exchange.](calendars-and-ews-in-exchange.md) Les participants ne peuvent pas être capturés dans le flux MIME. 
  
L’exemple de code suivant vous montre comment importer un fichier .ics simple dans la boîte aux lettres d’un utilisateur.
  
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

Vous pouvez utiliser [l’opération CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS pour importer des éléments EML et iCal à l’aide de leur flux MIME. 
  
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

Après avoir importé des éléments dans une boîte aux lettres, vous pouvez créer un dossier personnalisé pour stocker vos éléments importés [ou](how-to-work-with-folders-by-using-ews-in-exchange.md)synchroniser vos éléments de client et de boîte [aux lettres.](mailbox-synchronization-and-ews-in-exchange.md)
  
## <a name="see-also"></a>Voir aussi


- [Exportation et importation d’éléments à l’aide d’EWS Exchange](exporting-and-importing-items-by-using-ews-in-exchange.md)
    
- [Exporter des éléments à l’aide d’EWS dans Exchange](how-to-export-items-by-using-ews-in-exchange.md)
    
- [Dossiers et éléments dans EWS dans Exchange](folders-and-items-in-ews-in-exchange.md)
    
- [Synchronisation de la boîte aux lettres et les services EWS d'Exchange](mailbox-synchronization-and-ews-in-exchange.md)
    

