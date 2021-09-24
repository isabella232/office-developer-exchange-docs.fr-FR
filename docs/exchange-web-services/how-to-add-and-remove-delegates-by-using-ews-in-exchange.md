---
title: Ajouter et supprimer des délégués à l’aide d’EWS dans Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: cc7760bf-633b-483a-84ae-b52f437af2d3
description: Découvrez comment ajouter ou supprimer des délégués des boîtes aux lettres des utilisateurs à l’aide de l’API gérée EWS ou d’EWS dans Exchange.
ms.openlocfilehash: 67370360e24da55b7a908d0a34b7ac1ec949877d
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59520205"
---
# <a name="add-and-remove-delegates-by-using-ews-in-exchange"></a>Ajouter et supprimer des délégués à l’aide d’EWS dans Exchange

Découvrez comment ajouter ou supprimer des délégués des boîtes aux lettres des utilisateurs à l’aide de l’API gérée EWS ou d’EWS dans Exchange.
  
Vous pouvez utiliser l’API gérée EWS ou EWS pour permettre aux délégués d’agir au nom d’un propriétaire de boîte aux lettres ou de supprimer l’accès d’un délégué à une boîte aux lettres. Les utilisateurs qui sont ajoutés en tant que délégués et qui ont reçu des autorisations peuvent effectuer des tâches au nom du propriétaire de la boîte aux lettres. Par exemple, ils peuvent créer et envoyer des invitations à une réunion, envoyer des courriers électroniques et répondre aux demandes de réunion au nom du propriétaire de la boîte aux lettres. 
  
**Tableau 1. Méthodes d’API gérées EWS et opérations EWS pour l’ajout et la suppression de délégués**

