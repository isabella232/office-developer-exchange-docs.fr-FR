---
title: Courrier électronique et les services EWS d’Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 4d7bdb37-f7f1-409f-9749-f8bcde7dc52a
description: Découvrez comment travailler avec les messages électroniques, y compris comment créer un message électronique et comment effectuer d’autres tâches liées à la messagerie à l’aide de l’API managée EWS ou EWS dans Exchange.
ms.openlocfilehash: d222be7409a3c3f4613a2be39b83b977fabb09e8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19754770"
---
# <a name="email-and-ews-in-exchange"></a>Courrier électronique et les services EWS d’Exchange

Découvrez comment travailler avec les messages électroniques, y compris comment créer un message électronique et comment effectuer d’autres tâches liées à la messagerie à l’aide de l’API managée EWS ou EWS dans Exchange.
  

  
Fondamentalement, Exchange est à la messagerie. Mais ce qui rend un message électronique, un message électronique ? Eh bien, les messages électroniques font partie des [fortement typées éléments](folders-and-items-in-ews-in-exchange.md#bk_item) dans Exchange, ce qui signifie qu’ils contiennent d’un particulier de [définir des propriétés](email-properties-and-elements-in-ews-in-exchange.md), avant même qu’ils sont envoyés. Les messages électroniques sont représentées par la classe [EmailMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) dans l’API managée EWS, ainsi que par l’élément de [Message](http://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx) et ses éléments enfants dans EWS. 
  
Dans l’API managée EWS, l’objet **EmailMessage** dérive de l’objet [d’élément](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) . La classe **EmailMessage** étend la classe **d’élément** en fournissant des propriétés supplémentaires, telles que [EmailMessage.Sender](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.sender%28v=exchg.80%29.aspx) et [EmailMessage.IsRead](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.isread%28v=exchg.80%29.aspx), qui sont maintenant communs à presque tous les scénarios de messagerie. Lorsque vous recevez, mettre à jour ou supprimer un message électronique, dans la plupart des cas que possible à l’aide de l’objet **EmailMessage** ou l’objet **élément de** base, selon que les propriétés que vous travaillez dans [EmailMessageSchema](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessageschema%28v=exchg.80%29.aspx) ou le [ ItemSchema](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemschema%28v=exchg.80%29.aspx) classe. Création de l’élément est différente, car la classe de **l’élément** ne dispose pas d’un constructeur, donc lorsque vous créez un message électronique, vous allez utiliser le [constructeur EmailMessage](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.emailmessage%28v=exchg.80%29.aspx) pour créer et la [EmailMessage.Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.save%28v=exchg.80%29.aspx) ou [EmailMessage.SendAndSaveCopy ](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx)méthodes, enregistrer ou envoyer et l’enregistrer. 
  
De même, dans les services EWS, utilisez l’opération [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) avec l’élément de [Message](http://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx) pour créer un message électronique. Pour obtenir, mettre à jour ou supprimer des messages électroniques à l’aide de EWS, le fait que l’élément en cours de modification est un message électronique n’est pas important, outre le fait que les propriétés supplémentaires sont disponibles sur les messages électroniques. Les mêmes opérations qui sont utilisées pour les autres éléments fortement typées sont également utilisées pour les messages électroniques. 
  
|**Tâche**|**Méthode d'API managée EWS**|**Opération EWS**|
|:-----|:-----|:-----|
|Créer  <br/> |[EmailMessage.Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.save%28v=exchg.80%29.aspx) <br/> |[CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) <br/> |
|Télécharger  <br/> |[EmailMessage.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) <br/> |[GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) <br/> |
|Mise à jour  <br/> |[Item.Update](http://msdn.microsoft.com/en-us/library/dd635915%28v=exchg.80%29.aspx) <br/> |[UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |
|Suppression  <br/> |[Item.Delete](http://msdn.microsoft.com/en-us/library/dd635072%28v=exchg.80%29.aspx) <br/> |[DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |
   
Étant donné que les messages électroniques sont simplement [fortement typées éléments](folders-and-items-in-ews-in-exchange.md#bk_item), dans certains cas, vous travaillez avec eux de la même manière que vous [travailler avec des éléments génériques](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md). 
  
## <a name="create-an-email-message-by-using-the-ews-managed-api"></a>Créer un message électronique à l’aide de l’API managée EWS
<a name="bk_createewsma"> </a>

Vous pouvez créer un message électronique à l’aide de la méthode API managées [Enregistrer](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.save%28v=exchg.80%29.aspx) , comme indiqué dans le code dans l’exemple suivant. Notez que l’exemple enregistre uniquement le message dans le dossier Brouillons, il n’envoie pas le message. Pour savoir comment envoyer le message ou créer et envoyer le message en une seule étape, voir [Envoyer des messages électroniques à l’aide de EWS dans Exchange](how-to-send-email-messages-by-using-ews-in-exchange.md).
  
Cet exemple suppose que ce **service** est un objet [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur a été authentifié sur un serveur Exchange. 
  
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

## <a name="create-an-email-message-by-using-ews"></a>Créer un message électronique à l’aide de EWS
<a name="bk_createews"> </a>

Vous pouvez créer un message électronique à l’aide de l’opération EWS [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) , comme illustré dans l’exemple suivant. C’est également la demande XML que l’API managée EWS envoie lorsque vous [créez un message électronique](#bk_createewsma). Notez que l’exemple suivant enregistre uniquement le message dans le dossier Brouillons, il n’envoie pas le message. Pour savoir comment envoyer le message ou créer et envoyer le message d’un coller, voir [Envoyer des messages électroniques à l’aide de EWS dans Exchange](how-to-send-email-messages-by-using-ews-in-exchange.md).
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

Le serveur répond à la demande **CreateItem** avec un message [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) qui contient une valeur [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, ce qui indique que le courrier électronique a été créé avec succès et l' [ID d’élément](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) de la nouvelle message créé. 
  
## <a name="get-update-and-delete-an-email-message-by-using-the-ews-managed-api"></a>Obtenir, mettre à jour et supprimer un message électronique à l’aide de l’API managée EWS
<a name="bk_getewsma"> </a>

Vous pouvez utiliser l’API managée EWS pour obtenir, mettre à jour ou supprimer un message électronique de la même manière que vous effectuez ces actions sur n’importe quel élément générique à partir de la banque d’informations Exchange. Pour plus d’informations, voir [utilisation des éléments de boîte aux lettres Exchange à l’aide de EWS dans Exchange](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md).
  
Si vous mettez à jour un message électronique, voir [messagerie dans Exchange les propriétés et les éléments dans les services EWS](email-properties-and-elements-in-ews-in-exchange.md) pour obtenir la liste des propriétés de message électronique accessible en écriture. Pour envoyer un brouillon de message une fois que vous avez mis à jour, voir [Envoyer un message électronique de brouillon à l’aide de l’API managée EWS](how-to-send-email-messages-by-using-ews-in-exchange.md#bk_senddraftewsma).
  
## <a name="get-update-and-delete-an-email-message-by-using-ews"></a>Obtenir, mettre à jour et supprimer un message électronique à l’aide de EWS
<a name="bk_getews"> </a>

Vous pouvez utiliser EWS pour obtenir, mettre à jour et supprimer un message électronique de la même manière que vous effectuez ces actions sur n’importe quel élément générique à partir de la banque d’informations Exchange. Pour plus d’informations, voir [utilisation des éléments de boîte aux lettres Exchange à l’aide de EWS dans Exchange](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md).
  
Si vous mettez à jour un message électronique, voir [messagerie dans Exchange les propriétés et les éléments dans les services EWS](email-properties-and-elements-in-ews-in-exchange.md) pour obtenir la liste des propriétés de message électronique accessible en écriture. Pour envoyer un brouillon de message une fois que vous avez mis à jour, voir [Envoyer un message électronique de brouillon à l’aide de EWS](how-to-send-email-messages-by-using-ews-in-exchange.md#bk_senddraftews).
  
## <a name="in-this-section"></a>Dans cette section
<a name="bk_inthissection"> </a>

- [Propriétés et éléments dans les services EWS de messagerie dans Exchange](email-properties-and-elements-in-ews-in-exchange.md)
    
- [Envoyer des messages électroniques à l’aide de EWS dans Exchange](how-to-send-email-messages-by-using-ews-in-exchange.md)
    
- [Répondre aux messages électroniques à l’aide de EWS dans Exchange](how-to-respond-to-email-messages-by-using-ews-in-exchange.md)
    
- [Déplacer et copier des messages électroniques à l’aide de EWS dans Exchange](how-to-move-and-copy-email-messages-by-using-ews-in-exchange.md)
    
- [Utilisation de conversations à l’aide de EWS dans Exchange](how-to-work-with-conversations-by-using-ews-in-exchange.md)
    
- [Extraire une entité d’un message électronique à l’aide de EWS dans Exchange](how-to-extract-an-entity-from-an-email-message-by-using-ews-in-exchange.md)
    
- [Traiter les messages électroniques par lots à l’aide de EWS dans Exchange](how-to-process-email-messages-in-batches-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a>Voir aussi


- [Développer des clients de service web pour Exchange](develop-web-service-clients-for-exchange.md)
    
- [Dossiers et éléments dans EWS dans Exchange](folders-and-items-in-ews-in-exchange.md)
    

