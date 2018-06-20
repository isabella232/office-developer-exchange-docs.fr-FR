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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19754837"
---
# <a name="get-room-lists-by-using-ews-in-exchange"></a><span data-ttu-id="64898-103">Obtenir les listes de salle à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="64898-103">Get room lists by using EWS in Exchange</span></span>

<span data-ttu-id="64898-104">Découvrez comment obtenir une liste de toutes les listes de salle de votre organisation ou d’une liste de salles unique à partir d’un serveur Exchange à l’aide de l’API managée EWS ou EWS.</span><span class="sxs-lookup"><span data-stu-id="64898-104">Learn how to get a list of all the room lists in your organization or a single room list from an Exchange server by using the EWS Managed API or EWS.</span></span>
  
<span data-ttu-id="64898-105">Vous pouvez utiliser les API managées EWS pour obtenir des informations sur les salles et comment les salles sont regroupés dans votre organisation.</span><span class="sxs-lookup"><span data-stu-id="64898-105">You can use the EWS Managed API or EWS to get information about rooms and how the rooms are grouped in your organization.</span></span> <span data-ttu-id="64898-106">Listes d’espace n’existent pas par défaut ; votre administrateur doit créer et organisez-les.</span><span class="sxs-lookup"><span data-stu-id="64898-106">Room lists don't exist by default; your administrator needs to create and organize them.</span></span> <span data-ttu-id="64898-107">En règle générale, elles sont organisées par emplacement ou un département, comme illustré dans l’exemple suivant.</span><span class="sxs-lookup"><span data-stu-id="64898-107">Typically, they're organized by location or department, as shown in the following example.</span></span>
  
<span data-ttu-id="64898-108">**Lister les noms de salle Contoso et les adresses de messagerie**</span><span class="sxs-lookup"><span data-stu-id="64898-108">**Contoso room list names and email addresses**</span></span>

|<span data-ttu-id="64898-109">**Nom de la liste de salles**</span><span class="sxs-lookup"><span data-stu-id="64898-109">**Name of room list**</span></span>|<span data-ttu-id="64898-110">**Adresse de messagerie de la liste de salles**</span><span class="sxs-lookup"><span data-stu-id="64898-110">**Email address of room list**</span></span>|
|:-----|:-----|
|<span data-ttu-id="64898-111">Création de la liste des salles 11</span><span class="sxs-lookup"><span data-stu-id="64898-111">Building 11 room list</span></span>  <br/> |<span data-ttu-id="64898-112">Bldg11rooms@contoso.com</span><span class="sxs-lookup"><span data-stu-id="64898-112">Bldg11rooms@contoso.com</span></span>  <br/> |
|<span data-ttu-id="64898-113">Liste de salles de conférence d’intégrité Science construction</span><span class="sxs-lookup"><span data-stu-id="64898-113">Health Science Building Conference Room List</span></span>  <br/> |<span data-ttu-id="64898-114">HSbldgrooms@contoso.edu</span><span class="sxs-lookup"><span data-stu-id="64898-114">HSbldgrooms@contoso.edu</span></span>  <br/> |
|<span data-ttu-id="64898-115">Gestion des salles de réunion étage</span><span class="sxs-lookup"><span data-stu-id="64898-115">Accounting Floor Meeting Rooms</span></span>  <br/> |<span data-ttu-id="64898-116">Acctfloor300@contoso.com</span><span class="sxs-lookup"><span data-stu-id="64898-116">Acctfloor300@contoso.com</span></span>  <br/> |
   
<span data-ttu-id="64898-117">Chaque salle dans une liste de salles a une nom et adresse e-mail lui est associée.</span><span class="sxs-lookup"><span data-stu-id="64898-117">Each room in a room list has a name and email address associated with it.</span></span>
  
<span data-ttu-id="64898-118">**Les noms de salle de Contoso et les adresses de messagerie**</span><span class="sxs-lookup"><span data-stu-id="64898-118">**Contoso room names and email addresses**</span></span>

