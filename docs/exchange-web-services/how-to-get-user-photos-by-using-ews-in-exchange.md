---
title: Obtenir les photos de l’utilisateur à l’aide de EWS dans Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: f86d1099-1f57-47dc-abf2-4d5ae4e900a9
description: Découvrez comment obtenir les photos de l’utilisateur qui sont associés à une boîte aux lettres ou de contact à l’aide de l’API managée EWS ou EWS dans Exchange.
ms.openlocfilehash: f0f5cddd41fc563fb9ed38e75b505830a3992411
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754871"
---
# <a name="get-user-photos-by-using-ews-in-exchange"></a>Obtenir les photos de l’utilisateur à l’aide de EWS dans Exchange

Découvrez comment obtenir les photos de l’utilisateur qui sont associés à une boîte aux lettres ou de contact à l’aide de l’API managée EWS ou EWS dans Exchange.
  
C’est agréable à associer un visage à un nom. Si vos utilisateurs comme mettre des noms aux faces, votre application peut demander une image, généralement une photo, à partir d’Exchange qui représente un compte de messagerie. Vous pouvez obtenir une photo stockée sur un serveur Exchange pour une boîte aux lettres de l’utilisateur, ou vous pouvez obtenir une photo du contact à partir de contacts stockés dans votre boîte aux lettres.
  
Vous pouvez utiliser les différentes technologies pour obtenir des photos à partir des boîtes aux lettres ou les Services de domaine Active Directory (AD DS). La meilleure façon pour obtenir une photo varie selon le type de contact que vous souhaitez obtenir à partir d’une photo. 
  
**Le tableau 1. Technologies à utiliser pour obtenir les photos de l’utilisateur selon le type de contact**

