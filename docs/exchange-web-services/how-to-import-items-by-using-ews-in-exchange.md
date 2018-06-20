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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19754894"
---
# <a name="import-items-by-using-ews-in-exchange"></a>Importer des éléments à l’aide de EWS dans Exchange

Découvrez comment importer les rendez-vous, les messages électroniques, contacts, tâches et autres éléments à l’aide de l’API managée EWS ou EWS dans Exchange.
  
De nombreux systèmes contiennent des messages électroniques, contacts, tâches et rendez-vous et vous pouvez importer ces éléments dans Exchange dans un certain nombre de différentes manières. Importation d’éléments dans Exchange est simple lorsque les relations de boîte aux lettres ne sont pas conservées sur ces éléments. Vous pouvez utiliser la méthode d’API managées [Item.Save](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.item.save%28v=exchg.80%29.aspx) ou l’opération EWS [CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) pour créer les éléments dans une boîte aux lettres Exchange. L’approche simple ne prend pas en charge tous les scénarios, par exemple : 
  
- Vous ne pouvez pas mettre à jour la relation entre les organisateurs et les participants lors de l’importation des rendez-vous avec les participants (réunions). Cela signifie que l’organisateur de la réunion vous devrez renvoyer des invitations de réunion aux participants afin de rétablir la relation entre l’organisateur et les participants. Si le rendez-vous a été importé dans le calendrier du participant, le rendez-vous ne sera pas être lié à un rendez-vous de l’organisateur de la réunion. Les participants devez accepter l’invitation à la réunion récente de la bibliothèque multimédia afin de rétablir la relation participant à la bibliothèque multimédia.
    
- Plus d’informations sur les intervenants ne sont pas conservées lors de l’importation des tâches affectées.
    
Toutes les options d’importation permet d’importer des éléments de lot dans Exchange.
  
## <a name="use-ews-managed-api-or-ews-item-types-to-import-an-item"></a>Utilisation API managées ou EWS types pour importer un élément d’éléments
<a name="bk_importproperties"> </a>

Vous pouvez utiliser les API managées EWS pour importer les messages électroniques, des contacts, des rendez-vous ou des tâches à partir d’autres systèmes. Définissez simplement les [Propriétés](properties-and-extended-properties-in-ews-in-exchange.md) à partir de votre format source sur un des objets suivants, selon que vous importez. 
  
**Le tableau 1. Objets d’API managées et éléments EWS**