|<span data-ttu-id="64898-119">**Nom de la salle**</span><span class="sxs-lookup"><span data-stu-id="64898-119">**Name of room**</span></span>|<span data-ttu-id="64898-120">**Adresse de messagerie de salle**</span><span class="sxs-lookup"><span data-stu-id="64898-120">**Email address of room**</span></span>|
|:-----|:-----|
|<span data-ttu-id="64898-121">Salle de conférence 11/101 (8) a/v</span><span class="sxs-lookup"><span data-stu-id="64898-121">Conf Room 11/101 (8) AV</span></span>  <br/> |<span data-ttu-id="64898-122">Cf11101@contoso.com</span><span class="sxs-lookup"><span data-stu-id="64898-122">Cf11101@contoso.com</span></span>  <br/> |
|<span data-ttu-id="64898-123">Laboratoire de démonstration sh (100)</span><span class="sxs-lookup"><span data-stu-id="64898-123">HS Demonstration Lab (100)</span></span>  <br/> |<span data-ttu-id="64898-124">Hs101@contoso.edu</span><span class="sxs-lookup"><span data-stu-id="64898-124">Hs101@contoso.edu</span></span>  <br/> |
|<span data-ttu-id="64898-125">Comptabilité 305 WB</span><span class="sxs-lookup"><span data-stu-id="64898-125">Accounting 305 WB</span></span>  <br/> |<span data-ttu-id="64898-126">Acct305@contoso.com</span><span class="sxs-lookup"><span data-stu-id="64898-126">Acct305@contoso.com</span></span>  <br/> |
   
