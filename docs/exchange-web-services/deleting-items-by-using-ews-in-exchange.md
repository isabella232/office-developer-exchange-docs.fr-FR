---
title: Supprimer des éléments à l’aide d’EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: c81e3160-e12b-47e0-b3d6-4be28537f301
description: Découvrez comment vous pouvez utiliser l’API managée EWS ou EWS dans Exchange pour supprimer des éléments soit en les déplaçant vers le dossier éléments supprimés, soit vers la benne.
localization_priority: Priority
ms.openlocfilehash: 83317ccd0fa1db64e14df68652489009fea4ea07
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456135"
---
# <a name="deleting-items-by-using-ews-in-exchange"></a>Supprimer des éléments à l’aide d’EWS dans Exchange

Découvrez comment vous pouvez utiliser l’API managée EWS ou EWS dans Exchange pour supprimer des éléments soit en les déplaçant vers le dossier éléments supprimés, soit vers la benne.
  
Vous êtes-vous déjà demandé quelle est la différence entre le mouvement d’éléments dans le dossier éléments supprimés et leur transfert vers la benne ? Vous pouvez être curieux de connaître les différentes options de gestion des éléments supprimés et la façon d’implémenter ces options dans votre application. Les services Web Exchange (EWS) incluent trois options de gestion des éléments supprimés. Cet article vous permettra de clarifier toute confusion concernant les différences qui existent entre eux.
  
## <a name="deleting-items---what-are-my-options"></a>Suppression d’éléments : Quelles sont mes options ?
<a name="bk_DeletingItemsOptions"> </a>

Avant de pouvoir comprendre le contexte général de suppression des éléments, il est important de connaître la différence entre les éléments suivants :
  
- Le dossier éléments supprimés : lorsque vous supprimez des éléments dans une boîte aux lettres, c’est là où ils se trouvent.
    
- La benne (également appelée dossier éléments récupérables)-lorsque vous supprimez des éléments d’une boîte aux lettres, c’est là où ils sont placés.
    
Les figures 1 et 2 montrent à quoi ressemble le processus de suppression pour les éléments et les dossiers d’une boîte aux lettres. 

**Figure 1. Processus de suppression d’éléments d’une boîte aux lettres**

![Illustration montrant où les articles vont lorsqu’ils sont supprimés. Les éléments supprimés sont déplacés vers le dossier éléments supprimés, puis déplacés dans le dossier éléments récupérables par stratégie de rétention, leur date d’expiration et permantently supprimé.](media/Ex_DeleteItems_Source.png)

<br/>

**Figure 2. Processus de suppression de dossiers d’une boîte aux lettres**

![Illustration indiquant comment les dossiers supprimés sont déplacés dans le dossier Éléments supprimés, puis peuvent être définitivement supprimés de la boîte aux lettres.](media/Ex_.png)
   
Vous pouvez supprimer des éléments et des dossiers de trois manières différentes, en fonction de la façon dont vous souhaitez que la suppression soit « définitive ».
  
**Tableau 1 : options pour la suppression d’éléments à l’aide d’EWS**

