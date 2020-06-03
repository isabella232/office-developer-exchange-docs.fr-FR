---
title: Courrier électronique et les services EWS d'Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 4d7bdb37-f7f1-409f-9749-f8bcde7dc52a
description: Découvrez comment utiliser les messages électroniques, y compris comment créer un courrier électronique et effectuer d’autres tâches liées à la messagerie à l’aide de l’API managée EWS ou d’EWS dans Exchange.
localization_priority: Priority
ms.openlocfilehash: 323d9d2cc40aa86044a439ad53e53a4808916783
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455442"
---
# <a name="email-and-ews-in-exchange"></a>Courrier électronique et les services EWS d'Exchange

Découvrez comment utiliser les messages électroniques, y compris comment créer un courrier électronique et effectuer d’autres tâches liées à la messagerie à l’aide de l’API managée EWS ou d’EWS dans Exchange.
  

  
Exchange est à la base du courrier électronique. Qu’est-ce qu’un courrier électronique ? Eh bien, les messages électroniques sont l’un des [éléments fortement typés](folders-and-items-in-ews-in-exchange.md#bk_item) dans Exchange, ce qui signifie qu’ils contiennent un [ensemble particulier de propriétés](email-properties-and-elements-in-ews-in-exchange.md), même avant leur envoi. Les messages électroniques sont représentés par la classe [EmailMessage](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) dans l’API managée EWS et par l’élément [message](https://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx) et ses éléments enfants dans EWS. 
  
Dans l’API managée EWS, l’objet **EmailMessage** est dérivé de l’objet [Item](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) . La classe **EmailMessage** étend la classe **Item** en fournissant des propriétés supplémentaires, telles que [EmailMessage. sender](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.sender%28v=exchg.80%29.aspx) et [EmailMessage. IsRead](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.isread%28v=exchg.80%29.aspx), qui sont désormais communes à presque tous les scénarios de messagerie. Lorsque vous obtenez, mettez à jour ou supprimez un message électronique, dans la plupart des cas, vous pouvez le faire à l’aide de l’objet **EmailMessage** ou de l’objet d' **élément** de base, selon que les propriétés que vous utilisez sont dans la [EmailMessageSchema](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessageschema%28v=exchg.80%29.aspx) ou la classe [ItemSchema](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemschema%28v=exchg.80%29.aspx) . La création d’élément est différente étant donné que la classe d' **élément** n’a pas de constructeur, ainsi, lorsque vous créez un message électronique, vous utiliserez le [constructeur EmailMessage](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.emailmessage%28v=exchg.80%29.aspx) pour le créer et les méthodes [EmailMessage. Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.save%28v=exchg.80%29.aspx) ou [EmailMessage. méthodesendandsavecopy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) pour l’enregistrer, ou l’envoyer et l’enregistrer. 
  
De même, dans EWS, utilisez l’opération [CreateItem](https://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) avec l’élément [message](https://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx) pour créer un message électronique. Pour obtenir, mettre à jour ou supprimer des courriers électroniques à l’aide d’EWS, le fait que l’élément en cours de modification soit un message électronique n’est pas important, hormis le fait que des propriétés supplémentaires sont disponibles pour les messages électroniques. Les mêmes opérations utilisées pour d’autres éléments fortement typés sont également utilisées pour les messages électroniques. 
  
|**Tâche**|**Méthode d'API managée EWS**|**Opération EWS**|
|:-----|:-----|:-----|
|Créer  <br/> |[EmailMessage. Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.save%28v=exchg.80%29.aspx) <br/> |[CreateItem](https://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) <br/> |
|Obtenir  <br/> |[EmailMessage. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) <br/> |[GetItem](https://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) <br/> |
|Update  <br/> |[Item.Update](https://msdn.microsoft.com/library/dd635915%28v=exchg.80%29.aspx) <br/> |[UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |
|Supprimer  <br/> |[Item.Delete](https://msdn.microsoft.com/library/dd635072%28v=exchg.80%29.aspx) <br/> |[DeleteItem](../web-service-reference/deleteitem-operation.md) <br/> |
   
Étant donné que les messages électroniques sont simplement des [éléments fortement typés](folders-and-items-in-ews-in-exchange.md#bk_item), dans certains cas, vous les utilisez de la même manière que pour les [éléments génériques](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md). 
  
## <a name="create-an-email-message-by-using-the-ews-managed-api"></a>Créer un message électronique à l’aide de l’API managée EWS
<a name="bk_createewsma"> </a>

Vous pouvez créer un message électronique à l’aide de la méthode [Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.save%28v=exchg.80%29.aspx) de l’API managée EWS, comme illustré dans le code de l’exemple suivant. Notez que l’exemple enregistre uniquement le message dans le dossier Brouillons, il n’envoie pas le message. Pour plus d’informations sur la façon d’envoyer le message ou de créer et d’envoyer le message en une seule étape, consultez la rubrique [Envoyer des messages électroniques à l’aide d’EWS dans Exchange](how-to-send-email-messages-by-using-ews-in-exchange.md).
  
Cet exemple suppose que le **service** est un objet[ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur a bien été authentifié pour un serveur Exchange. 
  
```cs
// Create a new email message.
EmailMessage message = new EmailMessage(service);
// Set properties on the email message.
message.ToRecipients.Add("mack@contoso.com");
message.Subject = "Project priorities";
message.Body = "(1) Buy pizza, (2) Eat pizza";
// Save the email message to the Drafts folder (where it can be retrieved, updated, and sent at a later time).
// This method call results in a CreateItem call to EWS.
message.Save(WellKnownFolderName.Drafts);
Console.WriteLine("A draft email message with the subject '" + message.Subject + "' has been saved to the Drafts folder.");
```

## <a name="create-an-email-message-by-using-ews"></a>Créer un message électronique à l’aide d’EWS
<a name="bk_createews"> </a>

Vous pouvez créer un message électronique à l’aide de l’opération [CREATEITEM](https://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) EWS, comme illustré dans l’exemple suivant. Il s’agit également de la demande XML que l’API managée EWS envoie lorsque vous [créez un message électronique](#bk_createewsma). Notez que l’exemple suivant enregistre uniquement le message dans le dossier Brouillons, il n’envoie pas le message. Pour plus d’informations sur l’envoi du message ou sur la création et l’envoi du message dans un Ste, voir [Envoyer des messages électroniques à l’aide d’EWS dans Exchange](how-to-send-email-messages-by-using-ews-in-exchange.md).
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010_SP2" />
  </soap:Header>
  <soap:Body>
    <m:CreateItem MessageDisposition="SaveOnly">
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="drafts" />
      </m:SavedItemFolderId>
      <m:Items>
        <t:Message>
          <t:Subject>Project priorities</t:Subject>
          <t:Body BodyType="HTML">(1) Buy pizza, (2) Eat pizza</t:Body>
          <t:ToRecipients>
            <t:Mailbox>
              <t:EmailAddress>mack@contoso.com</t:EmailAddress>
            </t:Mailbox>
          </t:ToRecipients>
        </t:Message>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>

```

Le serveur répond à la demande**CreateItem** par un message [GetItemResponse](https://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx), qui inclut [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) renvoyant la valeur **NoError**, indiquant que le message a bien été créé, et où apparaît l’élément [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) du nouveau message. 
  
## <a name="get-update-and-delete-an-email-message-by-using-the-ews-managed-api"></a>Obtenir, mettre à jour et supprimer un message électronique à l’aide de l’API managée EWS
<a name="bk_getewsma"> </a>

Vous pouvez utiliser l’API managée EWS pour obtenir, mettre à jour ou supprimer un message électronique de la même façon que vous effectuez ces actions sur n’importe quel élément générique de la Banque d’aide Exchange. Pour plus d’informations, consultez la rubrique [utilisation des éléments de boîte aux lettres Exchange à l’aide d’EWS dans Exchange](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md).
  
Si vous mettez à jour un message électronique, consultez la rubrique [Propriétés et éléments de messagerie dans EWS dans Exchange](email-properties-and-elements-in-ews-in-exchange.md) pour obtenir la liste des propriétés d’un message électronique accessible en écriture. Pour envoyer un brouillon de message une fois que vous l’avez mis à jour, consultez [la rubrique envoyer un brouillon de message électronique à l’aide de l’API managée EWS](how-to-send-email-messages-by-using-ews-in-exchange.md#bk_senddraftewsma).
  
## <a name="get-update-and-delete-an-email-message-by-using-ews"></a>Obtenir, mettre à jour et supprimer un message électronique à l’aide d’EWS
<a name="bk_getews"> </a>

Vous pouvez utiliser EWS pour obtenir, mettre à jour et supprimer un message électronique de la même façon que vous effectuez ces actions sur n’importe quel élément générique de la Banque d’aide Exchange. Pour plus d’informations, consultez la rubrique [utilisation des éléments de boîte aux lettres Exchange à l’aide d’EWS dans Exchange](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md).
  
Si vous mettez à jour un message électronique, consultez la rubrique [Propriétés et éléments de messagerie dans EWS dans Exchange](email-properties-and-elements-in-ews-in-exchange.md) pour obtenir la liste des propriétés d’un message électronique accessible en écriture. Pour envoyer un brouillon de message une fois que vous l’avez mis à jour, consultez [la rubrique envoyer un brouillon de message électronique à l’aide d’EWS](how-to-send-email-messages-by-using-ews-in-exchange.md#bk_senddraftews).
  
## <a name="in-this-section"></a>Dans cette section
<a name="bk_inthissection"> </a>

- [Propriétés et éléments de messagerie dans EWS dans Exchange](email-properties-and-elements-in-ews-in-exchange.md)
    
- [Envoyer des messages électroniques à l’aide d’EWS dans Exchange](how-to-send-email-messages-by-using-ews-in-exchange.md)
    
- [Répondre à des messages électroniques à l’aide d’EWS dans Exchange](how-to-respond-to-email-messages-by-using-ews-in-exchange.md)
    
- [Déplacer et copier des messages électroniques à l’aide d’EWS dans Exchange](how-to-move-and-copy-email-messages-by-using-ews-in-exchange.md)
    
- [Utiliser des conversations à l’aide d’EWS dans Exchange](how-to-work-with-conversations-by-using-ews-in-exchange.md)
    
- [Extraire une entité à partir d’un message électronique à l’aide d’EWS dans Exchange](how-to-extract-an-entity-from-an-email-message-by-using-ews-in-exchange.md)
    
- [Traiter les messages électroniques par lots à l’aide d’EWS dans Exchange](how-to-process-email-messages-in-batches-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a>Voir aussi


- [Développer des clients de service web pour Exchange](develop-web-service-clients-for-exchange.md)
    
- [Dossiers et éléments dans EWS dans Exchange](folders-and-items-in-ews-in-exchange.md)
    