|**Tâche**|**Méthode d'API managée EWS**|**Opération EWS**|
|:-----|:-----|:-----|
|Ajouter des délégués  <br/> |[ExchangeService.AddDelegates](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.adddelegates%28v=exchg.80%29.aspx) <br/> |[AddDelegate](https://msdn.microsoft.com/library/646fb994-229e-4d90-8b95-6541191cb3ae%28Office.15%29.aspx) <br/> |
|Supprimer des délégués  <br/> |[ExchangeService.RemoveDelegates](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.removedelegates%28v=exchg.80%29.aspx) <br/> |[RemoveDelegate](https://msdn.microsoft.com/library/f21c5171-62e7-47c8-99b1-22e1ff5883bb%28Office.15%29.aspx) <br/> |
   
Une fois qu’un délégué a reçu des autorisations sur un dossier, il peut agir sur les éléments du dossier et tous les sous-dossiers, en fonction de leurs [autorisations de délégué.](delegate-access-and-ews-in-exchange.md#bk_delegateperms) Les autorisations pour les délégués s’appliquent uniquement aux sous-foldeurs créés après l’octroi de l’accès délégué. Pour mettre à jour les autorisations de dossier pour les dossiers pré-existants ou d’autres dossiers, voir Définir les autorisations de dossier pour un autre utilisateur à l’aide [d’EWS dans Exchange](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md).
  
Notez que les délégués ne peuvent être ajoutés qu’aux comptes à boîte aux lettres, y compris aux groupes de sécurité à messagerie. Par défaut, un seul appel d’accès délégué EWS peut accéder à un maximum de 255 boîtes aux lettres différentes.

<a name="bk_adddelegateewsma"> </a>

## <a name="add-delegates-by-using-the-ews-managed-api"></a>Ajouter des délégués à l’aide de l’API gérée EWS

Vous pouvez ajouter des délégués à une boîte aux lettres à l’aide de la méthode d’API gérée EWS [AddDelegates.](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.adddelegates%28v=exchg.80%29.aspx) Dans cet exemple, un nouvel objet [DelegateUser](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.delegateuser%28v=exchg.80%29.aspx) de calendrier, de contact et de messagerie est créé, et chaque délégué se vu donner des [autorisations](delegate-access-and-ews-in-exchange.md#bk_delegateperms) d’éditeur pour son dossier respectif. Vous pouvez modifier l’exemple pour ajouter un délégué à l’un des dossiers spécifiés par les [propriétés DelegatePermissions](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.delegatepermissions_properties%28v=exchg.80%29.aspx)et vous pouvez définir les autorisations sur n’importe quelle valeur spécifiée par l’éumération [DelegateFolderPermissionLevel.](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.delegatefolderpermissionlevel%28v=exchg.80%29.aspx) 
  
Cet exemple suppose que **le service** est un objet [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide pour le propriétaire de la boîte aux lettres et que l’utilisateur a été authentifié sur Exchange serveur. 
  
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

<a name="bk_adddelegateews"> </a>

## <a name="add-delegates-by-using-ews"></a>Ajouter des délégués à l’aide d’EWS

L’exemple de code suivant montre comment ajouter des délégués de calendrier, de contact et de messagerie distincts à l’aide de l’opération [AddDelegate](https://msdn.microsoft.com/library/012d8cc5-648c-4ba0-a155-15c422b1e994%28Office.15%29.aspx) EWS. La boîte aux lettres à modifier est [](delegate-access-and-ews-in-exchange.md#bk_delegateperms) spécifiée par l’élément [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) et les paramètres d’autorisation pour chaque délégué sont contenus dans l’élément [DelegateUser.](https://msdn.microsoft.com/library/aac4e74e-f69b-4c41-a0c9-489610330fbf%28Office.15%29.aspx) Chacun des délégués a reçu des autorisations d’éditeur sur son dossier cible. 
  
Il s’agit également de la demande XML que l’API gérée EWS envoie lorsque vous utilisez la méthode **AddDelegates** pour ajouter [des délégués.](#bk_adddelegateewsma)
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

Le serveur répond à la demande **AddDelegate** avec un message [AddDelegateResponse](https://msdn.microsoft.com/library/d7e6bebb-5dbf-43c1-aacf-4b3ca6a7c429%28Office.15%29.aspx) qui inclut une valeur d’élément [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NoError**, qui indique que les délégués ont été créés avec succès.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="888"
                         MinorBuildNumber="9"
                         Version="V2_10"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:AddDelegateResponse ResponseClass="Success"
                           xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                           xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

<a name="bk_removedelegateewsma"> </a>

## <a name="remove-delegates-by-using-the-ews-managed-api"></a>Supprimer des délégués à l’aide de l’API gérée EWS

Vous pouvez supprimer des délégués d’une boîte aux lettres cible à l’aide de la méthode d’API gérée EWS [ExchangeService.RemoveDelegates.](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.removedelegates%28v=exchg.80%29.aspx) Dans cet exemple, les autorisations [](#bk_adddelegateewsma) de délégué définies dans l’exemple Ajouter un délégué sont supprimées. 
  
Cet exemple suppose que **le service** est un objet [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide pour le propriétaire de la boîte aux lettres et que l’utilisateur a été authentifié sur Exchange serveur. 
  
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

<a name="bk_removedelegateews"> </a>

## <a name="remove-delegates-by-using-ews"></a>Supprimer des délégués à l’aide d’EWS

Vous pouvez supprimer des délégués d’une boîte aux lettres à l’aide de [l’opération RemoveDelegate](https://msdn.microsoft.com/library/1d42d5ff-8fde-4f8a-b18d-57b1ef7a946a%28Office.15%29.aspx) EWS. Dans cet exemple, les autorisations [](#bk_adddelegateews) de délégué définies dans l’exemple Ajouter un délégué sont supprimées. 
  
Il s’agit également de la demande XML que l’API gérée EWS envoie lorsque vous utilisez la **méthode RemoveDelegates** pour supprimer [des délégués.](#bk_removedelegateewsma)
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

Le serveur répond à la demande **RemoveDelegate** avec un message [AddDelegateResponse](https://msdn.microsoft.com/library/d7e6bebb-5dbf-43c1-aacf-4b3ca6a7c429%28Office.15%29.aspx) qui inclut une valeur d’élément [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NoError**, qui indique que les délégués ont été supprimés avec succès.

<a name="bk_nextsteps"> </a>

## <a name="next-steps"></a>Étapes suivantes

Une fois que vous avez ajouté des délégués à des dossiers de calendrier, de courrier électronique et de tâche, le délégué peut accéder aux éléments des dossiers. Pour en savoir plus, consultez les articles suivants :
  
- [Accéder à la messagerie en tant que délégué à l’aide d’EWS dans Exchange](how-to-access-email-as-a-delegate-by-using-ews-in-exchange.md)
    
- [Accéder à un calendrier en tant que délégué à l’aide d’EWS dans Exchange](how-to-access-a-calendar-as-a-delegate-by-using-ews-in-exchange.md)
    
- [Accéder aux contacts en tant que délégué à l’aide d’EWS dans Exchange](how-to-access-contacts-as-a-delegate-by-using-ews-in-exchange.md)
    
Si les dossiers pour lesquels vous avez ajouté des délégués incluent des dossiers enfants qui ont été créés avant que vous n’accordiez l’accès délégué, le délégué ne pourra pas accéder à ces dossiers sans autorisations supplémentaires. Pour ajouter ces autorisations ou modifier des autorisations pour d’autres dossiers, voir Définir les autorisations de dossier pour un autre utilisateur à l’aide [d’EWS dans Exchange](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md).
  
## <a name="see-also"></a>Voir aussi

- [Accès délégué et EWS dans Exchange](delegate-access-and-ews-in-exchange.md)
- [Exchange 2013 : Ajouter des utilisateurs délégués à un compte de messagerie par programme](https://code.msdn.microsoft.com/exchange/Exchange-2013-Adding-1024511f)   
- [Exchange 2013 : Mise à jour des délégués associés aux comptes de messagerie par programme](https://code.msdn.microsoft.com/exchange/Exchange-2013-Update-b40d3bac)   
- [Exchange 2013 : Suppression des délégués associés à des comptes de messagerie par programme](https://code.msdn.microsoft.com/exchange/Exchange-2013-Remove-686f7714)
    

