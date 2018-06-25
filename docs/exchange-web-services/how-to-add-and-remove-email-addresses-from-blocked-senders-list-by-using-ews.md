---
title: Ajouter et supprimer des adresses de messagerie à partir de la liste des expéditeurs bloqués à l’aide de EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: b88288ee-6af7-45b5-a55c-5929cd0c16f1
description: Découvrez comment utiliser les API managées EWS pour ajouter des adresses de messagerie et les supprimer de la liste des expéditeurs bloqués.
ms.openlocfilehash: c03ed585ebd62802000179d8c837786ba5f9aab4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754783"
---
# <a name="add-and-remove-email-addresses-from-the-blocked-senders-list-by-using-ews-in-exchange"></a>Ajouter et supprimer des adresses de messagerie à partir de la liste des expéditeurs bloqués à l’aide de EWS dans Exchange

Découvrez comment utiliser les API managées EWS pour ajouter des adresses de messagerie et les supprimer de la liste des expéditeurs bloqués.
  
La liste des expéditeurs bloqués dans options du courrier indésirable d’un utilisateur fournit un moyen pour déplacer tous les messages électroniques provenant d’expéditeurs spécifiés vers le dossier courrier indésirable. Vous pouvez activer votre API managées ou les applications EWS ajouter des adresses de messagerie ou de les supprimer de la liste des expéditeurs bloqués.
  
