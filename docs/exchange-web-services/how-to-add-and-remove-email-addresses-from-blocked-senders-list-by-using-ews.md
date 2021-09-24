---
title: Ajouter et supprimer des adresses de messagerie de la liste des expéditeurs bloqués à l’aide d’EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: b88288ee-6af7-45b5-a55c-5929cd0c16f1
description: Découvrez comment utiliser l’API gérée EWS ou EWS pour ajouter des adresses de messagerie et les supprimer de la liste des expéditeurs bloqués.
ms.openlocfilehash: 4deacbfa6e146675e3248e3932734a1492645246
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59512204"
---
# <a name="add-and-remove-email-addresses-from-the-blocked-senders-list-by-using-ews-in-exchange"></a>Ajouter et supprimer des adresses de messagerie de la liste des expéditeurs bloqués à l’aide d’EWS dans Exchange

Découvrez comment utiliser l’API gérée EWS ou EWS pour ajouter des adresses de messagerie et les supprimer de la liste des expéditeurs bloqués.
  
La liste des expéditeurs bloqués dans les options Courrier indésirable d’un utilisateur permet de déplacer tous les messages électroniques des expéditeurs spécifiés vers le dossier Courrier indésirable. Vous pouvez activer votre API gérée EWS ou votre application EWS pour ajouter des adresses de messagerie à la liste des expéditeurs bloqués ou les supprimer.
  
Notez qu’un message de l’adresse de messagerie doit exister dans la boîte aux lettres de l’utilisateur avant que vous ne pouvez l’ajouter à la liste des expéditeurs bloqués ou la supprimer de celle-ci. La méthode d’API gérée [ExchangeService.MarkAsJunk](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.markasjunk%28v=exchg.80%29.aspx) EWS et l’opération EWS [MarkAsJunk](https://msdn.microsoft.com/library/1f71f04d-56a9-4fee-a4e7-d1034438329e%28Office.15%29.aspx) utilisent une collection d’ID d’élément. Les ID d’élément dans la collection indiquent les messages dans la boîte aux lettres pour lesquels l’état du courrier indésirable doit être modifié. 
  
Vous pouvez utiliser les cmdlets [Get-MailboxJunkEmailConfiguration](https://technet.microsoft.com/library/dd979784%28v=exchg.150%29.aspx) et [Set-MailboxJunkEmailConfiguration](https://technet.microsoft.com/library/dd979780%28v=exchg.150%29.aspx) Exchange Management Shell pour accéder directement à la liste des expéditeurs bloqués. 
  
## <a name="add-an-email-address-to-or-remove-it-from-the-blocked-senders-list-by-using-the-ews-managed-api"></a>Ajouter une adresse e-mail à la liste des expéditeurs bloqués ou la supprimer à l’aide de l’API gérée EWS
<a name="bk_AddRemoveEWSMA"> </a>

Pour ajouter l’expéditeur d’un message électronique à la liste des expéditeurs bloqués, utilisez la méthode **MarkAsJunk** et définissez le **paramètre isJunk** sur **true**. Pour supprimer l’expéditeur d’un message électronique de la liste des expéditeurs bloqués, définissez le **paramètre isJunk** sur **false**.
  
L’exemple suivant montre comment utiliser la **méthode MarkAsJunk** pour modifier le statut de courrier indésirable d’un message. 
  
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

## <a name="add-an-email-address-to-or-remove-it-from-the-blocked-senders-list-by-using-ews"></a>Ajouter une adresse de messagerie à la liste des expéditeurs bloqués ou la supprimer à l’aide d’EWS
<a name="bk_AddRemoveEWS"> </a>

La requête SOAP EWS suivante marque un élément comme indésirable en attribuant la valeur **true** à l’attribut **IsJunk** de l’élément [MarkAsJunk.](https://msdn.microsoft.com/library/f06bafc6-7ee3-4b2b-9fd1-7c51328f4729%28Office.15%29.aspx) Il déplace également le message vers le dossier Courrier indésirable en attribuant la valeur **true** à l’attribut **MoveItem** de l’élément **MarkAsJunk.**
  
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
    <m:MarkAsJunk IsJunk="true" MoveItem="true">
      <m:ItemIds>
        <t:ItemId Id="AAMkADg1OWUwODcyLTg4M2MtNDAyMS05YjI0LTI5ZGM5OTU4Njk3YwBGAAAAAADPriAxh444TpHj2GoQxWQNBwAN+VjmVZl5Rq1ymCq5eFKOAAAAAAENAAAN+VjmVZl5Rq1ymCq5eFKOAAAAAAEuAAA=" 
            ChangeKey="CQAAABYAAAAN+VjmVZl5Rq1ymCq5eFKOAAAAAADi" />
      </m:ItemIds>
    </m:MarkAsJunk>
  </soap:Body>
</soap:Envelope>
```

La réponse SOAP EWS suivante illustre la réponse réussie. [L’élément MovedItemId de](https://msdn.microsoft.com/library/7d5425ab-1e75-43d1-b801-802ff5139df6%28Office.15%29.aspx) la réponse contient l’ID d’élément de l’élément après son déplacer. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="712" MinorBuildNumber="22" Version="V2_3" 
        xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:MarkAsJunkResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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
- [ExchangeService.MarkAsJunk](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.markasjunk%28v=exchg.80%29.aspx)   
- [Opération MarkAsJunk](https://msdn.microsoft.com/library/1f71f04d-56a9-4fee-a4e7-d1034438329e%28Office.15%29.aspx)   
- [Get-MailboxJunkEmailConfiguration](https://technet.microsoft.com/library/dd979784%28v=exchg.150%29.aspx)   
- [Set-MailboxJunkEmailConfiguration](https://technet.microsoft.com/library/dd979780%28v=exchg.150%29.aspx) 
- [Exchange Management Shell](../management/exchange-management-shell.md)
    

