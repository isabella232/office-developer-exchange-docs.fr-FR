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
# <a name="export-items-by-using-ews-in-exchange"></a>Exporter les éléments à l’aide de EWS dans Exchange

Découvrez comment exporter les rendez-vous, les messages électroniques, contacts, tâches et autres éléments à l’aide de l’API managée EWS ou EWS dans Exchange.
  
Vous pouvez exporter les éléments à partir d’Exchange à l’aide de l’API managée EWS ou EWS dans un certain nombre de différentes manières. Dépend de l’option que vous utilisez :
  
- Le type d’élément qui est exporté.
    
- Degré de fidélité que vous voulez maintenir entre l’état de l’élément dans Exchange et de l’élément exporté.
    
- Le format de l’élément exporté.
    
- Les exigences de post-traitement.
    
- Si vous souhaitez importer l’élément précédent dans Exchange.
    
Cet article explique comment utiliser chacune des options différentes pour exporter les éléments. Vous pouvez utiliser n’importe quelle option pour exporter des éléments en dehors d’Exchange.
  
## <a name="export-an-item-into-a-custom-format"></a>Exporter un élément dans un format personnalisé
<a name="bk_exportcustom"> </a>

Vous pouvez utiliser les résultats d’un appel de méthode d’API managées [Item.Bind](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getewsma) ou analyser les résultats d’une opération EWS [GetItem](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getews) dans un format qui fonctionne avec les exigences de votre application. Utilisez cette option lorsque vous exportez des éléments afin de les importer dans une base de données, fichier .csv, ou un autre format ou système. Vous pouvez même enregistrer l’élément dans le formulaire de l’élément XML EWS, qui peut être utile car de nombreux systèmes possèdent des capacités d’analyse XML. Nous vous recommandons d’utiliser la méthode **Item.Bind** ou l’opération de **GetItem** (sans la propriété [Item.MimeContent](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.mimecontent%28v=exchg.80%29.aspx) ), car cette option vous permet de contrôler les propriétés qui est exportés. 
  
## <a name="export-items-with-full-fidelity"></a>Exporter des éléments de fidélité
<a name="bk_exportfullfidelity"> </a>

