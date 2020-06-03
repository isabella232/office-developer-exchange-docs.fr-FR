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
# <a name="export-items-by-using-ews-in-exchange"></a>Exporter des éléments à l’aide d’EWS dans Exchange

Découvrez comment exporter des rendez-vous, des courriers électroniques, des contacts, des tâches et d’autres éléments à l’aide de l’API managée EWS ou d’EWS dans Exchange.
  
Vous pouvez exporter des éléments à partir d’Exchange à l’aide de l’API managée EWS ou d’EWS de différentes manières. L’option que vous utilisez dépend des éléments suivants :
  
- Type d’élément exporté.
    
- Degré de fidélité que vous souhaitez conserver entre l’état de l’élément dans Exchange et l’élément exporté.
    
- Format de l’élément exporté.
    
- Toutes les exigences de post-traitement.
    
- Si vous souhaitez réimporter l’élément dans Exchange.
    
Cet article explique comment utiliser chacune des différentes options pour exporter des éléments. Vous pouvez utiliser n’importe quelle option pour exporter des éléments en dehors d’Exchange.
  
## <a name="export-an-item-into-a-custom-format"></a>Exporter un élément dans un format personnalisé
<a name="bk_exportcustom"> </a>

Vous pouvez utiliser les résultats d’un [élément. lier](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getewsma) l’appel de la méthode d’API managée EWS ou analyser les résultats d’une opération EWS de [GetItem](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getews) dans un format qui fonctionne avec les exigences de votre application. Utilisez cette option lorsque vous exportez des éléments afin de les importer dans une base de données, un fichier. csv ou un autre format ou système. Vous pouvez même enregistrer l’élément sous la forme du XML EWS de l’élément, ce qui peut être utile, car de nombreux systèmes disposent d’une fonctionnalité d’analyse XML. Nous vous recommandons d’utiliser la méthode **Item. bind** ou l’opération **GetItem** (sans la propriété [Item. lamimecontent](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.mimecontent%28v=exchg.80%29.aspx) ) car cette option vous permet de contrôler les propriétés exportées. 
  
## <a name="export-items-with-full-fidelity"></a>Exporter des éléments avec une fidélité totale
<a name="bk_exportfullfidelity"> </a>

