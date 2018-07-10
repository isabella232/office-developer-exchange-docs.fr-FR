---
title: Ajouter et supprimer des délégués à l’aide de EWS dans Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: cc7760bf-633b-483a-84ae-b52f437af2d3
description: Découvrez comment ajouter des délégués pour ou supprimer des délégués de boîtes aux lettres des utilisateurs à l’aide de l’API managée EWS ou EWS dans Exchange.
ms.openlocfilehash: d55ef6c5c4e434603d293dbe30c6147ceb73b08b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754796"
---
# <a name="add-and-remove-delegates-by-using-ews-in-exchange"></a><span data-ttu-id="0daef-103">Ajouter et supprimer des délégués à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="0daef-103">Add and remove delegates by using EWS in Exchange</span></span>

<span data-ttu-id="0daef-104">Découvrez comment ajouter des délégués pour ou supprimer des délégués de boîtes aux lettres des utilisateurs à l’aide de l’API managée EWS ou EWS dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="0daef-104">Learn how to add delegates to or remove delegates from users' mailboxes by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="0daef-105">Vous pouvez utiliser les API managées EWS pour permettre aux délégués agir au nom d’un propriétaire de boîte aux lettres ou de supprimer l’accès d’un délégué pour une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="0daef-105">You can use the EWS Managed API or EWS to enable delegates to act on behalf of a mailbox owner or remove a delegate's access to a mailbox.</span></span> <span data-ttu-id="0daef-106">Les utilisateurs qui sont ajoutés en tant que délégué et disposent d’autorisations, peuvent effectuer des tâches pour le compte du propriétaire de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="0daef-106">Users who are added as a delegate, and are given permissions, can perform tasks on behalf of the mailbox owner.</span></span> <span data-ttu-id="0daef-107">Par exemple, ils peuvent créer et envoyer des invitations aux réunions, envoyer des messages électroniques et répondre aux demandes de réunion à part du propriétaire de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="0daef-107">For example, they can create and send meeting invitations, send emails, and respond to meeting requests on the mailbox owner's behalf.</span></span> 
  
<span data-ttu-id="0daef-108">**Le tableau 1. Opérations EWS pour ajouter et supprimer des délégués et les méthodes de l’API managée EWS**</span><span class="sxs-lookup"><span data-stu-id="0daef-108">**Table 1. EWS Managed API methods and EWS operations for adding and removing delegates**</span></span>

|<span data-ttu-id="0daef-109">**Tâche**</span><span class="sxs-lookup"><span data-stu-id="0daef-109">**Task**</span></span>|<span data-ttu-id="0daef-110">**Méthode d'API managée EWS**</span><span class="sxs-lookup"><span data-stu-id="0daef-110">**EWS Managed API method**</span></span>|<span data-ttu-id="0daef-111">**Opération EWS**</span><span class="sxs-lookup"><span data-stu-id="0daef-111">**EWS operation**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="0daef-112">Ajouter des délégués</span><span class="sxs-lookup"><span data-stu-id="0daef-112">Add delegates</span></span>  <br/> |[<span data-ttu-id="0daef-113">ExchangeService.AddDelegates</span><span class="sxs-lookup"><span data-stu-id="0daef-113">ExchangeService.AddDelegates</span></span>](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice.adddelegates%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="0daef-114">AddDelegate</span><span class="sxs-lookup"><span data-stu-id="0daef-114">AddDelegate</span></span>](http://msdn.microsoft.com/library/646fb994-229e-4d90-8b95-6541191cb3ae%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="0daef-115">Supprimer des délégués</span><span class="sxs-lookup"><span data-stu-id="0daef-115">Remove delegates</span></span>  <br/> |[<span data-ttu-id="0daef-116">ExchangeService.RemoveDelegates</span><span class="sxs-lookup"><span data-stu-id="0daef-116">ExchangeService.RemoveDelegates</span></span>](http://msdn.microsoft.com/fr-fr/library/office/microsoft.exchange.webservices.data.exchangeservice.removedelegates%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="0daef-117">RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="0daef-117">RemoveDelegate</span></span>](http://msdn.microsoft.com/library/f21c5171-62e7-47c8-99b1-22e1ff5883bb%28Office.15%29.aspx) <br/> |
   