Notez qu’un message à partir de l’adresse de messagerie doit exister dans la boîte aux lettres de l’utilisateur avant de pouvoir ajouter l’adresse de messagerie ou supprimer de la liste des expéditeurs bloqués. La méthode [ExchangeService.MarkAsJunk](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.markasjunk%28v=exchg.80%29.aspx) API managées et l’opération EWS [MarkAsJunk](http://msdn.microsoft.com/library/1f71f04d-56a9-4fee-a4e7-d1034438329e%28Office.15%29.aspx) utilisent une collection d’ID d’élément. L’élément ID dans la collection indiquent des messages dans la boîte aux lettres pour laquelle l’état de courrier indésirable doit être modifiée. 
  
Vous pouvez utiliser les applets de commande [Get-MailboxJunkEmailConfiguration](http://technet.microsoft.com/en-us/library/dd979784%28v=exchg.150%29.aspx) et [Set-MailboxJunkEmailConfiguration](http://technet.microsoft.com/en-us/library/dd979780%28v=exchg.150%29.aspx) Exchange Management Shell pour accéder directement à la liste des expéditeurs bloqués. 
  
## <a name="add-an-email-address-to-or-remove-it-from-the-blocked-senders-list-by-using-the-ews-managed-api"></a>Ajouter une adresse de messagerie ou le supprimer de la liste des expéditeurs bloqués à l’aide de l’API managée EWS
<a name="bk_AddRemoveEWSMA"> </a>

Pour ajouter l’expéditeur d’un message électronique à la liste des expéditeurs bloqués, utilisez la méthode **MarkAsJunk** et définissez le paramètre **isJunk** sur **true**. Pour supprimer l’expéditeur d’un message électronique à partir de la liste des expéditeurs bloqués, définissez le paramètre **isJunk** sur **false**.
  
L’exemple suivant montre comment utiliser la méthode **MarkAsJunk** pour modifier l’état d’un message de courrier indésirable. 
  
```cs
private static void MarkMessageAsJunk(ExchangeService service, ItemId messageId, bool isJunk, bool moveItem)
{
    List<ItemId> junkItemIds = new List<ItemId>();
    junkItemIds.Add(messageId);
    ServiceResponseCollection<MarkAsJunkResponse> responseCollection = null;
    try
    {
        // If isJunk is true, the sender of the email message is added to 
        // the Blocked Senders List. If isJunk is false, the sender is removed
        // from the list (if present).
        responseCollection = service.MarkAsJunk(junkItemIds, isJunk, moveItem);
    }
    catch (ServiceResponseException ex)
    {
        Console.WriteLine("Error marking item as junk: {0}", ex.ErrorCode);
        return;
    }
    foreach (MarkAsJunkResponse response in responseCollection)
    {
        if (response.Result == ServiceResult.Success)
        {
            Console.WriteLine("Successfully marked message as {0}junk.", isJunk ? "": "NOT ");
            if (moveItem)
            {
                Console.WriteLine("New item ID: {0}", response.MovedItemId.ToString());
            }
        }
        else
        {
            Console.WriteLine("[{0}]: {1}", response.Result.ToString(),
                response.ErrorCode.ToString());
        }
    }
}
```

## <a name="add-an-email-address-to-or-remove-it-from-the-blocked-senders-list-by-using-ews"></a>Ajouter une adresse de messagerie ou le supprimer de la liste des expéditeurs bloqués à l’aide de EWS
<a name="bk_AddRemoveEWS"> </a>

La demande SOAP EWS suivante marque un élément comme courrier indésirable en définissant l’attribut **IsJunk** sur l’élément [MarkAsJunk](http://msdn.microsoft.com/library/f06bafc6-7ee3-4b2b-9fd1-7c51328f4729%28Office.15%29.aspx) la **valeur true**. Il déplace également le message vers le dossier courrier indésirable en définissant l’attribut **MoveItem** sur l’élément **MarkAsJunk** la **valeur true**.
  
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
    <m:MarkAsJunk IsJunk="true" MoveItem="true">
      <m:ItemIds>
        <t:ItemId Id="AAMkADg1OWUwODcyLTg4M2MtNDAyMS05YjI0LTI5ZGM5OTU4Njk3YwBGAAAAAADPriAxh444TpHj2GoQxWQNBwAN+VjmVZl5Rq1ymCq5eFKOAAAAAAENAAAN+VjmVZl5Rq1ymCq5eFKOAAAAAAEuAAA=" 
            ChangeKey="CQAAABYAAAAN+VjmVZl5Rq1ymCq5eFKOAAAAAADi" />
      </m:ItemIds>
    </m:MarkAsJunk>
  </soap:Body>
</soap:Envelope>
```

La réponse SOAP EWS suivante montre la réponse correcte. L’élément [MovedItemId](http://msdn.microsoft.com/library/7d5425ab-1e75-43d1-b801-802ff5139df6%28Office.15%29.aspx) dans la réponse contient l’ID d’élément de l’élément après que qu’il a été déplacé. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="712" MinorBuildNumber="22" Version="V2_3" 
        xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:MarkAsJunkResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:MarkAsJunkResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:MovedItemId Id="AAMkADg1OWUwODcyLTg4M2MtNDAyMS05YjI0LTI5ZGM5OTU4Njk3YwBGAAAAAADPriAxh444TpHj2GoQxWQNBwAN+VjmVZl5Rq1ymCq5eFKOAAAAAAEbAAAN+VjmVZl5Rq1ymCq5eFKOAAAE59DIAAA="
              ChangeKey="CQAAABYAAAAN+VjmVZl5Rq1ymCq5eFKOAAAE59E+" />
        </m:MarkAsJunkResponseMessage>
      </m:ResponseMessages>
    </m:MarkAsJunkResponse>
  </s:Body>
</s:Envelope>
```

## <a name="see-also"></a>Voir aussi

- [Gestion de la boîte de réception et EWS dans Exchange](inbox-management-and-ews-in-exchange.md)   
- [ExchangeService.MarkAsJunk](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.markasjunk%28v=exchg.80%29.aspx)   
- [Opération MarkAsJunk](http://msdn.microsoft.com/library/1f71f04d-56a9-4fee-a4e7-d1034438329e%28Office.15%29.aspx)   
- [Get-MailboxJunkEmailConfiguration](http://technet.microsoft.com/en-us/library/dd979784%28v=exchg.150%29.aspx)   
- [Set-MailboxJunkEmailConfiguration](http://technet.microsoft.com/en-us/library/dd979780%28v=exchg.150%29.aspx) 
- [Exchange Management Shell](../management/exchange-management-shell.md)
    

