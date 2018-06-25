---
title: Opérations EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Exchange
api_type:
- schema
ms.assetid: cf6fd871-9a65-4f34-8557-c8c71dd7ce09
description: Trouvez des informations sur les opérations EWS qui sont disponibles dans Exchange.
ms.openlocfilehash: c56c3be746138cec251836fcb61ee3738d168869
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756250"
---
# <a name="ews-operations-in-exchange"></a>Opérations EWS dans Exchange

Trouvez des informations sur les opérations EWS qui sont disponibles dans Exchange.
  
Exchange Web Services (EWS) fournit de nombreuses opérations qui vous permettent d’accéder aux informations à partir de la banque d’informations Exchange. Les articles de cette section fournissent des informations sur la structure globale des demandes, réponses et les messages de réponse d’erreur pour les opérations EWS, ainsi que des exemples de code XML pour chaque opération. Elles fournissent une vue d’ensemble des structures de messages envoyés entre le client et le serveur. Vous pouvez utiliser ces informations pour déboguer des structures de messages et trouvez des informations sur ce que vous pouvez faire dans une demande EWS. Pour plus d’informations sur les qui représente de structure XML, voir - [éléments XML EWS dans Exchange](ews-xml-elements-in-exchange.md).
  
Toutes les fonctionnalités EWS sont associée à une version du schéma. Nouvelles versions de schéma EWS sont générées dans les nouvelles versions d’Exchange Server ou Exchange Online. L’élément [RequestServerVersion](requestserverversion.md) contient un attribut **Version** qui mappe la version du serveur vers la version de schéma. Cet article fournit des informations sur lorsque chaque opération a été introduite. Fonctionnalité spécifique au sein d’une opération peut nécessiter une version ultérieure du service. Les schémas de version sont implémentées pour que les clients qui sont conçus par rapport à une version antérieure de EWS fonctionnent avec une version plus récente de EWS. 
  
Ces opérations peuvent cibler le point de terminaison EWS que les services de votre boîte aux lettres. Vous pouvez parcourir au point de terminaison EWS en utilisant une URL qui est une structure semblable à http://<clientaccessserver>.com/ews/exchange.asmx, où <clientaccessserver> est le serveur d’accès au Client Exchange que les services de votre boîte aux lettres. Vous pouvez utiliser la découverte automatique pour obtenir l’URL pour le serveur d’accès au Client que les services de votre boîte aux lettres. Pour plus d’informations sur la découverte automatique, voir la [découverte automatique pour Exchange](../exchange-web-services/autodiscover-for-exchange.md).
  
## <a name="ediscovery-operations"></a>opérations de découverte électronique
<a name="bk_eDiscovery"> </a>

Les opérations de découverte électronique fournissent des opérations de recherche pour la conservation légale et identifient les données de boîte aux lettres ne peut pas être indexées et renvoyées dans les résultats de recherche de découverte.
  
Le tableau suivant répertorie les opérations eDiscovery.
  
|**Nom de l’opération**|**Introduite dans**|
|:-----|:-----|
|[Opération GetDiscoverySearchConfiguration](getdiscoverysearchconfiguration-operation.md) <br/> |Exchange 2013  <br/> |
|[Opération GetHoldOnMailboxes](getholdonmailboxes-operation.md) <br/> |Exchange 2013  <br/> |
|[Opération GetNonIndexableItemDetails](getnonindexableitemdetails-operation.md) <br/> |Exchange 2013  <br/> |
|[Opération GetNonIndexableItemStatistics](getnonindexableitemstatistics-operation.md) <br/> |Exchange 2013  <br/> |
|[Opération GetSearchableMailboxes](getsearchablemailboxes-operation.md) <br/> |Exchange 2013  <br/> |
|[Opération SearchMailboxes](searchmailboxes-operation.md) <br/> |Exchange 2013  <br/> |
|[Opération SetHoldOnMailboxes](setholdonmailboxes-operation.md) <br/> |Exchange 2013  <br/> |
   
## <a name="exchange-mailbox-data-operations"></a>Opérations de données de boîtes aux lettres Exchange
<a name="bk_Exchange_mailbox_data"> </a>