|**Option**|**Action exécutée**|
|:-----|:-----|
|déplacer vers le dossier Éléments supprimés  <br/> |Il s’agit de la méthode la moins permanente pour supprimer des éléments.<br/><br/>Cela revient à placer une feuille de papier dans la corbeille par votre bureau. Vous pouvez facilement le récupérer si vous en avez besoin à nouveau.<br/><br/>Vous pouvez utiliser n’importe quelle [opération de suppression](deleting-items-by-using-ews-in-exchange.md#bk_howdoIdeleteitems) qui implémente l’option déplacer vers le dossier éléments supprimés pour effectuer cette action.<br/><br/>Vous pouvez également utiliser l' [opération MoveItem](https://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) ( [Item. Move ()](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.move%28v=exchg.80%29.aspx)) ou l' [opération MoveFolder](https://msdn.microsoft.com/library/c7233966-6c87-4a14-8156-b1610760176d%28Office.15%29.aspx) ( [Folder. Move ()](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.move%28v=exchg.80%29.aspx)) pour déplacer un élément ou un dossier vers le dossier éléments supprimés.  <br/> |
|Supprimer (récupération possible)  <br/> |L’élément est déplacé vers le dossier des suppressions dans la benne.<br/><br/>Cela revient à vider votre corbeille dans votre conteneur Curbside. Vous pouvez toujours accéder à l’élément si nécessaire, mais ce n’est qu’un peu plus difficile.  <br/><br/>Pour en savoir plus sur la benne (également appelée dossier éléments récupérables) et des scénarios comme eDiscovery ou les conservations pour litige, consultez la rubrique [dossier éléments récupérables](https://technet.microsoft.com/library/ee364755%28v=exchg.150%29.aspx) sur TechNet.<br/><br/>Les suppressions logicielles ne sont pas recommandées pour les applications qui ciblent Exchange 2007. Dans Exchange 2007, les suppressions logicielles sont gérées en définissant un bit sur l’élément pour indiquer qu’il sera déplacé vers la benne à un moment non spécifié.<br/><br/>Les parcours de suppressions conditionnelles, ou les recherches d’éléments supprimés par le biais de l' [opération FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx), ne sont pas pris en charge dans Exchange Online, Exchange Online dans le cadre d’Office 365 et les versions d’Exchange à partir d’Exchange 2010.  <br/><br/>**Remarque**: les dossiers ne peuvent pas être supprimés de manière récupérable.           |
|Suppression définitive  <br/> |L’élément ou le dossier est définitivement supprimé.<br/><br/>Les éléments supprimés de manière irréversible sont placés dans le dossier purges de la benne. C’est comme lorsque le camion de recyclage vide votre conteneur de recyclage Curbside. Les éléments ne sont pas accessibles à partir d’un client de messagerie tel qu’Outlook ou Outlook Web App et, à moins qu’un blocage n’ait été défini sur la boîte aux lettres, les éléments seront définitivement supprimés après une période de temps définie.<br/><br/>Pour plus d’informations sur la rétention des éléments, consultez la rubrique [configure Deleted Item Retention and Recoverable](https://technet.microsoft.com/library/ee364752%28v=exchg.150%29.aspx)items quotas.<br/><br/>**Remarque**: les dossiers ne sont pas placés dans le dossier purges lorsqu’ils sont supprimés définitivement. Les dossiers supprimés définitivement sont supprimés de la boîte aux lettres.  |
   
Le déplacement vers le dossier éléments supprimés et les options de suppression définitive sont transactionnelles, ce qui signifie que, au moment de la fin de l’appel de service Web, l’élément a été déplacé vers le dossier éléments supprimés ou la benne.
  
Pour vous aider à mieux comprendre l’écosystème de dossiers utilisés pour stocker des éléments supprimés, la figure suivante montre la hiérarchie des dossiers pouvant contenir des éléments supprimés. Les noms de dossier sont tels qu’ils apparaissent dans le type de schéma **DistinguishedFolderIdNameType** , ou l’énumération **WELLKNOWNFOLDERNAME** dans l’API managée EWS. 
  
**Figure 3. Hiérarchie des dossiers contenant des éléments supprimés**

![Figure illustrant la hiérarchie des dossiers pouvant contenir des éléments supprimés à la fois dans une boîte aux lettres principale et d’archivage. Chaque dossier de l’image est représenté par son nom de dossier unique.](media/Ex_FolderHierarchyDeletedItems.png)
  
**Tableau 2 : dossiers contenant des éléments supprimés**

|**Nom du dossier**|**Nouveauté de**|**Description**|
|:-----|:-----|:-----|
|deleteditems  <br/> |Exchange 2007  <br/> |Dossier éléments supprimés par défaut. Les éléments restent dans ce dossier jusqu’à ce qu’ils soient supprimés, de manière logicielle ou matérielle, ou jusqu’à ce qu’une période de rétention ait été dépassée. Ils sont ensuite déplacés vers un dossier dans la benne. Les dossiers supprimés sont placés dans le dossier éléments supprimés et, lorsqu’ils sont supprimés de manière incorrecte ou irréversible, ils sont définitivement supprimés de la boîte aux lettres et ne sont pas récupérables.  <br/> |
|recoverableitemsroot  <br/> |Exchange 2010  <br/> |La racine de la benne ou le dossier éléments récupérables. L’accès à la benne a été implémenté dans EWS dans Exchange 2010. Le nom complet de ce dossier est « éléments récupérables ».  <br/> |
|recoverableitemsdeletions  <br/> |Exchange 2010  <br/> |Dossier de la benne principale pour une boîte aux lettres. Les éléments supprimés (récupérables) et les éléments déplacés du dossier éléments supprimés par une stratégie de rétention sont placés dans ce dossier. Le nom complet de ce dossier est « suppressions ».  <br/> |
|recoverableitemsversions  <br/> |Exchange 2010  <br/> |Emplacement de stockage des versions antérieures d’un élément. Les anciennes versions d’un élément sont créées lors de la mise à jour d’un élément. Les versions des éléments de brouillon ne sont pas enregistrées dans ce dossier. Le nom complet de ce dossier est « versions ».  <br/> |
|recoverableitemspurges  <br/> |Exchange 2010  <br/> |Où sont stockés les éléments supprimés du dossier de suppressions. Tous les éléments supprimés définitivement dans le magasin sont déplacés vers ce dossier. Le nom complet de ce dossier est « purge ».  <br/> |
|archiveddeletedtitems  <br/> |Exchange 2010  <br/> |Dossier éléments supprimés par défaut pour une boîte aux lettres d’archivage.  <br/> |
|archiverecoverablesitemsroot  <br/> |Exchange 2010  <br/> |Dossier de la benne racine d’une boîte aux lettres d’archivage. Les éléments archivés qui sont supprimés de manière récupérable sont déplacés vers un sous-dossier de ce dossier.  <br/> |
|archiverecoverableitemsdeletions  <br/> |Exchange 2010  <br/> |Dossier de la benne principale pour une boîte aux lettres d’archivage. Les éléments archivés déplacés vers la benne sont placés ici.  <br/> |
|archiverecoverableitemsversions  <br/> |Exchange 2010  <br/> |Emplacement de stockage des versions antérieures des éléments archivés.  <br/> |
|archiverecoverableitemspurges  <br/> |Exchange 2010  <br/> |Où sont stockés les éléments supprimés de manière irréversible dans le dossier de suppressions d’archive de la benne. Tous les éléments archivés supprimés définitivement dans le magasin sont déplacés vers ce dossier.  <br/> |
   
## <a name="how-do-i-delete-items"></a>Comment supprimer des éléments ?
<a name="bk_howdoIdeleteitems"> </a>

Utilisez l’une des options suivantes pour indiquer si un élément doit être déplacé vers le dossier éléments supprimés ou si vous souhaitez effectuer une suppression logicielle ou une suppression définitive :
  
- Le type simple **DisposalType** , si vous utilisez EWS pour accéder à Exchange. 
    
- L' [énumération DeleteMode](https://msdn.microsoft.com/library/exchange/microsoft.exchange.webservices.data.deletemode%28v=exchg.80%29.aspx), si vous utilisez l’API managée EWS.
    
Vous pouvez utiliser plusieurs opérations EWS ou méthodes d’API managée EWS pour supprimer des éléments et des dossiers d’une boîte aux lettres.
  
**Tableau 3 : opérations EWS et méthodes de l’API managée EWS pour la suppression d’éléments**

|**Opération EWS**|**Méthode d'API managée EWS**|**Nouveauté de**|**Fonction**|
|:-----|:-----|:-----|:-----|
|[Opération DeleteFolder](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |[Méthode Folder. Delete](https://msdn.microsoft.com/library/exchange/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) <br/> |Exchange 2007  <br/> |Supprime les dossiers d’une boîte aux lettres. Avec EWS, vous pouvez supprimer des dossiers par lots. Avec l’API managée EWS, vous ne pouvez supprimer qu’un seul dossier par appel.  <br/> |
|[Opération DeleteItem](https://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |[Méthode Item. Delete](https://msdn.microsoft.com/library/exchange/microsoft.exchange.webservices.data.item.delete%28v=exchg.80%29.aspx)<br/><br/>[Méthode ExchangeService. DeleteItems](https://msdn.microsoft.com/library/exchange/microsoft.exchange.webservices.data.exchangeservice.deleteitems%28v=exchg.80%29.aspx) <br/> |Exchange 2007  <br/> |Supprime des éléments d’une boîte aux lettres.  <br/> |
|[Opération EmptyFolder](https://msdn.microsoft.com/library/98161486-e2f2-480f-8d5d-708ba81b208a%28Office.15%29.aspx) <br/> |[Méthode Folder. Empty](https://msdn.microsoft.com/library/exchange/microsoft.exchange.webservices.data.folder.empty%28v=exchg.80%29.aspx) <br/> |Exchange 2010  <br/> |Supprime tous les éléments d’un dossier et, éventuellement, supprime tous les sous-dossiers d’un dossier.  <br/> |
|[Opération de ApplyConversationAction](https://msdn.microsoft.com/library/73d7943d-d361-4f8b-9948-d85f886efa1a%28Office.15%29.aspx) <br/> |[Méthode conversation. EnableAlwaysDeleteItems](https://msdn.microsoft.com/library/exchange/microsoft.exchange.webservices.data.conversation.enablealwaysdeleteitems%28v=exchg.80%29.aspx)<br/><br/>[Méthode conversation. DeleteItems](https://msdn.microsoft.com/library/exchange/microsoft.exchange.webservices.data.conversation.deleteitems%28v=exchg.80%29.aspx) <br/> |Exchange 2010  <br/> |Définit une action de traitement de suppression sur les messages électroniques d’une conversation afin qu’ils soient supprimés.  <br/> |
|[Opération DeleteUserConfiguration](https://msdn.microsoft.com/library/93e44690-be2d-4fdb-96a8-4ded3c193aed%28Office.15%29.aspx) <br/> |[Méthode UserConfiguration. Delete](https://msdn.microsoft.com/library/exchange/microsoft.exchange.webservices.data.userconfiguration.delete%28v=exchg.80%29.aspx) <br/> |Exchange 2010  <br/> |Supprime un élément associé à un dossier et le déplace vers la benne.  <br/> |
|[Opération CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) <br/> |[Méthode appointment. Accept](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.accept%28v=exchg.80%29.aspx) <br/><br/>[Méthode appointment. AcceptTentatively](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.accepttentatively%28v=exchg.80%29.aspx)<br/><br/>[Méthode appointment. CancelMeeting](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.cancelmeeting%28v=exchg.80%29.aspx)<br/><br/>[Rendez-vous. refuser](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.decline%28v=exchg.80%29.aspx)<br/><br/>[Propriété meetingrequest. Accept, méthode](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.meetingrequest.accept%28v=exchg.80%29.aspx)<br/><br/>[Méthode propriété meetingrequest. AcceptTentatively](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.meetingrequest.accepttentatively%28v=exchg.80%29.aspx)<br/><br/>[Propriété meetingrequest. Reverse, méthode](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.meetingrequest.decline%28v=exchg.80%29.aspx) <br/> |Exchange 2007  <br/> |Déplace indirectement un élément vers le dossier éléments supprimés chaque fois qu’une réponse à une demande de réunion est envoyée ou que la réponse est définie sur le rendez-vous.<br/><br/>Le type de suppression n’est pas défini sur cette opération. Les messages de réunion sont déplacés vers le dossier éléments supprimés lorsqu’un objet réponse est traité avec succès par le service.  <br/> |
   
Vous pouvez également déplacer des éléments vers le dossier éléments supprimés à l’aide de règles de boîte de réception. Par exemple, vous pouvez [créer des règles](inbox-management-and-ews-in-exchange.md) qui comportent une action DELETE. 
  
Voici quelques points à noter concernant la suppression d’éléments :
  
- La suppression d’une occurrence d’un élément périodique ne déclenche pas un déplacement vers le dossier éléments supprimés ou la benne. Il en résulte une mise à jour de l’élément maître périodique de la série périodique.
    
- Vous ne pouvez pas supprimer des dossiers par défaut de la boîte aux lettres.
    
- Évitez de supprimer des réunions ou des messages de réunion, tels que des demandes de réunion ou des mises à jour de réunion. Répondez plutôt à ces éléments à l’aide d’objets Response. De cette façon, les éléments de calendrier associés sont mis à jour pour refléter les actions de l’organisateur ou du répondeur.
    
- La clé de modification d’un élément n’est pas mise à jour lorsque l’élément est déplacé vers le dossier éléments supprimés ou suppressions.
    
- Si vous effectuez une suppression matérielle sur un élément, puis appelez une [opération opérationsyncfolderhierarchy](https://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) ou une méthode d’API managée EWS [opérationsyncfolderhierarchy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderhierarchy%28v=exchg.80%29.aspx) , ou une [opération SyncFolderItems](https://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx) ou [SyncFolderItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderitems%28v=exchg.80%29.aspx) , une entrée **de modification sera** renvoyée. Si vous déplacez un élément vers le dossier éléments supprimés, une entrée de modification de **mise à jour** est renvoyée. Cela est dû au fait que l’élément ou le dossier aura une nouvelle valeur de propriété [ParentFolderId](https://msdn.microsoft.com/library/258f4b1f-367e-4c7d-9c29-eb775a2398c7%28Office.15%29.aspx) . Pour [en savoir plus sur la synchronisation](mailbox-synchronization-and-ews-in-exchange.md) , si la synchronisation des éléments supprimés fait partie de votre scénario. 
    
## <a name="find-out-more-about-deleting-items"></a>En savoir plus sur la suppression d’éléments
<a name="findoutmore"> </a>

- [Notifications de type pull pour les événements de boîte aux lettres liés à la suppression EWS dans Exchange](pull-notifications-for-ews-deletion-related-mailbox-events-in-exchange.md)
    
- [Gestion des erreurs liées à la suppression dans EWS dans Exchange](handling-deletion-related-errors-in-ews-in-exchange.md)
    
## <a name="see-also"></a>Voir aussi

- [Dossiers et éléments dans EWS dans Exchange](folders-and-items-in-ews-in-exchange.md)    
- [Développer des clients de service web pour Exchange](develop-web-service-clients-for-exchange.md)    
- [Dossier éléments récupérables](https://technet.microsoft.com/library/ee364755.aspx)    
- [Récupération d’élément unique dans Exchange Server 2010](https://blogs.technet.com/b/exchange/archive/2009/09/25/3408389.aspx#_Single_Item_Recovery)    
- [Exchange 2013 : supprimer une série périodique par programme des serveurs Exchange](https://code.msdn.microsoft.com/exchange/Exchange-2013-Delete-a-e1c7b89d)    
- [Exchange 2013 : supprimer des tâches d’un compte sur des serveurs Exchange par programme](https://code.msdn.microsoft.com/exchange/Exchange-2013-Delete-tasks-13824637)    
- [Exchange 2013 : dossiers vides sur les serveurs Exchange par programme](https://code.msdn.microsoft.com/exchange/Exchange-2013-Empty-6487df37)    
- [Exchange 2013 : suppression de dossiers par programmation à partir de serveurs Exchange](https://code.msdn.microsoft.com/exchange/Exchange-2013-Delete-aa1a5823)    
- [Exchange 2013 : supprimer de nombreux éléments par programme des serveurs Exchange](https://code.msdn.microsoft.com/exchange/Exchange-2013-Delete-many-064f8760)    
- [Exchange 2013 : suppression de contacts par programmation à partir de serveurs Exchange](https://code.msdn.microsoft.com/exchange/Exchange-2013-Delete-3b8b0640)    
- [Supprimer des rendez-vous et annuler des réunions à l'aide d’EWS dans Exchange](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md)    
- [Gérer les paramètres d’application permanente à l’aide d’EWS dans Exchange](how-to-manage-persistent-application-settings-by-using-ews-in-exchange.md)
    