|**Objet d’API managées**|**Élément EWS**|
|:-----|:-----|
|[EmailMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) <br/> |[Message](http://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx) <br/> |
|[Contact](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx) <br/> |[Contact](http://msdn.microsoft.com/library/66bfff50-7a91-4d81-b6a0-610b9962f677%28Office.15%29.aspx) <br/> |
|[Rendez-vous](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) <br/> |[CalendarItem](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) <br/> |
|[Tâche](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.task%28v=exchg.80%29.aspx) <br/> |[Tâche](http://msdn.microsoft.com/library/7c84927e-db28-4c5d-b0b5-cbcc2b88d869%28Office.15%29.aspx) <br/> |
   
Utilisez la méthode d’API managées [Item.Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.save%28v=exchg.80%29.aspx) ou l’opération EWS [CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) pour effectuer l’importation d’éléments. Nous vous recommandons cette approche lorsque vous importez des éléments à partir d’autres systèmes, car vous avez le contrôle sur lequel les propriétés sont importées. Pour plus d’informations sur la façon de définir les propriétés sur les éléments, puis enregistrez l’élément, voir [créer un élément à l’aide de l’API managée EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_createewsma) ou [créer un élément à l’aide de EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_createews).
  
## <a name="import-items-with-full-fidelity"></a>Importer des éléments de fidélité
<a name="bk_importproperties"> </a>

Vous pouvez utiliser l’opération EWS [UploadItems](http://msdn.microsoft.com/library/a88cbe99-7968-454d-a545-4f92c330909f%28Office.15%29.aspx) pour télécharger un élément en tant qu’un flux de données. Cette représentation du flux de données d’un élément doit provenir les résultats d’un appel d’opération [ExportItems](http://msdn.microsoft.com/library/e2846abb-0b16-4732-bbd8-038a674672f6%28Office.15%29.aspx) . Étant donné que l’API managée EWS n’implémente pas l’opération **UploadItems** , si vous utilisez l’API managée EWS, vous devrez écrire une routine pour envoyer les requêtes web. 
  
C’est la plus simple pour importer des éléments qui ont été exportés à partir d’un autre serveur Exchange.
  
Dans l’exemple suivant, les identificateurs et le contenu de l’élément de **données** sont limitent pour une meilleure lisibilité. 
  
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

Le serveur répond à la demande **UploadItems** avec un élément [UploadItemsResponse](http://msdn.microsoft.com/library/93044d39-4489-456a-8cce-b6d69873348f%28Office.15%29.aspx) incluant la valeur [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) élément **NoError**, ce qui indique que l’élément a été téléchargé avec succès. La réponse inclut également l’ID d’élément de l’élément téléchargé. 
  
## <a name="use-the-mime-stream-to-import-from-common-file-formats"></a>Utilisez le flux MIME pour importer à partir de formats de fichiers communs
<a name="bk_importproperties"> </a>

EWS peut importer EML (.eml) et fichiers iCal (.ics). Vous souhaiterez tester votre contenu MIME pour voir comment l’analyseur MIME Exchange gère le contenu de votre flux de données MIME. Bien que l’utilisation du flux MIME est pratique, il est généralement préférable [d’utiliser API managées ou EWS item types pour importer un élément](#bk_importproperties). Voici un exemple de la façon [d’Importer un fichier vCard](http://code.msdn.microsoft.com/How-to-Import-vCard-Files-ffa0ff50).
  
### <a name="use-the-ews-managed-api-to-import-an-email-from-an-eml-file-by-using-the-mime-stream"></a>Utiliser l’API managée EWS pour importer un message électronique à partir d’un fichier EML à l’aide du flux MIME

L’exemple suivant montre comment définir la propriété [MimeContent](http://msdn.microsoft.com/EN-US/library/microsoft.exchange.webservices.data.item.mimecontent%28v=exchg.80%29.aspx) avec le contenu d’un fichier EML, puis importer le courrier électronique dans une boîte aux lettres. Cet exemple montre également comment définir le [PidTagMessageFlags (0x0E07)](http://msdn.microsoft.com/en-us/library/office/cc839733%28v=office.15%29.aspx) propriété sur un message électronique importé étendue afin qu’il n’apparaît pas dans la boîte aux lettres comme un élément de brouillon. Cet exemple suppose que ce **service** est un objet [ExchangeService](http://msdn.microsoft.com/EN-US/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide, et que l’utilisateur peut s’authentifier à un serveur Exchange. 
  
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

Vous pouvez importer des rendez-vous simples sous la forme de fichiers iCalendar en utilisant le flux MIME. Vous ne pouvez pas importer de réunions, qui sont des rendez-vous avec les participants, car la relation entre les organisateurs de réunion et les participants doit être définie dans le cadre du flux de travail [du calendrier Exchange](calendars-and-ews-in-exchange.md) . Participants ne peuvent pas être capturés dans le flux MIME. 
  
L’exemple de code suivant montre comment importer un fichier .ics simple dans la boîte aux lettres d’un utilisateur.
  
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

Vous pouvez utiliser l’opération EWS [CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) pour importer EML et des éléments iCal à l’aide de leur flux de données MIME. 
  
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

## <a name="next-steps"></a>Étapes suivantes
<a name="bk_importproperties"> </a>

Une fois que vous importez des éléments dans une boîte aux lettres, vous souhaitez [créer un dossier personnalisé pour stocker vos éléments importés](how-to-work-with-folders-by-using-ews-in-exchange.md)ou [synchroniser vos éléments de client et boîte aux lettres](mailbox-synchronization-and-ews-in-exchange.md).
  
## <a name="see-also"></a>Voir aussi


- [Exporter et importer des éléments à l’aide de EWS dans Exchange](exporting-and-importing-items-by-using-ews-in-exchange.md)
    
- [Exporter les éléments à l’aide de EWS dans Exchange](how-to-export-items-by-using-ews-in-exchange.md)
    
- [Dossiers et éléments dans EWS dans Exchange](folders-and-items-in-ews-in-exchange.md)
    
- [Synchronisation de la boîte aux lettres et les services EWS d'Exchange](mailbox-synchronization-and-ews-in-exchange.md)
    