Les opérations de données de boîtes aux lettres Exchange permettent aux clients de gérer et organiser les éléments, dossiers et pièces jointes, ainsi qu’extension de nom ambigu résolution et la distribution la liste. Opérations de données de boîtes aux lettres Exchange sont élément, dossier, pièce jointe et opérations utilitaires.
  
Le tableau suivant répertorie les opérations de données de boîtes aux lettres Exchange.
  
|**Nom de l’opération**|**Introduite dans**|
|:-----|:-----|
|[Opération ArchiveItem](archiveitem-operation.md) <br/> |Exchange 2013  <br/> |
|[CreateItem Operation](createitem-operation.md) <br/> |Exchange 2007  <br/> |
|[Opération CopyItem](copyitem-operation.md) <br/> |Exchange 2007  <br/> |
|[Opération DeleteItem](deleteitem-operation.md) <br/> |Exchange 2007  <br/> |
|[Opération FindItem](finditem-operation.md) <br/> |Exchange 2007  <br/> |
|[GetItem Operation](getitem-operation.md) <br/> |Exchange 2007  <br/> |
|[Opération MarkAllItemsAsRead](markallitemsasread-operation.md) <br/> |Exchange 2013  <br/> |
|[Opération MoveItem](moveitem-operation.md) <br/> |Exchange 2007  <br/> |
|[Opération SendItem](senditem-operation.md) <br/> |Exchange 2007  <br/> |
|[UpdateItem Operation](updateitem-operation.md) <br/> |Exchange 2007  <br/> |
   
Le tableau suivant répertorie les opérations de dossier de données de boîtes aux lettres Exchange.
  
