---
title: Opérations EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
api_name:
- Exchange
api_type:
- schema
ms.assetid: cf6fd871-9a65-4f34-8557-c8c71dd7ce09
description: Trouvez des informations sur les opérations EWS disponibles dans Exchange.
localization_priority: Priority
ms.openlocfilehash: 143903d9198a7e31e876adcbbb336df34ecf01fa
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526122"
---
# <a name="ews-operations-in-exchange"></a>Opérations EWS dans Exchange

Trouvez des informations sur les opérations EWS disponibles dans Exchange.
  
Les services Web Exchange (EWS) fournissent de nombreuses opérations qui vous permettent d’accéder à des informations à partir de la Banque d’informations Exchange. Les Articles de cette section fournissent des informations sur la structure globale des demandes, des réponses et des messages de réponse d’erreur pour les opérations EWS, ainsi que des exemples XML pour chaque opération. Elles fournissent une vue d’ensemble des structures de messages qui sont envoyées entre le client et le serveur. Vous pouvez utiliser ces informations pour déboguer des structures de messages et trouver des informations sur ce que vous pouvez faire dans une demande EWS. Pour plus d’informations sur ce que représente la structure XML, voir- [EWS XML Elements in Exchange](ews-xml-elements-in-exchange.md).
  
Toutes les fonctionnalités EWS sont associées à une version du schéma. De nouvelles versions de schéma EWS sont introduites dans les nouvelles versions d’Exchange Server ou d’Exchange Online. L’élément [RequestServerVersion](requestserverversion.md) contient un attribut de **version** qui mappe la version du serveur à la version de schéma. Cet article fournit des informations sur le moment où chaque opération a été introduite. Une fonctionnalité spécifique au sein d’une opération peut nécessiter une version ultérieure du service. Les schémas de version sont implémentés de sorte que les clients conçus avec une version antérieure d’EWS fonctionnent avec une version plus récente d’EWS. 
  
Ces opérations peuvent cibler le point de terminaison EWS qui services votre boîte aux lettres. Vous pouvez accéder au point de terminaison EWS à l’aide d’une URL de structure similaire à http:// <clientaccessserver> . com/EWS/Exchange. asmx, où <clientaccessserver> est le serveur d’accès au client Exchange qui sert de service à votre boîte aux lettres. Vous pouvez utiliser la découverte automatique pour obtenir l’URL du serveur d’accès au client qui utilise votre boîte aux lettres. Pour plus d’informations sur la découverte automatique, consultez la rubrique [découverte automatique pour Exchange](../exchange-web-services/autodiscover-for-exchange.md).
  
## <a name="ediscovery-operations"></a>opérations eDiscovery
<a name="bk_eDiscovery"> </a>

Les opérations eDiscovery fournissent des opérations de recherche pour les conservations légales et l’identification des données de boîte aux lettres qui ne peuvent pas être indexées et renvoyées dans les résultats de recherche de découverte.
  
Le tableau suivant répertorie les opérations eDiscovery.
  
|**Nom de l’opération**|**Nouveauté de**|
|:-----|:-----|
|[Opération GetDiscoverySearchConfiguration](getdiscoverysearchconfiguration-operation.md) <br/> |Exchange 2013  <br/> |
|[Opération GetHoldOnMailboxes](getholdonmailboxes-operation.md) <br/> |Exchange 2013  <br/> |
|[Opération GetNonIndexableItemDetails](getnonindexableitemdetails-operation.md) <br/> |Exchange 2013  <br/> |
|[Opération GetNonIndexableItemStatistics](getnonindexableitemstatistics-operation.md) <br/> |Exchange 2013  <br/> |
|[Opération GetSearchableMailboxes](getsearchablemailboxes-operation.md) <br/> |Exchange 2013  <br/> |
|[Opération SearchMailboxes](searchmailboxes-operation.md) <br/> |Exchange 2013  <br/> |
|[Opération SetHoldOnMailboxes](setholdonmailboxes-operation.md) <br/> |Exchange 2013  <br/> |
   
## <a name="exchange-mailbox-data-operations"></a>Opérations de données de boîte aux lettres Exchange
<a name="bk_Exchange_mailbox_data"> </a>

