---
title: Déplacer et copier des messages électroniques à l’aide de EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 4771668f-5623-4397-a5c0-b75a7ba01698
description: Découvrez comment déplacer et copier des messages électroniques à l’aide de l’API managée EWS ou EWS dans Exchange.
ms.openlocfilehash: 16f0604a16785c34dd04bdabedeedd331668a479
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19754908"
---
# <a name="move-and-copy-email-messages-by-using-ews-in-exchange"></a>Déplacer et copier des messages électroniques à l’aide de EWS dans Exchange

Découvrez comment déplacer et copier des messages électroniques à l’aide de l’API managée EWS ou EWS dans Exchange.
  
Vous pouvez utiliser l’API managée EWS ou EWS pour déplacer et copier les messages dans une boîte aux lettres.
  
**Le tableau 1. Méthodes d’API managées et opérations EWS pour déplacer et copier des messages électroniques**

|**Tâche**|**Méthode d'API managée EWS**|**Opération EWS**|
|:-----|:-----|:-----|
|Déplacer un message électronique  <br/> |[EmailMessage.Move](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.move%28v=exchg.80%29.aspx) <br/> |[MoveItem](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/> |
|Copier un message électronique  <br/> |[EmailMessage.Copy](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.copy%28v=exchg.80%29.aspx) <br/> |[CopyItem](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> |
   
Il est important de noter que lorsque vous déplacez ou copiez un message électronique dans un autre dossier, un nouvel élément est créé dans le nouveau dossier avec un ID d’élément unique et le message d’origine est supprimé. Si vous êtes en déplacement ou copie d’un message électronique entre deux dossiers dans la même boîte aux lettres, le nouvel élément est retourné dans la réponse, qui vous permet d’accéder à l’ID d’élément nouveau. Toutefois, si vous êtes déplacement ou la copie d’un message électronique entre deux boîtes aux lettres ou une boîte aux lettres et d’un dossier public, le nouvel élément n’est pas retourné dans la réponse. Pour accéder au message déplacé dans ce scénario, utilisez la méthode de l' API managée EWS [FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) ou d’une opération EWS [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) , [créer une définition de la propriété étendue](properties-and-extended-properties-in-ews-in-exchange.md) de la propriété [PidTagSearchKey](http://msdn.microsoft.com/en-us/library/cc839918.aspx) (0x300B0102), ou créer et définir une personnalisé étendu propriété et recherchez la propriété étendue personnalisée dans le nouveau dossier. 
  
Suppression d’un message électronique est différente de celui de déplacement d’un élément dans le dossier éléments supprimés. Si vous utilisez la méthode API managées [Item.Delete](http://msdn.microsoft.com/en-us/library/office/dd635072%28v=exchg.80%29.aspx) ou l’opération EWS [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) , l’élément spécifié dans la demande est supprimée à partir du dossier d’origine, et une copie est placée dans le dossier éléments supprimés avec un nouvel ID d’élément. Contrairement à lorsque vous déplacez ou copiez n’importe quel élément, le nouvel élément n’est pas retourné dans la réponse d’opération **DeleteItem** ou de la méthode **Delete** . Les étapes nécessaires lors de la [suppression d’un message électronique à l’aide de l’API managée EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteewsma) ou [EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteews) sont les mêmes que celles permettant de supprimer n’importe quel élément générique de la banque d’informations Exchange. 
  
## <a name="move-an-email-message-by-using-the-ews-managed-api"></a>Déplacer un message électronique à l’aide de l’API managée EWS
<a name="bk_moveewsma"> </a>

L’exemple de code suivant montre comment utiliser la méthode [EmailMessage.Move](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.move%28v=exchg.80%29.aspx) pour déplacer un message électronique existant d’un dossier à un autre. 
  
Cet exemple suppose que **le service** est un objet [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et **ItemId** est l' [Id](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) du message électronique pour déplacer ou copier. 
  
```cs
// As a best practice, limit the properties returned by the Bind method to only those that are required.
PropertySet propSet = new PropertySet(BasePropertySet.IdOnly, EmailMessageSchema.Subject, EmailMessageSchema.ParentFolderId);
// Bind to the existing item by using the ItemId.
// This method call results in a GetItem call to EWS.
EmailMessage beforeMessage = EmailMessage.Bind(service, ItemId, propSet);
// Move the specified mail to the JunkEmail folder and store the returned item.
Item item = beforeMessage.Move(WellKnownFolderName.JunkEmail);
// Check that the item was moved by binding to the moved email message 
// and retrieving the new ParentFolderId.
// This method call results in a GetItem call to EWS.
EmailMessage movedMessage = EmailMessage.Bind(service, item.Id, propSet);
Console.WriteLine("An email message with the subject '" + beforeMessage.Subject + "' has been moved from the '" + beforeMessage.ParentFolderId + "' folder to the '" + movedMessage.ParentFolderId + "' folder.");
```

## <a name="move-an-email-message-by-using-ews"></a>Déplacer un message électronique à l’aide de EWS
<a name="bk_moveews"> </a>

L’exemple de code suivant montre comment utiliser l’opération [MoveItem](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) pour déplacer un message électronique vers le dossier courrier indésirable. 
  
C’est également la demande XML qui est envoyée par l’API managée EWS lors de l’appel de la méthode [Move](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.move%28v=exchg.80%29.aspx) . Les valeurs de certains attributs et éléments ont été raccourcies pour des raisons de lisibilité. 
  
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
    <m:MoveItem>
      <m:ToFolderId>
        <t:DistinguishedFolderId Id="junkemail" />
      </m:ToFolderId>
      <m:ItemIds>
        <t:ItemId Id="AfwDoAAA="
                  ChangeKey="CQAAABYAAAApjGm7TnMWQ5TzjbhziLL0AAF25sM1" />
      </m:ItemIds>
    </m:MoveItem>
  </soap:Body>
</soap:Envelope>
```

Le serveur répond à la demande **MoveItem** avec un message [MoveItemResponse](http://msdn.microsoft.com/library/77be5104-1e09-4d50-abec-4fadb3a230e5%28Office.15%29.aspx) qui contient une valeur [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, ce qui indique que le message électronique a été déplacé avec succès. La réponse inclut également les **ItemId** pour le message électronique dans le nouveau dossier, ce qui est important car les **ItemId** est différentes dans le nouveau dossier. 
  
## <a name="copy-an-email-message-by-using-the-ews-managed-api"></a>Copier un message électronique à l’aide de l’API managée EWS
<a name="bk_copyewsma"> </a>

L’exemple de code suivant montre comment utiliser la méthode [EmailMessage.Copy](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.copy%28v=exchg.80%29.aspx) pour copier un message électronique existant d’un dossier à un autre. 
  
Cet exemple suppose que **le service** est un objet [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide, et **ItemId** est l' [Id](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) du message électronique à copier. Les valeurs de certains paramètres ont été raccourcies pour des raisons de lisibilité. 
  
```cs
// As a best practice, limit the properties returned by the Bind method to only those that are required.
PropertySet propSet = new PropertySet(BasePropertySet.IdOnly, EmailMessageSchema.Subject, EmailMessageSchema.ParentFolderId);
// Bind to the existing item by using the ItemId.
// This method call results in a GetItem call to EWS.
EmailMessage originalMessage = EmailMessage.Bind(service, ItemId, propSet);
// Copy the orignal message into another folder in the mailbox and store the returned item.
Item item = originalMessage.Copy("epQ/3AAA=");
// Check that the item was copied by binding to the copied email message 
// and retrieving the new ParentFolderId.
// This method call results in a GetItem call to EWS.
EmailMessage copiedMessage = EmailMessage.Bind(service, item.Id, propSet);
Console.WriteLine("An email message with the subject '" + originalMessage.Subject + "' has been copied from the '" + originalMessage.ParentFolderId + "' folder to the '" + copiedMessage.ParentFolderId + "' folder.");
```

## <a name="copy-an-email-message-by-using-ews"></a>Copier un message électronique à l’aide de EWS
<a name="bk_copyews"> </a>

L’exemple de code suivant montre comment utiliser l’opération [CopyItem](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) pour copier un message électronique dans un dossier différent dans la même boîte aux lettres en envoyant [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) du message électronique pour déplacer et en spécifiant le dossier de destination dans la [ToFolderId ](http://msdn.microsoft.com/library/bd6a4265-ad40-43f6-bcc4-0bf5df4e984c%28Office.15%29.aspx)élément. 
  
C’est également la demande XML qui est envoyée par l’API managée EWS lors de l’appel de la méthode [Copy](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.copy%28v=exchg.80%29.aspx) . Les valeurs de certains attributs et éléments ont été raccourcies pour des raisons de lisibilité. 
  
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
    <m:CopyItem>
      <m:ToFolderId>
        <t:FolderId Id="pQ/3AAA=" />
      </m:ToFolderId>
      <m:ItemIds>
        <t:ItemId Id="2TSeSAAA="
                  ChangeKey="CQAAABYAAAApjGm7TnMWQ5TzjbhziLL0AAF2d+3+" />
      </m:ItemIds>
    </m:CopyItem>
  </soap:Body>
</soap:Envelope>
```

Le serveur répond à la demande **CopyItem** avec un message [CopyItemResponse](http://msdn.microsoft.com/library/ae402bc1-4589-45e0-a929-f368c916a7e4%28Office.15%29.aspx) qui contient une valeur [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, ce qui indique que le message électronique a été correctement copié. La réponse inclut également les **ItemId** pour le message électronique dans le nouveau dossier, ce qui est important car les **ItemId** est différentes dans le nouveau dossier. 
  
## <a name="see-also"></a>Voir aussi


- [Courrier électronique et les services EWS d'Exchange](email-and-ews-in-exchange.md)
    
- [Envoyer des messages électroniques à l’aide de EWS dans Exchange](how-to-send-email-messages-by-using-ews-in-exchange.md)
    