|**Nom de l’opération**|**Introduite dans**|
|:-----|:-----|
|[Opération CreateFolder](createfolder-operation.md) <br/> |Exchange 2007  <br/> |
|[Opération CreateFolderPath](createfolderpath-operation.md) <br/> |Exchange 2013  <br/> |
|[Opération CreateManagedFolder](createmanagedfolder-operation.md) <br/> |Exchange 2007. Cette fonctionnalité a été deemphasized dans les versions d’Exchange commençant par Exchange 2010. Pour plus d’informations sur la migration vers à l’aide des balises et stratégies de gestion des enregistrements de messagerie, voir [migrer à partir de dossiers gérés](http://technet.microsoft.com/en-us/library/dd298032%28v=exchg.141%29.aspx).  <br/> |
|[Opération CopyFolder](copyfolder-operation.md) <br/> |Exchange 2007  <br/> |
|[Opération DeleteFolder](deletefolder-operation.md) <br/> |Exchange 2007  <br/> |
|[Opération EmptyFolder](emptyfolder-operation.md) <br/> |Exchange 2010  <br/> |
|[Opération FindFolder](findfolder-operation.md) <br/> |Exchange 2007  <br/> |
|[Opération GetFolder](getfolder-operation.md) <br/> |Exchange 2007  <br/> |
|[Opération MoveFolder](movefolder-operation.md) <br/> |Exchange 2007  <br/> |
|[Opération UpdateFolder](updatefolder-operation.md) <br/> |Exchange 2007  <br/> |
   
Le tableau suivant répertorie les opérations de pièce jointe de données de boîtes aux lettres Exchange.
  
|**Nom de l’opération**|**Introduite dans**|
|:-----|:-----|
|[Opération CreateAttachment](createattachment-operation.md) <br/> |Exchange 2007  <br/> |
|[Opération GetAttachment](getattachment-operation.md) <br/> |Exchange 2007  <br/> |
|[Opération DeleteAttachment](deleteattachment-operation.md) <br/> |Exchange 2007  <br/> |
   
Le tableau suivant répertorie les opérations de rappel de boîte aux lettres Exchange.
  
|**Nom de l’opération**|**Introduite dans**|
|:-----|:-----|
|[Opération GetReminders](getreminders-operation.md) <br/> |Exchange 2013  <br/> |
|[Opération PerformReminderAction](performreminderaction-operation.md) <br/> |Exchange 2013  <br/> |
   
Le tableau suivant répertorie les opérations de conversation de données de boîtes aux lettres Exchange.
  
|**Nom de l’opération**|**Introduite dans**|
|:-----|:-----|
|[Opération de ApplyConversationAction](applyconversationaction-operation.md) <br/> |Exchange 2010 Service Pack 1 (SP1)  <br/> |
|[FindConversation Operation](findconversation-operation.md) <br/> |Exchange 2010 SP1  <br/> |
|[Opération GetConversationItems](getconversationitems-operation.md) <br/> |Exchange 2013  <br/> |
   
Le tableau suivant répertorie les opérations d’utilitaires de données de boîtes aux lettres Exchange.
  
|**Nom de l’opération**|**Introduite dans**|
|:-----|:-----|
|[Opération ConvertId](convertid-operation.md) <br/> |Exchange 2007 Service Pack 1  <br/> |
|[Opération ExpandDL](expanddl-operation.md) <br/> |Exchange 2007  <br/> |
|[Opération GetUserPhoto](getuserphoto-operation.md) <br/> |Exchange 2013. Cette opération dispose d’un REST et une implémentation SOAP.  <br/> |
|[Opération MarkAsJunk](markasjunk-operation.md) <br/> |Exchange 2013  <br/> |
|[Opération ResolveNames](resolvenames-operation.md) <br/> |Exchange 2007  <br/> |
|[Opération GetPasswordExpirationDate](getpasswordexpirationdate-operation.md) <br/> |Exchange 2010 SP1  <br/> |
   
## <a name="availability-operations"></a>Opérations de disponibilité
<a name="bk_Availability"> </a>

Les opérations de disponibilité améliorent le calendrier et l’expérience de partage en fournissant plus riches, sécurisées et à jour et de disponibilité des informations disponible/occupé. Disponibilité des données sont un composant essentiel de la planification de réunions. Les opérations de disponibilité constituent un socle fiable pour une planification efficace. 
  
Le tableau suivant répertorie les opérations de disponibilité.
  
|**Nom de l’opération**|**Introduite dans**|
|:-----|:-----|
|[Opération GetUserAvailability](getuseravailability-operation.md) <br/> |Exchange 2007  <br/> |
|[Opération GetRoomLists](getroomlists-operation.md) <br/> |Exchange 2010  <br/> |
|[Opération GetRooms](getrooms-operation.md) <br/> |Exchange 2010  <br/> |
|[Opération GetUserOofSettings](getuseroofsettings-operation.md) <br/> |Exchange 2007  <br/> |
|[Opération SetUserOofSettings](setuseroofsettings-operation.md) <br/> |Exchange 2007  <br/> |
   
## <a name="bulk-transfer-operations"></a>Opérations de transfert en bloc
<a name="bk_bulk_transfer"> </a>

Les opérations de transfert en bloc permettent aux éléments de flux de données clients connecter et se déconnecter d’une boîte aux lettres. 
  
Le tableau suivant répertorie les opérations de transfert en bloc.
  
|**Nom de l’opération**|**Introduite dans**|
|:-----|:-----|
|[Opération UploadItems](uploaditems-operation.md) <br/> |Exchange 2010 SP1  <br/> |
|[Opération ExportItems](exportitems-operation.md) <br/> |Exchange 2010 SP1  <br/> |
   
## <a name="delegate-management-operations"></a>Déléguer les opérations de gestion
<a name="bk_delegate_management"> </a>

Opérations de gestion du délégué permettent aux clients d’ajouter, obtenir, mettre à jour et supprimer des délégués leurs boîtes aux lettres. 
  
Le tableau suivant répertorie les opérations de gestion de délégué.
  
|**Nom de l’opération**|**Introduite dans**|
|:-----|:-----|
|[Opération AddDelegate](adddelegate-operation.md) <br/> |Exchange 2007 Service Pack 1 (SP1)  <br/> |
|[Opération GetDelegate](getdelegate-operation.md) <br/> |Exchange 2007 SP1  <br/> |
|[Opération UpdateDelegate](updatedelegate-operation.md) <br/> |Exchange 2007 SP1  <br/> |
|[Opération RemoveDelegate](removedelegate-operation.md) <br/> |Exchange 2007 SP1  <br/> |
   
## <a name="inbox-rules-operations"></a>Opérations de règles de boîte de réception
<a name="bk_inbox_rules"> </a>

Les opérations de règles de boîte de réception permettent aux clients d’obtenir les règles de boîte de réception et les mettre à jour pour les messages sur le serveur. Les règles de boîte de réception sont des ensembles de conditions et actions associées qui permettent aux clients automatiquement organiser, classer et agir sur les messages que les messages sont remis dans un dossier. 
  
Le tableau suivant répertorie les opérations de règles de boîte de réception.
  
|**Nom de l’opération**|**Introduite dans**|
|:-----|:-----|
|[Opération de GetInboxRules](getinboxrules-operation.md) <br/> |Exchange 2010 SP1  <br/> |
|[Opération de UpdateInboxRules](updateinboxrules-operation.md) <br/> |Exchange 2010 SP1  <br/> |
   
## <a name="mail-app-management-operations"></a>Opérations de gestion d’application de messagerie
<a name="bk_mail_apps"> </a>

Les opérations de gestion des applications de messagerie permettent de gérer les applications de messagerie pour Outlook. Vous pouvez utiliser ces opérations pour installer, désinstaller, désactiver et obtenir des informations sur les applications de messagerie qui sont disponibles pour Outlook Web App et Outlook 2013.
  
Le tableau suivant répertorie les opérations de gestion des applications de messagerie.
  
|**Nom de l’opération**|**Introduite dans**|
|:-----|:-----|
|[Opération DisableApp](disableapp-operation.md) <br/> |Exchange 2013  <br/> |
|[Opération GetAppManifests](getappmanifests-operation.md) <br/> |Exchange 2013  <br/> |
|[Opération GetAppMarketplaceUrl](getappmarketplaceurl-operation.md) <br/> |Exchange 2013  <br/> |
|[Opération GetClientAccessToken](getclientaccesstoken-operation.md) <br/> |Exchange 2013  <br/> |
|[Opération InstallApp](installapp-operation.md) <br/> |Exchange 2013  <br/> |
|[Opération UninstallApp](uninstallapp-operation.md) <br/> |Exchange 2013  <br/> |
   
## <a name="mail-tips-operation"></a>Opération de conseils de messagerie
<a name="bk_mail_tips"> </a>

L’opération de conseils de messagerie permet aux clients pour demander des informations à partir du serveur sur les boîtes aux lettres de destinataires lorsqu’un auteur compose un message. Le tableau suivant répertorie l’opération de conseils de messagerie.
  
|**Nom de l’opération**|**Introduite dans**|
|:-----|:-----|
|[Opération GetMailTips](getmailtips-operation.md) <br/> |Exchange 2010  <br/> |
   
## <a name="message-tracking-operations"></a>Opérations de suivi des messages
<a name="bk_message_tracking"> </a>

Les opérations de suivi de message permettent aux clients pour rechercher les messages qui répondent aux critères spécifiés et pour obtenir des informations de suivi détaillé sur chaque message dans un rapport de suivi des messages. 
  
Le tableau suivant répertorie les opérations de suivi des messages.
  
|**Nom de l’opération**|**Introduite dans**|
|:-----|:-----|
|[Opération FindMessageTrackingReport](findmessagetrackingreport-operation.md) <br/> |Exchange 2010  <br/> |
|[Opération de GetMessageTrackingReport](getmessagetrackingreport-operation.md) <br/> |Exchange 2010  <br/> |
   
## <a name="notification-operations"></a>Opérations de notification
<a name="bk_notification"> </a>

Les opérations de notification avertir l’application cliente d’événements qui sont associés à des éléments et les dossiers à une boîte aux lettres spécifiée. Le modèle d’abonnement peut être basé sur push, type pull ou basée sur la diffusion en continu. 
  
Le tableau suivant répertorie les opérations de notification.
  
|**Nom de l’opération**|**Introduite dans**|
|:-----|:-----|
|[Opération de GetEvents](getevents-operation.md) <br/> |Exchange 2007  <br/> |
|[Opération de GetStreamingEvents](getstreamingevents-operation.md) <br/> |Exchange 2010 SP1  <br/> |
|[Opération d'abonnement](subscribe-operation.md) <br/> |Exchange 2007  <br/> |
|[Opération de résiliation d'abonnement](unsubscribe-operation.md) <br/> |Exchange 2007  <br/> |
   
## <a name="persona-operations"></a>Opérations de personnages
<a name="bk_personas"> </a>

Les opérations de personnage fournissent une interface pour rechercher et obtenir des informations sur un contact lié. Le tableau suivant répertorie les opérations personnage.
  
|**Nom de l’opération**|**Introduite dans**|
|:-----|:-----|
|[Opération FindPeople](findpeople-operation.md) <br/> |Exchange 2013  <br/> |
|[Opération GetPersona](getpersona-operation.md) <br/> |Exchange 2013  <br/> |
   
## <a name="retention-policy-operation"></a>Opération de stratégie de rétention
<a name="bk_retention_policy"> </a>

L’opération de stratégie de rétention fournit une liste de toutes les balises de rétention liées à la stratégie de rétention d’un utilisateur. 
  
Le tableau suivant répertorie l’opération de stratégie de rétention.
  
|**Nom de l’opération**|**Introduite dans**|
|:-----|:-----|
|[Opération GetUserRetentionPolicyTags](getuserretentionpolicytags-operation.md) <br/> |Exchange 2013  <br/> |
   
## <a name="service-configuration-operation"></a>Opération de configuration de service
<a name="bk_service_config"> </a>

L’opération de configuration de service permet aux clients d’obtenir des informations de configuration pour les services de messagerie unifiée, les règles de Protection, les conseils de stratégie et conseils de messagerie. 
  
Le tableau suivant répertorie l’opération de configuration de service.
  
|**Nom de l’opération**|**Introduite dans**|
|:-----|:-----|
|[Opération GetServiceConfiguration](getserviceconfiguration-operation.md) <br/> |Exchange 2010  <br/> |
   
## <a name="sharing-operations"></a>Opérations de partage
<a name="bk_sharing"> </a>

Les opérations de partage permettent aux clients de partager des données de calendrier et de contacts. 
  
Le tableau suivant répertorie les opérations de partage.
  
|**Nom de l’opération**|**Introduite dans**|
|:-----|:-----|
|[CreateItem (AcceptSharingInvitation)](createitem-acceptsharinginvitation.md) <br/> |Exchange 2010. Bien que l’opération **CreateItem** est applicable à toutes les versions de EWS, l’objet de réponse **AcceptSharingInvitation** est uniquement applicable à EWS dans les versions d’Exchange commençant par Exchange 2010.  <br/> |
|[Opération GetSharingFolder](getsharingfolder-operation.md) <br/> |Exchange 2010  <br/> |
|[Opération de GetSharingMetadata](getsharingmetadata-operation.md) <br/> |Exchange 2010  <br/> |
|[Opération RefreshSharingFolder](refreshsharingfolder-operation.md) <br/> |Exchange 2010  <br/> |
   
## <a name="synchronization-operations"></a>Opérations de synchronisation
<a name="bk_synchronization"> </a>

Les opérations de synchronisation fournissent une copie de mise en cache synchronisée à sens unique des dossiers et des éléments d’un utilisateur. 
  
Le tableau suivant répertorie les opérations de synchronisation.
  
|**Nom de l’opération**|**Introduite dans**|
|:-----|:-----|
|[Opération SyncFolderHierarchy](syncfolderhierarchy-operation.md) <br/> |Exchange 2007  <br/> |
|[Opération SyncFolderItems](syncfolderitems-operation.md) <br/> |Exchange 2007  <br/> |
   
## <a name="time-zone-operation"></a>Opération de fuseau horaire
<a name="bk_timezone"> </a>

L’opération de fuseau horaire permet aux clients d’obtenir une liste de définitions de fuseau horaire sont prises en charge par le serveur. 
  
Le tableau suivant répertorie l’opération de fuseau horaire.
  
|**Nom de l’opération**|**Introduite dans**|
|:-----|:-----|
|[Opération GetServerTimeZones](getservertimezones-operation.md) <br/> |Exchange 2010  <br/> |
   
## <a name="unified-messaging-operations"></a>Opérations de messagerie unifiées
<a name="bk_um"> </a>

Les opérations de la messagerie unifiée permettent aux clients pour lire les informations sur les propriétés de la messagerie unifiée et pour lire des messages de messagerie vocale par téléphone. 
  
Le tableau suivant répertorie les opérations de la messagerie unifiée.
  
|**Nom de l’opération**|**Introduite dans**|
|:-----|:-----|
|[Opération DisconnectPhoneCall](disconnectphonecall-operation.md) <br/> |Exchange 2010  <br/> |
|[Opération GetPhoneCallInformation](getphonecallinformation-operation.md) <br/> |Exchange 2010  <br/> |
|[Opération PlayOnPhone (EWS)](playonphone-operation-ews.md) <br/> |Exchange 2010  <br/> |
   
Utilisez l' [opération GetServiceConfiguration](getserviceconfiguration-operation.md) pour obtenir les informations de configuration de la messagerie unifiée pour une boîte aux lettres. Utilisez le service web de messagerie unifiée pour les applications de messagerie unifiée qui ciblent Exchange 2007. Pour plus d’informations, voir [messagerie unifiée une référence de service web pour Exchange](unified-messaging-web-service-reference-for-exchange.md).
  
## <a name="unified-contact-store-operations"></a>Opérations de magasin de contacts unifiées
<a name="bk_ucs"> </a>

Le magasin de contacts unifié fournit une expérience cohérente contact entre les produits Office et agit en tant que point d’intégration aux applications de tiers d’utiliser le même magasin de contacts. Il permet aux utilisateurs et applications stocker, gérer et accéder aux informations de contact et les rendre disponibles globalement dans Lync, Exchange 2013, Outlook, Outlook Web App et toute autre application qui implémente l’accès pour le magasin de contacts unifié. Exchange est le magasin de contenu pour l’expérience de magasin de contacts unifié.
  
Le tableau suivant répertorie les opérations de magasin de contacts unifié.
  
|**Nom de l’opération**|**Introduite dans**|
|:-----|:-----|
|[Opération AddNewImContactToGroup](addnewimcontacttogroup-operation.md) <br/> |Exchange 2013  <br/> |
|[Opération AddImContactToGroup](addimcontacttogroup-operation.md) <br/> |Exchange 2013  <br/> |
|[Opération AddImGroup](addimgroup-operation.md) <br/> |Exchange 2013  <br/> |
|[Opération AddNewTelUriContactToGroup](addnewteluricontacttogroup-operation.md) <br/> |Exchange 2013  <br/> |
|[Opération AddDistributionGroupToImList](adddistributiongrouptoimlist-operation.md) <br/> |Exchange 2013  <br/> |
|[Opération GetImItemList](getimitemlist-operation.md) <br/> |Exchange 2013  <br/> |
|[Opération GetImItems](getimitems-operation.md) <br/> |Exchange 2013  <br/> |
|[Opération RemoveContactFromImList](removecontactfromimlist-operation.md) <br/> |Exchange 2013  <br/> |
|[Opération RemoveImContactFromGroup](removeimcontactfromgroup-operation.md) <br/> |Exchange 2013  <br/> |
|[Opération RemoveDistributionGroupFromImList](removedistributiongroupfromimlist-operation.md) <br/> |Exchange 2013  <br/> |
|[Opération RemoveImGroup](removeimgroup-operation.md) <br/> |Exchange 2013  <br/> |
|[Opération SetImGroup](setimgroup-operation.md) <br/> |Exchange 2013  <br/> |
   
## <a name="user-configuration-operations"></a>Opérations de configuration utilisateur
<a name="bk_user_config"> </a>

Les opérations de configuration utilisateur permettent aux clients créer, supprimer, obtenir et mettre à jour les informations de configuration utilisateur. 
  
Le tableau suivant répertorie les opérations de configuration utilisateur.
  
|**Nom de l’opération**|**Introduite dans**|
|:-----|:-----|
|[Opération CreateUserConfiguration](createuserconfiguration-operation.md) <br/> |Exchange 2010  <br/> |
|[Opération DeleteUserConfiguration](deleteuserconfiguration-operation.md) <br/> |Exchange 2010  <br/> |
|[Opération GetUserConfiguration](getuserconfiguration-operation.md) <br/> |Exchange 2010  <br/> |
|[Opération UpdateUserConfiguration](updateuserconfiguration-operation.md) <br/> |Exchange 2010  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Explorer l'API managée EWS, EWS et les services web dans Exchange](../exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)
- [Commencer à utiliser les services web dans Exchange](../exchange-web-services/start-using-web-services-in-exchange.md)
- [Découverte automatique pour Exchange](../exchange-web-services/autodiscover-for-exchange.md)
    

