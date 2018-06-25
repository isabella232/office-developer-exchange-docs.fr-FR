---
title: Obtenir les listes de salle à l’aide de EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 15980e4a-e41c-4194-829a-cadbdf365bf1
description: Découvrez comment obtenir une liste de toutes les listes de salle de votre organisation ou d’une liste de salles unique à partir d’un serveur Exchange à l’aide de l’API managée EWS ou EWS.
ms.openlocfilehash: 404a31fb6c8d98bdbba4c79ed6912c333a44d04b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754837"
---
# <a name="get-room-lists-by-using-ews-in-exchange"></a>Obtenir les listes de salle à l’aide de EWS dans Exchange

Découvrez comment obtenir une liste de toutes les listes de salle de votre organisation ou d’une liste de salles unique à partir d’un serveur Exchange à l’aide de l’API managée EWS ou EWS.
  
Vous pouvez utiliser les API managées EWS pour obtenir des informations sur les salles et comment les salles sont regroupés dans votre organisation. Listes d’espace n’existent pas par défaut ; votre administrateur doit créer et organisez-les. En règle générale, elles sont organisées par emplacement ou un département, comme illustré dans l’exemple suivant.
  
**Lister les noms de salle Contoso et les adresses de messagerie**

|**Nom de la liste de salles**|**Adresse de messagerie de la liste de salles**|
|:-----|:-----|
|Création de la liste des salles 11  <br/> |Bldg11rooms@contoso.com  <br/> |
|Liste de salles de conférence d’intégrité Science construction  <br/> |HSbldgrooms@contoso.edu  <br/> |
|Gestion des salles de réunion étage  <br/> |Acctfloor300@contoso.com  <br/> |
   
Chaque salle dans une liste de salles a une nom et adresse e-mail lui est associée.
  
**Les noms de salle de Contoso et les adresses de messagerie**

|**Nom de la salle**|**Adresse de messagerie de salle**|
|:-----|:-----|
|Salle de conférence 11/101 (8) a/v  <br/> |Cf11101@contoso.com  <br/> |
|Laboratoire de démonstration sh (100)  <br/> |Hs101@contoso.edu  <br/> |
|Comptabilité 305 WB  <br/> |Acct305@contoso.com  <br/> |
   