<span data-ttu-id="64898-127">Vous pouvez obtenir une liste qui contient toutes les listes de salle à l’aide de la méthode API managées [ExchangeService.GetRoomLists](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.getroomlists%28v=exchg.80%29.aspx) ou l’opération EWS [GetRoomLists](http://msdn.microsoft.com/library/55d451f9-547f-44ac-872e-9cb220ea7b7c%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="64898-127">You can get a list that contains all room lists by using either the [ExchangeService.GetRoomLists](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.getroomlists%28v=exchg.80%29.aspx) EWS Managed API method or the [GetRoomLists](http://msdn.microsoft.com/library/55d451f9-547f-44ac-872e-9cb220ea7b7c%28Office.15%29.aspx) EWS operation.</span></span> 
  
<span data-ttu-id="64898-128">Vous pouvez récupérer une liste de salles unique qui contient toutes les salles pour un emplacement ou un service en fournissant son adresse de messagerie à l’aide de la méthode d’API managées [GetRooms](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.getrooms%28v=exchg.80%29.aspx) ou l’opération EWS [GetRooms](http://msdn.microsoft.com/library/5501ddc0-3bfa-4da6-8e15-4223ca5499a3%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="64898-128">You can retrieve a single room list that contains all the rooms for a location or department by supplying its email address by using the [GetRooms](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.getrooms%28v=exchg.80%29.aspx) EWS Managed API method or the [GetRooms](http://msdn.microsoft.com/library/5501ddc0-3bfa-4da6-8e15-4223ca5499a3%28Office.15%29.aspx) EWS operation.</span></span> <span data-ttu-id="64898-129">Lorsque vous disposez d’une collection de salles associé à une liste de salles, vous pouvez ensuite rechercher dans la collection pour identifier l’emplacement ou les salles que vous le souhaitez, soit par une adresse de messagerie, soit en recherchant des mots clés dans le nom, tel que « AV » ou « Laboratoire ».</span><span class="sxs-lookup"><span data-stu-id="64898-129">When you have a collection of rooms associated with a room list, you can then search through the collection to identify the room or rooms you want, either by email address, or by looking for key words in the name, such as "AV", or "Lab".</span></span> 
  
## <a name="get-all-room-lists-by-using-the-ews-managed-api"></a><span data-ttu-id="64898-130">Obtenir toutes les listes de salle à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="64898-130">Get all room lists by using the EWS Managed API</span></span>
<span data-ttu-id="64898-131"><a name="bk_GetRoomListewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="64898-131"></span></span>

<span data-ttu-id="64898-132">L’exemple suivant montre comment obtenir une liste qui contient toutes les listes de salle de votre organisation à l’aide de la méthode [GetRoomLists](https://msdn.microsoft.com/library/Microsoft.Exchange.WebServices.Data.ExchangeService.GetRoomLists.aspx) .</span><span class="sxs-lookup"><span data-stu-id="64898-132">The following example shows how to get a list that contains all the room lists in your organization by using the [GetRoomLists](https://msdn.microsoft.com/library/Microsoft.Exchange.WebServices.Data.ExchangeService.GetRoomLists.aspx) method.</span></span> 
  
<span data-ttu-id="64898-133">Cet exemple suppose que vous ont été authentifiés auprès d'un serveur Exchange et que vous avez acquis un [ExchangeService ](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span><span class="sxs-lookup"><span data-stu-id="64898-133">This example assumes that you have authenticated to an Exchange server and have acquired an [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span></span> 
  
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

## <a name="get-all-room-lists-by-using-ews"></a><span data-ttu-id="64898-134">Obtenir toutes les listes de salle à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="64898-134">Get all room lists by using EWS</span></span>
<span data-ttu-id="64898-135"><a name="bk_GetRoomListews"> </a></span><span class="sxs-lookup"><span data-stu-id="64898-135"></span></span>

<span data-ttu-id="64898-136">L’exemple suivant montre comment obtenir une collection de tous les votre organisation [RoomLists](http://msdn.microsoft.com/library/2b190823-b11e-4635-97e4-3aba5865fd05%28Office.15%29.aspx) à l’aide de l’opération [GetRoomLists](http://msdn.microsoft.com/library/55d451f9-547f-44ac-872e-9cb220ea7b7c%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="64898-136">The following example shows how to get a collection of all your organization's [RoomLists](http://msdn.microsoft.com/library/2b190823-b11e-4635-97e4-3aba5865fd05%28Office.15%29.aspx) by using the [GetRoomLists](http://msdn.microsoft.com/library/55d451f9-547f-44ac-872e-9cb220ea7b7c%28Office.15%29.aspx) operation.</span></span> <span data-ttu-id="64898-137">C’est également la demande XML qui envoie de l’API managée EWS lorsque vous utilisez l’API managée EWS pour [obtenir toutes les listes d’espace](#bk_GetRoomListewsma).</span><span class="sxs-lookup"><span data-stu-id="64898-137">This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [get all room lists](#bk_GetRoomListewsma).</span></span>
  
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

<span data-ttu-id="64898-138">Le serveur répond à la demande [GetRoomLists](http://msdn.microsoft.com/library/55d451f9-547f-44ac-872e-9cb220ea7b7c%28Office.15%29.aspx) avec un message [GetRoomListsResponse](http://msdn.microsoft.com/library/8c736f68-1026-496a-b12f-c169c078abd0%28Office.15%29.aspx) qui contient les listes de salle pour votre organisation.</span><span class="sxs-lookup"><span data-stu-id="64898-138">The server responds to the [GetRoomLists](http://msdn.microsoft.com/library/55d451f9-547f-44ac-872e-9cb220ea7b7c%28Office.15%29.aspx) request with a [GetRoomListsResponse](http://msdn.microsoft.com/library/8c736f68-1026-496a-b12f-c169c078abd0%28Office.15%29.aspx) message that contains the room lists for your organization.</span></span> 
  
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

## <a name="get-all-the-rooms-in-a-room-list-by-using-the-ews-managed-api"></a><span data-ttu-id="64898-139">Obtenir toutes les salles dans une liste de salles à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="64898-139">Get all the rooms in a room list by using the EWS Managed API</span></span>
<span data-ttu-id="64898-140"><a name="bk_FindRoomewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="64898-140"></span></span>

<span data-ttu-id="64898-141">L’exemple suivant montre comment obtenir une collection de salles dans une liste de salles à l’aide de la méthode [GetRooms](https://msdn.microsoft.com/library/Microsoft.Exchange.WebServices.Data.ExchangeService.GetRooms.aspx) .</span><span class="sxs-lookup"><span data-stu-id="64898-141">The following example shows how to get a collection of rooms in a room list by using the [GetRooms](https://msdn.microsoft.com/library/Microsoft.Exchange.WebServices.Data.ExchangeService.GetRooms.aspx) method.</span></span> 
  
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

## <a name="get-all-the-rooms-in-a-room-list-by-using-ews"></a><span data-ttu-id="64898-142">Obtenir toutes les salles dans une liste de salles à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="64898-142">Get all the rooms in a room list by using EWS</span></span>
<span data-ttu-id="64898-143"><a name="bk_FindRoomews"> </a></span><span class="sxs-lookup"><span data-stu-id="64898-143"></span></span>

<span data-ttu-id="64898-144">L’exemple suivant montre comment obtenir une liste de [salles](http://msdn.microsoft.com/library/57b6079a-3d83-4429-861e-c551e9e1a991%28Office.15%29.aspx) dans un [RoomList](http://msdn.microsoft.com/library/cb02bdf0-df9f-4e31-b7dd-cd9f2f2cc2b2%28Office.15%29.aspx) à l’aide de l’opération [GetRooms](http://msdn.microsoft.com/library/5501ddc0-3bfa-4da6-8e15-4223ca5499a3%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="64898-144">The following example shows how to get a list of [rooms](http://msdn.microsoft.com/library/57b6079a-3d83-4429-861e-c551e9e1a991%28Office.15%29.aspx) in a [RoomList](http://msdn.microsoft.com/library/cb02bdf0-df9f-4e31-b7dd-cd9f2f2cc2b2%28Office.15%29.aspx) by using the [GetRooms](http://msdn.microsoft.com/library/5501ddc0-3bfa-4da6-8e15-4223ca5499a3%28Office.15%29.aspx) operation.</span></span> <span data-ttu-id="64898-145">C’est également la demande XML qui envoie de l’API managée EWS lorsque vous utilisez l’API managée EWS pour [obtenir toutes les salles dans une liste de salles](#bk_FindRoomewsma).</span><span class="sxs-lookup"><span data-stu-id="64898-145">This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [get all the rooms in a room list](#bk_FindRoomewsma).</span></span>
  
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

<span data-ttu-id="64898-146">Le serveur répond à la demande [GetRooms](http://msdn.microsoft.com/library/5501ddc0-3bfa-4da6-8e15-4223ca5499a3%28Office.15%29.aspx) avec un message [GetRoomsResponse](http://msdn.microsoft.com/library/a8c85f65-bb63-4e7a-b0ca-7c9a04560a58%28Office.15%29.aspx) qui contient les salles dans la liste de salles.</span><span class="sxs-lookup"><span data-stu-id="64898-146">The server responds to the [GetRooms](http://msdn.microsoft.com/library/5501ddc0-3bfa-4da6-8e15-4223ca5499a3%28Office.15%29.aspx) request with a [GetRoomsResponse](http://msdn.microsoft.com/library/a8c85f65-bb63-4e7a-b0ca-7c9a04560a58%28Office.15%29.aspx) message that contains the rooms in the room list.</span></span> 
  
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

## <a name="see-also"></a><span data-ttu-id="64898-147">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="64898-147">See also</span></span>


- [<span data-ttu-id="64898-148">Calendriers et EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="64898-148">Calendars and EWS in Exchange</span></span>](calendars-and-ews-in-exchange.md)
    
- [<span data-ttu-id="64898-149">Obtenir des informations de disponibilité à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="64898-149">Get free/busy information by using EWS in Exchange</span></span>](how-to-get-free-busy-information-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="64898-150">Créer et gérer des boîtes aux lettres de salle</span><span class="sxs-lookup"><span data-stu-id="64898-150">Create and Manage Room Mailboxes</span></span>](http://technet.microsoft.com/en-us/library/jj215781%28v=exchg.150%29.aspx)
    

