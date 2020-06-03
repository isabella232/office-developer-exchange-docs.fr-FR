---
title: Accès délégué et EWS dans Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.assetid: 240d1776-7adc-46cd-9099-88ffeba0a8aa
description: Découvrez comment utiliser l’API managée EWS et EWS dans Exchange pour fournir un accès délégué aux boîtes aux lettres des utilisateurs.
localization_priority: Priority
ms.openlocfilehash: 4223d625213a3f71726ec5b8d3f09f9e2e7e7e51
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528453"
---
# <a name="delegate-access-and-ews-in-exchange"></a>Accès délégué et EWS dans Exchange

Découvrez comment utiliser l’API managée EWS et EWS dans Exchange pour fournir un accès délégué aux boîtes aux lettres des utilisateurs.
  
Vous pouvez permettre à des utilisateurs d'accéder aux boîtes aux lettres d'autres utilisateurs de trois façons : 
  
- En ajoutant des délégués et en spécifiant des autorisations pour chacun d’entre eux.
    
- En modifiant directement les autorisations du dossier.
    
- En utilisant l’emprunt d’identité.
    
La délégation et les autorisations de dossier conviennent mieux si vous souhaitez accorder l'accès uniquement à certains utilisateurs, car vous devez ajouter les autorisations individuellement pour chaque boîte aux lettres. L’emprunt d’identité est le meilleur choix lorsque vous avez affaire à des quantités de boîtes aux lettres, car vous pouvez facilement activer un compte de service pour accéder à chaque boîte aux lettres dans une base de données. La Figure 1 présente quelques-unes des différences entre chaque type d'accès.
  
**Figure 1. Méthodes d'accès aux boîtes aux lettres des autres utilisateurs**

![Diagramme montrant les types d’accès à la boîte aux lettres, la relation entre les propriétaires de boîtes aux lettres et le délégué pour chaque type, ainsi que le type d’autorisation. Autorisations « Envoyer pour le compte de » pour les autorisations de dossier et/ou délégation. Autorisations « Envoyer en tant que » pour l’emprunt d’identité.](media/Ex15_Delegate_Overview.png)
  
Lorsqu’il s’agit d’envoyer ou de planifier des réunions, les délégués peuvent recevoir des autorisations « Envoyer de la part de », de sorte que le destinataire d’un courrier électronique ou d’une demande de réunion envoyé par un délégué verra « *délégué* de la part du propriétaire de la *boîte aux lettres* » lorsqu’il recevra la demande de réunion ou de messagerie dans Outlook. Y compris le texte « envoyer de la part de » est un détail d’implémentation cliente qui peut être créé à l’aide des valeurs « de » et « expéditeur ». La valeur « de » indique le propriétaire de la boîte aux lettres, et la valeur « sender » indique le délégué qui a envoyé le message. Si un compte de service qui emprunte l’identité d’un utilisateur envoie un message électronique ou planifie une réunion pour le propriétaire de la boîte aux lettres, le message est « envoyé en tant que » le propriétaire de la boîte aux lettres. Il n'existe aucun moyen pour le destinataire de savoir que le message a été envoyé par le compte de service. Les utilisateurs disposant des autorisations de dossier et non de l’accès délégué ne sont pas en mesure de « envoyer en tant que » ou « envoyer de la part de » d’un propriétaire de boîte aux lettres. Ils ont accès aux dossiers de boîte aux lettres et peuvent être en mesure de créer des éléments dans les dossiers, mais ils ne peuvent pas envoyer les éléments. 
  
