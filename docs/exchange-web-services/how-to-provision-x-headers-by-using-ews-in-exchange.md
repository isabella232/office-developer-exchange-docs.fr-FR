---
title: Mettre en service les en-têtes x à l’aide de EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 45a99a14-a85f-47f8-af48-18eb6c6cc230
description: Découvrez comment mettre en service les en-têtes x pour une boîte aux lettres à l’aide de l’API managée EWS ou EWS dans Exchange.
ms.openlocfilehash: de572764921da432cfa203b3dcf166d1d34dd0cd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19754925"
---
# <a name="provision-x-headers-by-using-ews-in-exchange"></a>Mettre en service les en-têtes x à l’aide de EWS dans Exchange

Découvrez comment mettre en service les en-têtes x pour une boîte aux lettres à l’aide de l’API managée EWS ou EWS dans Exchange.
  
Les en-têtes X sont des en-têtes standard qui sont ajoutés à la collection d’en-tête d’un message électronique pour communiquer des informations. Par exemple, échanger des messages de cachets avec l’en-tête **X-MS-Exchange-organisation-SCL** pour indiquer le niveau de confiance du courrier indésirable (SCL) attribué à la messagerie électronique. Clients de messagerie comme Outlook peut utiliser ces informations pour déterminer le type d’action à effectuer sur le courrier électronique (par exemple, Outlook peut empêcher un images d’afficher, sauf si l’utilisateur exécute une action). 
  
Exchange ajoute les en-têtes x entrants au schéma de boîte aux lettres comme une heure de la propriété nommée le premier qu’il reçoit un message électronique avec cet en-tête x. La valeur de l’en-tête x n’est pas enregistrée sur ce premier e-mail ; Toutefois, il est enregistré sur tous les messages électroniques suivants qui incluent l’en-tête x. Pour cette raison, votre application doit mettre en service les en-têtes x avant que vous prévoyez de les utiliser. Le mappage entre une propriété nommée et un en-tête x-lors de la remise de transport du courrier électronique à la boîte aux lettres. Cela signifie que vous avez besoin pour recevoir le courrier électronique par le biais de livraison de transport ; Impossible d’enregistrer seulement un message électronique qui inclut l’en-tête x-pour une boîte aux lettres pour créer le mappage à une propriété nommée.
  
