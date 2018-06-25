---
title: Suppression d’éléments à l’aide de EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: c81e3160-e12b-47e0-b3d6-4be28537f301
description: Découvrez comment vous pouvez utiliser l’API managée EWS ou EWS dans Exchange pour supprimer les éléments soit en les déplaçant vers le dossier éléments supprimés ou à la benne.
ms.openlocfilehash: a475ebc6677e5f5003cc790a2d4d2b83c513f309
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754788"
---
# <a name="deleting-items-by-using-ews-in-exchange"></a>Suppression d’éléments à l’aide de EWS dans Exchange

Découvrez comment vous pouvez utiliser l’API managée EWS ou EWS dans Exchange pour supprimer les éléments soit en les déplaçant vers le dossier éléments supprimés ou à la benne.
  
Avez vous jamais demandé quel est la différence entre le déplacement d’éléments dans le dossier éléments supprimés et les déplacer vers la benne ? Vous devez connaître les différentes options pour les éléments supprimée de gestion et comment implémenter ces options dans votre application. Exchange Web Services (EWS) inclut trois options pour les éléments supprimée de gestion. Cet article fournit effacera toute confusion, que vous devrez peut-être sur les différences entre eux.
  
## <a name="deleting-items---what-are-my-options"></a>Suppression d’éléments - quelles sont mes options ?
<a name="bk_DeletingItemsOptions"> </a>

Avant de vous permettre de comprendre l’ensemble du paysage de suppression des éléments, il est important de la différence entre les éléments suivants :
  
- Le dossier éléments supprimés - lorsque vous supprimez des éléments dans une boîte aux lettres, c’est là qu’ils.
    
- La benne (alias du dossier éléments récupérables) - lorsque vous supprimez des éléments d’une boîte aux lettres, c’est là qu’ils.
    
Les figures 1 et 2 indiquent à quoi ressemble le processus de suppression des éléments et des dossiers dans une boîte aux lettres. 

**La figure 1. Processus de suppression des éléments à partir d’une boîte aux lettres**

![Une illustration montre où aller d’éléments lorsqu’ils sont supprimés. Éléments supprimés sont déplacés vers le dossier éléments supprimés, puis sont déplacés vers le dossier éléments récupérables par la stratégie de rétention, où leur expiration et sont supprimé de permantently.](media/Ex_DeleteItems_Source.png)

<br/>

**La figure 2. Processus de suppression des dossiers à partir d’une boîte aux lettres**

![Illustration indiquant comment les dossiers supprimés sont déplacés dans le dossier Éléments supprimés, puis peuvent être définitivement supprimés de la boîte aux lettres.](media/Ex_.png)
   
Vous pouvez supprimer des éléments et les dossiers de trois façons différentes, selon « permanent », vous souhaitez que la suppression à.
  
**Tableau 1 : Options de suppression des éléments à l’aide de EWS**