Si vous souhaitez exporter les éléments avec une fidélité totale, vous pouvez utiliser l’opération EWS [ExportItems](https://msdn.microsoft.com/library/e2846abb-0b16-4732-bbd8-038a674672f6%28Office.15%29.aspx) . L’opération **ExportItems** exporte chaque élément en tant que flux de données. Ce flux de données n’est pas destiné à l’analyse, mais peut être utilisé comme une sauvegarde au niveau des éléments qui peut être réimportée dans une boîte aux lettres Exchange. Vous pouvez inclure de nombreux éléments dans chaque demande **ExportItems** , bien que nous vous recommandons de ne pas inclure plus de 100 éléments dans chaque appel. Étant donné que l’API managée EWS n’implémente pas l’opération **ExportItems** , si vous utilisez l’API managée EWS, vous devez écrire une routine pour envoyer les requêtes Web. Vous pouvez éventuellement utiliser la méthode [Item. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) pour obtenir des métadonnées sur l’élément de sorte que vous puissiez indexer et stocker des informations sur le flux de données. 
  
Nous vous recommandons d’utiliser l’opération **ExportItems** pour exporter les éléments que vous envisagez d’importer dans une boîte aux lettres Exchange. 
  
L’exemple suivant montre comment utiliser l’opération **ExportItems** . Dans cet exemple, l’identificateur de l’élément est raccourci pour des raisons de lisibilité. 
  
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

Le serveur répond à la demande **ExportItems** avec un élément [ExportItemsResponse](https://msdn.microsoft.com/library/ef44354b-fbdb-4f7c-b6bd-b27f56a1d018%28Office.15%29.aspx) qui inclut une valeur d’élément [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NOERROR**, ce qui indique que l’élément a été correctement exporté. La réponse inclut également l’ID de l’élément exporté et le flux de données qui contient le contenu exporté. L’exemple suivant montre le corps SOAP qui contient l’élément exporté.
  
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

## <a name="use-the-mime-stream-to-export-into-common-file-formats"></a>Utiliser le flux MIME pour exporter dans des formats de fichiers communs
<a name="bk_exportfullfidelity"> </a>

Vous pouvez utiliser la méthode de l’API managée EWS de l' [élément. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) ou l’opération EWS de [GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) pour obtenir une représentation MIME d’un élément. Étant donné qu’Exchange ne stocke pas le contenu MIME de chaque élément, il doit convertir la représentation de la base de données de chaque élément dans le flux MIME. Étant donné que cette conversion est coûteuse, nous vous déconseillons de demander le flux MIME pour les éléments à grande échelle. Notez également que le flux MIME contient un ensemble limité de propriétés ; vous devrez peut-être prendre en compte d’autres options si le jeu de propriétés ne contient pas les propriétés dont vous avez besoin. 
  
### <a name="use-the-ews-managed-api-to-export-an-email-into-an-eml-and-mht-file-by-using-the-mime-stream"></a>Utiliser l’API managée EWS pour exporter un courrier électronique dans un fichier. eml et. mht à l’aide du flux MIME
<a name="bk_exportemailmime"> </a>

Outlook et d’autres applications de messagerie courantes peuvent ouvrir le format de fichier EML (. eml). L’exemple suivant montre comment vous pouvez exporter un courrier électronique à l’aide du flux MIME et utiliser le flux MIME pour créer un fichier EML et un fichier MIME HTML (. mht). De nombreux navigateurs Web prennent en charge le format de fichier HTML MIME. Cet exemple suppose que le **service** est un objet [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur puisse s’authentifier auprès d’un serveur Exchange. 
  
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

Outlook et d’autres applications de calendrier courantes peuvent ouvrir le format de fichier iCal (. ICS). L’exemple suivant montre comment exporter un rendez-vous à l’aide du flux MIME et utiliser le flux MIME pour créer un fichier iCal. Notez que de nombreuses propriétés ne sont pas exportées avec le flux MIME, y compris les participants et les propriétés associées aux pièces jointes. Vous pouvez capturer d’autres propriétés à partir d’EWS en les demandant et en les enregistrant dans le fichier iCal en tant qu’extensions privées. Ces extensions privées sont précédées du préfixe « x- ». 
  
Cet exemple suppose que le **service** est un objet [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur puisse s’authentifier auprès d’un serveur Exchange. Cet exemple suppose également que vous avez un rendez-vous avec l’objet « 2015 projections financières » dans le dossier calendrier. 
  
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

Outlook et d’autres applications de gestion des contacts courantes peuvent ouvrir le format de fichier vCard (. vcf). L’exemple suivant montre comment exporter un contact à l’aide du flux MIME et comment utiliser le flux MIME pour créer une vCard. Vous pouvez capturer d’autres propriétés à partir d’EWS en les demandant et en les enregistrant dans le. vCard en tant qu’extensions privées. Ces extensions sont précédées du préfixe « x- ». 
  
Cet exemple suppose que le **service** est un objet [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur puisse s’authentifier auprès d’un serveur Exchange. 
  
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
> Vous ne pouvez pas importer de fichiers vCard à l’aide de la propriété **lamimecontent** . Vous pouvez importer des contacts à l’aide de la méthode [contact. Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contact.save%28v=exchg.80%29.aspx) de l’API managée EWS ou de la commande [CreateItem](https://msdn.microsoft.com/library/417e994b-0a17-4c24-9527-04796b80b029%28Office.15%29.aspx) EWS. 
  
### <a name="use-ews-to-export-any-item-by-using-the-mime-stream"></a>Utiliser EWS pour exporter un élément à l’aide du flux MIME
<a name="bk_exportewsmime"> </a>

Utilisez l’opération **GetItem** pour obtenir le flux MIME d’un élément. La demande **GetItem** suivante montre comment demander le contenu MIME d’un élément. 
  
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

L’exemple suivant montre la réponse à une demande pour obtenir le flux MIME. Le flux MIME a été raccourci pour des raisons de lisibilité.
  
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
<a name="bk_exportfullfidelity"> </a>

Après avoir exporté des éléments, vous souhaiterez peut-être [importer des éléments dans Exchange](how-to-import-items-by-using-ews-in-exchange.md).
  
## <a name="see-also"></a>Voir aussi


- [Exportation et importation d’éléments à l’aide d’EWS dans Exchange](exporting-and-importing-items-by-using-ews-in-exchange.md)
    
- [Importer des éléments à l’aide d’EWS dans Exchange](how-to-import-items-by-using-ews-in-exchange.md)
    
- [Dossiers et éléments dans EWS dans Exchange](folders-and-items-in-ews-in-exchange.md)
    
- [Synchronisation de la boîte aux lettres et les services EWS d'Exchange](mailbox-synchronization-and-ews-in-exchange.md)
    

