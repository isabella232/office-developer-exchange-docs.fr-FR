---
title: Mise en service des en-têtes x à l’aide d’EWS Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 45a99a14-a85f-47f8-af48-18eb6c6cc230
description: Découvrez comment mettre en service des en-têtes x pour une boîte aux lettres à l’aide de l’API gérée EWS ou d’EWS dans Exchange.
ms.openlocfilehash: e60092e0d40d5815cdf3fd4ed588e2f74978c245
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521115"
---
# <a name="provision-x-headers-by-using-ews-in-exchange"></a>Mise en service des en-têtes x à l’aide d’EWS Exchange

Découvrez comment mettre en service des en-têtes x pour une boîte aux lettres à l’aide de l’API gérée EWS ou d’EWS dans Exchange.
  
Les en-têtes X sont des en-têtes non standard qui sont ajoutés à la collection d’en-têtes d’un e-mail pour communiquer des informations. Par exemple, Exchange les messages avec **l’en-tête X-MS-Exchange-Organization-SCL** pour indiquer le niveau de confiance du courrier indésirable (SCL) attribué à l’e-mail. Les clients de messagerie tels que Outlook peuvent utiliser ces informations pour déterminer le type d’action à prendre sur le courrier électronique (par exemple, Outlook peut empêcher l’affichage des images, sauf si l’utilisateur prend une action). 
  
Exchange ajoute des en-têtes x entrants au schéma de boîte aux lettres en tant que propriété nommée la première fois qu’il reçoit un message électronique avec cet en-tête x. La valeur d’en-tête x n’est pas enregistrée sur ce premier e-mail . toutefois, il est enregistré sur tous les messages électroniques suivants qui incluent l’en-tête x. Pour cette raison, votre application doit mettre en service des en-têtes x avant de les utiliser. Le mappage entre une propriété nommée et un en-tête x se produit lors de la remise du courrier électronique à la boîte aux lettres. Cela signifie que vous devez recevoir le courrier électronique via la remise du transport ; vous ne pouvez pas simplement enregistrer un message électronique qui inclut l’en-tête x dans une boîte aux lettres pour créer le mappage sur une propriété nommée.
  
> [!NOTE]
> Si vous constatez que les en-têtes x ne sont [](https://technet.microsoft.com/library/bb232136%28v=exchg.150%29.aspx) pas enregistrés, déterminez si un agent de [transport](https://code.msdn.microsoft.com/Exchange-2013-Build-an-32f62f5a) ou un pare-feu d’en-tête filtre vos en-têtes x avant qu’ils n’entrent dans la boîte aux lettres. r
  
## <a name="provision-an-x-header-by-using-the-ews-managed-api"></a>Mise en service d’un en-tête x à l’aide de l’API gérée EWS
<a name="bk_example1"> </a>

L’exemple de code suivant montre comment utiliser la méthode [EmailMessage.Send](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.send%28v=exchg.80%29.aspx) de l’API gérée EWS pour mettre en service un en-tête x pour une boîte aux lettres. Cet exemple suppose que **le service** est un objet [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que la boîte aux lettres cible n’a pas dépassé le [quota pour les propriétés nommées](https://technet.microsoft.com/library/bb851492%28v=EXCHG.80%29.aspx).
  
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

## <a name="provision-an-x-header-by-using-ews"></a>Mise en service d’un en-tête x à l’aide d’EWS
<a name="bk_example1"> </a>

L’exemple de code suivant montre comment utiliser l’opération [CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS pour créer et envoyer un message électronique afin de mettre en service une boîte aux lettres avec un en-tête x. Il s’agit de la demande XML envoyée par l’API gérée EWS lorsque vous provisionniez un en-tête x à l’aide de [l’API gérée EWS.](#bk_example1)
  
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

Lors de la première mise en service d’un en-tête x dans Exchange Online, Exchange Online dans le cadre de Office 365 ou d’une version locale de Exchange à partir de Exchange Server 2010, la valeur d’un nouvel en-tête x personnalisé ne sera pas écrite dans le message stocké. Cela est dû au fait que l’en-tête x doit d’abord être mappé à une propriété nommée dans la boîte aux lettres de l’utilisateur. Le mappage se produit lors de la première demande d’ajout des propriétés nommées. Lorsqu’une demande ultérieure de création de la propriété nommée se produit, la propriété et la valeur sont stockées dans le message. Dans Exchange 2007, la première fois qu’un en-tête x est écrit dans une base de données de boîtes aux lettres, un mappage est créé pour l’en-tête x sur une propriété nommée dans la base de données de boîtes aux lettres. Lorsqu’une demande ultérieure de création de la propriété nommée se produit, l’en-tête x est traitée et stockée pour n’importe quelle boîte aux lettres dans la base de données Exchange 2007.
  
## <a name="next-steps"></a>Étapes suivantes
<a name="bk_example1"> </a>

Cet article vous montre comment mettre en service un en-tête x pour une seule boîte aux lettres en envoyant un message électronique à un utilisateur. Vous pouvez également mettre en service un en-tête x pour de nombreux utilisateurs en envoyant un courrier électronique par lot à une liste de [destinataires](how-to-process-email-messages-in-batches-by-using-ews-in-exchange.md) dans l’organisation de l’appelant. 
  
## <a name="see-also"></a>Voir aussi


- [Les propriétés et les propriétés étendues dans EWS dans Exchange](properties-and-extended-properties-in-ews-in-exchange.md)
    
- [Exchange 2013 : Mise en service d’en-têtes X personnalisés par programme](https://code.msdn.microsoft.com/exchange/Exchange-2013-Provision-d4ef5719)
    
- [Propriétés nommées, en-têtes X et vous](https://blogs.technet.com/b/exchange/archive/2009/04/06/3407221.aspx)
    
- [Propriétés nommées, série 2 : ce qui se trouve devant](https://blogs.technet.com/b/exchange/archive/2009/06/12/3407672.aspx)
    
- [Pare-feu d’en-tête](https://technet.microsoft.com/library/bb232136%28v=exchg.150%29.aspx)
    
- [EWS, MIME et en-têtes de message Internet manquants](https://msdn.microsoft.com/library/office/hh545614%28v=exchg.140%29.aspx)
    
- [Traiter les messages électroniques par lots à l’aide d’EWS Exchange](how-to-process-email-messages-in-batches-by-using-ews-in-exchange.md)
    