|**Option**|**Que se passe-t-il**|
|:-----|:-----|
|Déplacer vers le dossier éléments supprimés  <br/> |Il s’agit moins permanent permet de supprimer des éléments.<br/><br/>Il s’agit comme le fait de placer une feuille de papier dans la Corbeille à votre bureau. Vous pouvez facilement récupérer il si vous le souhaitez.<br/><br/>Vous pouvez utiliser toute [opération de suppression](deleting-items-by-using-ews-in-exchange.md#bk_howdoIdeleteitems) qui implémente le déplacement à l’option du dossier éléments supprimés pour effectuer cette action.<br/><br/>Vous pouvez également utiliser l' [opération MoveItem](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) ( [Item.Move()](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.move%28v=exchg.80%29.aspx)) ou l' [opération MoveFolder](http://msdn.microsoft.com/library/c7233966-6c87-4a14-8156-b1610760176d%28Office.15%29.aspx) ( [Folder.Move()](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.move%28v=exchg.80%29.aspx)) pour déplacer un élément ou un dossier vers le dossier éléments supprimés.  <br/> |
|Suppression réversible  <br/> |L’élément est déplacé vers le dossier suppressions dans la benne.<br/><br/>Cela équivaut à vider la Corbeille dans votre conteneur taxi. Vous pouvez accéder à l’élément si vous avez besoin, c’est juste un peu plus complexe.  <br/><br/>Pour plus d’informations sur la benne (également appelé le dossier éléments récupérables) et scénarios tels que des blocages eDiscovery ou pour litige, consultez le [Dossier éléments récupérables](http://technet.microsoft.com/en-us/library/ee364755%28v=exchg.150%29.aspx) sur TechNet.<br/><br/>Suppressions logicielles ne sont pas recommandées pour les applications qui ciblent Exchange 2007. Dans Exchange 2007, suppressions logicielles sont gérées par les paramètre un peu sur l’élément pour indiquer qu’il sera déplacé vers la benne à un moment non spécifié.<br/><br/>Parcours de suppression réversible ou recherches d’éléments qui ont été paramétrés supprimés par le biais de l' [opération FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx), ne sont pas pris en charge dans Exchange Online, Exchange Online dans le cadre d’Office 365 et les versions d’Exchange commençant par Exchange 2010.  <br/><br/>**Remarque**: les dossiers ne peuvent pas être supprimés logicielle.           |
|Suppression définitive  <br/> |L’élément ou le dossier est définitivement supprimé.<br/><br/>Éléments supprimés définitivement sont placés dans le dossier de la purge de la benne. Il s’agit comme lorsque le recyclage automobiles vide votre conteneur recycle taxi. Les éléments n’est pas accessible à partir d’un client de messagerie comme Outlook ou Outlook Web App et, sauf s’il existe une suspension définie dans la boîte aux lettres, les éléments seront définitivement supprimés après un laps de temps.<br/><br/>Vous pouvez en savoir plus sur la rétention des éléments dans l’article [configurer la rétention des éléments supprimés et les Quotas d’éléments récupérables](http://technet.microsoft.com/en-us/library/ee364752%28v=exchg.150%29.aspx).<br/><br/>**Remarque**: les dossiers ne sont pas placés dans le dossier de purge lorsqu’ils sont définitivement supprimés. Dossiers supprimée sont supprimés de la boîte aux lettres.  |
   
Le déplacement vers le dossier éléments supprimés et les options de suppression définitive sont transactionnelles, ce qui signifie que, lors de la fin de l’appel au service web, l’élément a été déplacé vers le dossier éléments supprimés ou la benne.
  
Pour vous aider à mieux comprendre l’écosystème des dossiers qui sont utilisés pour stocker les éléments supprimés, la figure suivante illustre la hiérarchie de dossiers qui peut contenir les éléments supprimés. Les noms de dossier sont lorsqu’ils s’affichent dans le type de schéma **DistinguishedFolderIdNameType** , ou l’énumération **WellKnownFolderName** dans l’API managée EWS. 
  
**La figure 3. Hiérarchie de dossiers qui contiennent des éléments supprimés**

![Figure illustrant la hiérarchie des dossiers pouvant contenir des éléments supprimés à la fois dans une boîte aux lettres principale et d’archivage. Chaque dossier de l’image est représenté par son nom de dossier unique.](media/Ex_FolderHierarchyDeletedItems.png)
  
**Tableau 2 : Dossiers qui contiennent les éléments supprimés**

|**Nom du dossier**|**Introduite dans**|**Description**|
|:-----|:-----|:-----|
|deleteditems  <br/> |Exchange 2007  <br/> |Le dossier éléments supprimés par défaut. Éléments demeurent dans ce dossier jusqu'à ce qu’ils soient ou dur-récupérable ou jusqu'à ce qu’une période de rétention a été dépassée. Puis ils sont déplacés vers un dossier dans la benne. Dossiers supprimés sont placés dans le dossier éléments supprimés, et lorsqu’ils sont ou dur-récupérable, ils sont définitivement supprimés de la boîte aux lettres et ne sont pas récupérables.  <br/> |
|recoverableitemsroot  <br/> |Exchange 2010  <br/> |La racine de la benne, ou dans le dossier éléments récupérables. Accès benne a implémenté dans EWS dans Exchange 2010. Le nom complet de ce dossier est « Éléments récupérables ».  <br/> |
|recoverableitemsdeletions  <br/> |Exchange 2010  <br/> |Le principal benne de dossier pour une boîte aux lettres. Éléments supprimés et déplacé à partir du dossier éléments supprimés par une stratégie de rétention sont placés dans ce dossier. Le nom complet de ce dossier est « Suppression ».  <br/> |
|recoverableitemsversions  <br/> |Exchange 2010  <br/> |Où sont stockées les anciennes versions d’un élément. Anciennes versions d’un élément sont créées lorsqu’un élément est mis à jour. Versions d’éléments de brouillon ne sont pas enregistrées dans ce dossier. Le nom complet de ce dossier est « Versions ».  <br/> |
|recoverableitemspurges  <br/> |Exchange 2010  <br/> |Où sont stockés les éléments qui sont supprimés du dossier des suppressions. Tous les éléments de la banque supprimée sont déplacés vers ce dossier. Le nom complet de ce dossier est « Purge ».  <br/> |
|archiveddeletedtitems  <br/> |Exchange 2010  <br/> |Le dossier éléments supprimés par défaut pour une boîte aux lettres d’archive.  <br/> |
|archiverecoverablesitemsroot  <br/> |Exchange 2010  <br/> |La racine benne de dossier pour une boîte aux lettres d’archive. Les éléments archivés sont supprimés sont déplacés vers un sous-dossier dans ce dossier.  <br/> |
|archiverecoverableitemsdeletions  <br/> |Exchange 2010  <br/> |Le principal benne de dossier pour une boîte aux lettres d’archive. Archiver des éléments déplacés vers la benne sont placés ici.  <br/> |
|archiverecoverableitemsversions  <br/> |Exchange 2010  <br/> |Où sont stockées les anciennes versions d’éléments archivés.  <br/> |
|archiverecoverableitemspurges  <br/> |Exchange 2010  <br/> |Où les éléments qui sont supprimés de l’archive suppressions dossier dans la benne sont stockés. Tous les éléments de la banque supprimée archivé sont déplacés vers ce dossier.  <br/> |
   
## <a name="how-do-i-delete-items"></a>Comment supprimer des éléments
<a name="bk_howdoIdeleteitems"> </a>

Supprimer, utilisez une des options suivantes pour indiquer si vous souhaitez déplacer un élément vers le dossier éléments supprimés ou effectuez une logicielle ou un disque dur :
  
- Le **DisposalType** type simple, si vous utilisez EWS pour accéder à Exchange. 
    
- L' [énumération DeleteMode](http://msdn.microsoft.com/en-us/library/exchange/microsoft.exchange.webservices.data.deletemode%28v=exchg.80%29.aspx), si vous utilisez l’API managée EWS.
    
Vous pouvez utiliser un nombre de différentes opérations EWS ou méthodes API managées pour supprimer des éléments et des dossiers à partir d’une boîte aux lettres.
  
**Tableau 3 : Opérations EWS et méthodes d’API managées pour supprimer des éléments**

|**Opération EWS**|**Méthode d'API managée EWS**|**Introduite dans**|**Fonction**|
|:-----|:-----|:-----|:-----|
|[Opération DeleteFolder](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |[Méthode Folder.Delete](http://msdn.microsoft.com/en-us/library/exchange/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) <br/> |Exchange 2007  <br/> |Supprime les dossiers d’une boîte aux lettres. Avec EWS, vous pouvez par lot Supprimer les dossiers. Avec l’API managée EWS, vous ne pouvez supprimer un dossier unique par appel.  <br/> |
|[Opération DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |[Méthode Item.Delete](http://msdn.microsoft.com/en-us/library/exchange/microsoft.exchange.webservices.data.item.delete%28v=exchg.80%29.aspx)<br/><br/>[Méthode ExchangeService.DeleteItems](http://msdn.microsoft.com/en-us/library/exchange/microsoft.exchange.webservices.data.exchangeservice.deleteitems%28v=exchg.80%29.aspx) <br/> |Exchange 2007  <br/> |Supprime les éléments d’une boîte aux lettres.  <br/> |
|[Opération EmptyFolder](http://msdn.microsoft.com/library/98161486-e2f2-480f-8d5d-708ba81b208a%28Office.15%29.aspx) <br/> |[Méthode Folder.Empty](http://msdn.microsoft.com/en-us/library/exchange/microsoft.exchange.webservices.data.folder.empty%28v=exchg.80%29.aspx) <br/> |Exchange 2010  <br/> |Supprime tous les éléments dans un dossier et, le cas échéant, supprime tous les sous-dossiers dans un dossier.  <br/> |
|[Opération de ApplyConversationAction](http://msdn.microsoft.com/library/73d7943d-d361-4f8b-9948-d85f886efa1a%28Office.15%29.aspx) <br/> |[Méthode Conversation.EnableAlwaysDeleteItems](http://msdn.microsoft.com/en-us/library/exchange/microsoft.exchange.webservices.data.conversation.enablealwaysdeleteitems%28v=exchg.80%29.aspx)<br/><br/>[Méthode Conversation.DeleteItems](http://msdn.microsoft.com/en-us/library/exchange/microsoft.exchange.webservices.data.conversation.deleteitems%28v=exchg.80%29.aspx) <br/> |Exchange 2010  <br/> |Définit une suppression de traitement de l’action sur les messages électroniques dans une conversation pour qu’ils sont supprimés.  <br/> |
|[Opération DeleteUserConfiguration](http://msdn.microsoft.com/library/93e44690-be2d-4fdb-96a8-4ded3c193aed%28Office.15%29.aspx) <br/> |[Méthode UserConfiguration.Delete](http://msdn.microsoft.com/en-us/library/exchange/microsoft.exchange.webservices.data.userconfiguration.delete%28v=exchg.80%29.aspx) <br/> |Exchange 2010  <br/> |Supprime un dossier associé élément et le déplace vers la benne.  <br/> |
|[CreateItem Operation](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) <br/> |[Méthode Appointment.Accept](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.accept%28v=exchg.80%29.aspx) <br/><br/>[Méthode Appointment.AcceptTentatively](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.accepttentatively%28v=exchg.80%29.aspx)<br/><br/>[Méthode Appointment.CancelMeeting](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.cancelmeeting%28v=exchg.80%29.aspx)<br/><br/>[Appointment.Decline](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.decline%28v=exchg.80%29.aspx)<br/><br/>[Méthode MeetingRequest.Accept](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.meetingrequest.accept%28v=exchg.80%29.aspx)<br/><br/>[Méthode MeetingRequest.AcceptTentatively](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.meetingrequest.accepttentatively%28v=exchg.80%29.aspx)<br/><br/>[Méthode MeetingRequest.Decline](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.meetingrequest.decline%28v=exchg.80%29.aspx) <br/> |Exchange 2007  <br/> |Indirectement déplace un élément vers le dossier éléments supprimés lorsqu’une réponse à une demande de réunion est envoyée ou de la réponse est définie sur le rendez-vous.<br/><br/>Le type de suppression n’est pas défini sur cette opération. Les messages de réunion sont déplacés vers le dossier éléments supprimés lorsqu’un objet de réponse est correctement traité par le service.  <br/> |
   
Vous pouvez également déplacer des éléments dans le dossier éléments supprimés à l’aide de règles de boîte de réception. Par exemple, vous pouvez [créer des règles](inbox-management-and-ews-in-exchange.md) qui ont une action de suppression. 
  
Certains points à noter concernant la suppression d’éléments :
  
- Suppression d’une occurrence d’un élément périodique ne déclenche pas un déplacement vers le dossier éléments supprimés ou la benne. Le résultat dans une mise à jour à l’élément périodique principal de la série périodique.
    
- Vous ne pouvez pas supprimer les dossiers par défaut à partir de la boîte aux lettres.
    
- Évitez de supprimer des réunions ou des messages de la réunion, telles que les demandes de réunion et ou mises à jour de la réunion. Au lieu de cela, répondre à ces éléments à l’aide des objets de réponse. De cette manière, les éléments de calendrier associées sont mises à jour pour refléter les actions du répondeur ou l’organisateur.
    
- Modifier la clé d’un élément n’est pas mis à jour lors de l’élément est déplacé vers le dossier éléments supprimés et les suppressions.
    
- Si vous effectuez un disque dur supprimer un élément et ensuite appeler une [opération SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) ou méthode d’API managées [SyncFolderHierarchy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderhierarchy%28v=exchg.80%29.aspx) ou une méthode [opération SyncFolderItems](http://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx) ou [SyncFolderItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderitems%28v=exchg.80%29.aspx) , une modification à **Supprimer** entrée est retournée. Si vous déplacez un élément vers le dossier éléments supprimés, une entrée de changement de **mise à jour** est renvoyée. Il s’agit, car l’élément ou le dossier aura une nouvelle valeur de la propriété [ParentFolderId](http://msdn.microsoft.com/library/258f4b1f-367e-4c7d-9c29-eb775a2398c7%28Office.15%29.aspx) . [En savoir plus sur la synchronisation](mailbox-synchronization-and-ews-in-exchange.md) si la synchronisation des éléments supprimés fait partie de votre scénario. 
    
## <a name="find-out-more-about-deleting-items"></a>En savoir plus sur la suppression d’éléments
<a name="findoutmore"> </a>

- [Extraction des notifications pour les événements liés à la suppression de boîte aux lettres EWS dans Exchange](pull-notifications-for-ews-deletion-related-mailbox-events-in-exchange.md)
    
- [Gestion des erreurs liées aux suppression dans EWS dans Exchange](handling-deletion-related-errors-in-ews-in-exchange.md)
    
## <a name="see-also"></a>Voir aussi

- [Dossiers et éléments dans EWS dans Exchange](folders-and-items-in-ews-in-exchange.md)    
- [Développer des clients de service web pour Exchange](develop-web-service-clients-for-exchange.md)    
- [Dossier éléments récupérables](http://technet.microsoft.com/en-us/library/ee364755.aspx)    
- [Récupération d’élément unique dans Exchange Server 2010](http://blogs.technet.com/b/exchange/archive/2009/09/25/3408389.aspx#_Single_Item_Recovery)    
- [Exchange 2013 : Supprimer par programme une série périodique à partir des serveurs Exchange](http://code.msdn.microsoft.com/exchange/Exchange-2013-Delete-a-e1c7b89d)    
- [Exchange 2013 : Supprimer par programme des tâches à partir d’un compte sur les serveurs Exchange](http://code.msdn.microsoft.com/exchange/Exchange-2013-Delete-tasks-13824637)    
- [Exchange 2013 : Vider les dossiers sur des serveurs Exchange par programme](http://code.msdn.microsoft.com/exchange/Exchange-2013-Empty-6487df37)    
- [Exchange 2013 : Supprimer par programme des dossiers à partir des serveurs Exchange](http://code.msdn.microsoft.com/exchange/Exchange-2013-Delete-aa1a5823)    
- [Exchange 2013 : Supprimer par programme le nombre d’éléments à partir des serveurs Exchange](http://code.msdn.microsoft.com/exchange/Exchange-2013-Delete-many-064f8760)    
- [Exchange 2013 : Supprimer par programme des contacts à partir des serveurs Exchange](http://code.msdn.microsoft.com/exchange/Exchange-2013-Delete-3b8b0640)    
- [Supprimer des rendez-vous et annuler des réunions à l’aide de EWS dans Exchange](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md)    
- [Gérer les paramètres de l’application permanente à l’aide de EWS dans Exchange](how-to-manage-persistent-application-settings-by-using-ews-in-exchange.md)
    

