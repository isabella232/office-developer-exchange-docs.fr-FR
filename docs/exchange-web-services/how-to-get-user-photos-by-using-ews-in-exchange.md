---
title: Obtenir des photos de l’utilisateur à l’aide d’EWS dans Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.assetid: f86d1099-1f57-47dc-abf2-4d5ae4e900a9
description: Découvrez comment obtenir des photos de l’utilisateur qui sont associées à une boîte aux lettres ou à un contact à l’aide de l’API managée EWS ou d’EWS dans Exchange.
localization_priority: Priority
ms.openlocfilehash: 14f2bc6bef1ce3c3529f03e213e3ada7c45a5a71
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455785"
---
# <a name="get-user-photos-by-using-ews-in-exchange"></a>Obtenir des photos de l’utilisateur à l’aide d’EWS dans Exchange

Découvrez comment obtenir des photos de l’utilisateur qui sont associées à une boîte aux lettres ou à un contact à l’aide de l’API managée EWS ou d’EWS dans Exchange.
  
Il est agréable de présenter un visage à un nom. Si vos utilisateurs aiment mettre des noms à des faces, votre application peut demander une image, généralement une photo, à partir d’Exchange qui représente un compte de messagerie. Vous pouvez obtenir une photo d’utilisateur stockée sur un serveur Exchange pour une boîte aux lettres, ou vous pouvez obtenir une photo de contact à partir de contacts stockés dans votre boîte aux lettres.
  
Vous pouvez utiliser plusieurs technologies différentes pour obtenir des photos à partir de boîtes aux lettres ou de services de domaine Active Directory (AD DS). La meilleure façon d’obtenir une photo dépend du type de contact à partir duquel vous souhaitez obtenir une photo. 
  
**Tableau 1. Technologies à utiliser pour obtenir des photos de l’utilisateur en fonction du type de contact**