Quand est-il approprié de modifier directement les autorisations de dossier ? En règle générale, lorsque vous souhaitez fournir à un utilisateur l’accès à un dossier, mais ne pas accorder à l’utilisateur les autorisations « Envoyer de la part de », lorsque vos autorisations requises ne correspondent pas aux valeurs d’énumération de l’API managée EWS [DelegateFolderPermissionLevel](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.delegatefolderpermissionlevel%28v=exchg.80%29.aspx) ou aux valeurs de l’élément [permissionLevel](https://msdn.microsoft.com/library/87978600-3523-451e-a725-ef092c543e2a%28Office.15%29.aspx) EWS, ou lorsque vous souhaitez fournir à un utilisateur l’accès à un seul dossier personnalisé. 
  
Si vous avez uniquement besoin de modifier les autorisations de dossier pour atteindre votre objectif, et que vous n’avez pas besoin d’ajouter un délégué (autrement dit, vous n’avez pas besoin des autorisations « Envoyer de la part de »), consultez la rubrique [définir les autorisations de dossier pour un autre utilisateur à l’aide d’EWS dans Exchange](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md). 

Notez que vous pouvez également utiliser [Outlook](https://office.microsoft.com/outlook-help/allow-someone-else-to-manage-your-mail-and-calendar-HA102749417.aspx) ou [Exchange Server PowerShell (Exchange Management Shell)](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps) pour configurer l’accès délégué. 

  
## <a name="how-does-delegate-access-work"></a>Comment fonctionne l’accès délégué ?

L’accès délégué permet aux utilisateurs d’accéder à tout ou partie des dossiers du propriétaire de la boîte aux lettres et d’agir au nom du propriétaire de la boîte aux lettres. Le propriétaire de la boîte aux lettres peut être un utilisateur ou une ressource, comme une salle de conférence. Par exemple, un réceptionniste peut recevoir des autorisations déléguées pour le dossier calendrier d’une salle de conférence, afin de gérer les demandes de réservation. Vous pouvez utiliser l’API managée EWS ou EWS pour autoriser le propriétaire de la boîte aux lettres ou un administrateur à ajouter un délégué, à spécifier les dossiers auxquels le délégué peut accéder, puis à spécifier les autorisations pour ce dossier. Les délégués peuvent être autorisés à accéder aux dossiers suivants : 
  
- Calendrier
    
- Tâches
    
- Boîte de réception
    
- Contacts
    
- Notes
    
- Journal
    
Lorsqu’un utilisateur dispose d’un accès délégué à un ou plusieurs de ces dossiers, il peut créer, obtenir, mettre à jour, supprimer, copier et Rechercher des éléments de ce dossier et de tous les dossiers enfants, en fonction des [autorisations](#bk_delegateperms) définies sur le dossier. La manière dont l’application effectue ces actions varie selon que l’accès [explicite](#bk_explicit) ou [implicite](#bk_implicit) est requis. 
  
## <a name="delegate-permissions"></a>Déléguer des autorisations
<a name="bk_delegateperms"> </a>

Lorsqu’un administrateur ou un propriétaire de boîte aux lettres ajoute un délégué à une boîte aux lettres, il peut également définir le niveau d’autorisation pour un ou plusieurs dossiers. Si aucun niveau d’autorisation n’est défini pour un dossier, la valeur d’autorisation est définie par défaut sur aucun. Plusieurs utilisateurs peuvent avoir le même niveau d’autorisation sur un dossier, et les utilisateurs peuvent avoir différents niveaux d’autorisation pour différents dossiers. Si vous utilisez l’API managée EWS, vous utilisez la propriété [DelegateUser. Permissions](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.delegateuser.permissions%28v=exchg.80%29.aspx) , qui contient l’une des valeurs d’énumération [DelegateFolderPermissionLevel](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.delegatefolderpermissionlevel%28v=exchg.80%29.aspx) pour chaque dossier, pour définir des autorisations de délégué sur les dossiers. Si vous utilisez EWS, vous utilisez l’élément [DelegatePermissions](https://msdn.microsoft.com/library/292badc7-bab3-4368-9d7c-9a8b7edb279b%28Office.15%29.aspx) pour définir des autorisations de délégué et l’élément [permissionLevel](https://msdn.microsoft.com/library/87978600-3523-451e-a725-ef092c543e2a%28Office.15%29.aspx) pour définir le niveau d’autorisation. 
  
**Tableau 2. Niveaux d’autorisation de délégué**

|**Niveau d’autorisation**|**Description**|
|:-----|:-----|
|Aucune  <br/> |Il s’agit de la valeur par défaut de tous les dossiers.  <br/> |
|Auteur  <br/> |Un délégué peut lire et créer des éléments, et modifier et supprimer des éléments qu’ils créent. Par exemple, un délégué peut créer des demandes de tâches et des demandes de réunion directement dans le dossier de tâches ou de calendrier du propriétaire de la boîte aux lettres, puis envoyer l’un ou l’autre élément du nom du propriétaire de la boîte aux lettres.  <br/> |
|Éditeur  <br/> |Un délégué peut effectuer tout ce qu’un auteur peut faire, et également modifier et supprimer les éléments créés par le propriétaire de la boîte aux lettres.  <br/> |
|Relecteur  <br/> |Un délégué peut lire des éléments ; par exemple, un délégué avec l’autorisation relecteur peut lire les messages de la boîte de réception d’une autre personne.  <br/> |
|Personnalisé  <br/> |Le propriétaire de la boîte aux lettres a accordé un ensemble personnalisé d’autorisations au délégué.  <br/> |
   
La propriété de l’API managée EWS [DelgateUser. ViewPrivateItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.delegateuser.viewprivateitems%28v=exchg.80%29.aspx) et l’élément [ViewPrivateItems](https://msdn.microsoft.com/library/80b949ac-440c-4a01-b428-ebafb5b1b802%28Office.15%29.aspx) EWS sont un paramètre global qui affecte tous les dossiers du propriétaire de la boîte aux lettres, y compris tous les dossiers courrier, contacts, calendrier, tâches, notes et journal. Vous ne pouvez pas autoriser l’accès aux éléments privés dans un seul dossier. 
  
## <a name="explicit-access"></a>Accès explicite
<a name="bk_explicit"> </a>

En d’autres termes, l’accès explicite est le moyen pour les délégués d’effectuer des actions sur les dossiers ou les éléments d’un propriétaire de boîte aux lettres. L’accès explicite est accordé à un délégué lorsqu’il inclut le nom de dossier connu du dossier d’un propriétaire de boîte aux lettres, ainsi que l’adresse SMTP du propriétaire de la boîte aux lettres dans une demande adressée au serveur. L’accès est explicite car la demande du délégué indique explicitement que le contexte de la méthode ou de l’opération est la boîte aux lettres du propriétaire de la boîte aux lettres, et non la boîte aux lettres du délégué.
  
L’accès explicite définit le contexte de toutes les méthodes ou opérations effectuées sur les dossiers ou les éléments qui déplacent vers l’avant. Tous les ID d’élément et de dossier renvoyés lorsque l’accès explicite est défini de manière unique comme appartenant au propriétaire de la boîte aux lettres (mais pas au format lisible par l’utilisateur). De cette manière, l’application n’a pas besoin de spécifier à nouveau l’adresse SMTP du propriétaire de la boîte aux lettres ; le contexte est masqué dans les identificateurs. Une fois qu’un élément ou un dossier est identifié, un délégué utilise l' [accès implicite](#bk_implicit) pour modifier l’élément. La figure suivante illustre le processus d’accès explicite et implicite. 
  
**Figure 2. Demande d’accès explicite et implicite à un élément ou dossier**

![Diagramme qui illustre l’application envoyant une demande d’accès explicite, une réponse du serveur, puis d’une demande d’accès implicite et une réponse du serveur.](media/Ex15_Delegate_ExplictImplicit.png)
  
Vous pouvez définir un accès explicite dans de nombreux scénarios différents. En gros, chaque fois que vous envoyez un ID de dossier dans une méthode ou une opération, vous pouvez définir un accès explicite. Il peut s’agir notamment de trouver des dossiers, de trouver des rendez-vous, d’obtenir des éléments, de trouver des conversations, etc.
  
### <a name="explicit-access-and-the-ews-managed-api"></a>Accès explicite et API managée EWS
<a name="bk_explicitewsma"> </a>

Vous pouvez lancer un accès délégué explicite à l’aide de l’une des méthodes surchargées suivantes qui prennent un paramètre d’entrée [FolderId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) pour identifier le dossier cible : 
  
- [Folder. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx)
    
- [ExchangeService. FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)
    
- [ExchangeService. Findappointmentspour](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx)
    
- [ExchangeService. FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx)
    
- Et bien plus encore !
    
Vous pouvez utiliser le paramètre **FolderId** dans chacune de ces méthodes pour identifier le dossier cible du propriétaire de la boîte aux lettres, comme suit. 
  
```cs
new FolderId(WellKnownFolderName.Calendar, "primary@contoso.com");
```

Par exemple, pour établir une liaison avec le dossier de calendrier, le **FolderId** dans cette méthode de **liaison** spécifie le nom de dossier connu et l’adresse SMTP du propriétaire de la boîte aux lettres. 
  
```cs
CalendarFolder calendar = CalendarFolder.Bind(service, new FolderId(WellKnownFolderName.Calendar, "primary@contoso.com"), new PropertySet());
```

En spécifiant le nom de dossier connu et l’adresse SMTP, le délégué peut établir une liaison avec le dossier de calendrier du propriétaire de la boîte aux lettres, ce qui permet un accès explicite au dossier. Toutes les demandes ultérieures d' [accès implicite](#bk_implicit) aux éléments du dossier dépendent du contexte renvoyé dans les ID d’élément et les ID de dossier. Les identificateurs contiennent essentiellement le contexte pour les appels d’accès délégué implicite. Pour récupérer l’ID d’un élément qui répond à des critères spécifiques, procédez comme suit. 
  
```cs
FindItemsResults<Item> results = service.FindItems(new FolderId(WellKnownFolderName.Calendar, "primary@contoso.com"), filter, view);
```

Dans ce cas, l’ID d’élément est renvoyé, puis le délégué peut ensuite utiliser l’accès implicite pour modifier l’élément à l’aide de l’ID d’élément.
  
Il n’est pas nécessaire de lancer à nouveau un accès explicite tant que vous n’avez pas besoin d’un ID d’élément ou d’un ID de dossier que vous n’avez pas accessible via l’accès explicite existant. 
  
### <a name="explicit-access-and-ews"></a>Accès explicite et EWS
<a name="bk_explicitewsma"> </a>

Vous pouvez lancer un accès explicite à l’aide des opérations [GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx), [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)ou [FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) . Ces opérations offrent la possibilité d’utiliser l’élément [DistinguishedFolderId](https://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) pour identifier le dossier cible. L’élément **DistinguishedFolderId** possède un seul élément enfant facultatif, l’élément [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) . L’élément **Mailbox** , lorsqu’il est utilisé en tant qu’enfant de l’élément **DistinguishedFolderId** , spécifie la boîte aux lettres pour laquelle le délégué accède. Si l’utilisateur appelant est autorisé à accéder au dossier du propriétaire de la boîte aux lettres, la réponse contiendra une collection d’identificateurs vers des éléments ou des dossiers de cette boîte aux lettres. Les identificateurs d’élément et de dossier qui sont renvoyés dans la réponse peuvent être utilisés pour l’accès délégué implicite. 
  
## <a name="implicit-access"></a>Accès implicite
<a name="bk_implicit"> </a>

L’accès implicite est utilisé après qu’un délégué a récupéré l’ID d’un élément ou d’un dossier dans la boîte aux lettres du propriétaire de la boîte aux lettres et que le délégué souhaite mettre à jour, supprimer ou copier l’élément. Lorsque le délégué utilise cet ID d’élément ou de dossier dans une demande, les modifications sont apportées à l’élément dans la boîte aux lettres du propriétaire de la boîte aux lettres. Le délégué n’a pas besoin d’inclure l’adresse SMTP du propriétaire de la boîte aux lettres. 
  
Par exemple, lorsqu’un délégué a l’ID de l’un des dossiers du propriétaire de la boîte aux lettres, le délégué peut effectuer une opération **FindItem** sur ce dossier à l’aide de l’ID de dossier, sans identifier explicitement la boîte aux lettres du propriétaire de la boîte aux lettres. À ce stade, le délégué peut effectuer des actions sur le dossier du propriétaire de la boîte aux lettres à l’aide des ID renvoyés dans les réponses. 
  
### <a name="implicit-access-and-the-ews-managed-api"></a>Accès implicite et API managée EWS

Si un ID d’élément a été récupéré par la méthode [FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) , cet ID d’élément peut être utilisé dans un appel de méthode suivant [. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) pour établir une liaison avec l’élément. Vous pouvez ensuite appeler la méthode [Item. Update](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.item.update%28v=exchg.80%29.aspx), [Item. Delete](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.item.delete%28v=exchg.80%29.aspx)ou [Item. Copy](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.item.copy%28v=exchg.80%29.aspx) , ou un appel de méthode qui requiert un ID d’élément, si nécessaire pour effectuer votre tâche. Tant que le délégué dispose des autorisations appropriées sur le dossier qui contient l’élément (et, le cas échéant, le dossier vers lequel se déplace l’élément), le délégué peut effectuer des modifications en fonction de leurs niveaux d’autorisation. 
  
### <a name="implicit-access-and-ews"></a>Accès implicite et EWS

Si un ID d’élément a été récupéré par l’opération [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) , cet ID d’élément peut être utilisé dans les opérations [GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) suivantes pour effectuer une liaison à l’élément. Vous pouvez ensuite appeler l’opération [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx), [DeleteItem](../web-service-reference/deleteitem-operation.md)ou [CopyItem](https://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) , ou toute opération nécessitant un ID d’élément, selon vos besoins pour effectuer votre tâche. Tant que le délégué dispose des autorisations appropriées sur le dossier qui contient l’élément (et, le cas échéant, le dossier vers lequel se déplace l’élément), le délégué peut effectuer des modifications en fonction de leurs niveaux d’autorisation. 
  
## <a name="in-this-section"></a>Dans cette section
<a name="bk_implicit"> </a>

- [Ajouter et supprimer des délégués à l’aide d’EWS dans Exchange](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)
    
- [Accéder à un calendrier en tant que délégué à l’aide d’EWS dans Exchange](how-to-access-a-calendar-as-a-delegate-by-using-ews-in-exchange.md)
    
- [Accéder aux contacts en tant que délégué à l’aide d’EWS dans Exchange](how-to-access-contacts-as-a-delegate-by-using-ews-in-exchange.md)
    
- [Accéder à la messagerie électronique en tant que délégué à l’aide d’EWS dans Exchange](how-to-access-email-as-a-delegate-by-using-ews-in-exchange.md)
    
- [Définir les autorisations de dossier pour un autre utilisateur à l’aide d’EWS dans Exchange](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md)
    
- [Gestion des erreurs liées à la délégation dans EWS dans Exchange](handling-delegation-related-errors-in-ews-in-exchange.md)
    
## <a name="see-also"></a>Voir aussi


- [Développer des clients de service web pour Exchange](develop-web-service-clients-for-exchange.md)

- [Autoriser quelqu’un d’autre à gérer votre courrier et votre calendrier](https://office.microsoft.com/outlook-help/allow-someone-else-to-manage-your-mail-and-calendar-HA102749417.aspx)  

- [Add-MailboxPermission](https://technet.microsoft.com/library/bb124097%28v=exchg.150%29.aspx)
    