Vous pouvez obtenir une liste qui contient toutes les listes de salle à l’aide de la méthode API managées [ExchangeService.GetRoomLists](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.getroomlists%28v=exchg.80%29.aspx) ou l’opération EWS [GetRoomLists](http://msdn.microsoft.com/library/55d451f9-547f-44ac-872e-9cb220ea7b7c%28Office.15%29.aspx) . 
  
Vous pouvez récupérer une liste de salles unique qui contient toutes les salles pour un emplacement ou un service en fournissant son adresse de messagerie à l’aide de la méthode d’API managées [GetRooms](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.getrooms%28v=exchg.80%29.aspx) ou l’opération EWS [GetRooms](http://msdn.microsoft.com/library/5501ddc0-3bfa-4da6-8e15-4223ca5499a3%28Office.15%29.aspx) . Lorsque vous disposez d’une collection de salles associé à une liste de salles, vous pouvez ensuite rechercher dans la collection pour identifier l’emplacement ou les salles que vous le souhaitez, soit par une adresse de messagerie, soit en recherchant des mots clés dans le nom, tel que « AV » ou « Laboratoire ». 
  
## <a name="get-all-room-lists-by-using-the-ews-managed-api"></a>Obtenir toutes les listes de salle à l’aide de l’API managée EWS
<a name="bk_GetRoomListewsma"> </a>

L’exemple suivant montre comment obtenir une liste qui contient toutes les listes de salle de votre organisation à l’aide de la méthode [GetRoomLists](https://msdn.microsoft.com/library/Microsoft.Exchange.WebServices.Data.ExchangeService.GetRoomLists.aspx) . 
  
Cet exemple suppose que vous ont été authentifiés auprès d'un serveur Exchange et que vous avez acquis un [ExchangeService ](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**. 
  
```cs
// Return all the room lists in the organization.
// This method call results in a GetRoomLists call to EWS.
EmailAddressCollection myRoomLists = service.GetRoomLists();
// Display the room lists.
foreach (EmailAddress address in myRoomLists)
{
    Console.WriteLine("Email Address: {0} Mailbox Type: {1}", address.Address, address.MailboxType);
}

```

## <a name="get-all-room-lists-by-using-ews"></a>Obtenir toutes les listes de salle à l’aide de EWS
<a name="bk_GetRoomListews"> </a>

L’exemple suivant montre comment obtenir une collection de tous les votre organisation [RoomLists](http://msdn.microsoft.com/library/2b190823-b11e-4635-97e4-3aba5865fd05%28Office.15%29.aspx) à l’aide de l’opération [GetRoomLists](http://msdn.microsoft.com/library/55d451f9-547f-44ac-872e-9cb220ea7b7c%28Office.15%29.aspx) . C’est également la demande XML qui envoie de l’API managée EWS lorsque vous utilisez l’API managée EWS pour [obtenir toutes les listes d’espace](#bk_GetRoomListewsma).
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010" />
  </soap:Header>
  <soap:Body>
    <m:GetRoomLists />
  </soap:Body>
</soap:Envelope>

```

Le serveur répond à la demande [GetRoomLists](http://msdn.microsoft.com/library/55d451f9-547f-44ac-872e-9cb220ea7b7c%28Office.15%29.aspx) avec un message [GetRoomListsResponse](http://msdn.microsoft.com/library/8c736f68-1026-496a-b12f-c169c078abd0%28Office.15%29.aspx) qui contient les listes de salle pour votre organisation. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="868" MinorBuildNumber="8" Version="V2_9" 
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetRoomListsResponse ResponseClass="Success" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                            xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseCode>NoError</m:ResponseCode>
      <m:RoomLists>
        <t:Address>
          <t:Name>Contoso Building 1 Room List</t:Name>
          <t:EmailAddress>bldg1rooms@contoso.com</t:EmailAddress>
          <t:RoutingType>SMTP</t:RoutingType>
          <t:MailboxType>PublicDL</t:MailboxType>
        </t:Address>
        <t:Address>
          <t:Name>Contoso Building 2 Room List</t:Name>
          <t:EmailAddress>bldg2rooms@contoso.com</t:EmailAddress>
          <t:RoutingType>SMTP</t:RoutingType>
          <t:MailboxType>PublicDL</t:MailboxType>
        </t:Address>
        <t:Address>
          <t:Name>Contoso Building 3 Room List</t:Name>
          <t:EmailAddress>bldg3rooms@contoso.com</t:EmailAddress>
          <t:RoutingType>SMTP</t:RoutingType>
          <t:MailboxType>PublicDL</t:MailboxType>
        </t:Address>
      </m:RoomLists>
    </m:GetRoomListsResponse>
  </s:Body>
</s:Envelope>

```

## <a name="get-all-the-rooms-in-a-room-list-by-using-the-ews-managed-api"></a>Obtenir toutes les salles dans une liste de salles à l’aide de l’API managée EWS
<a name="bk_FindRoomewsma"> </a>

L’exemple suivant montre comment obtenir une collection de salles dans une liste de salles à l’aide de la méthode [GetRooms](https://msdn.microsoft.com/library/Microsoft.Exchange.WebServices.Data.ExchangeService.GetRooms.aspx) . 
  
```cs
EmailAddress myRoomList = "bldg3rooms@contoso.com";
// This method call results in a GetRooms call to EWS.
System.Collections.ObjectModel.Collection<EmailAddress> myRoomAddresses = service.GetRooms(myRoomList);
// Display the individual rooms.
foreach (EmailAddress address in myRoomAddresses)
{
    Console.WriteLine("Email Address: {0}", address.Address);
}

```

## <a name="get-all-the-rooms-in-a-room-list-by-using-ews"></a>Obtenir toutes les salles dans une liste de salles à l’aide de EWS
<a name="bk_FindRoomews"> </a>

L’exemple suivant montre comment obtenir une liste de [salles](http://msdn.microsoft.com/library/57b6079a-3d83-4429-861e-c551e9e1a991%28Office.15%29.aspx) dans un [RoomList](http://msdn.microsoft.com/library/cb02bdf0-df9f-4e31-b7dd-cd9f2f2cc2b2%28Office.15%29.aspx) à l’aide de l’opération [GetRooms](http://msdn.microsoft.com/library/5501ddc0-3bfa-4da6-8e15-4223ca5499a3%28Office.15%29.aspx) . C’est également la demande XML qui envoie de l’API managée EWS lorsque vous utilisez l’API managée EWS pour [obtenir toutes les salles dans une liste de salles](#bk_FindRoomewsma).
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010" />
  </soap:Header>
  <soap:Body>
    <m:GetRooms>
      <m:RoomList>
        <t:EmailAddress>bldg3rooms@contoso.com</t:EmailAddress>
      </m:RoomList>
    </m:GetRooms>
  </soap:Body>
</soap:Envelope>

```

Le serveur répond à la demande [GetRooms](http://msdn.microsoft.com/library/5501ddc0-3bfa-4da6-8e15-4223ca5499a3%28Office.15%29.aspx) avec un message [GetRoomsResponse](http://msdn.microsoft.com/library/a8c85f65-bb63-4e7a-b0ca-7c9a04560a58%28Office.15%29.aspx) qui contient les salles dans la liste de salles. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="873" MinorBuildNumber="9" 
                         Version="V2_9" xmlns:h="http://scemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetRoomsResponse ResponseClass="Success" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://scemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseCode>NoError</m:ResponseCode>
      <m:Rooms>
        <t:Room>
          <t:Id>
            <t:Name>Conf Room 3/101 (16) AV</t:Name>
            <t:EmailAddress>cf3101@contoso.com</t:EmailAddress>
            <t:RoutingType>SMTP</t:RoutingType>
            <t:MailboxType>Mailbox</t:MailboxType>
          </t:Id>
        </t:Room>
        <t:Room>
          <t:Id>
            <t:Name>Conf Room 3/102 (8) AV</t:Name>
            <t:EmailAddress>cf3102@contoso.com</t:EmailAddress>
            <t:RoutingType>SMTP</t:RoutingType>
            <t:MailboxType>Mailbox</t:MailboxType>
          </t:Id>
        </t:Room>
        <t:Room>
          <t:Id>
            <t:Name>Conf Room 3/103 (14) AV RoundTable</t:Name>
            <t:EmailAddress>cf3103@contoso.com</t:EmailAddress>
            <t:RoutingType>SMTP</t:RoutingType>
            <t:MailboxType>Mailbox</t:MailboxType>
          </t:Id>
        </t:Room>
      </m:Rooms>
    </m:GetRoomsResponse>
  </s:Body>
</s:Envelope>

```

## <a name="see-also"></a>Voir aussi


- [Calendriers et EWS dans Exchange](calendars-and-ews-in-exchange.md)
    
- [Obtenir des informations de disponibilité à l’aide de EWS dans Exchange](how-to-get-free-busy-information-by-using-ews-in-exchange.md)
    
- [Créer et gérer des boîtes aux lettres de salle](http://technet.microsoft.com/en-us/library/jj215781%28v=exchg.150%29.aspx)
    