|**Type de contact**|**Technologies à utiliser**|
|:-----|:-----|
|Photo d’utilisateur de boîte aux lettres  <br/> |[Obtenir une photo d’utilisateur de boîte aux lettres à l’aide de REST](#bk_REST)<br/><br/> [Obtenir une photo de l’utilisateur à l’aide d’EWS](#bk_EWS) <br/> |
|Photo de contact pour les utilisateurs  <br/> |[Obtenir une photo d’utilisateur de contact à l’aide de l’API managée EWS](#bk_EWSMA)<br/><br/> [Obtenir une photo de l’utilisateur à l’aide d’EWS](#bk_EWS) <br/> |

<a name="bk_REST"> </a>

## <a name="get-a-mailbox-user-photo-by-using-rest"></a>Obtenir une photo d’utilisateur de boîte aux lettres à l’aide de REST

Vous pouvez demander des photos de l’utilisateur à partir d’un serveur Exchange à l’aide d’une requête **Get** HTTPS standard. Dans la demande, spécifiez l’adresse du compte de messagerie et un code de taille pour l’image, comme illustré dans l’exemple suivant. 
  
```HTML
https://Exchange Server/ews/Exchange.asmx/s/GetUserPhoto?email=email address&amp;size=size code
```

Utilisez l’opération [GetUserSettings](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) du service de découverte automatique pour récupérer le paramètre **ExternalEwsUrl** , qui contient l’URL du point de terminaison des services Web Exchange (EWS) et l’emplacement du gestionnaire HTTP **. asmx Exchange** qui renvoie les photos de l’utilisateur. 
  
Chaque code de taille indique la hauteur et la largeur de l’image en pixels. Par exemple, le code de taille **HR48x48** renvoie une image de 48 pixels de haut par 48 pixels de large. Les valeurs possibles pour le paramètre de code de taille sont les mêmes que les valeurs possibles pour l’élément [SizeRequested](https://msdn.microsoft.com/library/e86f98b6-83b5-4530-80eb-dc5df42e2c62%28Office.15%29.aspx) . Si la demande spécifie une taille qui n’est pas disponible, la plus grande photo disponible sera renvoyée. Si aucune photo n’est stockée sur le serveur Exchange, l’image miniature stockée dans AD DS pour le compte sera renvoyée. 
  
> [!NOTE]
> Le code de taille **HR48x48** renvoie toujours l’image de miniature AD DS si elle est disponible. 
  
L’exemple suivant montre comment utiliser la requête GET pour récupérer la photo de l’utilisateur pour Sadie et l’enregistrer sur votre ordinateur local.
  
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

La demande renverra une réponse HTTP. 
  
**Tableau 2. Codes de réponse pour une demande GetUserPhoto**

|**Code de réponse**|**Description**|
|:-----|:-----|
|200  <br/> |Une image est disponible pour le compte de messagerie spécifié et l’image binaire est contenue dans la réponse.  <br/> |
|304  <br/> |L’image n’a pas changé depuis le dernier renvoi de l' **ETag** à l’application.  <br/> |
|404  <br/> |Aucune image n’est disponible pour le compte de messagerie spécifié.  <br/> |

<a name="bk_REST"> </a>

## <a name="cache-user-photos"></a>Mettre en cache les photos des utilisateurs

Exchange renvoie les données avec un type de contenu image/JPEG, ainsi qu’une collection de valeurs d’en-tête. L’en-tête **ETag** est similaire à une clé de modification. La valeur est une chaîne qui représente la dernière fois que la photo a été mise à jour. L' **ETag** reste identique pour la photo de l’utilisateur jusqu’à ce que la photo soit modifiée. Vous pouvez envoyer cette valeur **ETag** au serveur dans la requête **Get** https dans un en-tête **If-None-Match** . Si la photo n’a pas changé depuis la dernière demande, le serveur répond par une réponse HTTP 304 qui indique en tant que telle. Cela signifie que vous pouvez utiliser la photo de l’utilisateur que vous avez précédemment demandée et enregistrée au lieu d’en traiter une nouvelle. 

<a name="bk_EWSMA"> </a>

## <a name="get-a-contact-user-photo-by-using-ews-managed-api"></a>Obtenir une photo d’utilisateur de contact à l’aide de l’API managée EWS

Votre application peut utiliser l’API managée EWS pour récupérer des photos pour des contacts, si le contact est stocké dans un dossier de contacts dans la boîte aux lettres de l’utilisateur. Pour ce faire, recherchez d’abord l' **ID ItemId** pour le contact que vous souhaitez utiliser. Ensuite, une fois que vous êtes lié à ce contact, chargez-le dans la collection de pièces jointes. Si le contact a une photo, la photo sera l’une des pièces jointes. Parcourez la collection Attachments, en vérifiant la valeur de la propriété **IsContactPhoto** . Lorsque vous trouvez la photo de contact, vous pouvez l’enregistrer sur votre ordinateur local et votre application peut y accéder. 
  
L’exemple suivant illustre ce processus. Cet exemple suppose que le **service** est un objet[ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur a bien été authentifié pour un serveur Exchange. 
  
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

## <a name="get-a-user-photo-by-using-ews"></a>Obtenir une photo de l’utilisateur à l’aide d’EWS

Si vous obtenez une photo d’utilisateur à partir d’AD DS, vous pouvez utiliser l’opération [GetUserPhoto](https://msdn.microsoft.com/library/f6e8143d-4235-428e-8f9c-ab6e9b1cfa6e%28Office.15%29.aspx) (si vous connaissez l’adresse de messagerie) ou l’opération [ResolveNames](https://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) (si vous ne connaissez pas l’adresse de messagerie). Si vous obtenez une photo de l’utilisateur à partir d’un dossier de contacts dans la boîte aux lettres, utilisez l’opération [GetItem](https://msdn.microsoft.com/library/6b96dace-1260-4b83-869a-7c31c5583daa%28Office.15%29.aspx) suivie de l’opération [GetAttachment](https://msdn.microsoft.com/library/24d10a15-b942-415e-9024-a6375708f326%28Office.15%29.aspx) . Dans les deux cas, la photo est renvoyée sous la forme d’une chaîne codée en Base64 dans la réponse XML. 
  
### <a name="get-a-mailbox-user-photo-by-using-the-getuserphoto-operation"></a>Obtenir une photo d’utilisateur de boîte aux lettres à l’aide de l’opération GetUserPhoto

L’utilisation de l’opération **GetUserPhoto** est simple. Dans la requête XML, spécifiez l’adresse de messagerie de l’utilisateur et la [taille de la photo](https://msdn.microsoft.com/library/e86f98b6-83b5-4530-80eb-dc5df42e2c62%28Office.15%29.aspx) à renvoyer (dans l’élément [SizeRequested](https://msdn.microsoft.com/library/e86f98b6-83b5-4530-80eb-dc5df42e2c62%28Office.15%29.aspx) ). L’exemple de requête XML suivant montre comment obtenir une photo pour Sadie Daniels d’une largeur de 360 pixels sur une hauteur de 360 pixels. 
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

Voici la réponse XML. La photo codée en base64 est contenue dans l’élément [PictureData](https://msdn.microsoft.com/library/1124eac3-ebf2-4b81-96d3-96838c840433%28Office.15%29.aspx) (le contenu a été raccourci pour des raisons de lisibilité). 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
         xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetUserPhotoResponse ResponseClass="Success" 
         xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <HasChanged>true</HasChanged>
      <PictureData>/9j/4AAQSkZJRgABAQEAYABgAAD/2wBDAAg... wATRRRSuB//2Q==</PictureData>
    </GetUserPhotoResponse>
  </s:Body>
</s:Envelope>

```

### <a name="get-a-mailbox-user-photo-by-using-the-resolvenames-operation"></a>Obtenir une photo d’utilisateur de boîte aux lettres à l’aide de l’opération ResolveNames

Si vous ne connaissiez pas l’adresse de messagerie de l’utilisateur pour lequel vous obtenez une photo, vous pouvez [utiliser l’opération ResolveNames](how-to-resolve-ambiguous-names-by-using-ews-in-exchange-2013.md) pour obtenir les candidats pour une correspondance possible. Si vous spécifiez « AllProperties » pour l’attribut **ContactDataShape** de l’élément [ResolveNames](https://msdn.microsoft.com/library/c85207e1-1315-443b-94ec-2b58f405076b%28Office.15%29.aspx) , beaucoup de données, y compris les photos des utilisateurs, seront renvoyées pour chaque candidat. L’exemple suivant montre la requête XML pour résoudre le nom « Sadie » et renvoyer toutes les propriétés de chaque candidat. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

Un grand nombre de données seront renvoyées dans la réponse. L’exemple suivant montre uniquement les données relatives à la photo de l’utilisateur. L’élément **photo** contient la photo de l’utilisateur encodé en base64 (le contenu a été raccourci pour des raisons de lisibilité). 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
         xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:ResolveNamesResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

### <a name="get-a-contact-user-photo-by-using-the-getattachment-operation"></a>Obtenir une photo d’utilisateur de contact à l’aide de l’opération GetAttachment

Vous pouvez utiliser EWS pour obtenir des photos à partir de contacts stockés dans votre boîte aux lettres. Tout d’abord, vous utilisez l’opération **GetItem** pour renvoyer toutes les propriétés afin de pouvoir Rechercher des photos. L’exemple suivant montre une requête XML pour obtenir un élément de contact. L’ID de l’élément a été raccourci pour des raisons de lisibilité. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetItem xmlns='https://schemas.microsoft.com/exchange/services/2006/messages'>
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

Recherchez l’élément [haspicture,](https://msdn.microsoft.com/library/922a43fe-01bd-49f2-9261-e00e4699b8da%28Office.15%29.aspx) pour vérifier que le contact a une photo associée. Recherchez ensuite dans la collection de pièces jointes une valeur de true pour l’élément [IsContactPhoto](https://msdn.microsoft.com/library/ae36b5f9-a787-4863-9dbc-258ad724801d%28Office.15%29.aspx) . L’exemple de réponse suivant montre uniquement les données pertinentes. Les valeurs d’ID sont raccourcies pour des raisons de lisibilité. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
         xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

Ensuite, utilisez l’opération **GetAttachment** avec le **attachmentid** pour demander la pièce jointe contenant la photo de contact. L’exemple suivant montre la requête XML permettant d’obtenir la pièce jointe. L’ID est raccourci pour des raisons de lisibilité. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
xmlns:xsd="http://www.w3.org/2001/XMLSchema"
xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/"
xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetAttachment xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <AttachmentShape/>
      <AttachmentIds>
         <t:AttachmentId Id="1LGlhgpgoA="/>
      </AttachmentIds>
    </GetAttachment>
  </soap:Body>
</soap:Envelope>

```

L’exemple suivant montre la réponse XML avec les informations sur la pièce jointe que vous avez demandée. L’élément [content](https://msdn.microsoft.com/library/24f8c54a-505f-4fc0-b7e7-93ad50b97070%28Office.15%29.aspx) contient la chaîne codée en base 64 pour la photo de l’utilisateur, raccourcie dans cet exemple pour des raisons de lisibilité. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
         xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetAttachmentResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="decode-a-base64-encoded-string"></a>Décoder une chaîne codée en base64

Quelle que soit l’opération que vous utilisez pour obtenir une photo de l’utilisateur, vous devez décoder cette chaîne afin de pouvoir l’utiliser dans votre application. L’exemple suivant montre comment décoder la chaîne, puis l’enregistrer sur votre ordinateur local afin que votre application puisse y accéder ultérieurement.
  
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
- [Résoudre des noms ambigus à l’aide d’EWS dans Exchange 2013](how-to-resolve-ambiguous-names-by-using-ews-in-exchange-2013.md)    
- [Traiter les contacts par lots à l’aide d’EWS dans Exchange](how-to-process-contacts-in-batches-by-using-ews-in-exchange.md)
    

