---
title: Déplacer et copier des messages électroniques à l’aide d’EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 4771668f-5623-4397-a5c0-b75a7ba01698
description: Découvrez comment déplacer et copier des messages électroniques à l’aide de l’API managée EWS ou d’EWS dans Exchange.
localization_priority: Priority
ms.openlocfilehash: d13e84648f194dd4f431cf128396daf016addb22
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527935"
---
# <a name="move-and-copy-email-messages-by-using-ews-in-exchange"></a>Déplacer et copier des messages électroniques à l’aide d’EWS dans Exchange

Découvrez comment déplacer et copier des messages électroniques à l’aide de l’API managée EWS ou d’EWS dans Exchange.
  
Vous pouvez utiliser l’API managée EWS ou EWS pour déplacer et copier des messages électroniques dans une boîte aux lettres.
  
**Tableau 1. Méthodes d’API managée EWS et opérations EWS pour le transfert et la copie de messages électroniques**

|**Tâche**|**Méthode d'API managée EWS**|**Opération EWS**|
|:-----|:-----|:-----|
|Déplacer un message électronique  <br/> |[EmailMessage. Move](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.move%28v=exchg.80%29.aspx) <br/> |[MoveItem](https://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/> |
|Copier un message électronique  <br/> |[EmailMessage. Copy](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.copy%28v=exchg.80%29.aspx) <br/> |[CopyItem](https://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> |
   
Il est important de noter que lorsque vous déplacez ou copiez un message électronique dans un autre dossier, un nouvel élément est créé dans le nouveau dossier avec un ID d’élément unique et le message d’origine est supprimé. Si vous déplacez ou copiez un message électronique entre deux dossiers dans la même boîte aux lettres, le nouvel élément est renvoyé dans la réponse, qui vous donne accès au nouvel ID d’élément. Toutefois, si vous déplacez ou copiez un message électronique entre deux boîtes aux lettres ou entre une boîte aux lettres et un dossier public, le nouvel élément n’est pas renvoyé dans la réponse. Pour accéder au message déplacé dans ce scénario, utilisez la méthode [FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) de l’API managée EWS ou l’opération EWS [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) , [créez une définition de propriété étendue](properties-and-extended-properties-in-ews-in-exchange.md) pour la propriété [PidTagSearchKey](https://msdn.microsoft.com/library/cc839918.aspx) (0x300B0102) ou créez et définissez une propriété étendue personnalisée, puis recherchez la propriété étendue personnalisée dans le nouveau dossier. 
  
La suppression d’un message électronique est différente de celle du transfert d’un élément dans le dossier éléments supprimés. Si vous utilisez l’élément de l’API managée EWS [. Delete](https://msdn.microsoft.com/library/office/dd635072%28v=exchg.80%29.aspx) ou [l’opération EWS](../web-service-reference/deleteitem-operation.md) EWS, l’élément spécifié dans la demande est supprimé du dossier d’origine, et une copie est placée dans le dossier éléments supprimés avec un nouvel ID d’élément. Contrairement à ce qui se passe lorsque vous déplacez ou copiez un élément, le nouvel élément n’est pas renvoyé dans la méthode **Delete** ou la réponse de l’opération **DeleteItem** . La procédure de [Suppression d’un courrier électronique à l’aide de l’API managée EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteewsma) ou [EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteews) est identique à celle de la suppression d’un élément générique de la Banque d’informations Exchange. 
  
## <a name="move-an-email-message-by-using-the-ews-managed-api"></a>Déplacer un message électronique à l’aide de l’API managée EWS
<a name="bk_moveewsma"> </a>

L’exemple de code suivant montre comment utiliser la méthode [EmailMessage. Move](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.move%28v=exchg.80%29.aspx) pour déplacer un message électronique existant d’un dossier à un autre. 
  
Cet exemple part du principe que le **service** est un objet [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’ID **ItemId** est l' [ID](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) du message électronique à déplacer ou à copier. 
  
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

## <a name="move-an-email-message-by-using-ews"></a>Déplacer un message électronique à l’aide d’EWS
<a name="bk_moveews"> </a>

L’exemple de code suivant montre comment utiliser l’opération [MoveItem](https://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) pour déplacer un message électronique dans le dossier courrier indésirable. 
  
Il s’agit également de la requête XML envoyée par l’API managée EWS lors de l’appel de la méthode [Move](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.move%28v=exchg.80%29.aspx) . Les valeurs de certains attributs et éléments ont été raccourcies pour des raisons de lisibilité. 
  
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

Le serveur répond à la demande **MoveItem** avec un message [MoveItemResponse](https://msdn.microsoft.com/library/77be5104-1e09-4d50-abec-4fadb3a230e5%28Office.15%29.aspx) qui inclut une valeur [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NOERROR**, ce qui indique que le message électronique a été déplacé avec succès. La réponse inclut également l' **ItemId** pour le message électronique dans le nouveau dossier, ce qui est important pour le stockage car l' **ItemId** est différent dans le nouveau dossier. 
  
## <a name="copy-an-email-message-by-using-the-ews-managed-api"></a>Copier un message électronique à l’aide de l’API managée EWS
<a name="bk_copyewsma"> </a>

L’exemple de code suivant montre comment utiliser la méthode [EmailMessage. Copy](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.copy%28v=exchg.80%29.aspx) pour copier un message électronique existant d’un dossier vers un autre. 
  
Cet exemple part du principe que le **service** est un objet [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’ID **ItemId** est l' [ID](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) du message électronique à copier. Les valeurs de certains paramètres ont été raccourcies pour des raisons de lisibilité. 
  
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

## <a name="copy-an-email-message-by-using-ews"></a>Copier un message électronique à l’aide d’EWS
<a name="bk_copyews"> </a>

L’exemple de code suivant montre comment utiliser l’opération [CopyItem](https://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) pour copier un message électronique dans un autre dossier de la même boîte aux lettres en envoyant l' [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) du message électronique à déplacer et en spécifiant le dossier de destination dans l’élément [ToFolderId](https://msdn.microsoft.com/library/bd6a4265-ad40-43f6-bcc4-0bf5df4e984c%28Office.15%29.aspx) . 
  
Il s’agit également de la requête XML envoyée par l’API managée EWS lors de l’appel de la méthode [Copy](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.copy%28v=exchg.80%29.aspx) . Les valeurs de certains attributs et éléments ont été raccourcies pour des raisons de lisibilité. 
  
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

Le serveur répond à la demande **CopyItem** avec un message [CopyItemResponse](https://msdn.microsoft.com/library/ae402bc1-4589-45e0-a929-f368c916a7e4%28Office.15%29.aspx) qui inclut une valeur [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NOERROR**, ce qui indique que le message électronique a été correctement copié. La réponse inclut également l' **ItemId** pour le message électronique dans le nouveau dossier, ce qui est important pour le stockage car l' **ItemId** est différent dans le nouveau dossier. 
  
## <a name="see-also"></a>Voir aussi


- [Courrier électronique et les services EWS d'Exchange](email-and-ews-in-exchange.md)
    
- [Envoyer des messages électroniques à l’aide d’EWS dans Exchange](how-to-send-email-messages-by-using-ews-in-exchange.md)
    