Si vous souhaitez exporter les éléments avec fidélité, vous pouvez utiliser l’opération EWS [ExportItems](http://msdn.microsoft.com/library/e2846abb-0b16-4732-bbd8-038a674672f6%28Office.15%29.aspx) . L’opération **ExportItems** exporte chaque élément sous la forme d’un flux de données. Ce flux de données pour l’analyse n’est pas, mais peut être utilisé comme une sauvegarde au niveau des éléments qui peut être importée dans une boîte aux lettres Exchange. Vous pouvez inclure le nombre d’éléments dans chaque demande **ExportItems** , bien qu’il est recommandé que vous n’incluez pas plus de 100 éléments dans chaque appel. Étant donné que l’API managée EWS n’implémente pas l’opération **ExportItems** , si vous utilisez l’API managée EWS, vous devrez écrire une routine pour envoyer les requêtes web. Vous pouvez également utiliser la méthode [Item.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) pour obtenir les métadonnées relatives à l’élément de sorte que vous pouvez indexer et de stocker des informations sur le flux de données. 
  
Nous vous recommandons d’utiliser l’opération **ExportItems** pour exporter les éléments que vous souhaitez importer dans une boîte aux lettres Exchange. 
  
L’exemple suivant montre comment utiliser l’opération **ExportItems** . Dans cet exemple, l’identificateur d’élément est réduite pour une meilleure lisibilité. 
  
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

Le serveur répond à la demande **ExportItems** avec un élément [ExportItemsResponse](http://msdn.microsoft.com/library/ef44354b-fbdb-4f7c-b6bd-b27f56a1d018%28Office.15%29.aspx) qui contient une valeur élément [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, ce qui indique que l’élément a été correctement exporté. La réponse inclut également l’ID d’élément de l’élément exporté et le flux de données qui contient le contenu exporté. L’exemple suivant montre le corps SOAP qui contient l’élément exporté.
  
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

## <a name="use-the-mime-stream-to-export-into-common-file-formats"></a>Le flux MIME permet d’exporter dans des formats de fichiers communs
<a name="bk_exportfullfidelity"> </a>

Vous pouvez utiliser la méthode d’API managées [Item.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) ou l’opération EWS [GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) pour obtenir une représentation sous forme de MIME d’un élément. Dans la mesure où Exchange ne stocke pas le contenu MIME de chaque élément, il doit convertir la représentation sous forme de base de données de chaque élément dans le flux MIME. Étant donné que la conversion est coûteuse, qu'il n’est pas recommandé que vous demandez le flux MIME pour les éléments à grande échelle. Notez également que le flux MIME contient un ensemble limité de propriétés. Vous devrez peut-être envisager d’autres options si le jeu de propriétés ne contienne pas les propriétés dont vous avez besoin. 
  
### <a name="use-the-ews-managed-api-to-export-an-email-into-an-eml-and-mht-file-by-using-the-mime-stream"></a>Utiliser l’API managée EWS pour exporter un message électronique dans un fichier .eml et .mht à l’aide du flux MIME
<a name="bk_exportemailmime"> </a>

Outlook et autres applications de messagerie courantes peuvent ouvrir le format de fichier EML (.eml). L’exemple suivant vous montre comment vous pouvez exporter un message électronique à l’aide du flux MIME et utilisez le flux MIME pour créer un EML et un fichier MIME HTML (.mht). De nombreux navigateurs web prennent en charge le format de fichier HTML MIME. Cet exemple suppose que ce **service** est un objet [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide, et que l’utilisateur peut s’authentifier à un serveur Exchange. 
  
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

### <a name="use-the-ews-managed-api-to-export-an-appointment-into-an-ical-file-by-using-the-mime-stream"></a>Utiliser l’API managée EWS pour exporter un rendez-vous dans un fichier iCal à l’aide du flux MIME
<a name="bk_exporticalmime"> </a>

Outlook et autres applications calendrier peuvent ouvrir le format de fichier iCal (.ics). L’exemple suivant montre comment exporter un rendez-vous à l’aide du flux MIME, utilisez le flux MIME pour créer un fichier iCal. Notez que de nombreuses propriétés ne sont pas exportées avec le flux MIME, y compris les participants et les propriétés liées à la pièce jointe. Vous pouvez capturer des autres propriétés de EWS par leur demandant et en les enregistrant dans le fichier iCal comme des extensions privées. Ces extensions privées portent le préfixe « x- ». 
  
Cet exemple suppose que ce **service** est un objet [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide, et que l’utilisateur peut s’authentifier à un serveur Exchange. Cet exemple part également du principe que vous disposez d’un rendez-vous dont l’objet est « Projections financières 2015 » dans le dossier calendrier. 
  
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

### <a name="use-the-ews-managed-api-to-export-a-contact-into-a-vcard-file-by-using-the-mime-stream"></a>Utiliser l’API managée EWS pour exporter un contact dans un fichier vCard à l’aide du flux MIME
<a name="bk_exportvcardmime"> </a>

Outlook et autres applications de gestion des contacts commune peuvent ouvrir le format de fichier vCard (.vcf). L’exemple suivant montre comment exporter un contact à l’aide du flux MIME et utilisez le flux MIME pour créer une carte de visite. Vous pouvez capturer des autres propriétés de EWS en leur demandant et en enregistrant dans le. carte de visite comme des extensions privées. Ces extensions portent le préfixe « x- ». 
  
Cet exemple suppose que ce **service** est un objet [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide, et que l’utilisateur peut s’authentifier à un serveur Exchange. 
  
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
> Vous ne pouvez pas importer les fichiers vCard à l’aide de la propriété **MimeContent** . Vous pouvez importer des contacts à l’aide de la méthode d’API managées [Contact.Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contact.save%28v=exchg.80%29.aspx) ou l’opération EWS [CreateItem](http://msdn.microsoft.com/library/417e994b-0a17-4c24-9527-04796b80b029%28Office.15%29.aspx) . 
  
### <a name="use-ews-to-export-any-item-by-using-the-mime-stream"></a>Utiliser EWS pour exporter n’importe quel élément à l’aide du flux MIME
<a name="bk_exportewsmime"> </a>

Utilisez l’opération **GetItem** pour obtenir le flux MIME d’un élément. La demande de **GetItem** suivante montre comment demander le contenu MIME d’un élément. 
  
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

L’exemple suivant montre la réponse à une demande pour obtenir le flux MIME. Le flux MIME a été raccourci pour des raisons de lisibilité.
  
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
<a name="bk_exportfullfidelity"> </a>

Après l’exportation d’éléments, vous souhaiterez [Importer les éléments dans Exchange](how-to-import-items-by-using-ews-in-exchange.md).
  
## <a name="see-also"></a>Voir aussi


- [Exporter et importer des éléments à l’aide de EWS dans Exchange](exporting-and-importing-items-by-using-ews-in-exchange.md)
    
- [Importer des éléments à l’aide de EWS dans Exchange](how-to-import-items-by-using-ews-in-exchange.md)
    
- [Dossiers et éléments dans EWS dans Exchange](folders-and-items-in-ews-in-exchange.md)
    
- [Synchronisation de la boîte aux lettres et les services EWS d'Exchange](mailbox-synchronization-and-ews-in-exchange.md)
    