Les opérations de données de boîte aux lettres Exchange permettent aux clients de gérer et d’organiser des éléments, des dossiers et des pièces jointes, ainsi que la résolution de nom ambiguë et l’extension de liste de distribution. Les opérations de données de boîte aux lettres Exchange incluent les opérations sur les éléments, les dossiers, les pièces jointes et les utilitaires.
  
Le tableau suivant répertorie les opérations de données de boîte aux lettres Exchange.
  
|**Nom de l’opération**|**Nouveauté de**|
|:-----|:-----|
|[Opération ArchiveItem](archiveitem-operation.md) <br/> |Exchange 2013  <br/> |
|[Opération CreateItem](createitem-operation.md) <br/> |Exchange 2007  <br/> |
|[Opération CopyItem](copyitem-operation.md) <br/> |Exchange 2007  <br/> |
|[Opération DeleteItem](deleteitem-operation.md) <br/> |Exchange 2007  <br/> |
|[Opération FindItem](finditem-operation.md) <br/> |Exchange 2007  <br/> |
|[Opération GetItem](getitem-operation.md) <br/> |Exchange 2007  <br/> |
|[Opération MarkAllItemsAsRead](markallitemsasread-operation.md) <br/> |Exchange 2013  <br/> |
|[Opération MoveItem](moveitem-operation.md) <br/> |Exchange 2007  <br/> |
|[Opération SendItem](senditem-operation.md) <br/> |Exchange 2007  <br/> |
|[Opération UpdateItem](updateitem-operation.md) <br/> |Exchange 2007  <br/> |
   
Le tableau suivant répertorie les opérations de dossier de données de boîte aux lettres Exchange.
  
