---
title: Mise en service des en-têtes x à l’aide d’EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 45a99a14-a85f-47f8-af48-18eb6c6cc230
description: Découvrez comment mettre en service des en-têtes x pour une boîte aux lettres à l’aide de l’API managée EWS ou EWS dans Exchange.
ms.openlocfilehash: 409ddb944bbac7a60242de39cdf7ae13b17cc76a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527767"
---
# <a name="provision-x-headers-by-using-ews-in-exchange"></a>Mise en service des en-têtes x à l’aide d’EWS dans Exchange

Découvrez comment mettre en service des en-têtes x pour une boîte aux lettres à l’aide de l’API managée EWS ou EWS dans Exchange.
  
Les en-têtes X sont des en-têtes non standard ajoutés à la collection d’en-têtes d’un message électronique pour communiquer des informations. Par exemple, Exchange marque les messages à l’aide de l’en-tête **X-MS-Exchange-Organization-SCL** pour indiquer le seuil de probabilité de courrier indésirable (SCL) attribué au courrier électronique. Les clients de messagerie comme Outlook peuvent utiliser ces informations pour déterminer le type d’action à effectuer sur le courrier électronique (par exemple, Outlook peut empêcher les images de s’afficher sauf si l’utilisateur effectue une action). 
  
Exchange ajoute des en-têtes x entrants au schéma de boîte aux lettres en tant que propriété nommée la première fois qu’il reçoit un message électronique avec cet en-tête x. La valeur de l’en-tête x n’est pas enregistrée dans le premier message électronique ; Toutefois, il est enregistré sur tous les messages électroniques suivants qui incluent l’en-tête x. Pour cette raison, votre application doit mettre en service les en-têtes x avant de les utiliser. Le mappage entre une propriété nommée et un en-tête x se produit dans la remise du courrier électronique à la boîte aux lettres. Cela signifie que vous devez recevoir le courrier électronique via la remise du transport ; vous ne pouvez pas simplement enregistrer un message électronique qui inclut l’en-tête x dans une boîte aux lettres pour créer le mappage à une propriété nommée.
  
> [!NOTE]
> Si vous constatez que les en-têtes x ne sont pas enregistrés, déterminez si un [agent de transport](https://code.msdn.microsoft.com/Exchange-2013-Build-an-32f62f5a) ou un [pare-feu d’en-tête](https://technet.microsoft.com/library/bb232136%28v=exchg.150%29.aspx) filtre les en-têtes x avant qu’ils accèdent à la boîte aux lettres. r
  
## <a name="provision-an-x-header-by-using-the-ews-managed-api"></a>Approvisionner un en-tête x à l’aide de l’API managée EWS
<a name="bk_example1"> </a>

L’exemple de code suivant montre comment utiliser la méthode [EmailMessage. Send](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.send%28v=exchg.80%29.aspx) de l’API managée EWS pour mettre en service un en-tête x pour une boîte aux lettres. Cet exemple part du principe que le **service** est un objet [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que la boîte aux lettres cible n’a pas dépassé le [quota pour les propriétés nommées](https://technet.microsoft.com/library/bb851492%28v=EXCHG.80%29.aspx).
  
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

## <a name="provision-an-x-header-by-using-ews"></a>Approvisionner un en-tête x à l’aide d’EWS
<a name="bk_example1"> </a>

L’exemple de code suivant montre comment utiliser l’opération [CREATEITEM](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS pour créer et envoyer un message électronique pour approvisionner une boîte aux lettres avec un en-tête x. Il s’agit de la requête XML envoyée par l’API managée EWS lorsque vous configurez [un en-tête x à l’aide de l’API managée EWS](#bk_example1).
  
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

La première fois que vous approvisionnez un en-tête x dans Exchange Online, Exchange Online dans le cadre d’Office 365 ou d’une version locale d’Exchange à partir d’Exchange Server 2010, la valeur d’un nouvel en-tête x personnalisé n’est pas écrite dans le message stocké. Cela est dû au fait que l’en-tête x doit d’abord être mappé à une propriété nommée dans la boîte aux lettres de l’utilisateur. Le mappage se produit lors de la première demande d’ajout des propriétés nommées. Lorsqu’une demande ultérieure de création de la propriété nommée se produit, la propriété et la valeur sont stockées dans le message. Dans Exchange 2007, la première fois qu’un en-tête x est écrit dans une base de données de boîtes aux lettres, un mappage est créé pour l’en-tête x vers une propriété nommée dans la base de données de boîtes aux lettres. Lorsqu’une demande ultérieure de création de la propriété nommée se produit, l’en-tête x est traité et stocké pour toutes les boîtes aux lettres de la base de données Exchange 2007.
  
## <a name="next-steps"></a>Étapes suivantes
<a name="bk_example1"> </a>

Cet article vous explique comment mettre en service un en-tête x pour une seule boîte aux lettres en envoyant un message électronique à un utilisateur. Vous pouvez également configurer un en-tête x pour de nombreux utilisateurs en [envoyant un message électronique à une liste de destinataires](how-to-process-email-messages-in-batches-by-using-ews-in-exchange.md) dans l’organisation de l’appelant. 
  
## <a name="see-also"></a>Voir aussi


- [Les propriétés et les propriétés étendues dans EWS dans Exchange](properties-and-extended-properties-in-ews-in-exchange.md)
    
- [Exchange 2013 : mise en service des en-têtes X personnalisés par programme](https://code.msdn.microsoft.com/exchange/Exchange-2013-Provision-d4ef5719)
    
- [Propriétés nommées, en-têtes X et vous](https://blogs.technet.com/b/exchange/archive/2009/04/06/3407221.aspx)
    
- [Propriétés nommées, rond 2 : ce qui est en avance](https://blogs.technet.com/b/exchange/archive/2009/06/12/3407672.aspx)
    
- [Pare-feu d’en-tête](https://technet.microsoft.com/library/bb232136%28v=exchg.150%29.aspx)
    
- [EWS, MIME et les en-têtes de message Internet manquants](https://msdn.microsoft.com/library/office/hh545614%28v=exchg.140%29.aspx)
    
- [Traiter les messages électroniques par lots à l’aide d’EWS dans Exchange](how-to-process-email-messages-in-batches-by-using-ews-in-exchange.md)
    