|**Type de contact**|**Technologies à utiliser**|
|:-----|:-----|
|Photo de boîte aux lettres utilisateur  <br/> |[Obtenir une photo d’utilisateur de boîte aux lettres à l’aide de REST](#bk_REST)<br/><br/> [Obtenir une photo de l’utilisateur à l’aide de EWS](#bk_EWS) <br/> |
|Photo de contacter l’utilisateur  <br/> |[Obtenir une photo de contacter l’utilisateur à l’aide des API managées](#bk_EWSMA)<br/><br/> [Obtenir une photo de l’utilisateur à l’aide de EWS](#bk_EWS) <br/> |

<a name="bk_REST"> </a>

## <a name="get-a-mailbox-user-photo-by-using-rest"></a>Obtenir une photo d’utilisateur de boîte aux lettres à l’aide de REST

Vous pouvez demander des photos de l’utilisateur à partir d’un serveur Exchange à l’aide d’une demande HTTPS **GET** standard. Dans la demande, spécifiez l’adresse électronique du compte et un code de taille de l’image, comme indiqué dans l’exemple suivant. 
  
```HTML
https://Exchange Server/ews/Exchange.asmx/s/GetUserPhoto?email=email address&amp;size=size code
```

L’opération de [GetUserSettings](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) de service de découverte automatique permet de récupérer le paramètre **ExternalEwsUrl** , qui contient l’URL du point de terminaison Exchange Web Services (EWS) et l’emplacement du gestionnaire **Exchange.asmx** HTTP qui renvoie le photos de l’utilisateur. 
  
Chaque code taille indique la hauteur et la largeur de l’image en pixels. Par exemple, le code de taille **HR48x48** renvoie une image qui est 48 pixels de haut 48 pixels de large. Les valeurs possibles pour le paramètre de code de taille sont les mêmes que les valeurs possibles pour l’élément [SizeRequested](http://msdn.microsoft.com/library/e86f98b6-83b5-4530-80eb-dc5df42e2c62%28Office.15%29.aspx) . Si la demande spécifie une taille qui n’est pas disponible, la plus grande photo disponible est retournée. Si aucune photo n’est stocké sur le serveur Exchange, l’image miniature stocké dans AD DS pour le compte est retournée. 
  
> [!NOTE]
> Le code de taille **HR48x48** renvoie toujours l’image miniature de domaine Active Directory si elle est disponible. 
  
L’exemple suivant montre comment vous pouvez utiliser la requête GET pour récupérer la photo d’utilisateur pour Sadie et enregistrez-le sur votre ordinateur local.
  
```cs
// Create the web request with the REST URL.
HttpWebRequest request = 
   WebRequest.Create("https://www.contoso.com/ews/exchange.asmx/s/GetUserPhoto?email=sadie@contoso.com&amp;size=HR240x240") 
   as HttpWebRequest;
// Submit the request.
using (HttpWebResponse resp = request.GetResponse() as HttpWebResponse)
{
   // Take the response and save it as an image.
   Bitmap image = new Bitmap(resp.GetResponseStream());
   image.Save("Sadie.jpg");
}

```

La requête retourne une réponse HTTP. 
  
**Le tableau 2. Codes de réponse pour une demande de GetUserPhoto**

|**Code de réponse**|**Description**|
|:-----|:-----|
|200  <br/> |Une image est disponible pour le compte de messagerie spécifié et l’image binaire est contenue dans la réponse.  <br/> |
|304  <br/> |L’image n’a pas été modifié depuis la dernière exécution de que l' **ETag** a été renvoyée à l’application.  <br/> |
|404  <br/> |Aucune image n’est disponible pour le compte de messagerie spécifié.  <br/> |

<a name="bk_REST"> </a>

## <a name="cache-user-photos"></a>Photos de l’utilisateur du cache

Exchange renvoie les données avec un type de contenu d’image/jpeg, ainsi que d’une collection de valeurs d’en-tête. L’en-tête **ETag** est similaire à une clé de modification. La valeur est une chaîne qui représente la dernière mise à jour de la photo. L' **ETag** reste identique pour la photo d’utilisateur jusqu'à ce que la photo est modifiée. Vous pouvez envoyer cette valeur **ETag** sur le serveur de la demande dans un en-tête **If-None-Match** HTTPS à **obtenir** . Si la photo n’a pas changé depuis la dernière demande, le serveur répond avec une réponse HTTP 304 indiquant en tant que telles. Cela signifie que vous pouvez utiliser la photo de l’utilisateur demandé et enregistré précédemment au lieu de traitement d’une autre. 

<a name="bk_EWSMA"> </a>

## <a name="get-a-contact-user-photo-by-using-ews-managed-api"></a>Obtenir une photo de contacter l’utilisateur à l’aide des API managées

Votre application peut utiliser l’API managée EWS pour récupérer les photos des contacts, si le contact est stocké dans un dossier de contacts dans la boîte aux lettres de l’utilisateur. Pour ce faire, tout d’abord, recherchez l' **ID d’élément** pour le contact vous souhaitez utiliser. Ensuite, après avoir lié à ce contact, charger à la collection attachments. Si le contact dispose d’une photo, la photo sera une des pièces jointes. Boucle sur la collection de pièces jointes, en vérifiant la valeur de la propriété **IsContactPhoto** . Lorsque vous avez trouvé la photo du contact, vous pouvez l’enregistrer sur votre ordinateur local et vos applications peuvent y accéder. 
  
L’exemple suivant illustre ce processus. Cet exemple suppose que ce **service** est un objet [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur a été authentifié sur un serveur Exchange. 
  
```cs
private static void GetContactPhoto(ExchangeService service, string ItemId)
{
   // Bind to an existing contact by using the ItemId passed into this function.
   Contact contact = Contact.Bind(service, ItemId);
   // Load the contact to get access to the collection of attachments.
   contact.Load(new PropertySet(ContactSchema.Attachments));
   // Loop through the attachments looking for a contact photo.
   foreach (Attachment attachment in contact.Attachments)
   {
      if ((attachment as FileAttachment).IsContactPhoto)
      {
         // Load the attachment to access the content.
         attachment.Load();
      }
   }
   FileAttachment photo = contact.GetContactPictureAttachment();
   // Create a file stream and save the contact photo to your computer.
   using (FileStream file = new FileStream(photo.Name, FileMode.Create, System.IO.FileAccess.Write))
   {
      photo.Load(file);
   }
}

```

<a name="bk_EWS"> </a>

## <a name="get-a-user-photo-by-using-ews"></a>Obtenir une photo de l’utilisateur à l’aide de EWS

Si vous recevez une photo de l’utilisateur de domaine Active Directory, vous pouvez utiliser l’opération [GetUserPhoto](http://msdn.microsoft.com/library/f6e8143d-4235-428e-8f9c-ab6e9b1cfa6e%28Office.15%29.aspx) (si vous connaissez l’adresse de messagerie) ou [ResolveNames](http://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) (si vous ne connaissez pas l’adresse de messagerie). Si vous recevez une photo de l’utilisateur à partir d’un dossier contacts dans la boîte aux lettres, utilisez l’opération [GetItem](http://msdn.microsoft.com/library/6b96dace-1260-4b83-869a-7c31c5583daa%28Office.15%29.aspx) suivie de l’opération [GetAttachment](http://msdn.microsoft.com/library/24d10a15-b942-415e-9024-a6375708f326%28Office.15%29.aspx) . Dans les deux cas, la photo est renvoyée sous forme de chaîne codée en Base64 dans la réponse XML. 
  
### <a name="get-a-mailbox-user-photo-by-using-the-getuserphoto-operation"></a>Obtenir une photo d’utilisateur de boîte aux lettres à l’aide de l’opération GetUserPhoto

Utilisation de l’opération **GetUserPhoto** est simple. Dans la demande XML, spécifiez l’adresse de messagerie de l’utilisateur et la [taille de la photo](http://msdn.microsoft.com/library/e86f98b6-83b5-4530-80eb-dc5df42e2c62%28Office.15%29.aspx) à renvoyer (dans l’élément [SizeRequested](http://msdn.microsoft.com/library/e86f98b6-83b5-4530-80eb-dc5df42e2c62%28Office.15%29.aspx) ). L’exemple de requête XML suivant montre comment obtenir une photo pour Sadie Daniels 360 pixels de large par 360 pixels de haut. 
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013 "/>
   </soap:Header>
   <soap:Body>
      <m:GetUserPhoto>
         <m:Email>sadie@contoso.com</m:Email>
         <m:SizeRequested>HR360x360</m:SizeRequested>
      </m:GetUserPhoto>
   </soap:Body>
</soap:Envelope>

```

Voici la réponse XML. La photo codé en Base64 est contenue dans l’élément [PictureData](http://msdn.microsoft.com/library/1124eac3-ebf2-4b81-96d3-96838c840433%28Office.15%29.aspx) (le contenu a été raccourci pour des raisons de lisibilité). 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
         xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetUserPhotoResponse ResponseClass="Success" 
         xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <HasChanged>true</HasChanged>
      <PictureData>/9j/4AAQSkZJRgABAQEAYABgAAD/2wBDAAg... wATRRRSuB//2Q==</PictureData>
    </GetUserPhotoResponse>
  </s:Body>
</s:Envelope>

```

### <a name="get-a-mailbox-user-photo-by-using-the-resolvenames-operation"></a>Obtenir une photo d’utilisateur de boîte aux lettres à l’aide de l’opération ResolveNames

Si vous ne connaissez pas l’adresse de messagerie de l’utilisateur pour lequel vous obtenez une photo, vous pouvez [utiliser l’opération ResolveNames](how-to-resolve-ambiguous-names-by-using-ews-in-exchange-2013.md) pour obtenir des candidats pour une correspondance possible. Si vous spécifiez « AllProperties » pour l’attribut **ContactDataShape** de l’élément [ResolveNames](http://msdn.microsoft.com/library/c85207e1-1315-443b-94ec-2b58f405076b%28Office.15%29.aspx) , une grande quantité de données, y compris les photos de l’utilisateur, s’afficheront pour chaque candidat. L’exemple suivant montre la demande XML pour résoudre le nom « Sadie » et de renvoyer toutes les propriétés pour chaque candidat. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
<soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>  
<soap:Body>
  <m:ResolveNames ReturnFullContactData="true" ContactDataShape="AllProperties">
      <m:UnresolvedEntry>sadie</m:UnresolvedEntry>
    </m:ResolveNames>
  </soap:Body>
</soap:Envelope>
```

Une grande quantité de données s’afficheront dans la réponse. L’exemple suivant montre uniquement les données relatives à la photo de l’utilisateur. L’élément **Photo** contient la photo d’utilisateur codé en Base64 (le contenu a été raccourci pour des raisons de lisibilité). 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
         xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:ResolveNamesResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:ResolveNamesResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:ResolutionSet TotalItemsInView="1" IncludesLastItemInRange="true">
            <t:Resolution>
              <t:Mailbox>
                <t:Name>Sadie Daniels</t:Name>
                <t:EmailAddress>sadie@contoso.com</t:EmailAddress>
                <t:RoutingType>SMTP</t:RoutingType>
                <t:MailboxType>Mailbox</t:MailboxType>
              </t:Mailbox>
              <t:Contact>
                <t:DisplayName>Sadie Daniels</t:DisplayName>
                <t:GivenName>Sadie</t:GivenName>
                <t:Initials/>
                <t:CompanyName>CONTOSO</t:CompanyName>
......
                <t:Photo>/9j/4AAQSkZJRgABAQE...qKKKAP/2Q==</t:Photo>
......
              </t:Contact>
            </t:Resolution>
          </m:ResolutionSet>
        </m:ResolveNamesResponseMessage>
      </m:ResponseMessages>
    </m:ResolveNamesResponse>
  </s:Body>
</s:Envelope>

```

### <a name="get-a-contact-user-photo-by-using-the-getattachment-operation"></a>Obtenir une photo de contacter l’utilisateur à l’aide de l’opération GetAttachment

Vous pouvez utiliser EWS pour obtenir les photos des contacts stockés dans votre boîte aux lettres. Tout d’abord, vous utilisez l’opération **GetItem** pour renvoyer toutes les propriétés afin de vous permet de rechercher des photos. L’exemple suivant montre une requête XML pour obtenir un élément de contact. L’ID d’élément a été raccourcie pour des raisons de lisibilité. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetItem xmlns='http://schemas.microsoft.com/exchange/services/2006/messages'>
      <ItemShape>
        <t:BaseShape>AllProperties</t:BaseShape>
      </ItemShape>
      <ItemIds>
        <t:ItemId Id="AAAAGECXAAA=" ChangeKey="EQAAABYAAAD2WuN+TpqwSrNP9JCCMKC0AABLzXRv"/>
      </ItemIds>
    </GetItem>
  </soap:Body>
</soap:Envelope>

```

Recherchez l’élément [HasPicture](http://msdn.microsoft.com/library/922a43fe-01bd-49f2-9261-e00e4699b8da%28Office.15%29.aspx) vérifier que le contact dispose d’une photo associée. Recherchez par le biais de la collection de pièces jointes celui qui possède la valeur true pour l’élément [IsContactPhoto](http://msdn.microsoft.com/library/ae36b5f9-a787-4863-9dbc-258ad724801d%28Office.15%29.aspx) . L’exemple suivant de la réponse n'indique que les données pertinentes. Les valeurs d’ID sont raccourcis pour améliorer la lisibilité. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
         xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Contact>
              <t:ItemId Id="AAAAGECXAAA=" ChangeKey="EQAAABYAAAD2WuN+TpqwSrNP9JCCMKC0AABLzXRv"/>
              <t:ParentFolderId Id="nIxIAAA=" ChangeKey="AQAAAA=="/>
              <t:ItemClass>IPM.Contact</t:ItemClass>
              <t:Subject>Hope Gross</t:Subject>
              <t:Sensitivity>Normal</t:Sensitivity>
......
              <t:Attachments>
                <t:FileAttachment>
                  <t:AttachmentId Id="1LGlhgpgoA="/>
                  <t:Name>ContactPicture.jpg</t:Name>
                  <t:Size>6260</t:Size>
                  <t:LastModifiedTime>2011-03-09T16:55:55</t:LastModifiedTime>
                  <t:IsInline>false</t:IsInline>
                  <t:IsContactPhoto>true</t:IsContactPhoto>
                </t:FileAttachment>
              </t:Attachments>
......
              <t:HasPicture>true</t:HasPicture>
            </t:Contact>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </m:GetItemResponse>
  </s:Body>
</s:Envelope>

```

Ensuite, utilisez l’opération **GetAttachment** avec **AttachmentId** pour demander la pièce jointe ayant la photo du contact. L’exemple suivant montre la demande XML pour obtenir la pièce jointe. L’ID est réduite pour une meilleure lisibilité. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
xmlns:xsd="http://www.w3.org/2001/XMLSchema"
xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetAttachment xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <AttachmentShape/>
      <AttachmentIds>
         <t:AttachmentId Id="1LGlhgpgoA="/>
      </AttachmentIds>
    </GetAttachment>
  </soap:Body>
</soap:Envelope>

```

L’exemple suivant montre la réponse XML avec les informations sur la pièce jointe que vous avez demandé. L’élément de [contenu](http://msdn.microsoft.com/library/24f8c54a-505f-4fc0-b7e7-93ad50b97070%28Office.15%29.aspx) contient la chaîne codée en Base64 pour la photo de l’utilisateur, raccourcie dans cet exemple, pour une meilleure lisibilité. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
         xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetAttachmentResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetAttachmentResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Attachments>
            <t:FileAttachment>
              <t:AttachmentId Id="+KsDBEr1LGlhgpgoA="/>
              <t:Name>ContactPicture.jpg</t:Name>
              <t:Content>/9j/4AAQSkZJRgABAQEAYABgAAD/2wBDAAg...D//2Q==</t:Content>
            </t:FileAttachment>
          </m:Attachments>
        </m:GetAttachmentResponseMessage>
      </m:ResponseMessages>
    </m:GetAttachmentResponse>
  </s:Body>
</s:Envelope>

```

<a name="bk_EWS"> </a>

## <a name="decode-a-base64-encoded-string"></a>Décoder une chaîne codée en Base64

Quel que soit l’opération que vous permet d’obtenir une photo de l’utilisateur, vous devez décoder cette chaîne, vous pouvez l’utiliser dans votre application. L’exemple suivant montre comment décoder la chaîne et enregistrez-le sur votre ordinateur local afin de l’application vous pouvez y accéder ultérieurement.
  
```cs
// Convert the encoded string into a byte array.
byte[] data = System.Convert.FromBase64String(Photo);
// Create a memory stream to read the data.
MemoryStream ms = new MemoryStream(data);
// Save the data on your local computer as a JPG image.
using (FileStream file = new FileStream(ContactName + ".jpg", FileMode.Create, System.IO.FileAccess.Write))
{
   byte[] bytes = new byte[ms.Length];
   ms.Read(bytes, 0, (int)ms.Length);
   file.Write(bytes, 0, bytes.Length);
   ms.Close();
}

```

## <a name="see-also"></a>Voir aussi

- [Personnes et contacts dans EWS dans Exchange](people-and-contacts-in-ews-in-exchange.md)    
- [Résoudre des noms ambigus en utilisant EWS dans Exchange 2013](how-to-resolve-ambiguous-names-by-using-ews-in-exchange-2013.md)    
- [Contacts processus par lots à l’aide de EWS dans Exchange](how-to-process-contacts-in-batches-by-using-ews-in-exchange.md)
    