> [!NOTE]
> Si vous trouvez que les en-têtes x ne sont pas enregistrées, déterminez si un [agent de transport](http://code.msdn.microsoft.com/Exchange-2013-Build-an-32f62f5a) ou un [pare-feu d’en-tête](http://technet.microsoft.com/en-us/library/bb232136%28v=exchg.150%29.aspx) est filtrant les en-têtes x-avant qu’ils n’atteignent la boîte aux lettres. 
  
## <a name="provision-an-x-header-by-using-the-ews-managed-api"></a>Mettre en service un en-tête x à l’aide de l’API managée EWS
<a name="bk_example1"> </a>

L’exemple de code suivant montre comment utiliser la méthode API managées [EmailMessage.Send](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.send%28v=exchg.80%29.aspx) pour mettre en service un en-tête x-pour une boîte aux lettres. Cet exemple suppose que ce **service** est un objet [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) et que la boîte aux lettres cible n’a pas dépassé le [quota pour les propriétés nommées](http://technet.microsoft.com/en-us/library/bb851492%28v=EXCHG.80%29.aspx).
  
```cs
private static void ProvisionCustomXHeaderByEmail(ExchangeService service)
{
    // Create a definition for an extended property that will represent a custom x-header. X-headers must be created in the
    // InternetHeaders property set. The x-header name must match the name of the x-header sent in the subsequent emails so
    // the x-header and value are saved on the email.
    ExtendedPropertyDefinition xExperimentalHeader = new ExtendedPropertyDefinition(DefaultExtendedPropertySet.InternetHeaders,
                                                                                            "X-Experimental",
                                                                                            MapiPropertyType.String);
    // Create an item that is used to provision the custom x-header.
    EmailMessage email = new EmailMessage(service);
    email.ToRecipients.Add("user@contoso.com");
    email.SetExtendedProperty(xExperimentalHeader, "Provision X-Experimental Internet message header");
    try
    {
        // The mapping of the named property happens in transport delivery.
        email.Send();
        if (service.ServerInfo.MajorVersion == 12)
        {
            Console.WriteLine("Provisioned the X-Experimental across the mailbox database that hosts the user's mailbox.");
        }
        else // For versions of Exchange starting with Exchange 2010
        {
            Console.WriteLine("Provisioned the X-Experimental for the user's mailbox. You will need to run this " +
                                "for each mailbox that needs to process this x-header.");
        }
    }
    catch (Exception ex)
    {
        Console.WriteLine("Error: {0}", ex.Message);
    }
}
```

## <a name="provision-an-x-header-by-using-ews"></a>Mettre en service un en-tête x à l’aide de EWS
<a name="bk_example1"> </a>

L’exemple de code suivant montre comment utiliser l’opération EWS [CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) pour créer et envoyer un message électronique pour mettre en service une boîte aux lettres avec un en-tête x. Il s’agit de la demande XML qui est envoyée par l’API managée EWS lorsque vous [mettre en service un en-tête x à l’aide de l’API managée EWS](#bk_example1).
  
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
    <m:CreateItem MessageDisposition="SendOnly">
      <m:Items>
        <t:Message>
          <t:ExtendedProperty>
            <t:ExtendedFieldURI DistinguishedPropertySetId="InternetHeaders"
                                PropertyName="X-Experimental"
                                PropertyType="String" />
            <t:Value>Provision X-Experimental Internet message header</t:Value>
          </t:ExtendedProperty>
          <t:ToRecipients>
            <t:Mailbox>
              <t:EmailAddress>user@contoso.com</t:EmailAddress>
            </t:Mailbox>
          </t:ToRecipients>
        </t:Message>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>

```

## <a name="version-differences"></a>Différences entre les versions
<a name="bk_example1"> </a>

La première fois que vous mettez en service un en-tête x-dans Exchange Online, Exchange Online dans le cadre d’Office 365 ou une version locale d’Exchange commençant par Exchange Server 2010, la valeur d’un nouvel en-tête x personnalisé ne système pas écrites vers le message stocké. Il s’agit, car l’en-tête x-doit tout d’abord être mappé à une propriété nommée dans la boîte aux lettres de l’utilisateur. Le mappage se produit lors de la première demande pour ajouter des propriétés nommées. Lorsqu’une requête suivante pour créer la propriété nommée se produit, la propriété et la valeur sont stockés dans le message. Dans Exchange 2007, la première fois qu'un en-tête x est écrit dans une base de données de boîtes aux lettres, un mappage est créé pour l’en-tête x-pour une propriété nommée dans la base de données de boîtes aux lettres. Lorsqu’une requête suivante pour créer la propriété nommée se produit, l’en-tête x-est traité et stocké pour une boîte aux lettres dans la base de données Exchange 2007.
  
## <a name="next-steps"></a>Étapes suivantes
<a name="bk_example1"> </a>

Cet article vous montre comment mettre en service un en-tête x-pour une seule boîte aux lettres en envoyant un message électronique à un utilisateur. Vous pouvez également prévoir un en-tête x-pour de nombreux utilisateurs en [envoyant un message électronique de traitement par lots à une liste de destinataires](how-to-process-email-messages-in-batches-by-using-ews-in-exchange.md) dans l’organisation de l’appelant. 
  
## <a name="see-also"></a>Voir aussi


- [Les propriétés et les propriétés étendues dans EWS dans Exchange](properties-and-extended-properties-in-ews-in-exchange.md)
    
- [Exchange 2013 : Mettre en service les en-têtes X personnalisés par programme](http://code.msdn.microsoft.com/exchange/Exchange-2013-Provision-d4ef5719)
    
- [Propriétés, les en-têtes X et vous](http://blogs.technet.com/b/exchange/archive/2009/04/06/3407221.aspx)
    
- [Propriétés nommées, arrondi 2 : L’avenir](http://blogs.technet.com/b/exchange/archive/2009/06/12/3407672.aspx)
    
- [Pare-feu d’en-tête](http://technet.microsoft.com/en-us/library/bb232136%28v=exchg.150%29.aspx)
    
- [EWS, MIME et les en-têtes de message Internet manquants](http://msdn.microsoft.com/library/office/hh545614%28v=exchg.140%29.aspx)
    
- [Traiter les messages électroniques par lots à l’aide de EWS dans Exchange](how-to-process-email-messages-in-batches-by-using-ews-in-exchange.md)
    