<span data-ttu-id="0daef-118">Après qu’un délégué dispose d’autorisations sur un dossier, ils peuvent agir sur des éléments dans le dossier et tous les sous-dossiers, en fonction de leur [déléguer les autorisations](delegate-access-and-ews-in-exchange.md#bk_delegateperms).</span><span class="sxs-lookup"><span data-stu-id="0daef-118">After a delegate is granted permissions to a folder, they can act on items in the folder and any subfolders, according to their [delegate permissions](delegate-access-and-ews-in-exchange.md#bk_delegateperms).</span></span> <span data-ttu-id="0daef-119">Autorisations pour les délégués s’appliquent uniquement aux sous-dossiers sont créés après que l’accès délégué a été accordé.</span><span class="sxs-lookup"><span data-stu-id="0daef-119">Permissions for delegates only apply to subfolders that are created after the delegate access was granted.</span></span> <span data-ttu-id="0daef-120">Pour mettre à jour les autorisations du dossier pour les dossiers existants, ou d’autres dossiers, voir [définir des autorisations de dossier pour un autre utilisateur à l’aide de EWS dans Exchange](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="0daef-120">To update folder permissions for pre-existing folders, or other folders, see [Set folder permissions for another user by using EWS in Exchange](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md).</span></span>
  
<span data-ttu-id="0daef-121">Notez que les délégués peuvent être ajoutés uniquement à des comptes à extension boîte aux lettres, y compris les groupes de sécurité à extension messagerie.</span><span class="sxs-lookup"><span data-stu-id="0daef-121">Note that delegates can only be added to mailbox-enabled accounts, including mail-enabled security groups.</span></span> <span data-ttu-id="0daef-122">Par défaut, un seul appel de l’accès délégué EWS peut accéder à un maximum de 255 de boîtes aux lettres.</span><span class="sxs-lookup"><span data-stu-id="0daef-122">By default, a single EWS delegate access call can access a maximum of 255 different mailboxes.</span></span>

<span data-ttu-id="0daef-123"><a name="bk_adddelegateewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="0daef-123"></span></span>

## <a name="add-delegates-by-using-the-ews-managed-api"></a><span data-ttu-id="0daef-124">Ajouter des délégués à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="0daef-124">Add delegates by using the EWS Managed API</span></span>

<span data-ttu-id="0daef-125">Vous pouvez ajouter des délégués à une boîte aux lettres à l’aide de la méthode d’API managées [AddDelegates](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice.adddelegates%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="0daef-125">You can add delegates to a mailbox by using the [AddDelegates](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice.adddelegates%28v=exchg.80%29.aspx) EWS Managed API method.</span></span> <span data-ttu-id="0daef-126">Dans cet exemple, un nouveau calendrier, contacts et messagerie [Utilisateur_délégué](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.delegateuser%28v=exchg.80%29.aspx) est créé, et chaque délégué bénéficie des [autorisations d’éditeur](delegate-access-and-ews-in-exchange.md#bk_delegateperms) pour leur dossier respectif.</span><span class="sxs-lookup"><span data-stu-id="0daef-126">In this example, a new calendar, contact, and email [DelegateUser](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.delegateuser%28v=exchg.80%29.aspx) object is created, and each delegate is given [Editor permissions](delegate-access-and-ews-in-exchange.md#bk_delegateperms) for their respective folder.</span></span> <span data-ttu-id="0daef-127">Vous pouvez modifier l’exemple pour ajouter un délégué à tous les dossiers spécifiés par les [Propriétés DelegatePermissions](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.delegatepermissions_properties%28v=exchg.80%29.aspx), et vous pouvez définir les autorisations à une des valeurs spécifiées par l’énumération [DelegateFolderPermissionLevel](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.delegatefolderpermissionlevel%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="0daef-127">You can modify the example to add a delegate to any of the folders specified by the [DelegatePermissions properties](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.delegatepermissions_properties%28v=exchg.80%29.aspx), and you can set the permissions to any of the values specified by the [DelegateFolderPermissionLevel](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.delegatefolderpermissionlevel%28v=exchg.80%29.aspx) enumeration.</span></span> 
  
<span data-ttu-id="0daef-128">Cet exemple suppose que ce **service** est un objet [ExchangeService](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide pour le propriétaire de boîte aux lettres, et que l’utilisateur a été authentifié sur un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="0daef-128">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object for the mailbox owner, and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
public static Collection<DelegateUserResponse> AddDelegates(ExchangeService service)
{
    // Create a list to hold the new delegates to add.
    List<DelegateUser> newDelegates = new System.Collections.Generic.List<DelegateUser>();
    // Create a new delegate that has editor access to the mailbox owner's Calendar folder.
    DelegateUser calendarDelegate = new DelegateUser("calendardelegate@contoso.com");
    calendarDelegate.Permissions.CalendarFolderPermissionLevel = DelegateFolderPermissionLevel.Editor;
    // Add the delegate to the list of new delegates.
    newDelegates.Add(calendarDelegate);
    // Create a new delegate that has editor access to the mailbox owner's Contacts folder.
    DelegateUser contactDelegate = new DelegateUser("contactdelegate@contoso.com");
    contactDelegate.Permissions.ContactsFolderPermissionLevel = DelegateFolderPermissionLevel.Editor;
    // Add the delegate to the list of new delegates.
    newDelegates.Add(contactDelegate);
            
    // Create a new delegate that has editor access to the mailbox owner's Inbox folder.
    DelegateUser emailDelegate = new DelegateUser("emaildelegate@contoso.com");
    emailDelegate.Permissions.InboxFolderPermissionLevel = DelegateFolderPermissionLevel.Editor;
    // Add the delegate to the list of new delegates.
    newDelegates.Add(emailDelegate);
    // Create a mailbox object that represents the mailbox owner.
    Mailbox mailbox = new Mailbox("primary@contoso.com");
    // Call the AddDelegates method to add the delegates to the target mailbox.
    Collection<DelegateUserResponse> response = service.AddDelegates(mailbox, MeetingRequestsDeliveryScope.DelegatesAndSendInformationToMe, newDelegates);
            
    foreach (DelegateUserResponse resp in response)
    {
        // Print out the result and the last eight characters of the item ID.
        Console.WriteLine("For delegate " + resp.DelegateUser.UserId.PrimarySmtpAddress.ToString());
        Console.WriteLine("Result: {0}", resp.Result);
        Console.WriteLine("Error Code: {0}", resp.ErrorCode);
        Console.WriteLine("ErrorMessage: {0}\r\n", resp.ErrorMessage);
        Console.WriteLine("\r\n");
    }
    return response;
}
```

<span data-ttu-id="0daef-129"><a name="bk_adddelegateews"> </a></span><span class="sxs-lookup"><span data-stu-id="0daef-129"></span></span>

## <a name="add-delegates-by-using-ews"></a><span data-ttu-id="0daef-130">Ajouter des délégués à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="0daef-130">Add delegates by using EWS</span></span>

<span data-ttu-id="0daef-131">L’exemple de code suivant montre comment ajouter des délégués du courrier, contacts et calendrier distinct à l’aide de l’opération EWS [AddDelegate](http://msdn.microsoft.com/library/012d8cc5-648c-4ba0-a155-15c422b1e994%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="0daef-131">The following code example shows how to add separate calendar, contact, and email delegates by using the [AddDelegate](http://msdn.microsoft.com/library/012d8cc5-648c-4ba0-a155-15c422b1e994%28Office.15%29.aspx) EWS operation.</span></span> <span data-ttu-id="0daef-132">La boîte aux lettres à modifier est spécifiée par l’élément de [boîte aux lettres](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) , et les paramètres [d’autorisation](delegate-access-and-ews-in-exchange.md#bk_delegateperms) pour chaque délégué sont contenues dans l’élément [Utilisateur_délégué](http://msdn.microsoft.com/library/aac4e74e-f69b-4c41-a0c9-489610330fbf%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="0daef-132">The mailbox to modify is specified by the [Mailbox](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element, and the [permission](delegate-access-and-ews-in-exchange.md#bk_delegateperms) settings for each delegate are contained in the [DelegateUser](http://msdn.microsoft.com/library/aac4e74e-f69b-4c41-a0c9-489610330fbf%28Office.15%29.aspx) element.</span></span> <span data-ttu-id="0daef-133">Chacun des délégués bénéficie des autorisations d’éditeur à leur dossier cible.</span><span class="sxs-lookup"><span data-stu-id="0daef-133">Each of the delegates has been granted Editor permissions to their target folder.</span></span> 
  
<span data-ttu-id="0daef-134">C’est également la demande XML qui envoie de l’API managée EWS lorsque vous utilisez la méthode **AddDelegates** pour [Ajouter des délégués](#bk_adddelegateewsma).</span><span class="sxs-lookup"><span data-stu-id="0daef-134">This is also the XML request that the EWS Managed API sends when you use the **AddDelegates** method to [add delegates](#bk_adddelegateewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:AddDelegate>
      <m:Mailbox>
        <t:EmailAddress>primary@contoso.com</t:EmailAddress>
      </m:Mailbox>
      <m:DelegateUsers>
        <t:DelegateUser>
          <t:UserId>
            <t:PrimarySmtpAddress>calendardelegate@contoso.com</t:PrimarySmtpAddress>
          </t:UserId>
          <t:DelegatePermissions>
            <t:CalendarFolderPermissionLevel>Editor</t:CalendarFolderPermissionLevel>
            <t:TasksFolderPermissionLevel>None</t:TasksFolderPermissionLevel>
            <t:InboxFolderPermissionLevel>None</t:InboxFolderPermissionLevel>
            <t:ContactsFolderPermissionLevel>None</t:ContactsFolderPermissionLevel>
            <t:NotesFolderPermissionLevel>None</t:NotesFolderPermissionLevel>
            <t:JournalFolderPermissionLevel>None</t:JournalFolderPermissionLevel>
          </t:DelegatePermissions>
          <t:ReceiveCopiesOfMeetingMessages>false</t:ReceiveCopiesOfMeetingMessages>
          <t:ViewPrivateItems>false</t:ViewPrivateItems>
        </t:DelegateUser>
        <t:DelegateUser>
          <t:UserId>
            <t:PrimarySmtpAddress>contactdelegate@contoso.com</t:PrimarySmtpAddress>
          </t:UserId>
          <t:DelegatePermissions>
            <t:CalendarFolderPermissionLevel>None</t:CalendarFolderPermissionLevel>
            <t:TasksFolderPermissionLevel>None</t:TasksFolderPermissionLevel>
            <t:InboxFolderPermissionLevel>None</t:InboxFolderPermissionLevel>
            <t:ContactsFolderPermissionLevel>Editor</t:ContactsFolderPermissionLevel>
            <t:NotesFolderPermissionLevel>None</t:NotesFolderPermissionLevel>
            <t:JournalFolderPermissionLevel>None</t:JournalFolderPermissionLevel>
          </t:DelegatePermissions>
          <t:ReceiveCopiesOfMeetingMessages>false</t:ReceiveCopiesOfMeetingMessages>
          <t:ViewPrivateItems>false</t:ViewPrivateItems>
        </t:DelegateUser>
        <t:DelegateUser>
          <t:UserId>
            <t:PrimarySmtpAddress>emaildelegate@contoso.com</t:PrimarySmtpAddress>
          </t:UserId>
          <t:DelegatePermissions>
            <t:CalendarFolderPermissionLevel>None</t:CalendarFolderPermissionLevel>
            <t:TasksFolderPermissionLevel>None</t:TasksFolderPermissionLevel>
            <t:InboxFolderPermissionLevel>Editor</t:InboxFolderPermissionLevel>
            <t:ContactsFolderPermissionLevel>None</t:ContactsFolderPermissionLevel>
            <t:NotesFolderPermissionLevel>None</t:NotesFolderPermissionLevel>
            <t:JournalFolderPermissionLevel>None</t:JournalFolderPermissionLevel>
          </t:DelegatePermissions>
          <t:ReceiveCopiesOfMeetingMessages>false</t:ReceiveCopiesOfMeetingMessages>
          <t:ViewPrivateItems>false</t:ViewPrivateItems>
        </t:DelegateUser>
      </m:DelegateUsers>
      <m:DeliverMeetingRequests>DelegatesAndSendInformationToMe</m:DeliverMeetingRequests>
    </m:AddDelegate>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="0daef-135">Le serveur répond à la demande **AddDelegate** avec un message [AddDelegateResponse](http://msdn.microsoft.com/library/d7e6bebb-5dbf-43c1-aacf-4b3ca6a7c429%28Office.15%29.aspx) qui contient une valeur élément [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, ce qui indique que les délégués ont été créés.</span><span class="sxs-lookup"><span data-stu-id="0daef-135">The server responds to the **AddDelegate** request with an [AddDelegateResponse](http://msdn.microsoft.com/library/d7e6bebb-5dbf-43c1-aacf-4b3ca6a7c429%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the delegates were successfully created.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="888"
                         MinorBuildNumber="9"
                         Version="V2_10"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:AddDelegateResponse ResponseClass="Success"
                           xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                           xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseCode>NoError</m:ResponseCode>
      <m:ResponseMessages>
        <m:DelegateUserResponseMessageType ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:DelegateUser>
            <t:UserId>
              <t:SID>S-1-5-21-1337771579-694202782-848329751-1535221</t:SID>
              <t:PrimarySmtpAddress>calendardelegate@contoso.com</t:PrimarySmtpAddress>
              <t:DisplayName>calendardelegate</t:DisplayName>
            </t:UserId>
            <t:ReceiveCopiesOfMeetingMessages>false</t:ReceiveCopiesOfMeetingMessages>
            <t:ViewPrivateItems>false</t:ViewPrivateItems>
          </m:DelegateUser>
        </m:DelegateUserResponseMessageType>
        <m:DelegateUserResponseMessageType ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:DelegateUser>
            <t:UserId>
              <t:SID>S-1-5-21-1337771579-694202782-848329751-1535264</t:SID>
              <t:PrimarySmtpAddress>contactdelegate@contoso.com</t:PrimarySmtpAddress>
              <t:DisplayName>contactdelegate</t:DisplayName>
            </t:UserId>
            <t:ReceiveCopiesOfMeetingMessages>false</t:ReceiveCopiesOfMeetingMessages>
            <t:ViewPrivateItems>false</t:ViewPrivateItems>
          </m:DelegateUser>
        </m:DelegateUserResponseMessageType>
        <m:DelegateUserResponseMessageType ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:DelegateUser>
            <t:UserId>
              <t:SID>S-1-5-21-1337771579-694202782-848329751-1535223</t:SID>
              <t:PrimarySmtpAddress>emaildelegate@contoso.com</t:PrimarySmtpAddress>
              <t:DisplayName>emaildelegate</t:DisplayName>
            </t:UserId>
            <t:ReceiveCopiesOfMeetingMessages>false</t:ReceiveCopiesOfMeetingMessages>
            <t:ViewPrivateItems>false</t:ViewPrivateItems>
          </m:DelegateUser>
        </m:DelegateUserResponseMessageType>
      </m:ResponseMessages>
    </m:AddDelegateResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="0daef-136"><a name="bk_removedelegateewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="0daef-136"></span></span>

## <a name="remove-delegates-by-using-the-ews-managed-api"></a><span data-ttu-id="0daef-137">Supprimer des délégués à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="0daef-137">Remove delegates by using the EWS Managed API</span></span>

<span data-ttu-id="0daef-138">Vous pouvez supprimer des délégués à partir d’une boîte aux lettres cible à l’aide de la méthode d’API managées [ExchangeService.RemoveDelegates](http://msdn.microsoft.com/fr-fr/library/office/microsoft.exchange.webservices.data.exchangeservice.removedelegates%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="0daef-138">You can remove delegates from a target mailbox by using the [ExchangeService.RemoveDelegates](http://msdn.microsoft.com/fr-fr/library/office/microsoft.exchange.webservices.data.exchangeservice.removedelegates%28v=exchg.80%29.aspx) EWS Managed API method.</span></span> <span data-ttu-id="0daef-139">Dans cet exemple, le jeu d’autorisations de délégué dans [Ajouter un exemple de délégué](#bk_adddelegateewsma) sont supprimés.</span><span class="sxs-lookup"><span data-stu-id="0daef-139">In this example, the delegate permissions set in the [add a delegate example](#bk_adddelegateewsma) are removed.</span></span> 
  
<span data-ttu-id="0daef-140">Cet exemple suppose que ce **service** est un objet [ExchangeService](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide pour le propriétaire de boîte aux lettres, et que l’utilisateur a été authentifié sur un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="0daef-140">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object for the mailbox owner, and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
public static Collection<DelegateUserResponse> RemoveDelegates(ExchangeService service)
{
    // Create a list to hold the delegates to delete.
    List<UserId> deletedDelegates = new System.Collections.Generic.List<UserId>();
    // Add the delegate to the list of new delegates.
    deletedDelegates.Add("calendardelegate@contoso.com");
    // Add the delegate to the list of new delegates.
    deletedDelegates.Add("contactdelegate@contoso.com");
    // Add the delegate to the list of new delegates.
    deletedDelegates.Add("emaildelegate@contoso.com");
    // Create a mailbox object that represents the mailbox owner.
    Mailbox mailbox = new Mailbox("primary@contoso.com");
    // Call the AddDelegates method to add the delegates to the target mailbox.
    Collection<DelegateUserResponse> response = service.RemoveDelegates(mailbox, deletedDelegates);
    foreach (DelegateUserResponse resp in response)
    {
        // Print out the result and the last eight characters of the item ID.
        Console.WriteLine("Result: {0}", resp.Result);
        Console.WriteLine("Error Code: {0}", resp.ErrorCode);
        Console.WriteLine("ErrorMessage: {0}\r\n", resp.ErrorMessage);
    }
    return response;
}
```

<span data-ttu-id="0daef-141"><a name="bk_removedelegateews"> </a></span><span class="sxs-lookup"><span data-stu-id="0daef-141"></span></span>

## <a name="remove-delegates-by-using-ews"></a><span data-ttu-id="0daef-142">Supprimer des délégués à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="0daef-142">Remove delegates by using EWS</span></span>

<span data-ttu-id="0daef-143">Vous pouvez supprimer des délégués à partir d’une boîte aux lettres à l’aide de l’opération EWS [RemoveDelegate](http://msdn.microsoft.com/library/1d42d5ff-8fde-4f8a-b18d-57b1ef7a946a%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="0daef-143">You can remove delegates from a mailbox by using the [RemoveDelegate](http://msdn.microsoft.com/library/1d42d5ff-8fde-4f8a-b18d-57b1ef7a946a%28Office.15%29.aspx) EWS operation.</span></span> <span data-ttu-id="0daef-144">Dans cet exemple, le jeu d’autorisations de délégué dans [Ajouter un exemple de délégué](#bk_adddelegateews) sont supprimés.</span><span class="sxs-lookup"><span data-stu-id="0daef-144">In this example, the delegate permissions set in the [add a delegate example](#bk_adddelegateews) are removed.</span></span> 
  
<span data-ttu-id="0daef-145">C’est également la demande XML qui envoie de l’API managée EWS lorsque vous utilisez la méthode **RemoveDelegates** permet de [Supprimer des délégués](#bk_removedelegateewsma).</span><span class="sxs-lookup"><span data-stu-id="0daef-145">This is also the XML request that the EWS Managed API sends when you use the **RemoveDelegates** method to [remove delegates](#bk_removedelegateewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:RemoveDelegate>
      <m:Mailbox>
        <t:EmailAddress>primary@contoso.com</t:EmailAddress>
      </m:Mailbox>
      <m:UserIds>
        <t:UserId>
          <t:PrimarySmtpAddress>calendardelegate@contoso.com</t:PrimarySmtpAddress>
        </t:UserId>
        <t:UserId>
          <t:PrimarySmtpAddress>contactdelegate@contoso.com</t:PrimarySmtpAddress>
        </t:UserId>
        <t:UserId>
          <t:PrimarySmtpAddress>emaildelegate@contoso.com</t:PrimarySmtpAddress>
        </t:UserId>
      </m:UserIds>
    </m:RemoveDelegate>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="0daef-146">Le serveur répond à la demande **RemoveDelegate** avec un message [AddDelegateResponse](http://msdn.microsoft.com/library/d7e6bebb-5dbf-43c1-aacf-4b3ca6a7c429%28Office.15%29.aspx) qui contient une valeur élément [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, ce qui indique que les délégués ont été supprimés.</span><span class="sxs-lookup"><span data-stu-id="0daef-146">The server responds to the **RemoveDelegate** request with a [AddDelegateResponse](http://msdn.microsoft.com/library/d7e6bebb-5dbf-43c1-aacf-4b3ca6a7c429%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the delegates were successfully removed.</span></span>

<span data-ttu-id="0daef-147"><a name="bk_nextsteps"> </a></span><span class="sxs-lookup"><span data-stu-id="0daef-147"></span></span>

## <a name="next-steps"></a><span data-ttu-id="0daef-148">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="0daef-148">Next steps</span></span>

<span data-ttu-id="0daef-149">Après avoir ajouté les délégués calendrier, messagerie et des dossiers de tâches, le délégué peut accéder aux éléments dans les dossiers.</span><span class="sxs-lookup"><span data-stu-id="0daef-149">After you add delegates to calendar, email, and task folders, the delegate can access the items in the folders.</span></span> <span data-ttu-id="0daef-150">Pour plus d’informations, voir les articles suivants :</span><span class="sxs-lookup"><span data-stu-id="0daef-150">To learn more, see the following articles:</span></span>
  
- [<span data-ttu-id="0daef-151">Accéder à la messagerie en tant que délégué à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="0daef-151">Access email as a delegate by using EWS in Exchange</span></span>](how-to-access-email-as-a-delegate-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="0daef-152">Accéder à un calendrier en tant que délégué à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="0daef-152">Access a calendar as a delegate by using EWS in Exchange</span></span>](how-to-access-a-calendar-as-a-delegate-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="0daef-153">Contacts Access en tant que délégué à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="0daef-153">Access contacts as a delegate by using EWS in Exchange</span></span>](how-to-access-contacts-as-a-delegate-by-using-ews-in-exchange.md)
    
<span data-ttu-id="0daef-154">Si les dossiers pour lesquels vous avez ajouté les délégués sont les dossiers enfants qui ont été créées avant que vous avez accordé l’accès délégué, le délégué ne sera pas en mesure d’accéder à ces dossiers sans autorisations supplémentaires.</span><span class="sxs-lookup"><span data-stu-id="0daef-154">If the folders for which you added delegates include child folders that were created before you granted the delegate access, the delegate will not be able to access those folders without additional permissions.</span></span> <span data-ttu-id="0daef-155">Pour ajouter ces autorisations, ou modifier les autorisations pour tous les autres dossiers, voir [définir des autorisations de dossier pour un autre utilisateur à l’aide de EWS dans Exchange](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="0daef-155">To add these permissions, or modify permissions for any other folders, see [Set folder permissions for another user by using EWS in Exchange](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="0daef-156">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="0daef-156">See also</span></span>

- [<span data-ttu-id="0daef-157">Accès délégué et EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="0daef-157">Delegate access and EWS in Exchange</span></span>](delegate-access-and-ews-in-exchange.md)
- [<span data-ttu-id="0daef-158">Exchange 2013 : Ajouter déléguer aux utilisateurs d’un compte de messagerie par programme</span><span class="sxs-lookup"><span data-stu-id="0daef-158">Exchange 2013: Add delegate users to an email account programmatically</span></span>](http://code.msdn.microsoft.com/exchange/Exchange-2013-Adding-1024511f)   
- [<span data-ttu-id="0daef-159">Exchange 2013 : Mettre à jour les délégués associés par programme des comptes de messagerie</span><span class="sxs-lookup"><span data-stu-id="0daef-159">Exchange 2013: Update delegates associated with email accounts programmatically</span></span>](http://code.msdn.microsoft.com/exchange/Exchange-2013-Update-b40d3bac)   
- [<span data-ttu-id="0daef-160">Exchange 2013 : Supprimer des délégués associés par programme des comptes de messagerie</span><span class="sxs-lookup"><span data-stu-id="0daef-160">Exchange 2013: Remove delegates associated with email accounts programmatically</span></span>](http://code.msdn.microsoft.com/exchange/Exchange-2013-Remove-686f7714)
    