|**Nom de l’opération**|**Nouveauté de**|
|:-----|:-----|
|[Opération CreateFolder](createfolder-operation.md) <br/> |Exchange 2007  <br/> |
|[Opération CreateFolderPath](createfolderpath-operation.md) <br/> |Exchange 2013  <br/> |
|[Opération CreateManagedFolder](createmanagedfolder-operation.md) <br/> |Exchange 2007. Cette fonctionnalité a été déconseillée dans les versions d’Exchange à partir d’Exchange 2010. Pour plus d’informations sur la migration vers à l’aide de balises et de stratégies de rétention pour la gestion des enregistrements de messagerie, consultez la rubrique [migrer à partir de dossiers gérés](https://technet.microsoft.com/library/dd298032%28v=exchg.141%29.aspx).  <br/> |
|[CopyFolder, opération](copyfolder-operation.md) <br/> |Exchange 2007  <br/> |
|[Opération DeleteFolder](deletefolder-operation.md) <br/> |Exchange 2007  <br/> |
|[Opération EmptyFolder](emptyfolder-operation.md) <br/> |Exchange 2010  <br/> |
|[Opération FindFolder](findfolder-operation.md) <br/> |Exchange 2007  <br/> |
|[Opération GetFolder](getfolder-operation.md) <br/> |Exchange 2007  <br/> |
|[Opération MoveFolder](movefolder-operation.md) <br/> |Exchange 2007  <br/> |
|[Opération UpdateFolder](updatefolder-operation.md) <br/> |Exchange 2007  <br/> |
   
Le tableau suivant répertorie les opérations de pièces jointes de données de boîte aux lettres Exchange.
  
|**Nom de l’opération**|**Nouveauté de**|
|:-----|:-----|
|[Opération CreateAttachment](createattachment-operation.md) <br/> |Exchange 2007  <br/> |
|[Opération GetAttachment](getattachment-operation.md) <br/> |Exchange 2007  <br/> |
|[Opération DeleteAttachment](deleteattachment-operation.md) <br/> |Exchange 2007  <br/> |
   
Le tableau suivant répertorie les opérations de rappel de boîte aux lettres Exchange.
  
|**Nom de l’opération**|**Nouveauté de**|
|:-----|:-----|
|[Opération GetReminders](getreminders-operation.md) <br/> |Exchange 2013  <br/> |
|[Opération PerformReminderAction](performreminderaction-operation.md) <br/> |Exchange 2013  <br/> |
   
Le tableau suivant répertorie les opérations de conversation de données de boîte aux lettres Exchange.
  
|**Nom de l’opération**|**Nouveauté de**|
|:-----|:-----|
|[Opération de ApplyConversationAction](applyconversationaction-operation.md) <br/> |Exchange 2010 Service Pack 1 (SP1)  <br/> |
|[Opération FindConversation](findconversation-operation.md) <br/> |Exchange 2010 SP1  <br/> |
|[Opération GetConversationItems](getconversationitems-operation.md) <br/> |Exchange 2013  <br/> |
   
Le tableau suivant répertorie les opérations des utilitaires de données de boîte aux lettres Exchange.
  
|**Nom de l’opération**|**Nouveauté de**|
|:-----|:-----|
|[Opération ConvertId](convertid-operation.md) <br/> |Exchange 2007 Service Pack 1  <br/> |
|[Opération ExpandDL](expanddl-operation.md) <br/> |Exchange 2007  <br/> |
|[Opération GetUserPhoto](getuserphoto-operation.md) <br/> |Exchange 2013. Cette opération a un reste et une implémentation SOAP.  <br/> |
|[Opération MarkAsJunk](markasjunk-operation.md) <br/> |Exchange 2013  <br/> |
|[Opération ResolveNames](resolvenames-operation.md) <br/> |Exchange 2007  <br/> |
|[Opération GetPasswordExpirationDate](getpasswordexpirationdate-operation.md) <br/> |Exchange 2010 SP1  <br/> |
   
## <a name="availability-operations"></a>Opérations de disponibilité
<a name="bk_Availability"> </a>

Les opérations de disponibilité améliorent le calendrier et l’expérience de partage des informations de disponibilité en fournissant des informations de disponibilité et de disponibilité plus sûres, mises à jour et enrichies. Les données de disponibilité sont un élément essentiel de la planification des réunions. Les opérations de disponibilité fournissent une base fiable pour une planification efficace. 
  
Le tableau suivant répertorie les opérations de disponibilité.
  
|**Nom de l’opération**|**Nouveauté de**|
|:-----|:-----|
|[Opération GetUserAvailability](getuseravailability-operation.md) <br/> |Exchange 2007  <br/> |
|[Opération GetRoomLists](getroomlists-operation.md) <br/> |Exchange 2010  <br/> |
|[Opération GetRooms](getrooms-operation.md) <br/> |Exchange 2010  <br/> |
|[Opération GetUserOofSettings](getuseroofsettings-operation.md) <br/> |Exchange 2007  <br/> |
|[Opération SetUserOofSettings](setuseroofsettings-operation.md) <br/> |Exchange 2007  <br/> |
   
## <a name="bulk-transfer-operations"></a>Opérations de transfert en bloc
<a name="bk_bulk_transfer"> </a>

Les opérations de transfert en bloc permettent aux clients de diffuser des éléments dans une boîte aux lettres et de les en sortir. 
  
Le tableau suivant répertorie les opérations de transfert en bloc.
  
|**Nom de l’opération**|**Nouveauté de**|
|:-----|:-----|
|[Opération UploadItems](uploaditems-operation.md) <br/> |Exchange 2010 SP1  <br/> |
|[Opération ExportItems](exportitems-operation.md) <br/> |Exchange 2010 SP1  <br/> |
   
## <a name="delegate-management-operations"></a>Déléguer les opérations de gestion
<a name="bk_delegate_management"> </a>

Les opérations de gestion des délégués permettent aux clients d’ajouter, d’obtenir, de mettre à jour et de supprimer des délégués de leurs boîtes aux lettres. 
  
Le tableau suivant répertorie les opérations de gestion des délégués.
  
|**Nom de l’opération**|**Nouveauté de**|
|:-----|:-----|
|[Opération AddDelegate](adddelegate-operation.md) <br/> |Exchange 2007 Service Pack 1 (SP1)  <br/> |
|[Opération GetDelegate](getdelegate-operation.md) <br/> |Exchange 2007 SP1  <br/> |
|[Opération UpdateDelegate](updatedelegate-operation.md) <br/> |Exchange 2007 SP1  <br/> |
|[Opération RemoveDelegate](removedelegate-operation.md) <br/> |Exchange 2007 SP1  <br/> |
   
## <a name="inbox-rules-operations"></a>Opérations de règles de boîte de réception
<a name="bk_inbox_rules"> </a>

Les opérations de règles de boîte de réception permettent aux clients d’obtenir des règles de boîte de réception et de les mettre à jour pour les messages sur le serveur. Les règles de boîte de réception sont des ensembles de conditions et d’actions associées qui permettent aux clients d’organiser, de classer et d’agir automatiquement sur des messages lorsque les messages sont remis à un dossier. 
  
Le tableau suivant répertorie les opérations de règles de boîte de réception.
  
|**Nom de l’opération**|**Nouveauté de**|
|:-----|:-----|
|[Opération de GetInboxRules](getinboxrules-operation.md) <br/> |Exchange 2010 SP1  <br/> |
|[Opération de UpdateInboxRules](updateinboxrules-operation.md) <br/> |Exchange 2010 SP1  <br/> |
   
## <a name="mail-app-management-operations"></a>Opérations de gestion des applications de messagerie
<a name="bk_mail_apps"> </a>

Les opérations de gestion des applications de messagerie vous permettent de gérer les applications de messagerie pour Outlook. Vous pouvez utiliser ces opérations pour installer, désinstaller, désactiver et obtenir des informations sur les applications de messagerie disponibles pour Outlook Web App et Outlook 2013.
  
Le tableau suivant répertorie les opérations de gestion des applications de messagerie.
  
|**Nom de l’opération**|**Nouveauté de**|
|:-----|:-----|
|[Opération DisableApp](disableapp-operation.md) <br/> |Exchange 2013  <br/> |
|[Opération GetAppManifests](getappmanifests-operation.md) <br/> |Exchange 2013  <br/> |
|[Opération GetAppMarketplaceUrl](getappmarketplaceurl-operation.md) <br/> |Exchange 2013  <br/> |
|[Opération GetClientAccessToken](getclientaccesstoken-operation.md) <br/> |Exchange 2013  <br/> |
|[Opération InstallApp](installapp-operation.md) <br/> |Exchange 2013  <br/> |
|[Opération UninstallApp](uninstallapp-operation.md) <br/> |Exchange 2013  <br/> |
   
## <a name="mail-tips-operation"></a>Utilisation des conseils de messagerie
<a name="bk_mail_tips"> </a>

L’opération de conseils de messagerie permet aux clients de demander des informations au serveur sur les boîtes aux lettres des destinataires lorsqu’un auteur compose un message. Le tableau suivant répertorie l’opération de conseils de messagerie.
  
|**Nom de l’opération**|**Nouveauté de**|
|:-----|:-----|
|[Opération GetMailTips](getmailtips-operation.md) <br/> |Exchange 2010  <br/> |
   
## <a name="message-tracking-operations"></a>Opérations de suivi des messages
<a name="bk_message_tracking"> </a>

Les opérations de suivi des messages permettent aux clients de trouver les messages qui répondent aux critères spécifiés et d’obtenir des informations de suivi détaillées sur chaque message dans un rapport de suivi des messages. 
  
Le tableau suivant répertorie les opérations de suivi des messages.
  
|**Nom de l’opération**|**Nouveauté de**|
|:-----|:-----|
|[Opération FindMessageTrackingReport](findmessagetrackingreport-operation.md) <br/> |Exchange 2010  <br/> |
|[Opération de GetMessageTrackingReport](getmessagetrackingreport-operation.md) <br/> |Exchange 2010  <br/> |
   
## <a name="notification-operations"></a>Opérations de notification
<a name="bk_notification"> </a>

Les opérations de notification informent l’application cliente d’événements associés aux éléments et aux dossiers d’une boîte aux lettres spécifiée. Le modèle d’abonnement peut être basé sur les flux, l’extraction ou la diffusion en continu. 
  
Le tableau suivant répertorie les opérations de notification.
  
|**Nom de l’opération**|**Nouveauté de**|
|:-----|:-----|
|[Opération de GetEvents](getevents-operation.md) <br/> |Exchange 2007  <br/> |
|[Opération de GetStreamingEvents](getstreamingevents-operation.md) <br/> |Exchange 2010 SP1  <br/> |
|[Opération d'abonnement](subscribe-operation.md) <br/> |Exchange 2007  <br/> |
|[Opération de résiliation d'abonnement](unsubscribe-operation.md) <br/> |Exchange 2007  <br/> |
   
## <a name="persona-operations"></a>Opérations Persona
<a name="bk_personas"> </a>

Les opérations Persona dans le personnage fournissent une interface permettant de rechercher et d’obtenir des informations sur un contact lié. Le tableau suivant répertorie les opérations des personnages.
  
|**Nom de l’opération**|**Nouveauté de**|
|:-----|:-----|
|[Opération FindPeople](findpeople-operation.md) <br/> |Exchange 2013  <br/> |
|[Opération GetPersona](getpersona-operation.md) <br/> |Exchange 2013  <br/> |
   
## <a name="retention-policy-operation"></a>Opération de stratégie de rétention
<a name="bk_retention_policy"> </a>

L’opération de stratégie de rétention fournit une liste de toutes les balises de rétention liées à la stratégie de rétention d’un utilisateur. 
  
Le tableau suivant répertorie l’opération de stratégie de rétention.
  
|**Nom de l’opération**|**Nouveauté de**|
|:-----|:-----|
|[Opération GetUserRetentionPolicyTags](getuserretentionpolicytags-operation.md) <br/> |Exchange 2013  <br/> |
   
## <a name="service-configuration-operation"></a>Opération de configuration de service
<a name="bk_service_config"> </a>

L’opération de configuration du service permet aux clients d’obtenir des informations de configuration pour la messagerie unifiée, les règles de protection, les conseils de stratégie et les services de messagerie. 
  
Le tableau suivant répertorie l’opération de configuration de service.
  
|**Nom de l’opération**|**Nouveauté de**|
|:-----|:-----|
|[Opération GetServiceConfiguration](getserviceconfiguration-operation.md) <br/> |Exchange 2010  <br/> |
   
## <a name="sharing-operations"></a>Opérations de partage
<a name="bk_sharing"> </a>

Les opérations de partage permettent aux clients de partager des données de calendrier et des données de contacts. 
  
Le tableau suivant répertorie les opérations de partage.
  
|**Nom de l’opération**|**Nouveauté de**|
|:-----|:-----|
|[CreateItem (AcceptSharingInvitation)](createitem-acceptsharinginvitation.md) <br/> |Exchange 2010. Bien que l’opération **CreateItem** s’applique à toutes les versions d’EWS, l’objet de réponse **AcceptSharingInvitation** s’applique uniquement à EWS dans les versions d’exchange commençant par Exchange 2010.  <br/> |
|[Opération GetSharingFolder](getsharingfolder-operation.md) <br/> |Exchange 2010  <br/> |
|[Opération de GetSharingMetadata](getsharingmetadata-operation.md) <br/> |Exchange 2010  <br/> |
|[Opération RefreshSharingFolder](refreshsharingfolder-operation.md) <br/> |Exchange 2010  <br/> |
   
## <a name="synchronization-operations"></a>Opérations de synchronisation
<a name="bk_synchronization"> </a>

Les opérations de synchronisation fournissent une copie synchronisée unidirectionnelle mise en cache des dossiers et des éléments d’un utilisateur. 
  
Le tableau suivant répertorie les opérations de synchronisation.
  
|**Nom de l’opération**|**Nouveauté de**|
|:-----|:-----|
|[Opération Opérationsyncfolderhierarchy](syncfolderhierarchy-operation.md) <br/> |Exchange 2007  <br/> |
|[Opération SyncFolderItems](syncfolderitems-operation.md) <br/> |Exchange 2007  <br/> |
   
## <a name="time-zone-operation"></a>Opération de fuseau horaire
<a name="bk_timezone"> </a>

L’opération de fuseau horaire permet aux clients d’obtenir la liste des définitions de fuseau horaire prises en charge par le serveur. 
  
Le tableau suivant répertorie l’opération de fuseau horaire.
  
|**Nom de l’opération**|**Nouveauté de**|
|:-----|:-----|
|[Opération GetServerTimeZones](getservertimezones-operation.md) <br/> |Exchange 2010  <br/> |
   
## <a name="unified-messaging-operations"></a>Opérations de messagerie unifiée
<a name="bk_um"> </a>

Les opérations de messagerie unifiée permettent aux clients de lire des informations sur les propriétés de messagerie unifiée et de lire les messages vocaux par téléphone. 
  
Le tableau suivant répertorie les opérations de messagerie unifiée.
  
|**Nom de l’opération**|**Nouveauté de**|
|:-----|:-----|
|[Opération DisconnectPhoneCall](disconnectphonecall-operation.md) <br/> |Exchange 2010  <br/> |
|[Opération GetPhoneCallInformation](getphonecallinformation-operation.md) <br/> |Exchange 2010  <br/> |
|[Opération PlayOnPhone (EWS)](playonphone-operation-ews.md) <br/> |Exchange 2010  <br/> |
   
Utilisez l' [opération GetServiceConfiguration](getserviceconfiguration-operation.md) pour obtenir les informations de configuration de la messagerie unifiée pour une boîte aux lettres. Utilisez le service Web de messagerie unifiée pour les applications de messagerie unifiée qui ciblent Exchange 2007. Pour plus d’informations, consultez la rubrique [référence de service Web de messagerie unifiée pour Exchange](unified-messaging-web-service-reference-for-exchange.md).
  
## <a name="unified-contact-store-operations"></a>Opérations du magasin de contacts unifié
<a name="bk_ucs"> </a>

Le magasin de contacts unifié offre une expérience de contact cohérente entre les produits Office et agit comme un point d’intégration pour les applications tierces qui utiliseront le même magasin de contacts. Elle permet aux utilisateurs et aux applications de stocker, de gérer et d’accéder aux informations de contact et de les mettre à disposition de manière globale entre Lync, Exchange 2013, Outlook, Outlook Web App et toute autre application qui implémente l’accès au magasin de contacts unifié. Exchange est le magasin de contenu pour l’expérience du magasin de contacts unifié.
  
Le tableau suivant répertorie les opérations du magasin de contacts unifié.
  
|**Nom de l’opération**|**Nouveauté de**|
|:-----|:-----|
|[Opération AddNewImContactToGroup](addnewimcontacttogroup-operation.md) <br/> |Exchange 2013  <br/> |
|[Opération AddImContactToGroup](addimcontacttogroup-operation.md) <br/> |Exchange 2013  <br/> |
|[Opération AddImGroup](addimgroup-operation.md) <br/> |Exchange 2013  <br/> |
|[Opération AddNewTelUriContactToGroup](addnewteluricontacttogroup-operation.md) <br/> |Exchange 2013  <br/> |
|[Opération AddDistributionGroupToImList](adddistributiongrouptoimlist-operation.md) <br/> |Exchange 2013  <br/> |
|[Opération GetImItemList](getimitemlist-operation.md) <br/> |Exchange 2013  <br/> |
|[Opération GetImItems](getimitems-operation.md) <br/> |Exchange 2013  <br/> |
|[Opération RemoveContactFromImList](removecontactfromimlist-operation.md) <br/> |Exchange 2013  <br/> |
|[Opération RemoveImContactFromGroup](removeimcontactfromgroup-operation.md) <br/> |Exchange 2013  <br/> |
|[Opération RemoveDistributionGroupFromImList](removedistributiongroupfromimlist-operation.md) <br/> |Exchange 2013  <br/> |
|[Opération RemoveImGroup](removeimgroup-operation.md) <br/> |Exchange 2013  <br/> |
|[Opération SetImGroup](setimgroup-operation.md) <br/> |Exchange 2013  <br/> |
   
## <a name="user-configuration-operations"></a>Opérations de configuration de l’utilisateur
<a name="bk_user_config"> </a>

Les opérations de configuration de l’utilisateur permettent aux clients de créer, supprimer, obtenir et mettre à jour les informations de configuration de l’utilisateur. 
  
Le tableau suivant répertorie les opérations de configuration de l’utilisateur.
  
|**Nom de l’opération**|**Nouveauté de**|
|:-----|:-----|
|[Opération CreateUserConfiguration](createuserconfiguration-operation.md) <br/> |Exchange 2010  <br/> |
|[Opération DeleteUserConfiguration](deleteuserconfiguration-operation.md) <br/> |Exchange 2010  <br/> |
|[Opération GetUserConfiguration](getuserconfiguration-operation.md) <br/> |Exchange 2010  <br/> |
|[Opération UpdateUserConfiguration](updateuserconfiguration-operation.md) <br/> |Exchange 2010  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Explorer l'API managée EWS, l’EWS et les services web dans Exchange](../exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)
- [Commencer à utiliser les services web dans Exchange](../exchange-web-services/start-using-web-services-in-exchange.md)
- [Découverte automatique pour Exchange](../exchange-web-services/autodiscover-for-exchange.md)
    

