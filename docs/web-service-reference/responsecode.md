---
title: ResponseCode
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResponseCode
api_type:
- schema
ms.assetid: 4b84d670-74c9-4d6d-84e7-f0a9f76f0d93
description: L’élément ResponseCode fournit des informations d’état sur la demande.
ms.openlocfilehash: 7baeb0ab87ffb43ba9d6b4016477888aa4ed613e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829294"
---
# <a name="responsecode"></a>ResponseCode

L’élément **ResponseCode** fournit des informations d’état sur la demande. 
  
- [ResponseMessage](responsemessage.md) 
- [ResponseCode](responsecode.md)
  
```XML
<ResponseCode/>
```

**ResponseCodeType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|Élément|Description|
|:-----|:-----|
|[ResponseMessage](responsemessage.md) <br/> | Fournit des informations descriptives concernant l’état de réponse.<br/><br/>  Les expressions XPath possibles de cet élément sont les suivantes :<br/><br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/ResponseMessage` <br/><br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/ResponseMessage` <br/><br/>  `/SetUserOofSettingsResponse/ResponseMessage` <br/><br/>  `/GetUserOofSettingsResponse/ResponseMessage` <br/> |
|[DeleteItemResponseMessage](deleteitemresponsemessage.md) <br/> |Contient l’état et les résultats d’une seule demande [d’opération DeleteItem](deleteitem-operation.md) .  <br/> |
|[SendItemResponseMessage](senditemresponsemessage.md) <br/> |Contient l’état et les résultats d’une seule demande [d’opération SendItem](senditem-operation.md) .  <br/> |
|[DeleteFolderResponseMessage](deletefolderresponsemessage.md) <br/> |Contient l’état et les résultats d’une seule demande [d’opération DeleteFolder](deletefolder-operation.md) .  <br/> |
|[DeleteAttachmentResponseMessage](deleteattachmentresponsemessage.md) <br/> |Contient l’état et les résultats d’une seule demande [d’opération DeleteAttachment](deleteattachment-operation.md) .  <br/> |
|[UnsubscribeResponseMessage](unsubscriberesponsemessage.md) <br/> |Contient l’état et les résultats d’une seule demande [d’opération Annuler l’abonnement](unsubscribe-operation.md) .  <br/> |
|[CreateFolderResponseMessage](createfolderresponsemessage.md) <br/> |Contient l’état et les résultats d’une seule demande [d’opération CreateFolder](createfolder-operation.md) .  <br/> |
|[GetFolderResponseMessage](getfolderresponsemessage.md) <br/> |Contient l’état et les résultats d’une seule demande [d’opération GetFolder](getfolder-operation.md) .  <br/> |
|[UpdateFolderResponseMessage](updatefolderresponsemessage.md) <br/> |Contient l’état et les résultats d’une seule demande [d’opération UpdateFolder](updatefolder-operation.md) .  <br/> |
|[MoveFolderResponseMessage](movefolderresponsemessage.md) <br/> |Contient l’état et les résultats d’une seule demande [d’opération MoveFolder](movefolder-operation.md) .  <br/> |
|[CopyFolderResponseMessage](copyfolderresponsemessage.md) <br/> |Contient l’état et les résultats d’une seule demande [d’opération CopyFolder](copyfolder-operation.md).  <br/> |
|[CreateManagedFolderResponseMessage](createmanagedfolderresponsemessage.md) <br/> |Contient l’état et les résultats d’une seule demande [d’opération CreateManagedFolder](createmanagedfolder-operation.md) .  <br/> |
|[FindFolderResponseMessage](findfolderresponsemessage.md) <br/> |Contient l’état et les résultats d’une seule demande [d’opération FindFolder](findfolder-operation.md) .  <br/> |
|[CreateItemResponseMessage](createitemresponsemessage.md) <br/> |Contient l’état et les résultats d’une seule demande [CreateItem operation](createitem-operation.md) .  <br/> |
|[GetItemResponseMessage](getitemresponsemessage.md) <br/> |Contient l’état et les résultats d’une seule demande [GetItem operation](getitem-operation.md) .  <br/> |
|[UpdateItemResponseMessage](updateitemresponsemessage.md) <br/> |Contient l’état et les résultats d’une seule demande [d’opération UpdateItem](updateitem-operation.md) .  <br/> |
|[MoveItemResponseMessage](moveitemresponsemessage.md) <br/> |Contient l’état et les résultats d’une seule demande [d’opération MoveItem](moveitem-operation.md) .  <br/> |
|[CopyItemResponseMessage](copyitemresponsemessage.md) <br/> |Contient l’état et les résultats d’une seule demande [d’opération CopyItem](copyitem-operation.md) .  <br/> |
|[CreateAttachmentResponseMessage](createattachmentresponsemessage.md) <br/> |Contient l’état et les résultats d’une seule demande [d’opération CreateAttachment](createattachment-operation.md) .  <br/> |
|[GetAttachmentResponseMessage](getattachmentresponsemessage.md) <br/> |Contient l’état et les résultats d’une seule demande [d’opération GetAttachment](getattachment-operation.md) .  <br/> |
|[FindItemResponseMessage](finditemresponsemessage.md) <br/> |Contient l’état et les résultats d’une seule demande [d’opération FindItem](finditem-operation.md) .  <br/> |
|[ResolveNamesResponseMessage](resolvenamesresponsemessage.md) <br/> |Contient l’état et les résultats d’une demande [d’opération ResolveNames](resolvenames-operation.md) .  <br/> |
|[ExpandDLResponseMessage](expanddlresponsemessage.md) <br/> |Contient l’état et les résultats d’une seule demande [d’opération ExpandDL](expanddl-operation.md) .  <br/> |
|[SubscribeResponseMessage](subscriberesponsemessage.md) <br/> |Contient l’état et les résultats d’une seule demande [d’opération de s’abonner](subscribe-operation.md) .  <br/> |
|[GetEventsResponseMessage](geteventsresponsemessage.md) <br/> |Contient l’état et les résultats d’une seule demande [d’opération GetEvents](getevents-operation.md) .  <br/> |
|[SendNotificationResponseMessage](sendnotificationresponsemessage.md) <br/> |Contient l’état et les résultats d’une demande d’opération SendNotification unique.  <br/> |
|[SyncFolderHierarchyResponseMessage](syncfolderhierarchyresponsemessage.md) <br/> |Contient l’état et les résultats d’une demande [d’opération SyncFolderHierarchy](syncfolderhierarchy-operation.md) .  <br/> |
|[SyncFolderItemsResponseMessage](syncfolderitemsresponsemessage.md) <br/> |Contient l’état et les résultats d’une demande [d’opération SyncFolderItems](syncfolderitems-operation.md) .  <br/> |
|[ConvertIdResponseMessage](convertidresponsemessage.md) <br/> |Contient l’état et les résultats d’une demande [d’opération ConvertId](convertid-operation.md) .  <br/> |
|[AddDelegateResponse](adddelegateresponse.md) <br/> |Contient l’état et les résultats d’une requête [d’opération AddDelegate](adddelegate-operation.md) .  <br/> |
|[GetDelegateResponse](getdelegateresponse.md) <br/> |Contient l’état et les résultats d’une demande [d’opération GetDelegate](getdelegate-operation.md) .  <br/> |
|[RemoveDelegateResponse](removedelegateresponse.md) <br/> |Contient l’état et les résultats d’une demande [d’opération RemoveDelegate](removedelegate-operation.md) .  <br/> |
|[UpdateDelegateResponse](updatedelegateresponse.md) <br/> |Contient l’état et les résultats d’une requête [d’opération UpdateDelegate](updatedelegate-operation.md) .  <br/> |
|[GetServerTimeZonesResponseMessage](getservertimezonesresponsemessage.md) <br/> |Contient l’état et les résultats d’une demande [d’opération GetServerTimeZones](getservertimezones-operation.md) .  <br/> |
|[GetSharingFolderResponseMessage](getsharingfolderresponsemessage.md) <br/> |Contient l’état et les résultats d’une demande [d’opération GetSharingFolder](getsharingfolder-operation.md) .  <br/> |
|[GetSharingFolderResponse](getsharingfolderresponse.md) <br/> |Définit une réponse à une demande [d’opération GetSharingFolder](getsharingfolder-operation.md) .  <br/> |
|[GetSharingMetadataResponseMessage](getsharingmetadataresponsemessage.md) <br/> |Contient l’état et les résultats d’une demande [d’opération GetSharingMetadata](getsharingmetadata-operation.md) .  <br/> |
|[GetSharingMetadataResponse](getsharingmetadataresponse.md) <br/> |Définit une réponse à une demande de [Opération de GetSharingMetadata](getsharingmetadata-operation.md) .  <br/> |
|[RefreshSharingFolderResponseMessage](refreshsharingfolderresponsemessage.md) <br/> |Contient l’état et les résultats d’une demande [d’opération RefreshSharingFolder](refreshsharingfolder-operation.md) .  <br/> |
|[RefreshSharingFolderResponse](refreshsharingfolderresponse.md) <br/> |Définit une réponse à une demande [d’opération RefreshSharingFolder](refreshsharingfolder-operation.md) .  <br/> |
|[FindConversationResponse](findconversationresponse.md) <br/> |Contient l’état et les résultats d’une réponse de [l’opération FindConversation](findconversation-operation.md) .  <br/> |
|[ApplyConversationActionResponseMessage](applyconversationactionresponsemessage.md) <br/> |Contient l’état et les résultats d’une requête [d’opération ApplyConversationAction](applyconversationaction-operation.md) .  <br/> |
|[EmptyFolderResponseMessage](emptyfolderresponsemessage.md) <br/> |Contient l’état et les résultats d’une seule demande [d’opération EmptyFolder](emptyfolder-operation.md) .  <br/> |
|[UpdateInboxRulesResponse](updateinboxrulesresponse.md) <br/> |Contient un état et les résultats d’une requête [d’opération UpdateInboxRules](updateinboxrules-operation.md) .  <br/> |
|[UploadItemsResponseMessage](uploaditemsresponsemessage.md) <br/> |Contient un état et les résultats d’une requête [d’opération UploadItems](uploaditems-operation.md) .  <br/> |
|[GetInboxRulesResponse](getinboxrulesresponse.md) <br/> |Contient une réponse à une [opération GetInboxRules](getinboxrules-operation.md) *** demande.  <br/> |
|[GetServiceConfigurationResponse](getserviceconfigurationresponse.md) <br/> |Contient une réponse à une demande [d’opération GetServiceConfiguration](getserviceconfiguration-operation.md) .  <br/> |
|[ServiceConfigurationResponseMessageType](serviceconfigurationresponsemessagetype.md) <br/> |Contient les paramètres de configuration de service.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Une valeur de texte est obligatoire si cet élément est utilisé. Le tableau suivant décrit les valeurs qui sont retournées avec cet élément.
  
|Valeur|Description|
|:-----|:-----|
|NoError  <br/> |Aucune erreur ne s’est produite lors de la demande.  <br/> |
|ErrorAccessDenied  <br/> |Cette erreur se produit lorsque le compte d’appel n’a pas les droits pour exécuter l’action demandée.  <br/> |
|ErrorAccessModeSpecified  <br/> |Cette erreur est à usage interne uniquement. Cette erreur n’est pas retournée.  <br/> |
|ErrorAccountDisabled  <br/> |Cette erreur se produit lorsque le compte en question a été désactivé.  <br/> |
|ErrorAddDelegatesFailed  <br/> |Cette erreur se produit lorsqu’une liste avec ajoutés délégués ne peuvent pas être enregistrée.  <br/> |
|ErrorAddressSpaceNotFound  <br/> |Cette erreur se produit lorsque l’enregistrement d’espace d’adresse ou nom de domaine du nom de domaine DNS (Domain Name System), pour la disponibilité inter-forêts est introuvable dans la base de données Active Directory.  <br/> |
|ErrorADOperation  <br/> |Cette erreur se produit lorsque l’opération a échoué en raison de problèmes de communication avec les Services de domaine Active Directory (AD DS).  <br/> |
|ErrorADSessionFilter  <br/> |Cette erreur est retournée lorsqu’une demande d’opération **ResolveNames** spécifie un nom qui n’est pas valide.  <br/> |
|ErrorADUnavailable  <br/> |Cette erreur se produit lorsque les services AD DS n’est pas disponible. Réessayer ultérieurement.  <br/> |
|ErrorAffectedTaskOccurrencesRequired  <br/> |Cette erreur indique que l’attribut **AffectedTaskOccurrences** n’a pas été spécifié. Lorsque l’élément [DeleteItem](deleteitem.md) est utilisée pour supprimer au moins un élément est une tâche, et si cette tâche périodique ou non, indépendamment de l’attribut **AffectedTaskOccurrences** doit être spécifié pour pouvoir **DeleteItem** permet de déterminer si Pour supprimer l’occurrence en cours ou la série entière.  <br/> |
|ErrorArchiveFolderPathCreation  <br/> |Indique une erreur dans la création de chemin d’accès du dossier archive.  <br/> |
|ErrorArchiveMailboxNotEnabled  <br/> |Indique que la boîte aux lettres d’archive n’a pas été activé.  <br/> |
|ErrorArchiveMailboxServiceDiscoveryFailed  <br/> |Indique que détection du service archive boîte aux lettres a échoué.  <br/> |
|ErrorAttachmentNestLevelLimitExceeded  <br/> |Spécifie qu’une tentative a été effectuée pour créer un élément avec plus de 10 pièces jointes imbriquées. Cette valeur a été introduite dans Exchange Server 2010 Service Pack 2 (SP2).  <br/> |
|ErrorAttachmentSizeLimitExceeded  <br/> |L’élément [CreateAttachment](createattachment.md) renvoie cette erreur si une tentative est effectuée pour créer une pièce jointe avec une taille supérieure à Int32.MaxValue, en octets.  <br/> L’élément [GetAttachment](getattachment.md) renvoie cette erreur si vous tentez de récupérer une pièce jointe existante avec une taille supérieure à Int32.MaxValue, en octets.  <br/> |
|ErrorAutoDiscoverFailed  <br/> |Cette erreur indique que des Services Web Exchange a tenté de déterminer l’emplacement d’un ordinateur entre les forêts exécutant Exchange 2010 qui a le rôle de serveur d’accès au Client installé à l’aide du service de découverte automatique, mais l’appel vers le service de découverte automatique a échoué.  <br/> |
|ErrorAvailabilityConfigNotFound  <br/> |Cette erreur indique que les informations de configuration de disponibilité pour la forêt locale sont manquantes dans AD DS.  <br/> |
|ErrorBatchProcessingStopped  <br/> | Cette erreur indique qu’une exception s’est produite lors du traitement d’un élément et que l’exception est susceptible de se produire pour les éléments qui suivent. Demandes peuvent inclure plusieurs éléments ; par exemple, une demande d’opération GetItem peut contenir plusieurs identificateurs. En règle générale, les éléments sont traités un à la fois. Si une exception se produit lors du traitement d’un élément et que cette exception est susceptible de se produire pour les éléments qui suivent, les éléments qui suivent ne seront pas traitées.  <br/><br/>  Voici quelques exemples d’erreurs qui va arrêter le traitement des éléments qui suivent :<br/>  <br/>-ErrorAccessDenied  <br/>-ErrorAccountDisabled  <br/>-ErrorADUnavailable  <br/>-ErrorADOperation  <br/>-ErrorConnectionFailed  <br/>-ErrorMailboxStoreUnavailable  <br/>-ErrorMailboxMoveInProgress  <br/>-ErrorPasswordChangeRequired  <br/>-ErrorPasswordExpired  <br/>-ErrorQuotaExceeded  <br/>-ErrorInsufficientResources  <br/> |
|ErrorCalendarCannotMoveOrCopyOccurrence  <br/> |Cette erreur se produit lorsqu’une tentative est effectuée pour déplacer ou copier une occurrence d’un élément de calendrier périodique.  <br/> |
|ErrorCalendarCannotUpdateDeletedItem  <br/> | Cette erreur se produit lorsqu’une tentative est effectuée pour mettre à jour un élément de calendrier qui se trouve dans le dossier éléments supprimés et lorsque les mises à jour de réunion ou les annulations doivent être envoyées en fonction de la valeur de l’attribut **SendMeetingInvitationsOrCancellations** . <br/><br/>Les valeurs possibles de cet attribut sont les suivantes :  <br/><br/>-SendToAllAndSaveCopy  <br/>-SendToChangedAndSaveCopy  <br/>-SendOnlyToAll  <br/>-SendOnlyToChanged  <br/>  <br/>Toutefois, une mise à jour est autorisé uniquement lorsque la valeur de cet attribut est définie sur SendToNone.  <br/> |
|ErrorCalendarCannotUseIdForOccurrenceId  <br/> |Cette erreur se produit lorsque l’opération UpdateItem, GetItem, DeleteItem, MoveItem, CopyItem ou SendItem est appelée et l’ID spécifié n’est pas un ID d’occurrence d’un élément de calendrier périodique.  <br/> |
|ErrorCalendarCannotUseIdForRecurringMasterId  <br/> |Cette erreur se produit lorsque l’opération **UpdateItem**, **GetItem**, **DeleteItem**, **MoveItem**, **CopyItem**ou **SendItem** est appelée et l’ID spécifié n’est pas un ID d’un rendez-vous périodique.  <br/> |
|ErrorCalendarDurationIsTooLong  <br/> |Cette erreur se produit pendant une opération **CreateItem** ou **UpdateItem** lorsqu’une durée d’élément de calendrier dépasse le nombre maximal autorisé, qui est actuellement 5 ans.  <br/> |
|ErrorCalendarEndDateIsEarlierThanStartDate  <br/> |Cette erreur se produit lorsqu’une heure de fin du calendrier est définie sur le même temps ou après l’heure de début.  <br/> |
|ErrorCalendarFolderIsInvalidForCalendarView  <br/> |Cette erreur se produit lorsque le dossier spécifié pour une opération **FindItem** avec un élément [CalendarView](calendarview.md) n’est pas du type de dossier de calendrier.  <br/> |
|ErrorCalendarInvalidAttributeValue  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorCalendarInvalidDayForTimeChangePattern  <br/> |Cette erreur se produit pendant une opération **CreateItem** ou **UpdateItem** lorsque des valeurs non valides de jour, WeekendDay et Weekday sont utilisées pour définir le modèle de changement.  <br/> |
|ErrorCalendarInvalidDayForWeeklyRecurrence  <br/> |Cette erreur se produit pendant une opération **CreateItem** ou **UpdateItem** lorsque des valeurs non valides de jour, semaine et WeekendDay sont utilisées pour spécifier la périodicité hebdomadaire.  <br/> |
|ErrorCalendarInvalidPropertyState  <br/> |Cette erreur se produit lorsque l’état d’un calendrier élément périodicité BLOB binary large object () dans la banque d’informations Exchange n’est pas valide.  <br/> |
|ErrorCalendarInvalidPropertyValue  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorCalendarInvalidRecurrence  <br/> |Cette erreur se produit lorsque la périodicité spécifiée ne peut pas être créée.  <br/> |
|ErrorCalendarInvalidTimeZone  <br/> |Cette erreur se produit lorsqu’un fuseau horaire non valide est détecté.  <br/> |
|ErrorCalendarIsCancelledForAccept  <br/> |Cette erreur indique qu’un élément de calendrier a été annulé.  <br/> |
|ErrorCalendarIsCancelledForDecline  <br/> |Cette erreur indique qu’un élément de calendrier a été annulé.  <br/> |
|ErrorCalendarIsCancelledForRemove  <br/> |Cette erreur indique qu’un élément de calendrier a été annulé.  <br/> |
|ErrorCalendarIsCancelledForTentative  <br/> |Cette erreur indique qu’un élément de calendrier a été annulé.  <br/> |
|ErrorCalendarIsDelegatedForAccept  <br/> |Cette erreur indique que l’élément [AcceptItem](acceptitem.md) n’est pas valide pour une demande de réunion ou d’élément de calendrier dans un scénario de délégation.  <br/> |
|ErrorCalendarIsDelegatedForDecline  <br/> |Cette erreur indique que l’élément [DeclineItem](declineitem.md) est non valide pour une demande de réunion ou d’élément de calendrier dans un scénario de délégation.  <br/> |
|ErrorCalendarIsDelegatedForRemove  <br/> |Cette erreur indique que l’élément [RemoveItem](removeitem.md) est non valide pour une annulation de réunion dans un scénario de délégation.  <br/> |
|ErrorCalendarIsDelegatedForTentative  <br/> |Cette erreur indique que l’élément [TentativelyAcceptItem](tentativelyacceptitem.md) n’est pas valide pour une demande de réunion ou d’élément de calendrier dans un scénario de délégation.  <br/> |
|ErrorCalendarIsNotOrganizer  <br/> |Cette erreur indique que l’opération (actuellement CancelItem) sur l’élément de calendrier non valide pour un participant. L’organisateur de la réunion peut annuler la réunion.  <br/> |
|ErrorCalendarIsOrganizerForAccept  <br/> |Cette erreur indique que [AcceptItem](acceptitem.md) n’est pas valide pour l’élément de calendrier de l’organisateur.  <br/> |
|ErrorCalendarIsOrganizerForDecline  <br/> |Cette erreur indique que [DeclineItem](declineitem.md) est non valide pour l’élément de calendrier de l’organisateur.  <br/> |
|ErrorCalendarIsOrganizerForRemove  <br/> |Cette erreur indique que [RemoveItem](removeitem.md) est non valide pour l’élément de calendrier de l’organisateur. Pour supprimer une réunion à partir du calendrier, l’organisateur doit utiliser CancelCalendarItem.  <br/> |
|ErrorCalendarIsOrganizerForTentative  <br/> |Cette erreur indique que [TentativelyAcceptItem](tentativelyacceptitem.md) n’est pas valide pour l’élément de calendrier de l’organisateur.  <br/> |
|ErrorCalendarMeetingRequestIsOutOfDate  <br/> |Cette erreur indique qu’une demande de réunion est obsolète et ne peut pas être mis à jour.  <br/> |
|ErrorCalendarOccurrenceIndexIsOutOfRecurrenceRange  <br/> |Cette erreur indique que l’index de l’occurrence ne pointe pas vers une occurrence dans la périodicité actuelle. Par exemple, si votre modèle de périodicité définit un ensemble de trois occurrences de réunion et que vous essayez d’accéder à la cinquième occurrence, ce code de réponse entraînera.  <br/> |
|ErrorCalendarOccurrenceIsDeletedFromRecurrence  <br/> |Cette erreur indique que toute opération sur une occurrence supprimée (adressée via périodique index ID et l’occurrence maître) n’est pas valide.  <br/> |
|ErrorCalendarOutOfRange  <br/> |Cette erreur est signalée sur les opérations CreateItem et UpdateItem des éléments de calendrier ou des propriétés de périodicité de tâche lorsque la valeur de la propriété est en dehors des limites. Par exemple, spécifiant la semaine du mois quinzième entraînera ce code de réponse.  <br/> |
|ErrorCalendarViewRangeTooBig  <br/> |Cette erreur se produit quand commencer à la plage de fin pour l’élément [CalendarView](calendarview.md) est supérieure à la valeur maximale autorisée, actuellement 2 ans.  <br/> |
|ErrorCallerIsInvalidADAccount  <br/> |Cette erreur indique que le compte effectuant la demande n’est pas un compte valid dans la base de données de l’annuaire.  <br/> |
|ErrorCannotArchiveCalendarContactTaskFolderException  <br/> |Indique qu’une tentative a été effectuée pour archiver un dossier contacts de tâche de calendrier.  <br/> |
|ErrorCannotArchiveItemsInPublicFolders  <br/> |Indique qu’une tentative a été effectuée pour archiver des éléments dans les dossiers publics.  <br/> |
|ErrorCannotArchiveItemsInArchiveMailbox  <br/> |Indique que vous avez tenté d’archiver des éléments dans la boîte aux lettres d’archive.  <br/> |
|ErrorCannotCreateCalendarItemInNonCalendarFolder  <br/> |Cette erreur se produit lorsqu’un élément de calendrier est en cours de création et de l’attribut **SavedItemFolderId** fait référence à un dossier de calendrier non.  <br/> |
|ErrorCannotCreateContactInNonContactFolder  <br/> |Cette erreur se produit lorsqu’un contact est en cours de création et l’attribut **SavedItemFolderId** fait référence à un dossier sans contact.  <br/> |
|ErrorCannotCreatePostItemInNonMailFolder  <br/> |Cette erreur indique qu’un élément de publication ne peut pas être créé dans un dossier autre qu’un dossier de messagerie, tels que le calendrier, contacts, tâches, Notes et ainsi de suite.  <br/> |
|ErrorCannotCreateTaskInNonTaskFolder  <br/> |Cette erreur se produit lorsqu’une tâche est en cours de création et l’attribut **SavedItemFolderId** fait référence à un dossier autre tâche.  <br/> |
|ErrorCannotDeleteObject  <br/> |Cette erreur se produit lorsque l’élément ou le dossier à supprimer ne peut pas être supprimée.  <br/> |
|ErrorCannotDeleteTaskOccurrence  <br/> |L' [opération DeleteItem](deleteitem-operation.md) renvoie cette erreur lorsqu’il ne peut pas supprimer l’occurrence en cours d’une tâche périodique. Cela peut se produire uniquement si l’attribut **AffectedTaskOccurrences** a la valeur SpecifiedOccurrenceOnly.  <br/> |
|ErrorCannotDisableMandatoryExtension  <br/> |Indique qu’une tentative a été effectuée pour désactiver une extension mandatorty.  <br/> |
|ErrorCannotEmptyFolder  <br/> |Cette erreur doit être renvoyée lorsque le serveur ne peut pas vider un dossier.  <br/> |
|ErrorCannotGetSourceFolderPath  <br/> |Indique que le chemin d’accès du dossier source pas pu être récupéré.  <br/> |
|ErrorCannotGetExternalEcpUrl  <br/> |Spécifie que le serveur a pas pu récupérer l’URL externe pour les Options d’Outlook Web App.  <br/> |
|ErrorCannotOpenFileAttachment  <br/> |L’opération **GetAttachment** renvoie cette erreur si elle ne peut pas récupérer le corps d’une pièce jointe.  <br/> |
|ErrorCannotSetCalendarPermissionOnNonCalendarFolder  <br/> |Cette erreur indique que l’appelant a essayé de définir des autorisations de calendrier dans un dossier de calendrier non.  <br/> |
|ErrorCannotSetNonCalendarPermissionOnCalendarFolder  <br/> |Cette erreur indique que l’appelant a essayé de définir des autorisations de calendrier non sur un dossier de calendrier.  <br/> |
|ErrorCannotSetPermissionUnknownEntries  <br/> |Cette erreur indique que vous ne pouvez pas définir des autorisations inconnues dans un jeu d’autorisations.  <br/> |
|ErrorCannotSpecifySearchFolderAsSourceFolder  <br/> |Indique qu’une tentative a été effectuée pour spécifier le dossier de recherche que le dossier source.  <br/> |
|ErrorCannotUseFolderIdForItemId  <br/> |Cette erreur se produit lorsqu’une demande qui requiert un identificateur d’élément reçoit un identificateur de dossier.  <br/> |
|ErrorCannotUseItemIdForFolderId  <br/> |Cette erreur se produit lorsqu’une demande qui requiert un identificateur de dossier reçoit un identificateur d’élément.  <br/> |
|ErrorChangeKeyRequired  <br/> |Ce code de réponse a été remplacé par **ErrorChangeKeyRequiredForWriteOperations** <br/> |
|ErrorChangeKeyRequiredForWriteOperations  <br/> |Cette erreur est renvoyée lorsque la clé de modification pour un élément est manquant ou obsolètes. <br/><br/>Pour les opérations SendItem UpdateItem et UpdateFolder, l’appelant doit passer une clé correcte et en cours de modification de l’élément. Notez que c’est le cas avec UpdateItem même lors de la résolution des conflits est définie sur toujours remplacer.  <br/> |
|ErrorClientDisconnected  <br/> |Spécifie que le client a été déconnecté.  <br/> |
|ErrorClientIntentInvalidStateDefinition  <br/> |Cette erreur est destinée à une utilisation interne uniquement.  <br/> |
|ErrorClientIntentNotFound  <br/> |Cette erreur est destinée à une utilisation interne uniquement.  <br/> |
|ErrorConnectionFailed  <br/> |Cette erreur se produit lorsque les Services Web Exchange ne peut pas se connecter à la boîte aux lettres.  <br/> |
|ErrorContainsFilterWrongType  <br/> |Cette erreur indique que la propriété qui a été inspectée pour un filtre contient n’est pas un type string.  <br/> |
|ErrorContentConversionFailed  <br/> |L’opération **GetItem** renvoie cette erreur lorsque Exchange Web Services est impossible d’extraire le contenu MIME de l’élément demandé. <br/><br/>L’opération **CreateItem** renvoie cette erreur lorsque Exchange Web Services est impossible de créer l’élément de contenu MIME fourni. Il s’agit généralement d’une indication que la propriété item est endommagée ou tronquée.  <br/> |
|ErrorContentIndexingNotEnabled  <br/> |Cette erreur se produit lorsqu’une demande de recherche est effectuée à l’aide de l’option de chaîne de requête et indexation de contenu n’est pas activé pour la boîte aux lettres cible.  <br/> |
|ErrorCorruptData  <br/> |Cette erreur se produit lorsque les données sont endommagées et ne peut pas être traitées.  <br/> |
|ErrorCreateItemAccessDenied  <br/> |Cette erreur se produit lorsque l’appelant n’est pas autorisé à créer l’élément.  <br/> |
|ErrorCreateManagedFolderPartialCompletion  <br/> |Cette erreur se produit lorsqu’une ou plusieurs des dossiers gérés qui ont été spécifiées dans la requête d’opération CreateManagedFolder n’a pas pu être créé. Recherche pour chaque dossier afin de déterminer les dossiers qui ont été créés et les dossiers n’existent pas.  <br/> |
|ErrorCreateSubfolderAccessDenied  <br/> |Cette erreur se produit lorsque le compte d’appel n’a pas les autorisations requises pour créer le sous-dossier.  <br/> |
|ErrorCrossMailboxMoveCopy  <br/> |Cette erreur se produit lorsqu’une tentative est effectuée pour déplacer un élément ou un dossier à partir d’une boîte aux lettres vers un autre. Si la boîte aux lettres source et la boîte aux lettres de destination sont différentes, vous obtenez cette erreur.  <br/> |
|ErrorCrossSiteRequest  <br/> |Cette erreur indique que la demande n’est pas autorisée, car le serveur d’accès au Client qui doit traiter la demande est dans un autre site.  <br/> |
|ErrorDataSizeLimitExceeded  <br/> |Cette erreur peut se produire dans les scénarios suivants :<br/>  <br/>-Tentative d’accéder à ou une propriété d’écriture sur un élément et la valeur de propriété est trop grande.<br/>-Le codage Base64 MIME contenu longueur au sein de la requête XML dépasse la limite.<br/>-La taille du corps d’un élément de corps existant dépasse la limite.<br/>-Le consommateur tente de définir un corps HTML ou texte dont la longueur (ou la longueur dans le cas d’ajout) dépasse la limite. |
|ErrorDataSourceOperation  <br/> |Cette erreur se produit lorsque le fournisseur de données sous-jacent ne parvient pas à terminer l’opération.  <br/> |
|ErrorDelegateAlreadyExists  <br/> |Cette erreur se produit dans une opération **AddDelegate** lorsque l’utilisateur spécifié existe déjà dans la liste des délégués.  <br/> |
|ErrorDelegateCannotAddOwner  <br/> |Cette erreur se produit dans une opération **AddDelegate** lorsque l’utilisateur spécifié à ajouter est le propriétaire de la boîte aux lettres.  <br/> |
|ErrorDelegateMissingConfiguration  <br/> |Cette erreur se produit lors d’une opération **GetDelegate** lorsqu’il n’est pas délégué d’informations sur le message FreeBusy local ou aucun délégué public Active Directory (« aucun délégué public » ou aucune entrée « Envoyer de la part » dans AD DS).  <br/> |
|ErrorDelegateNoUser  <br/> |Cette erreur se produit lorsqu’un utilisateur spécifié ne peut pas être mappé à un utilisateur dans AD DS.  <br/> |
|ErrorDelegateValidationFailed  <br/> |Cette erreur se produit lors de l’opération **AddDelegate** lorsqu’un utilisateur délégué ajouté n’est pas valide.  <br/> |
|ErrorDeleteDistinguishedFolder  <br/> |Cette erreur se produit lorsqu’une tentative est effectuée pour supprimer un dossier unique.  <br/> |
|ErrorDeleteItemsFailed  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorDeleteUnifiedMessagingPromptFailed  <br/> |Cette erreur est destinée à une utilisation interne uniquement.  <br/> |
|ErrorDistinguishedUserNotSupported  <br/> |Cette erreur indique qu’un ID d’utilisateur unique n’est pas valide pour l’opération. **DistinguishedUserType** ne doit pas être présent dans la demande.  <br/> |
|ErrorDistributionListMemberNotExist  <br/> |Cette erreur indique qu’un membre de liste de distribution demande n’existe pas dans la liste de distribution.  <br/> |
|ErrorDuplicateInputFolderNames  <br/> |Cette erreur se produit lorsque les noms de dossier en double sont spécifiés dans l’élément de [noms de dossier](foldernames.md) de la requête d’opération **CreateManagedFolder** .  <br/> |
|ErrorDuplicateSOAPHeader  <br/> |Cette erreur indique qu’il n’y a des en-têtes SOAP en double.  <br/> |
|ErrorDuplicateUserIdsSpecified  <br/> |Cette erreur indique qu’un ID d’utilisateur en double a été trouvée dans un jeu d’autorisations par défaut ou anonyme sont définis plusieurs fois, ou des SID en double ou des destinataires.  <br/> |
|ErrorEmailAddressMismatch  <br/> |Cette erreur se produit lorsqu’une demande tente de créer/mettre à jour les paramètres de recherche d’un dossier de recherche. Par exemple, cela peut se produire lorsqu’un dossier de recherche est créé dans la boîte aux lettres, mais le dossier de recherche est destiné à rechercher dans une autre boîte aux lettres.  <br/> |
|ErrorEventNotFound  <br/> |Cette erreur se produit lorsque l’événement qui est associé à un filigrane est supprimé avant que l’événement soit retourné. Lorsque cette erreur est renvoyée, l’abonnement est également supprimé.  <br/> |
|ErrorExceededConnectionCount  <br/> |Cette erreur - indique qu’il y a plus simultané demande auprès du serveur que le nombre autorisé par la stratégie de l’utilisateur.  <br/> |
|ErrorExceededSubscriptionCount  <br/> |Cette erreur indique qu’un utilisateur de stratégie de limitation nombre maximal d’abonnement a été dépassé.  <br/> |
|ErrorExceededFindCountLimit  <br/> |Cette erreur indique qu’un appel d’opération de recherche a dépassé le nombre total d’éléments pouvant être renvoyés.  <br/> |
|ErrorExpiredSubscription  <br/> |Cette erreur se produit si l' [opération GetEvents](getevents-operation.md) est appelée comme un abonnement est supprimé car il a expiré.  <br/> |
|ErrorExtensionNotFound  <br/> |Indique que l’extension est introuvable.  <br/> |
|ErrorFolderCorrupt  <br/> |Cette erreur se produit lorsque le dossier est endommagé et ne peut pas être enregistré.  <br/> |
|ErrorFolderExists  <br/> |Cette erreur se produit lorsqu’une tentative est effectuée pour créer un dossier qui a le même nom en tant qu’un autre dossier dans le même parent. Noms des dossiers en double ne sont pas autorisés.  <br/> |
|ErrorFolderNotFound  <br/> |Cette erreur indique que l’ID du dossier qui a été spécifié ne correspond pas à un dossier valide ou que le délégué n’est pas autorisé à accéder au dossier.  <br/> |
|ErrorFolderPropertRequestFailed  <br/> |Cette erreur indique que la propriété demandée pas pu être récupérée. Cela ne signifie pas que la propriété n’existe pas, mais que la propriété a été endommagée afin que la récupération a échoué.  <br/> |
|ErrorFolderSave  <br/> |Cette erreur indique que le dossier ne peut pas créé ou mis à jour en raison d’un état non valide.  <br/> |
|ErrorFolderSaveFailed  <br/> |Cette erreur indique que le dossier ne peut pas créé ou mis à jour en raison d’un état non valide.  <br/> |
|ErrorFolderSavePropertyError  <br/> |Cette erreur indique que le dossier ne peut pas créé ou mis à jour en raison de valeurs de propriété non valide. Le code de réponse répertorie les propriétés de l’origine du problème.  <br/> |
|ErrorFreeBusyDLLimitReached  <br/> |Cette erreur indique que le nombre de membres du groupe maximale a été atteinte pour obtenir des informations de disponibilité pour une liste de distribution.  <br/> |
|ErrorFreeBusyGenerationFailed  <br/> |Cette erreur est renvoyée lorsque les informations de disponibilité ne peut pas être récupérées en raison d’un échec intermédiaire.  <br/> |
|ErrorGetServerSecurityDescriptorFailed  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorImContactLimitReached  <br/> |Cette erreur est renvoyée lorsque de contacts de messagerie instantanée ne peut pas être ajoutée car le nombre maximal de contacts a été atteint. Cette erreur a été introduite dans Exchange Server 2013.  <br/> |
|ErrorImGroupDisplayNameAlreadyExists  <br/> |Cette erreur est renvoyée lorsqu’une tentative est effectuée pour ajouter un nom d’affichage de groupe lorsqu’un groupe existant a déjà le même nom complet. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorImGroupLimitReached  <br/> |Cette erreur est renvoyée lorsque de nouveaux groupes de messagerie instantanée ne peut pas être ajoutés car le nombre maximal de groupes a été atteint. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorImpersonateUserDenied  <br/> |L’erreur est renvoyée dans le cas d’autorisation de serveur à serveur pour l’emprunt d’identité Exchange lorsque l’appelant n’a pas les droits appropriés pour emprunter l’identité de l’utilisateur en question. Cette erreur correspond à la ms-Exch-EPI-May-Impersonate étendu droit Active Directory.  <br/> |
|ErrorImpersonationDenied  <br/> |Cette erreur est renvoyée dans l’autorisation de serveur à serveur pour l’emprunt d’identité Exchange lorsque l’appelant n’a pas les droits appropriés pour emprunter l’identité via le serveur d’accès au Client qu’ils font la demande par rapport à. Correspond à le ms-Exch-EPI-emprunt d’identité étendu droit Active Directory.  <br/> |
|ErrorImpersonationFailed  <br/> |Cette erreur indique qu’une erreur inattendue lors de la tentative d’effectuer l’authentification de serveur à serveur. Ce code de réponse généralement indique soit que le compte de service qui exécute le pool d’applications est configuré correctement, Exchange Web Services que Exchange Web Services ne peut pas communiquer avec l’annuaire, ou qu’une approbation entre forêts n’est pas correctement configuré.  <br/> |
|ErrorIncorrectSchemaVersion  <br/> |Cette erreur indique que la demande a été valide pour la version d’Exchange Server en cours, mais n’était pas valide pour la version du serveur de requête qui a été spécifiée.  <br/> |
|ErrorIncorrectUpdatePropertyCount  <br/> |Cette erreur indique que chaque description de la modification dans les éléments [UpdateItem](updateitem.md) ou [UpdateFolder](updatefolder.md) doit indiquer qu’une seule propriété à mettre à jour.  <br/> |
|ErrorIndividualMailboxLimitReached  <br/> |Cette erreur se produit lorsque la requête contient trop de participants à résoudre. Par défaut, le nombre maximal de participants à résoudre est 100.  <br/> |
|ErrorInsufficientResources  <br/> |Cette erreur se produit lorsque le serveur de boîtes aux lettres est surchargé. Réessayer ultérieurement.  <br/> |
|ErrorInternalServerError  <br/> |Cette erreur indique que les Services Web Exchange a rencontré une erreur indiquant qu’il ne peut pas récupérer à partir, et un code de réponse plus spécifique qui est associé à l’erreur s’est produite n’existe pas.  <br/> |
|ErrorInternalServerTransientError  <br/> |Cette erreur indique qu’une erreur interne s’est produite et que vous devriez votre demande ultérieurement.  <br/> |
|ErrorInvalidAccessLevel  <br/> |Cette erreur indique que le niveau d’accès de l’appelant sur les données et de disponibilité n’est pas valide.  <br/> |
|ErrorInvalidArgument  <br/> |Cette erreur indique une erreur due à tous les arguments non valides transmis à l' [opération GetMessageTrackingReport](getmessagetrackingreport-operation.md).<br/><br/> Cette erreur est retournée dans les scénarios suivants : <br/><br/>-L’utilisateur spécifié dans le _envoi-en tant que_ paramètre n’existe pas dans le répertoire. <br/>-L’utilisateur spécifié dans le _envoi-en tant que_ paramètre n’est pas unique dans le répertoire. <br/>-La _envoi-en tant que_ adresse est vide.<br/>-La _envoi-en tant que_ adresse n’est pas une adresse de messagerie valide.  <br/> |
|ErrorInvalidAttachmentId  <br/> |Cette erreur est retournée par l' [opération GetAttachment](getattachment-operation.md) ou l' [opération DeleteAttachment](deleteattachment-operation.md) lorsqu’une pièce jointe qui correspond à l’ID spécifié est introuvable.  <br/> |
|ErrorInvalidAttachmentSubfilter  <br/> |Cette erreur se produit lorsque vous essayez de lier à un dossier de recherche existant en utilisant une restriction de tableau complexe de pièce jointe. Services Web Exchange uniquement prend en charge simple contient les filtres par rapport à la table des pièces jointes. Si vous essayez de lier à un dossier de recherche existant qui possède une restriction de tableau de pièce jointe plus complexe (un sous-filtre), Services Web Exchange ne peut pas afficher le code XML pour le filtre renvoie ce code de réponse. <br/><br/>Notez que vous pouvez toujours appeler l’opération GetFolder sur le dossier, mais ne pas demandez l’élément [SearchParameters](searchparameters.md) .  <br/> |
|ErrorInvalidAttachmentSubfilterTextFilter  <br/> |Cette erreur se produit lorsque vous essayez de lier à un dossier de recherche existant en utilisant une restriction de tableau complexe de pièce jointe. Services Web Exchange uniquement prend en charge simple contient les filtres par rapport à la table des pièces jointes. <br/><br/>Si vous essayez de lier à un dossier de recherche existant qui a une restriction de tableau de pièce jointe plus complexe, les Services Web Exchange ne peut pas afficher le code XML pour le filtre. Dans ce cas, le sous-filtre pièce jointe contient un filtre de texte, mais il est consultant pas le nom complet de pièce jointe.<br/><br/> Notez que vous pouvez toujours appeler l’opération GetFolder sur le dossier, mais ne pas demandez l’élément [SearchParameters](searchparameters.md) .  <br/> |
|ErrorInvalidAuthorizationContext  <br/> | Cette erreur indique que la procédure d’autorisation pour le demandeur a échoué.  <br/> |
|ErrorInvalidChangeKey  <br/> |Cette erreur se produit lorsqu’un consommateur passe dans un dossier ou un identificateur d’élément avec une clé de modification qui ne peut pas être analysée. Par exemple, il pourrait être contenu base64 non valide ou une chaîne vide.  <br/> |
|ErrorInvalidClientSecurityContext  <br/> |Cette erreur indique qu’une erreur interne lors de la tentative de résoudre l’identité de l’appelant.  <br/> |
|ErrorInvalidCompleteDate  <br/> |Cette erreur est renvoyée lorsqu’une tentative est effectuée pour définir la valeur d’élément [CompleteDate](completedate.md) d’une tâche à un moment précis. Lorsqu’elle est convertie à l’heure locale du serveur d’accès au Client, la [CompleteDate](completedate.md) d’une tâche ne peut avoir une valeur qui est postérieure à l’heure locale sur le serveur d’accès au Client.  <br/> |
|ErrorInvalidContactEmailAddress  <br/> |Cette erreur indique qu’une adresse de messagerie non valide a été fournie pour un contact.  <br/> |
|ErrorInvalidContactEmailIndex  <br/> |Cette erreur indique qu’une valeur d’index de messagerie non valide a été fournie pour une entrée d’adresse de messagerie.  <br/> |
|ErrorInvalidCrossForestCredentials  <br/> |Cette erreur se produit lorsque les informations d’identification qui sont utilisés pour le proxy d’une demande à une autre forêt du service ne peut être authentifié.  <br/> |
|ErrorInvalidDelegatePermission  <br/> |Cette erreur indique que les autorisations du dossier spécifié ne sont pas valides.  <br/> |
|ErrorInvalidDelegateUserId  <br/> |Cette erreur indique que l’ID d’utilisateur délégué spécifié n’est pas valide.  <br/> |
|ErrorInvalidExchangeImpersonationHeaderData  <br/> |Cette erreur se produit au cours de l’emprunt d’identité Exchange lorsque l’appelant ne spécifie pas un nom UPN, une adresse de messagerie ou un SID d’utilisateur. Cela se produit également si l’appelant spécifie un ou plusieurs de ces et les valeurs sont vides.  <br/> |
|ErrorInvalidExcludesRestriction  <br/> |Cette erreur se produit lorsque le masque de bits qui a été passée dans une restriction d’élément [exclut](excludes.md) ne peut pas être analysée.  <br/> |
|ErrorInvalidExpressionTypeForSubFilter  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorInvalidExtendedProperty  <br/> | Cette erreur se produit lorsque les événements suivants ont lieu : <br/> <br/>-L’appelant essaie d’utiliser une propriété étendue qui n’est pas pris en charge par les Services Web Exchange.  <br/>-L’appelant transmet une combinaison des valeurs d’attribut pour une propriété étendue non valide. Cela se produit également si aucuns attributs ne sont transmis. Uniquement certaines combinaisons sont autorisées.  <br/> |
|ErrorInvalidExtendedPropertyValue  <br/> |Cette erreur se produit lorsque la section de la valeur d’une propriété étendue ne correspond pas au type de la propriété. <br/><br/>Par exemple, si vous définissez une propriété étendue comportant PropertyType = « Chaîne » pour un tableau d’entiers provoque cette erreur. Une représentation de chaîne qui n’est pas être convertie dans le type qui est spécifié pour la propriété étendue génère cette erreur.  <br/> |
|ErrorInvalidExternalSharingInitiator  <br/> |Cette erreur indique que l’expéditeur invitation de partage n’a pas créé les métadonnées invitation de partage.  <br/> |
|ErrorInvalidExternalSharingSubscriber  <br/> |Cette erreur indique qu’un message de partage n’est pas destiné à l’appelant.  <br/> |
|ErrorInvalidFederatedOrganizationId  <br/> |Cette erreur indique que les objets de fédération du demandeur l’organisation ne sont pas configurés correctement.  <br/> |
|ErrorInvalidFolderId  <br/> |Cette erreur se produit lorsque l’ID de dossier est endommagé.  <br/> |
|ErrorInvalidFolderTypeForOperation  <br/> |Cette erreur indique que le type de dossier spécifié n’est pas valide pour l’opération en cours. Par exemple, Impossible de créer un dossier de recherche dans un dossier public.  <br/> |
|ErrorInvalidFractionalPagingParameters  <br/> | Cette erreur se produit dans une fraction pagination lorsque l’utilisateur a spécifié une des options suivantes : <br/> <br/>-Numérateur est supérieur au dénominateur  <br/>-Numérateur est inférieur à zéro  <br/>-Dénominateur est inférieure ou égale à zéro  <br/> |
|ErrorInvalidGetSharingFolderRequest  <br/> |Cette erreur indique que les éléments du [type de données](datatype.md) et ShareFolderId sont tous deux présents dans une requête.  <br/> |
|ErrorInvalidFreeBusyViewType  <br/> |Cette erreur se produit lorsque l' [opération GetUserAvailability](getuseravailability-operation.md) est appelée avec un [FreeBusyViewType](freebusyviewtype.md) None.  <br/> |
|ErrorInvalidId  <br/> |Cette erreur indique que la clé ID et/ou de modification est incorrecte.  <br/> |
|ErrorInvalidIdEmpty  <br/> |Cette erreur se produit lorsque l’appelant spécifie un attribut **d’Id** est vide.  <br/> |
|ErrorInvalidLikeRequest  <br/> |Cette erreur se produit lorsque l’élément ne peut pas être aimé. Versions d’Exchange commençant par le numéro de build 15.00.0913.09 incluent cette valeur.  <br/> |
|ErrorInvalidIdMalformed  <br/> |Cette erreur se produit lorsque l’appelant spécifie un attribut **d’Id** est incorrect.  <br/> |
|ErrorInvalidIdMalformedEwsLegacyIdFormat  <br/> |Cette erreur indique qu’un ID de dossier ou un élément qui utilise le format d’Exchange 2007 a été spécifié pour une demande avec une version d’Exchange 2007 SP1 ou version ultérieure. Vous ne pouvez pas utiliser Exchange 2007 ID dans Exchange 2007 SP1 ou version ultérieure demandes. Vous devez utiliser l' [opération ConvertId](convertid-operation.md) pour convertir en premier.  <br/> |
|ErrorInvalidIdMonikerTooLong  <br/> |Cette erreur se produit lorsque l’appelant spécifie un attribut **d’Id** est trop long.  <br/> |
|ErrorInvalidIdNotAnItemAttachmentId  <br/> |Cette erreur est renvoyée à chaque fois qu’un ID qui n’est pas une pièce jointe élément QU'ID est passé à une méthode de service Web qui attend un ID de pièce jointe.  <br/> |
|ErrorInvalidIdReturnedByResolveNames  <br/> |Cette erreur se produit lorsqu’un contact dans votre boîte aux lettres est endommagé.  <br/> |
|ErrorInvalidIdStoreObjectIdTooLong  <br/> |Cette erreur se produit lorsque l’appelant spécifie un attribut **d’Id** est trop long.  <br/> |
|ErrorInvalidIdTooManyAttachmentLevels  <br/> |Cette erreur est renvoyée lorsque la hiérarchie de pièce jointe dans un élément dépasse le nombre maximal de 255 niveaux.  <br/> |
|ErrorInvalidIdXml  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorInvalidImContactId  <br/> |Cette erreur est renvoyée lorsque l’identificateur de contact de messagerie instantanée spécifié ne représente pas un identificateur valide. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorInvalidImDistributionGroupSmtpAddress  <br/> |Cette erreur est renvoyée lorsque l’identificateur d’adresse SMTP spécifiée par messagerie instantanée distribution group ne représente pas un identificateur valide. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorInvalidImGroupId  <br/> |Cette erreur est renvoyée lorsque l’identificateur de groupe de messagerie instantanée spécifié ne représente pas un identificateur valide. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorInvalidIndexedPagingParameters  <br/> |Cette erreur se produit si le décalage de pagination indexé est négatif.  <br/> |
|ErrorInvalidInternetHeaderChildNodes  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorInvalidItemForOperationArchiveItem  <br/> |Indique que l’élément n’est pas valide pour une opération **ArchiveItem** .  <br/> |
|ErrorInvalidItemForOperationAcceptItem  <br/> |Cette erreur se produit lors de la tentative d’utiliser un objet de réponse AcceptItem pour un type d’élément autre qu’une demande de réunion ou un élément de calendrier, ou lorsqu’une tentative est effectuée pour accepter une occurrence d’élément de calendrier qui se trouve dans le dossier éléments supprimés.  <br/> |
|ErrorInvalidItemForOperationCancelItem  <br/> |Cette erreur se produit lors de la tentative d’utiliser un objet de réponse CancelItem sur un type d’élément autre qu’un élément de calendrier.  <br/> |
|ErrorInvalidItemForOperationCreateItemAttachment  <br/> | Cette erreur est renvoyée lorsqu’une tentative est effectuée pour créer une pièce jointe d’élément d’un type non pris en charge.  <br/><br/>  Types d’éléments pris en charge pour les pièces jointes d’élément sont les objets suivants :  <br/><br/>- [Élément](item.md) <br/>- [Message](message-ex15websvcsotherref.md) <br/>- [CalendarItem](calendaritem.md) <br/>- [Tâche](task.md) <br/>- [Contact](contact.md) <br/> <br/> Par exemple, si vous essayez de créer une pièce jointe [MeetingMessage](meetingmessage.md) , vous rencontrerez ce code de réponse.  <br/> |
|ErrorInvalidItemForOperationCreateItem  <br/> | Cette erreur est renvoyée à partir d’une [opération CreateItem](createitem-operation.md) si la requête contient un type d’élément non pris en charge. <br/><br/>Éléments pris en charge sont les objets suivants :<br/>  <br/>- [Élément](item.md) <br/>- [Message](message-ex15websvcsotherref.md) <br/>- [CalendarItem](calendaritem.md) <br/>- [Tâche](task.md) <br/>- [Contact](contact.md) <br/><br/>  Certains types sont créés en conséquence d’autre chose. Messages de réunion, par exemple, sont créés lorsque vous envoyez un élément de calendrier aux participants ; ils ne sont pas explicitement créés.  <br/> |
|ErrorInvalidItemForOperationDeclineItem  <br/> |Cette erreur se produit lors de la tentative d’utiliser un objet de réponse DeclineItem pour un type d’élément autre qu’une demande de réunion ou un élément de calendrier, ou lorsqu’une tentative est effectuée pour refuser une occurrence d’élément de calendrier qui se trouve dans le dossier éléments supprimés.  <br/> |
|ErrorInvalidItemForOperationExpandDL  <br/> |Cette erreur indique que l' [opération ExpandDL](expanddl-operation.md) est valide uniquement pour les listes de distribution privée.  <br/> |
|ErrorInvalidItemForOperationRemoveItem  <br/> |Cette erreur est renvoyée à partir d’un objet de réponse RemoveItem si la demande spécifie un élément qui n’est pas une réunion élément d’annulation.  <br/> |
|ErrorInvalidItemForOperationSendItem  <br/> |Cette erreur est renvoyée à partir d’une [opération SendItem](senditem-operation.md) si la demande spécifie un élément qui n’est pas un élément de message.  <br/> |
|ErrorInvalidItemForOperationTentative  <br/> |Cette erreur se produit lors de la tentative d’utiliser [TentativelyAcceptItem](tentativelyacceptitem.md) pour un type d’élément autre qu’une demande de réunion ou un élément de calendrier ou lors de la tentative d’accepter provisoirement une occurrence d’élément de calendrier qui se trouve dans le dossier éléments supprimés.  <br/> |
|ErrorInvalidLogonType  <br/> |Cette erreur est à usage interne uniquement. Cette erreur n’est pas retournée.  <br/> |
|ErrorInvalidMailbox  <br/> |Cette erreur indique que l' [opération CreateItem](createitem-operation.md) ou l' [opération UpdateItem](updateitem-operation.md) a échoué pendant la création ou mise à jour d’une liste de distribution personnelle.  <br/> |
|ErrorInvalidManagedFolderProperty  <br/> |Cette erreur se produit lorsque la structure du dossier géré est endommagée et ne peut pas être affichée.  <br/> |
|ErrorInvalidManagedFolderQuota  <br/> |Cette erreur se produit lorsque le quota est défini sur le dossier géré est inférieur à zéro, ce qui indique un dossier géré endommagé.  <br/> |
|ErrorInvalidManagedFolderSize  <br/> |Cette erreur se produit lorsque la taille est définie sur le dossier géré est inférieur à zéro, ce qui indique un dossier géré endommagé.  <br/> |
|ErrorInvalidMergedFreeBusyInterval  <br/> |Cette erreur se produit lorsque la fusionnée disponibilité interne valeur fournie n’est pas valide. La valeur minimale par défaut est de 5 minutes. La valeur maximale par défaut est 1 440 minutes.  <br/> |
|ErrorInvalidNameForNameResolution  <br/> |Cette erreur se produit lorsque le nom n’est pas valide pour l' [opération ResolveNames](resolvenames-operation.md). Par exemple, une chaîne de longueur nulle, un seul espace, une virgule et un tiret sont tous les noms non valides.  <br/> |
|ErrorInvalidNetworkServiceContext  <br/> |Cette erreur indique une erreur dans le compte Service réseau sur le serveur d’accès au Client.  <br/> |
|ErrorInvalidOofParameter  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorInvalidOperation  <br/> | Il s’agit d’une erreur générale qui est utilisée lorsque l’opération demandée n’est pas valide. <br/><br/>Vous ne pouvez pas, par exemple, procédez comme suit : <br/> <br/>-Effectuer « approfondies » à l’aide de l' [opération FindFolder](findfolder-operation.md) sur un dossier public.  <br/>-Permet de déplacer ou copier la racine du dossier public.  <br/>-Supprimer un élément associé à l’aide de n’importe quel mode, sauf supprimer « Dur ».  <br/>-Permet de déplacer ou copier un élément associé.  <br/> |
|ErrorInvalidOrganizationRelationshipForFreeBusy  <br/> |Cette erreur indique qu’un appelant a demandé des informations de disponibilité pour un utilisateur d’une autre organisation, mais la relation d’organisation n’a pas activé libre/occupé.  <br/> |
|ErrorInvalidPagingMaxRows  <br/> |Cette erreur se produit lorsqu’un consommateur passe un zéro ou une valeur négative pour le nombre maximal de lignes à renvoyer.  <br/> |
|ErrorInvalidParentFolder  <br/> |Cette erreur se produit lorsqu’un consommateur passe dans un dossier parent non valide pour une opération. Par exemple, cette erreur est retournée si vous essayez de créer un dossier dans un dossier de recherche.  <br/> |
|ErrorInvalidPercentCompleteValue  <br/> |Cette erreur est renvoyée lorsqu’une tentative est effectuée pour définir un pourcentage d’achèvement de tâche à une valeur non valide. La valeur doit être comprise entre 0 et 100 (inclus).  <br/> |
|ErrorInvalidPermissionSettings  <br/> |Cette erreur indique que le niveau d’autorisation n’est pas cohérent avec les paramètres d’autorisation.  <br/> |
|ErrorInvalidPhoneCallId  <br/> |Cette erreur indique que l’identificateur de l’appelant n’est pas valide.  <br/> |
|ErrorInvalidPhoneNumber  <br/> |Cette erreur indique que le numéro de téléphone n’est pas correct ou ne tient pas les règles de plan de numérotation.  <br/> |
|ErrorInvalidPropertyAppend  <br/> | Cette erreur se produit lorsque la propriété que vous essayez d’ajouter n’autorise pas l’ajout. <br/><br/>Voici les seules propriétés qui prennent en charge l’ajout de : <br/> <br/>-Collections destinataires (BccRecipients ToRecipients, CcRecipients)  <br/>-Collections attendee (RequiredAttendees, OptionalAttendees, ressources)  <br/>-Corps  <br/>-ReplyTo  <br/><br/>  En outre, cette erreur se produit lorsque vous ajoutez un corps de message si le format spécifié dans la demande ne correspond pas le format de l’élément dans le magasin.  <br/> |
|ErrorInvalidPropertyDelete  <br/> |Cette erreur se produit si l’opération de suppression est spécifiée dans un appel [opération UpdateItem](updateitem-operation.md) ou [UpdateFolder](updatefolder-operation.md) pour une propriété qui ne prend pas en charge l’opération de suppression. Par exemple, vous ne pouvez pas supprimer l’élément [ItemId](itemid.md) de [l’objet](item.md) .  <br/> |
|ErrorInvalidPropertyForExists  <br/> |Cette erreur se produit si le consommateur passe d’une des propriétés dans un filtre [Exists](exists.md) indicateur. Par exemple, cette erreur se produit si les indicateurs [estlu](isread.md) ou [IsFromMe](isfromme.md) sont spécifiés dans l’élément [existe](exists.md) . La requête doit utiliser l’élément [plutôt IsEqualTo](isequalto.md) à la place de ces comme ils sont indicateurs et par conséquent partie d’une propriété unique.  <br/> |
|ErrorInvalidPropertyForOperation  <br/> |Cette erreur se produit lorsque la propriété que vous tentez de manipuler ne gère pas l’opération est exécutée.  <br/> |
|ErrorInvalidPropertyRequest  <br/> | Cette erreur se produit si une propriété qui est spécifiée dans la demande n’est pas disponible pour le type d’élément. Par exemple, cette erreur est renvoyée si une propriété qui est disponible uniquement sur les éléments de calendrier est demandée dans une [opération GetItem](getitem-operation.md) appeler pour un message ou est mis à jour dans une [opération UpdateItem](updateitem-operation.md) appeler pour un message. <br/> <br/>  Cela se produit dans les opérations suivantes : <br/> <br/>- [Opération GetItem](getitem-operation.md) <br/>- [Opération GetFolder](getfolder-operation.md) <br/>- [Opération UpdateItem](updateitem-operation.md) <br/>- [Opération UpdateFolder](updatefolder-operation.md) <br/> |
|ErrorInvalidPropertySet  <br/> |Cette erreur indique que la propriété que vous tentez de manipuler ne gère pas l’opération est exécutée. Par exemple, cette erreur est retournée si vous essayez de définir la propriété est en lecture seule.  <br/> |
|ErrorInvalidPropertyUpdateSentMessage  <br/> | Cette erreur se produit pendant une [opération UpdateItem](updateitem-operation.md) lorsqu’un client tente de mettre à jour de certaines propriétés d’un message qui a déjà été envoyé.<br/><br/> Par exemple, les propriétés suivantes ne peuvent pas être mis à jour sur un message envoyé : <br/> <br/>- [IsReadReceiptRequested](isreadreceiptrequested.md) <br/>- [IsDeliveryReceiptRequested](isdeliveryreceiptrequested.md) <br/> |
|ErrorInvalidProxySecurityContext  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorInvalidPullSubscriptionId  <br/> |Cette erreur se produit si vous appelez l' [opération GetEvents](getevents-operation.md) ou l' [opération Annuler l’abonnement](unsubscribe-operation.md) à l’aide d’un ID d’abonnement push. Pour annuler l’abonnement à partir d’un abonnement, vous devez répondre à une demande de transmission avec une réponse d’annulation d’abonnement, ou se déconnecter de votre service Web et attendre les délai d’attente les notifications push.  <br/> |
|ErrorInvalidPushSubscriptionUrl  <br/> | Cette erreur est retournée par l' [opération de s’abonner](subscribe-operation.md) lorsqu’il crée un abonnement « push » et indique que l’URL qui est inclus dans la demande n’est pas valide.<br/><br/>Les conditions suivantes doivent être remplies pour accepter l’URL des Services Web Exchange : <br/> <br/>-Chaîne de longueur \> 0 et \< 2083.  <br/>-Le protocole est http ou https.  <br/>-L’URL peut être analysé par la classe URI Microsoft .NET Framework.  <br/> |
|ErrorInvalidRecipients  <br/> |Cette erreur indique que la collection de destinataires de votre message ou à la collection participant sur votre élément de calendrier n’est pas valide. Par exemple, cette erreur est renvoyée lorsqu’une tentative est effectuée pour envoyer un élément qui n’a pas de destinataire.  <br/> |
|ErrorInvalidRecipientSubfilter  <br/> |Cette erreur indique que le dossier de recherche a un filtre de tableau de destinataires qui ne peuvent pas représentent des Services Web Exchange. Pour résoudre cette erreur, récupérez le dossier sans demander les paramètres de recherche.  <br/> |
|ErrorInvalidRecipientSubfilterComparison  <br/> |Cette erreur indique que le dossier de recherche a un filtre de tableau de destinataires qui ne peuvent pas représentent des Services Web Exchange. Pour résoudre cette erreur, récupérez le dossier sans demander les paramètres de recherche.  <br/> |
|ErrorInvalidRecipientSubfilterOrder  <br/> |Cette erreur indique que le dossier de recherche a un filtre de tableau de destinataires qui ne peuvent pas représentent des Services Web Exchange. Pour résoudre cette erreur, récupérez le dossier sans demander les paramètres de recherche.  <br/> |
|ErrorInvalidRecipientSubfilterTextFilter  <br/> |Cette erreur indique que le dossier de recherche a un filtre de tableau de destinataires qui ne peuvent pas représentent des Services Web Exchange. Pour résoudre cette erreur, récupérez le dossier sans demander les paramètres de recherche.  <br/> |
|ErrorInvalidReferenceItem  <br/> | Cette erreur est renvoyée à partir de l' [opération CreateItem](createitem-operation.md) de réponse et transfert des objets de réponse dans les scénarios suivants :<br/>  <br/>-L’identificateur de l’élément référencé n’est pas un [Message](message-ex15websvcsotherref.md), un [CalendarItem](calendaritem.md)ou un descendant de **Message** ou **CalendarItem**.  <br/>-L’identificateur d’élément de référence est pour une **CalendarItem** et l’organisateur essaie de répondre ou répondre à tous à lui-même.  <br/>-Le message est un brouillon et répondre ou répondre à tous est sélectionné.  <br/>-L’élément de référence, pour [SuppressReadReceipt](suppressreadreceipt.md), n’est pas un **Message** ou un descendant d’un **Message**.  <br/> |
|ErrorInvalidRequest  <br/> |Cette erreur se produit lorsque la demande SOAP dispose d’un en-tête d’action SOAP, mais rien dans le corps SOAP. Notez que l’en-tête SOAP Action n’est pas nécessaire que les Services Web Exchange peut déterminer la méthode à appeler à partir du nom local de l’élément racine dans le corps SOAP.  <br/> |
|ErrorInvalidRestriction  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorInvalidRetentionTagTypeMismatch  <br/> |Cette erreur est renvoyée lorsque la balise de rétention spécifié a une action incorrecte lui est associée. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorInvalidRetentionTagInvisible  <br/> |Cette erreur est renvoyée lorsqu’une tentative est effectuée pour définir une balise inexistante ou invisible sur une propriété **PolicyTag** . Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorInvalidRetentionTagInheritance  <br/> |Cette erreur est renvoyée lorsqu’une tentative est effectuée pour définir une balise implicite de la propriété **PolicyTag** . Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorInvalidRetentionTagIdGuid  <br/> |Indique que la balise de rétention GUID n’est pas valide.  <br/> |
|ErrorInvalidRoutingType  <br/> |Cette erreur se produit si le type de routage qui est passé pour un élément [RoutingType (EmailAddressType)](routingtype-emailaddresstype.md) n’est pas valide. En règle générale, le type de routage est défini à SMTP Simple Mail Transfer Protocol ().  <br/> |
|ErrorInvalidScheduledOofDuration  <br/> |Cette erreur se produit si l’heure de fin d’une durée spécifiée n’est pas supérieur à l’heure de début, ou si l’heure de fin ne se produit pas dans le futur.  <br/> |
|ErrorInvalidSchemaVersionForMailboxVersion  <br/> |Cette erreur indique qu’une demande de proxy qui a été envoyée à un autre serveur n’est pas en mesure de traiter la demande en raison d’une incompatibilité de version.  <br/> |
|ErrorInvalidSecurityDescriptor  <br/> |Cette erreur indique que le descripteur de sécurité Exchange dans le dossier de calendrier dans le magasin est endommagé.  <br/> |
|ErrorInvalidSendItemSaveSettings  <br/> |Cette erreur se produit lors d’une tentative d’envoyer un élément où la [SavedItemFolderId](saveditemfolderid.md) est spécifié dans la demande, mais la propriété **SaveItemToFolder** est définie sur **false**.  <br/> |
|ErrorInvalidSerializedAccessToken  <br/> |Cette erreur indique que le jeton qui a été passé dans l’en-tête est incorrect, ne fait pas référence à un compte valide dans le répertoire ou ne contient pas le groupe principal **ConnectingSID**.  <br/> |
|ErrorInvalidSharingData  <br/> |Cette erreur indique que les métadonnées de partage ne sont pas valide. Cela peut être dû à XML non valide.  <br/> |
|ErrorInvalidSharingMessage  <br/> |Cette erreur indique que le message de partage n’est pas valide. Cela peut être dû à une propriété manquante.  <br/> |
|ErrorInvalidSid  <br/> |Cette erreur se produit lorsqu’un argument non valide que SID est passé dans une requête.  <br/> |
|ErrorInvalidSIPUri  <br/> |Cette erreur indique que le nom du SIP, plan de numérotation ou le numéro de téléphone sont des URI SIP non valide.  <br/> |
|ErrorInvalidServerVersion  <br/> |Cette erreur indique qu’une version de serveur de requête non valide a été spécifiée dans la demande.  <br/> |
|ErrorInvalidSmtpAddress  <br/> |Cette erreur se produit lorsque l’adresse SMTP ne peut pas être analysée.  <br/> |
|ErrorInvalidSubfilterType  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorInvalidSubfilterTypeNotAttendeeType  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorInvalidSubfilterTypeNotRecipientType  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorInvalidSubscription  <br/> |Cette erreur indique que l’abonnement n’est plus valide. Cela peut être car le serveur d’accès au Client redémarre ou l’abonnement a expiré.  <br/> |
|ErrorInvalidSubscriptionRequest  <br/> |Cette erreur indique que la demande subscribe inclus plusieurs ID de dossier public. Un abonnement peut inclure plusieurs dossiers à partir de la même boîte aux lettres ou un ID de dossier public.  <br/> |
|ErrorInvalidSyncStateData  <br/> |Cette erreur est renvoyée par [SyncFolderItems](syncfolderitems.md) ou [SyncFolderHierarchy](syncfolderhierarchy.md) si les données [SyncState](syncstate-ex15websvcsotherref.md) transmis ne sont pas valides. Pour corriger cette erreur, vous devez resynchroniser sans l’état de synchronisation. Assurez-vous que si vous êtes synchronisation persistance des objets BLOB d’état, vous ne sont pas tronquer accidentellement l’objet BLOB.  <br/> |
|ErrorInvalidTimeInterval  <br/> |Cette erreur indique que l’intervalle de temps spécifié n’est pas valide. L’heure de début doit être supérieure ou égale à la date de fin.  <br/> |
|ErrorInvalidUserInfo  <br/> |Cette erreur indique qu’une incohérence [UserId](userid.md) a été spécifié pour une opération d’autorisations. Par exemple, si un ID d’utilisateur unique est spécifié (par défaut ou anonyme), cette erreur est retournée si vous essayez également spécifier un identificateur de sécurité ou l’adresse SMTP principale ou nom complet pour cet utilisateur.  <br/> |
|ErrorInvalidUserOofSettings  <br/> |Cette erreur indique que les paramètres d’absence du bureau (OOF) l’utilisateur ne sont pas valides en raison d’une réponse interne ou externe manquante.  <br/> |
|ErrorInvalidUserPrincipalName  <br/> |Cette erreur se produit au cours de l’emprunt d’identité Exchange. L’appelant a passé un UPN non valide dans l’en-tête SOAP qui n’était pas accessible dans le répertoire.  <br/> |
|ErrorInvalidUserSid  <br/> |Cette erreur se produit lorsqu’un argument non valide que SID est passé dans une requête.  <br/> |
|ErrorInvalidUserSidMissingUPN  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorInvalidValueForProperty  <br/> |Cette erreur indique que la valeur de comparaison dans la restriction n’est pas valide pour la propriété par rapport à vous comparez.<br/><br/> Par exemple, la valeur de la comparaison de [DateTimeCreated](datetimecreated.md) > **true** renvoie ce code de réponse. <br/><br/>Ce code de réponse est également renvoyé si vous spécifiez une propriété d’énumération lors de la comparaison, mais la valeur que vous comparez contre n’est pas une valeur valide pour cette énumération.  <br/> |
|ErrorInvalidWatermark  <br/> |Cette erreur est provoquée par un filigrane non valide.  <br/> |
|ErrorIPGatewayNotFound  <br/> |Cette erreur indique qu’une passerelle VoIP valide n’est pas disponible.  <br/> |
|ErrorIrresolvableConflict  <br/> |Cette erreur indique que la résolution des conflits n’a pas pu résoudre des modifications pour les propriétés. Les éléments dans le magasin ont été modifiées et doivent être mis à jour. Récupérer la clé de modification mise à jour et réessayez.  <br/> |
|ErrorItemCorrupt  <br/> |Cette erreur indique que l’état de l’objet est endommagé et ne peut pas être récupéré. Lorsque vous récupérez un élément, seuls certains éléments seront dans cet état, telles que le [corps](body.md) et [MimeContent](mimecontent.md). Omettez ces éléments et recommencez l’opération.  <br/> |
|ErrorItemNotFound  <br/> |Cette erreur se produit lorsque l’élément est introuvable ou vous n’êtes pas autorisé à accéder à l’élément.  <br/> |
|ErrorItemPropertyRequestFailed  <br/> |Cette erreur se produit en cas d’échec d’une requête de propriété sur un élément. La propriété existe, mais il ne peut pas être récupéré.  <br/> |
|ErrorItemSave  <br/> |Cette erreur se produit lors de l’échouent des tentatives d’enregistrement de l’élément ou un dossier.  <br/> |
|ErrorItemSavePropertyError  <br/> |Cette erreur se produit lors de la tentative d’enregistrer l’élément ou le dossier échoue en raison de valeurs de propriété non valide. Le code de réponse inclut le chemin d’accès des propriétés non valides.  <br/> |
|ErrorLegacyMailboxFreeBusyViewTypeNotMerged  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorLocalServerObjectNotFound  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorLogonAsNetworkServiceFailed  <br/> |Cette erreur indique que le service de disponibilité n’a pas pu se connecter en tant que le service réseau pour les requêtes de proxy pour les sites appropriés ou les forêts. Cette réponse indique généralement une erreur de configuration.  <br/> |
|ErrorMailboxConfiguration  <br/> |Cette erreur indique que les informations de boîte aux lettres dans AD DS sont mal configurées.  <br/> |
|ErrorMailboxDataArrayEmpty  <br/> |Cette erreur indique que l’élément [MailboxDataArray](mailboxdataarray.md) dans la demande est vide. Vous devez fournir au moins un identificateur de boîte aux lettres.  <br/> |
|ErrorMailboxDataArrayTooBig  <br/> |Cette erreur se produit lorsque plus de 100 entrées sont fournies dans un élément [MailboxDataArray](mailboxdataarray.md) ...  <br/> |
|ErrorMailboxFailover  <br/> |Cette erreur indique que la tentative d’accéder à une boîte aux lettres a échoué, car la boîte aux lettres se trouve dans un processus de basculement.  <br/> |
|ErrorMailboxHoldNotFound  <br/> |Indique que la suspension de la boîte aux lettres est introuvable.  <br/> |
|ErrorMailboxLogonFailed  <br/> |Cette erreur se produit lors de l’échec de la connexion à la boîte aux lettres pour obtenir les informations d’affichage Calendrier.  <br/> |
|ErrorMailboxMoveInProgress  <br/> | Cette erreur indique que la boîte aux lettres est déplacée vers un serveur ou une banque de boîtes aux lettres différente. Cette erreur peut également indiquer que la boîte aux lettres est sur une autre base de données de boîte aux lettres ou le serveur.  <br/> |
|ErrorMailboxStoreUnavailable  <br/> | Cette erreur indique que l’une des conditions s’est produites le message d’erreur suivant :  <br/><br/>-La banque de boîtes aux lettres est endommagée.  <br/>-La banque de boîtes aux lettres est en cours d’arrêt.  <br/>-La banque de boîtes aux lettres est en mode hors connexion.  <br/>-Une erreur réseau s’est produite lors de la tentative d’accès à la banque de boîtes aux lettres.  <br/>-La banque de boîtes aux lettres est surchargée et ne peut pas accepter davantage de connexions.  <br/>-La banque de boîtes aux lettres a été suspendue.  <br/> |
|ErrorMailRecipientNotFound  <br/> |Cette erreur se produit si les informations de l’élément [MailboxData](mailboxdata.md) ne peut pas être mappées à un compte de boîte aux lettres valide.  <br/> |
|ErrorMailTipsDisabled  <br/> |Cette erreur indique que les astuces de la messagerie sont désactivés.  <br/> |
|ErrorManagedFolderAlreadyExists  <br/> |Cette erreur se produit si le dossier géré que vous tentez de créer déjà existe dans une boîte aux lettres.  <br/> |
|ErrorManagedFolderNotFound  <br/> |Cette erreur se produit lorsque le nom du dossier qui a été spécifié dans la demande ne correspond pas à une définition de dossier géré dans AD DS. Vous ne pouvez créer des instances de dossiers gérés pour les dossiers qui sont définies dans AD DS. Vérifiez le nom et réessayez.  <br/> |
|ErrorManagedFoldersRootFailure  <br/> |Cette erreur indique que la racine des dossiers gérés a été supprimée de la boîte aux lettres ou l’existence d’un dossier dans le même dossier parent qui porte le nom de la racine du dossier géré. Cela se produit également si la tentative de création de la racine géré dossier échoue.  <br/> |
|ErrorMeetingSuggestionGenerationFailed  <br/> |Cette erreur indique que le moteur de suggestions a rencontré un problème lors de son générer les suggestions.  <br/> |
|ErrorMessageDispositionRequired  <br/> | Cette erreur se produit si l’attribut **MessageDisposition** n’est pas définie.<br/><br/> Cet attribut est requis pour les éléments suivants : <br/> <br/>-L' [opération CreateItem](createitem-operation.md) et l' [opération UpdateItem](updateitem-operation.md) lors de l’élément créée ou mise à jour est un [Message](message-ex15websvcsotherref.md).  <br/>- Objets de réponse [CancelCalendarItem](cancelcalendaritem.md), [AcceptItem](acceptitem.md), [DeclineItem](declineitem.md)ou [TentativelyAcceptItem](tentativelyacceptitem.md) .  <br/> |
|ErrorMessageSizeExceeded  <br/> |Cette erreur indique que le message que vous essayez d’envoyer dépasse la limite autorisée.  <br/> |
|ErrorMessageTrackingNoSuchDomain  <br/> |Cette erreur indique que le domaine spécifié est introuvable.  <br/> |
|ErrorMessageTrackingPermanentError  <br/> |Cette erreur indique que le service de suivi de message ne peut pas suivre le message.  <br/> |
| ErrorMessageTrackingTransientError  <br/> |Cette erreur indique que le service de suivi des messages est arrêté ou occupé (e). Ce code d’erreur indique une erreur temporaire. Les clients peuvent réessayer de vous connecter au serveur lors de la réception de cette erreur.  <br/> |
|ErrorMimeContentConversionFailed  <br/> |Cette erreur se produit lorsque le contenu MIME n’est pas valide iCal pour une [opération CreateItem](createitem-operation.md). Pour une [opération GetItem](getitem-operation.md), cette réponse indique que le contenu MIME ne peut pas être généré.  <br/> |
|ErrorMimeContentInvalid  <br/> |Cette erreur se produit lorsque le contenu MIME n’est pas valide.  <br/> |
|ErrorMimeContentInvalidBase64String  <br/> |Cette erreur se produit lorsque le contenu MIME de la demande n’est pas une chaîne valide en 64 base.  <br/> |
|ErrorMissingArgument  <br/> |Cette erreur indique qu’un argument requis est manquant à partir de la demande. Texte du message de réponse indique quel argument à vérifier.  <br/> |
|ErrorMissingEmailAddress  <br/> |Cette erreur indique que vous avez spécifié un ID unique dans la demande, mais que le compte qui a fait la demande ne dispose pas d’une boîte aux lettres sur le système. Dans ce cas, vous devez fournir un sous-élément sous [DistinguishedFolderId](distinguishedfolderid.md) [boîte aux lettres](mailbox.md) .  <br/> |
|ErrorMissingEmailAddressForManagedFolder  <br/> |Cette erreur indique que vous avez spécifié un ID unique dans la demande, mais que le compte qui a fait la demande ne dispose pas d’une boîte aux lettres sur le système. Dans ce cas, vous devez fournir un sous-élément sous [DistinguishedFolderId](distinguishedfolderid.md) [boîte aux lettres](mailbox.md) . Cette réponse est renvoyée à partir de l' [opération CreateManagedFolder](createmanagedfolder-operation.md).  <br/> |
|ErrorMissingInformationEmailAddress  <br/> |Cette erreur se produit si l’élément [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) est manquant.  <br/> |
|ErrorMissingInformationReferenceItemId  <br/> |Cette erreur se produit si le [ReferenceItemId](referenceitemid.md) est manquant.  <br/> |
|ErrorMissingInformationSharingFolderId  <br/> |Ce code d’erreur n’est jamais retourné.  <br/> |
|ErrorMissingItemForCreateItemAttachment  <br/> |Cette erreur est renvoyée lorsqu’une tentative est effectuée pour ne pas inclure l’élément dans l’élément **ItemAttachment** d’une demande [d’opération CreateAttachment](createattachment-operation.md) .  <br/> |
|ErrorMissingManagedFolderId  <br/> |Cette erreur se produit lorsque la propriété ID de la stratégie, la balise de propriété 0x6732, pour le dossier est manquant. Vous devez envisager cela un dossier endommagé.  <br/> |
|ErrorMissingRecipients  <br/> |Cette erreur indique que vous avez essayé d’envoyer un élément sans inclure les destinataires. Notez que si vous appelez l' [opération CreateItem](createitem-operation.md) avec une disposition de message qui entraîne l’envoi du message, vous recevrez le code de réponse suivant : **ErrorInvalidRecipients**.  <br/> |
|ErrorMissingUserIdInformation  <br/> |Cette erreur indique qu’un [nom d’utilisateur](userid.md) n’a pas été entièrement spécifié dans un jeu d’autorisations.  <br/> |
|ErrorMoreThanOneAccessModeSpecified  <br/> |Cette erreur indique que vous avez spécifié plus d’une valeur de l’élément [ExchangeImpersonation](exchangeimpersonation.md) au sein d’une requête.  <br/> |
|ErrorMoveCopyFailed  <br/> |Cette erreur indique que l’opération de copie ou de déplacement a échoué. Déplacement de cet événement se produit lors de l' [opération CreateItem](createitem-operation.md) lorsque vous acceptez une demande de réunion qui se trouve dans le dossier éléments supprimés. En outre, si vous refusez une demande de réunion, annulez un élément de calendrier ou supprimez une réunion à partir de votre calendrier, il est déplacé vers le dossier éléments supprimés.  <br/> |
|ErrorMoveDistinguishedFolder  <br/> |Cette erreur se produit si vous tentez de déplacer un dossier unique.  <br/> |
|ErrorMultiLegacyMailboxAccess  <br/> |Cette erreur se produit lorsqu’une demande tente d’accéder à plusieurs serveurs de boîtes aux lettres. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorNameResolutionMultipleResults  <br/> |Cette erreur se produit si l' [opération ResolveNames](resolvenames-operation.md) renvoie plusieurs résultats ou le nom ambigu que vous avez spécifié correspond à plus d’un objet dans le répertoire. Le code de réponse inclut les noms correspondants dans les données de réponse.  <br/> |
|ErrorNameResolutionNoMailbox  <br/> |Cette erreur indique que l’appelant ne dispose pas d’une boîte aux lettres sur le système. [L’opération ResolveNames](resolvenames-operation.md) ou [ExpandDL](expanddl-operation.md) n’est pas valide pour la connexion d’un utilisateur sans une boîte aux lettres.  <br/> |
|ErrorNameResolutionNoResults  <br/> |Cette erreur indique que l' [opération ResolveNames](resolvenames-operation.md) ne renvoie aucun résultat.  <br/> |
|ErrorNoApplicableProxyCASServersAvailable  <br/> |Ce code d’erreur doit être renvoyé lorsque le service Web ne peut pas trouver un serveur pour traiter la demande.  <br/> |
|ErrorNoCalendar  <br/> |Cette erreur se produit si aucun dossier de calendrier pour la boîte aux lettres.  <br/> |
|ErrorNoDestinationCASDueToKerberosRequirements  <br/> |Cette erreur indique que la demande auquel une boîte aux lettres dans un autre site Active Directory, mais aucun serveur d’accès au Client dans le site de destination ont été configurées pour l’authentification Windows, et par conséquent, la demande n’a pas pu transmis par proxy.  <br/> |
|ErrorNoDestinationCASDueToSSLRequirements  <br/> |Cette erreur indique que la demande auquel une boîte aux lettres dans un autre site Active Directory, mais aucun serveur d’accès au Client dans le site de destination ont été configurés pour les connexions SSL et par conséquent, la demande n’a pas pu transmis par proxy.  <br/> |
|ErrorNoDestinationCASDueToVersionMismatch  <br/> |Cette erreur indique que la demande auquel une boîte aux lettres dans un autre site Active Directory, mais aucun serveur d’accès au Client dans le site de destination ont été d’une version de produit acceptable pour recevoir la demande et par conséquent, la demande n’a pas pu transmis par proxy.  <br/> |
|ErrorNoFolderClassOverride  <br/> |Cette erreur se produit si vous définissez l’élément de la [classe FolderClass](folderclass.md) lorsque vous créez un élément autre qu’un dossier générique. Pour les dossiers typées telles que [CalendarFolder](calendarfolder.md) et le [dossier tâches](tasksfolder.md), la classe de dossier est implicite. La définition de la classe d’un dossier à un type de dossier différent à l’aide de [l’opération UpdateFolder](updatefolder-operation.md) les résultats dans la réponse **ErrorObjectTypeChanged** . Au lieu de cela, utilisez un type de dossier générique mais la classe dossier la valeur dont vous avez besoin. Services Web Exchange créera le dossier fortement typé correct.  <br/> |
|ErrorNoFreeBusyAccess  <br/> |Cette erreur indique que l’appelant ne dispose pas des droits d’affichage et de disponibilité sur le dossier calendrier en question.  <br/> |
|ErrorNonExistentMailbox  <br/> | Cette erreur se produit dans les scénarios suivants : <br/> <br/>-L’adresse de messagerie est vide dans [CreateManagedFolder](createmanagedfolder.md).  <br/>-L’adresse de messagerie ne fait pas référence à un compte valide dans la demande est une adresse de messagerie dans le corps ou dans l’en-tête SOAP, comme dans un appel de l’emprunt d’identité Exchange.  <br/> |
|ErrorNonPrimarySmtpAddress  <br/> |Cette erreur se produit lorsque l’appelant passe de l’adresse SMTP non principal. La réponse inclut l’adresse SMTP à utiliser.  <br/> |
|ErrorNoPropertyTagForCustomProperties  <br/> |Cette erreur indique que les propriétés MAPI dans la plage 0 x 8000 personnalisée et versions ultérieures, ne peut pas être référencé par les balises de propriété. Vous devez utiliser la propriété API managées [PropertySetId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.extendedpropertydefinition.propertysetid%28v=exchg.80%29.aspx)ou l’élément EWS [ExtendedFieldURI](extendedfielduri.md) avec l’attribut PropertySetId.  <br/> |
|ErrorNoPublicFolderReplicaAvailable  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorNoPublicFolderServerAvailable  <br/> |Ce code d’erreur doit être renvoyé si aucun serveur de dossiers publics n’est disponible ou si l’appelant ne dispose pas d’un serveur public associé.  <br/> |
|ErrorNoRespondingCASInDestinationSite  <br/> |Cette erreur indique que la demande désigné une boîte aux lettres dans un autre site Active Directory, mais aucun des serveurs d’accès Client au site répondu, et par conséquent, la demande n’a pas pu transmis par proxy.  <br/> |
|ErrorNotAllowedExternalSharingByPolicy  <br/> |Cette erreur indique que l’appelant a essayé d’accorder des autorisations de son dossier calendrier ou les contacts à un utilisateur d’une autre organisation, et que la tentative a échoué.  <br/> |
|ErrorNotDelegate  <br/> |Cette erreur indique que l’utilisateur n’est pas un délégué pour la boîte aux lettres. Il est renvoyé par l' [opération GetDelegate](getdelegate-operation.md), l' [opération RemoveDelegate](removedelegate-operation.md)et l' [opération UpdateDelegate](updatedelegate-operation.md) lorsque l’utilisateur délégué spécifié est introuvable dans la liste des délégués.  <br/> |
|ErrorNotEnoughMemory  <br/> |Cette erreur indique que l’opération a échoué en raison de mémoire insuffisante.  <br/> |
|ErrorNotSupportedSharingMessage  <br/> |Cette erreur indique que le message de partage n’est pas pris en charge.  <br/> |
|ErrorObjectTypeChanged  <br/> |Cette erreur se produit si le type d’objet modifié.  <br/> |
|ErrorOccurrenceCrossingBoundary  <br/> |Cette erreur se produit lorsque l’heure de [début](start.md) ou de [fin](end-ex15websvcsotherref.md) d’une occurrence est mis à jour afin que l’occurrence est planifiée avant ou après l’occurrence correspondant précédent ou suivant.  <br/> |
|ErrorOccurrenceTimeSpanTooBig  <br/> |Cette erreur indique que l’unité de temps d’une occurrence donnée chevauche une autre occurrence du même élément périodique. Cette réponse cet événement se produit lorsque la durée en minutes d’une occurrence de donnée est supérieure à Int32.MaxValue.  <br/> |
|ErrorOperationNotAllowedWithPublicFolderRoot  <br/> |Cette erreur indique que l’opération en cours n’est pas valide pour la racine du dossier public.  <br/> |
|ErrorOrganizationNotFederated  <br/> |Cette erreur indique que l’organisation du demandeur n’est pas fédérée afin que le demandeur ne peut pas créer le partage de messages pour envoyer à un utilisateur externe ou ne peut pas accepter le partage de messages provenant d’un utilisateur externe.  <br/> |
|ErrorParentFolderIdRequired  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorParentFolderNotFound  <br/> |Cette erreur se produit lors de l' [opération CreateFolder](createfolder-operation.md) lorsque le dossier parent est introuvable.  <br/> |
|ErrorPasswordChangeRequired  <br/> |Cette erreur indique que vous devez modifier votre mot de passe avant d’accéder à cette boîte aux lettres. Cela se produit lorsqu’un nouveau compte a été créé et l’administrateur indiqué que l’utilisateur doit changer le mot de passe à la première ouverture de session. Vous ne pouvez pas mettre à jour le mot de passe à l’aide des Services Web Exchange. Vous devez utiliser un outil tel que Microsoft Office Outlook Web App pour modifier votre mot de passe.  <br/> |
|ErrorPasswordExpired  <br/> |Cette erreur indique que le mot de passe a expiré. Vous ne pouvez pas modifier le mot de passe à l’aide des Services Web Exchange. Vous devez utiliser un outil tel que Microsoft Outlook Web App pour modifier votre mot de passe.  <br/> |
|ErrorPermissionNotAllowedByPolicy  <br/> |Cette erreur indique que le demandeur a tenté d’accorder des autorisations dans son calendrier ou dossier de contacts à un utilisateur externe, mais la stratégie de partage associé au demandeur indique que le niveau d’autorisation demandée est supérieur à la stratégie de partage permet.  <br/> |
|ErrorPhoneNumberNotDialable  <br/> |Cette erreur indique que le numéro de téléphone n’était pas dans le formulaire.  <br/> |
|ErrorPropertyUpdate  <br/> |Cette erreur indique que la mise à jour a échoué en raison de valeurs de propriété non valide. Le message de réponse inclut les chemins d’accès de la propriété non valide.  <br/> |
|ErrorPromptPublishingOperationFailed  <br/> |Cette erreur est destinée à une utilisation interne uniquement. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorPropertyValidationFailure  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorProxiedSubscriptionCallFailure  <br/> |Cette erreur indique que la demande auquel un abonnement qui existe sur un autre serveur d’accès au Client, mais une tentative de proxy la demande à ce serveur d’accès au Client a échoué.  <br/> |
|ErrorProxyCallFailed  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorProxyGroupSidLimitExceeded  <br/> |Cette erreur indique que la demande auquel une boîte aux lettres dans un autre site Active Directory et l’appelant d’origine est un membre des groupes de plus de 3 000.  <br/> |
|ErrorProxyRequestNotAllowed  <br/> |Cette erreur indique que la demande de Services Web Exchange envoyés vers un autre serveur d’accès au Client lorsque vous essayez d’exécuter une requête [GetUserAvailabilityRequest](getuseravailabilityrequest.md) n’était pas valide. Ce code de réponse indique généralement qu’une erreur de configuration ou droits s’est produite, ou que quelqu'un a tenté sans succès simuler une demande de proxy de disponibilité.  <br/> |
|ErrorProxyRequestProcessingFailed  <br/> |Cette erreur indique que les Services Web Exchange essayé de proxy une demande de disponibilité vers un autre serveur d’accès au Client pour l’exécution des commandes, mais la demande a échoué. Cette réponse peut être dû à des problèmes de connectivité réseau ou demande des problèmes de délai d’expiration.  <br/> |
|ErrorProxyServiceDiscoveryFailed  <br/> |Ce code d’erreur doit être renvoyé si le service Web ne peut pas déterminer si la demande doit s’exécuter sur le serveur cible ou est transmis par proxy vers un autre serveur.  <br/> |
|ErrorProxyTokenExpired  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorPublicFolderMailboxDiscoveryFailed  <br/> |Cette erreur se produit lorsque la boîte aux lettres de dossier public URL est introuvable. Cette erreur est destinée à une utilisation interne uniquement. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorPublicFolderOperationFailed  <br/> |Cette erreur se produit lors de la tentative d’accéder à un dossier public et la tentative a échoué. Cette erreur a été introduite dans Exchange 2013Exchange Server 2013.  <br/> |
|ErrorPublicFolderRequestProcessingFailed  <br/> |Cette erreur se produit lorsque le destinataire a été passé à l' [opération GetUserAvailability](getuseravailability-operation.md) se trouve sur un ordinateur qui exécute une version d’Exchange Server antérieure à Exchange 2007 et la demande pour récupérer des informations de disponibilité pour le destinataire à partir du serveur de dossiers publics a échoué.  <br/> |
|ErrorPublicFolderServerNotFound  <br/> |Cette erreur se produit lorsque le destinataire a été passé à l' [opération GetUserAvailability](getuseravailability-operation.md) se trouve sur un ordinateur qui exécute une version d’Exchange Server antérieure à Exchange 2007 et la demande pour récupérer des informations de disponibilité pour le destinataire à partir du serveur de dossiers publics a échoué, car l’unité d’organisation ne dispose pas d’un serveur de dossiers publics associée.  <br/> |
|ErrorPublicFolderSyncException  <br/> |Cette erreur se produit lorsqu’une opération de synchronisation réussit par rapport à la boîte aux lettres de dossiers publics principale, mais ne fonctionne pas par rapport à la boîte aux lettres de dossiers publics secondaire. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorQueryFilterTooLong  <br/> |Cette erreur indique que la restriction du dossier de recherche peut être valide, mais il n’est pas pris en charge par EWS. Restrictions pour contenir un maximum de 255 expressions de filtre limite les Services Web Exchange. Si vous essayez de lier à un dossier de recherche existant qui dépasse 255, ce code de réponse est renvoyé.  <br/> |
|ErrorQuotaExceeded  <br/> |Cette erreur se produit lorsque le quota de boîte aux lettres est dépassé.  <br/> |
|ErrorReadEventsFailed  <br/> |Cette erreur est renvoyée par [l’opération GetEvents](getevents-operation.md) ou push notifications lorsqu’une erreur survient lors de la récupération des informations sur l’événement. Lorsque cette erreur est renvoyée, l’abonnement est supprimé. Recréer la synchronisation d’événement basée sur un dernière filigrane connu.  <br/> |
|ErrorReadReceiptNotPending  <br/> |Cette erreur est renvoyée par l' [opération CreateItem](createitem-operation.md) si un utilisateur a tenté de supprimer une confirmation de lecture lorsque l’expéditeur du message n’a pas demandé une confirmation de lecture sur le message ou si le message se trouve dans le dossier courrier indésirable.  <br/> |
|ErrorRecurrenceEndDateTooBig  <br/> |Cette erreur se produit lorsque la date de fin de la périodicité après 9/1/4500.  <br/> |
|ErrorRecurrenceHasNoOccurrence  <br/> |Cette erreur se produit lorsque la périodicité spécifiée n’a pas de toutes les instances occurrence dans la plage spécifiée.  <br/> |
|ErrorRemoveDelegatesFailed  <br/> |Cette erreur indique que la liste des délégués a échoué à enregistrer après que les délégués ont été supprimées.  <br/> |
|ErrorRequestAborted  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorRequestStreamTooBig  <br/> | Cette erreur se produit lorsque le flux de demande est supérieur à 400 Ko.  <br/> |
|ErrorRequiredPropertyMissing  <br/> |Cette erreur est renvoyée lorsque la propriété obligatoire est manquante dans une requête [d’opération CreateAttachment](createattachment-operation.md) . La propriété URI manquante est incluse dans la réponse.  <br/> |
|ErrorResolveNamesInvalidFolderType  <br/> |Cette erreur indique que l’appelant a spécifié un dossier qui n’est pas un dossier de contacts à l' [opération ResolveNames](resolvenames-operation.md).  <br/> |
|ErrorResolveNamesOnlyOneContactsFolderAllowed  <br/> |Cette erreur indique que l’appelant a spécifié plusieurs dossiers de contacts à l' [opération ResolveNames](resolvenames-operation.md).  <br/> |
|ErrorResponseSchemaValidation  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorRestrictionTooLong  <br/> |Cette erreur se produit si la restriction contient plus de 255 nœuds.  <br/> |
|ErrorRestrictionTooComplex  <br/> |Cette erreur se produit lorsque la restriction ne peut pas être évaluée par les Services Web Exchange.  <br/> |
|ErrorResultSetTooBig  <br/> |Cette erreur indique que le nombre d’entrées de calendrier pour un destinataire donné dépasse la limite autorisée de 1000. Réduire la fenêtre et réessayez.  <br/> |
|ErrorSavedItemFolderNotFound  <br/> |Cette erreur se produit lorsque le [SavedItemFolderId](saveditemfolderid.md) est introuvable.  <br/> |
|ErrorSchemaValidation  <br/> | Cette erreur se produit lorsque la demande ne peut pas être validée par rapport au schéma.  <br/> |
|ErrorSearchFolderNotInitialized  <br/> |Cette erreur indique que le dossier de recherche a été créé, mais les critères de recherche n’ont jamais été définies sur le dossier. Cela se produit uniquement lorsque vous accédez à des dossiers de recherche endommagé qui ont été créés à l’aide des API ou un autre client. Pour corriger cette erreur, utilisez l' [opération UpdateFolder](updatefolder-operation.md) pour définir l’élément [SearchParameters](searchparameters.md) pour inclure la restriction qui doit se trouver sur le dossier.  <br/> |
|ErrorSendAsDenied  <br/> | Cette erreur se produit lorsque les deux conditions suivantes se produisent : <br/> <br/>-Un utilisateur dispose des autorisations CanActAsOwner mais ne dispose pas des droits de délégué sur la boîte aux lettres de l’entité de sécurité.  <br/>-Le même utilisateur tente de créer et envoyer un message électronique dans la boîte aux lettres de l’entité de sécurité à l’aide de l’option SendAndSaveCopy.<br/>  <br/>  Le résultat est une erreur ErrorSendAsDenied et la création du message électronique dans le dossier Brouillons de celui du principal.  <br/> |
|ErrorSendMeetingCancellationsRequired  <br/> |Cette erreur est renvoyée par l' [opération DeleteItem](deleteitem-operation.md) si l’attribut **SendMeetingCancellations** est manquant dans la demande et l’élément à supprimer est un élément de calendrier.  <br/> |
|ErrorSendMeetingInvitationsOrCancellationsRequired  <br/> |Cette erreur est renvoyée par l' [opération UpdateItem](updateitem-operation.md) si l’attribut **SendMeetingInvitationsOrCancellations** est manquant dans la demande et de l’élément à mettre à jour est un élément de calendrier.  <br/> |
|ErrorSendMeetingInvitationsRequired  <br/> |Cette erreur est renvoyée par l' [opération CreateItem](createitem-operation.md) si l’attribut **SendMeetingInvitations** est manquant dans la demande et l’élément pour créer un élément de calendrier.  <br/> |
|ErrorSentMeetingRequestUpdate  <br/> |Cette erreur indique qu’une fois que l’organisateur envoie une demande de réunion, la demande ne peut pas être mis à jour. Pour modifier la réunion, modifiez l’élément de calendrier, pas la demande de réunion.  <br/> |
|ErrorSentTaskRequestUpdate  <br/> |Cette erreur indique qu’une fois que l’initiateur de la tâche envoie une demande de tâche, ce type de demande ne peut pas être mis à jour.  <br/> |
|ErrorServerBusy  <br/> |Cette erreur se produit lorsque le serveur est occupé (e).  <br/> |
|ErrorServiceDiscoveryFailed  <br/> |Cette erreur indique que les Services Web Exchange essayé proxy demande de disponibilité d’un utilisateur à la forêt appropriée pour le destinataire, mais il a pas pu déterminer où envoyer la demande en raison d’un échec de la découverte de service.  <br/> |
|ErrorSharingNoExternalEwsAvailable  <br/> |Cette erreur indique que la propriété URL externe n’a pas été définie dans la base de données Active Directory.  <br/> |
|ErrorSharingSynchronizationFailed  <br/> |Cette erreur indique qu’une tentative de synchronisation d’un dossier de partage a échoué. <br/><br/>Ce code d’erreur est renvoyé lorsque le des opérations suivantes se produisent :<br/><br/>-L’abonnement pour un dossier de partage est introuvable.<br/>-Le dossier de partage est introuvable.<br/>-L’utilisateur directory correspondant est introuvable.<br/>-L’utilisateur n’existe plus.<br/>-Le rendez-vous n’est pas valide.<br/>-L’élément de contact n’est pas valide.<br/>-Il existe un problème de communication avec le serveur distant.  <br/> |
|ErrorStaleObject  <br/> |Cette erreur se produit dans une [opération UpdateItem](updateitem-operation.md) ou une [opération SendItem](senditem-operation.md) lors de la touche de modification n’est pas à jour ou non fournie. Appeler l' [opération GetItem](getitem-operation.md) pour récupérer une clé de modification mise à jour et puis réessayez l’opération.  <br/> |
|ErrorSubmissionQuotaExceeded  <br/> |Cette erreur indique qu’un utilisateur ne peuvent pas envoyer immédiatement plusieurs demandes, car le quota d’envoi a été atteinte.  <br/> |
|ErrorSubscriptionAccessDenied  <br/> |Cette erreur se produit lorsque vous essayez d’accéder à un abonnement à l’aide d’un compte qui n’a pas créé de cet abonnement. Chaque abonnement est accessible uniquement par le créateur de l’abonnement.  <br/> |
|ErrorSubscriptionDelegateAccessNotSupported  <br/> |Cette erreur indique que vous ne pouvez pas créer un abonnement si vous n’êtes pas le propriétaire ou n’avez pas accès propriétaire à la boîte aux lettres.  <br/> |
|ErrorSubscriptionNotFound  <br/> |Cette erreur se produit si l’abonnement qui correspond à la [SubscriptionId (GetEvents)](subscriptionid-getevents.md) spécifié est introuvable. L’abonnement a expiré, le processus des Services Web Exchange ont été redémarré ou un abonnement non valide a été passé. Si l’abonnement est valide, recréer l’abonnement avec le filigrane le plus récent. Ceci est retourné par l' [opération Annuler l’abonnement](unsubscribe-operation.md) ou les réponses [GetEvents opération](getevents-operation.md) .  <br/> |
|ErrorSubscriptionUnsubsribed  <br/> |Ce code d’erreur doit être renvoyé lorsqu’une demande est effectuée pour un abonnement qui a été annulé.  <br/> |
|ErrorSyncFolderNotFound  <br/> |Cette erreur est renvoyée par l' [opération SyncFolderItems](syncfolderitems-operation.md) si le dossier parent spécifié est introuvable.  <br/> |
|ErrorTeamMailboxNotFound  <br/> |Cette erreur indique qu’une boîte aux lettres d’équipe est introuvable. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorTeamMailboxNotLinkedToSharePoint  <br/> |Cette erreur indique qu’une boîte aux lettres de l’équipe a été trouvée, mais qu’il n’est pas liée à un serveur SharePoint. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorTeamMailboxUrlValidationFailed  <br/> |Cette erreur indique qu’une boîte aux lettres de l’équipe a été trouvée, mais que le lien vers le serveur SharePoint n’est pas valide. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorTeamMailboxNotAuthorizedOwner  <br/> |Ce code d’erreur n’est pas utilisé. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorTeamMailboxActiveToPendingDelete  <br/> |Ce code d’erreur n’est pas utilisé. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorTeamMailboxFailedSendingNotifications  <br/> |Cette erreur indique qu’une tentative d’envoyer une notification aux propriétaires de boîte aux lettres de l’équipe a échoué. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorTeamMailboxErrorUnknown  <br/> |Cette erreur indique une erreur générale qui peut se produire lorsque vous essayez d’accéder à une boîte aux lettres d’équipe. Essayez d’envoyer la demande à une date ultérieure. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorTimeIntervalTooBig  <br/> |Cette erreur indique que la fenêtre de temps qui a été spécifiée est supérieure à la limite autorisée. Par défaut, la limite autorisée est de 42.  <br/> |
|ErrorTimeoutExpired  <br/> | Cette erreur se produit lorsqu’il n’existe pas de suffisamment de temps pour terminer le traitement de la demande.  <br/> |
|ErrorTimeZone  <br/> |Cette erreur indique qu’il existe une erreur de fuseau horaire.  <br/> |
|ErrorToFolderNotFound  <br/> |Cette erreur indique que le dossier de destination n’existe pas.  <br/> |
|ErrorTokenSerializationDenied  <br/> |Cette erreur se produit si l’appelant essaie de faire une demande de sérialisation de jeton mais n’a pas ms-Exch-EPI-TokenSerialization directement sur le serveur d’accès au Client.  <br/> |
|ErrorTooManyObjectsOpened  <br/> |Cette erreur se produit lorsque la limite interne sur les objets ouverts a été dépassé.  <br/> |
|ErrorUnifiedMessagingDialPlanNotFound  <br/> |Cette erreur indique que le plan de numérotation d’un utilisateur n’est pas disponible.  <br/> |
|ErrorUnifiedMessagingReportDataNotFound  <br/> |Cette erreur est destinée à une utilisation interne uniquement. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorUnifiedMessagingPromptNotFound  <br/> |Cette erreur est destinée à une utilisation interne uniquement. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorUnifiedMessagingRequestFailed  <br/> |Cette erreur indique que l’utilisateur est introuvable.  <br/> |
|ErrorUnifiedMessagingServerNotFound  <br/> |Cette erreur indique qu’un serveur valid pour le plan de numérotation peut être trouvé pour traiter la demande.  <br/> |
|ErrorUnableToGetUserOofSettings  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorUnableToRemoveImContactFromGroup  <br/> |Cette erreur se produit lors d’une tentative pour supprimer un contact de messagerie instantanée d’un groupe. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorUnsupportedCulture  <br/> |Cette erreur se produit lorsque vous essayez de définir la propriété **Culture** sur une valeur qui n’est pas analysable par la classe **System.Globalization.CultureInfo** .  <br/> |
|ErrorUnsupportedMapiPropertyType  <br/> |Cette erreur se produit lorsque l’appelant essaie d’utiliser les propriétés étendues d’objet types, tableau d’objets, erreur ou null.  <br/> |
|ErrorUnsupportedMimeConversion  <br/> |Cette erreur se produit lorsque vous tentez de récupérer ou définir le contenu MIME pour un élément autre qu’un objet [PostItem](postitem.md), un [Message](message-ex15websvcsotherref.md)ou [CalendarItem](calendaritem.md) .  <br/> |
|ErrorUnsupportedPathForQuery  <br/> |Cette erreur se produit lorsque l’appelant transmet une propriété qui n’est pas valide pour une requête. Cela peut se produire lorsque des propriétés calculées sont utilisées.  <br/> |
|ErrorUnsupportedPathForSortGroup  <br/> |Cette erreur se produit lorsque l’appelant transmet une propriété qui n’est pas valide pour un tri ou un groupe à la propriété. Cela peut se produire lorsque des propriétés calculées sont utilisées.  <br/> |
|ErrorUnsupportedPropertyDefinition  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorUnsupportedQueryFilter  <br/> |Cette erreur indique que la restriction du dossier de recherche peut être valide, mais il n’est pas pris en charge par EWS.  <br/> |
|ErrorUnsupportedRecurrence  <br/> |Cette erreur indique que la périodicité spécifiée n’est pas pris en charge pour les tâches.  <br/> |
|ErrorUnsupportedSubFilter  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorUnsupportedTypeForConversion  <br/> |Cette erreur indique que les Services Web Exchange a trouvé un type de propriété dans le magasin mais il ne peut pas générer du code XML pour le type de propriété.  <br/> |
|ErrorUpdateDelegatesFailed  <br/> |Cette erreur indique que la liste des délégués a échoué à enregistrer après que les délégués ont été mis à jour.  <br/> |
|ErrorUpdatePropertyMismatch  <br/> |Cette erreur se produit lorsque le chemin d’accès de la propriété unique qui est répertorié dans la description de la modification ne correspond pas à la propriété unique qui est définie dans l’objet réel de [l’élément](item.md) ou le [dossier](folder.md) .  <br/> |
|ErrorUserNotUnifiedMessagingEnabled  <br/> |Cette erreur indique que le demandeur n’est pas activé.  <br/> |
|ErrorUserNotAllowedByPolicy  <br/> |Cette erreur indique que le demandeur a tenté d’accorder des autorisations dans son calendrier ou dossier de contacts à un utilisateur externe, mais la stratégie de partage associé au demandeur indique que le domaine de l’utilisateur externe n’est pas répertorié dans la stratégie.  <br/> |
|ErrorUserWithoutFederatedProxyAddress  <br/> |Indique que l’organisation du demandeur dispose d’un ensemble de domaines fédérés, mais l’organisation du demandeur n’a pas d’adresse de proxy SMTP avec l’un des domaines fédérés.  <br/> |
|ErrorValueOutOfRange  <br/> |Cette erreur indique qu’un affichage Calendrier la date de début ou date de fin a été défini sur 1/1/0001 12:00:00 AM ou 12/31/9999 11:59:59 PM.  <br/> |
|ErrorVirusDetected  <br/> |Cette erreur indique que la banque d’informations Exchange a détecté un virus dans le message.  <br/> |
|ErrorVirusMessageDeleted  <br/> |Cette erreur indique que la banque d’informations Exchange a détecté un virus dans le message et supprimé.  <br/> |
|ErrorVoiceMailNotImplemented  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorWebRequestInInvalidState  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorWin32InteropError  <br/> |Cette erreur indique qu’une erreur interne lors de la communication avec le code non managé.  <br/> |
|ErrorWorkingHoursSaveFailed  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorWorkingHoursXmlMalformed  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorWrongServerVersion  <br/> |Cette erreur indique qu’une demande ne peut être effectuée sur un serveur qui est la même version que le serveur de boîtes aux lettres.  <br/> |
|ErrorWrongServerVersionDelegate  <br/> |Cette erreur indique qu’une demande a été effectuée par un délégué qui a une version serveur autre que le serveur de boîtes aux lettres de l’entité de sécurité.  <br/> |
|ErrorMissingInformationSharingFolderId  <br/> |Ce code d’erreur n’est jamais retourné.  <br/> |
|ErrorDuplicateSOAPHeader  <br/> |Spécifie qu’il n’y a des en-têtes SOAP en double.  <br/> |
|ErrorSharingSynchronizationFailed  <br/> | Spécifie qu’une tentative de synchronisation d’un dossier de partage a échoué.<br/><br/> Ce code d’erreur doit être renvoyé quand :<br/><br/>-L’abonnement pour un dossier de partage est introuvable.  <br/>-Le dossier de partage est introuvable.  <br/>-L’utilisateur directory correspondant est introuvable.  <br/>-L’utilisateur n’existe plus.  <br/>-Le rendez-vous n’est pas valide.  <br/>-L’élément de contact n’est pas valide.  <br/>-Il y a un échec de communication avec le serveur distant.  <br/> |
|ErrorSharingNoExternalEwsAvailable  <br/> |Spécifie que la propriété URL externe n’a pas été définie dans la base de données Active Directory. Ce code d’erreur doit être renvoyé si la propriété URL externe n’a pas été définie dans la base de données Active Directory.  <br/> |
|ErrorFreeBusyDLLimitReached  <br/> |Spécifie que le nombre de membres du groupe maximale a été atteinte pour obtenir des informations de disponibilité pour une liste de distribution. Cette erreur doit être renvoyée lorsque le nombre de membres du groupe maximale a été atteinte pour obtenir des informations de disponibilité pour une liste de distribution.  <br/> |
|ErrorInvalidGetSharingFolderRequest  <br/> |Spécifie que l’élément de type de données et ShareFolderId sont tous deux présents dans une requête. Ce code d’erreur doit être renvoyé si l’élément de type de données et ShareFolderId est tous deux présents dans une requête.  <br/> |
|ErrorNotAllowedExternalSharingByPolicy  <br/> |Spécifie que l’appelant a essayé d’accorder des autorisations de son dossier calendrier ou les contacts à un utilisateur dans une autre organisation et que la tentative a échoué. Ce code d’erreur doit être renvoyé lors de la stratégie de partage est désactivée pour l’appelant ou lorsque la stratégie de partage affectée à l’appelant n’autorise pas le partage pour le niveau demandé ou le type de dossier demandé.  <br/> |
|ErrorUserNotAllowedByPolicy  <br/> |Spécifie que le demandeur a tenté d’accorder des autorisations dans son calendrier ou dossier de contacts à un utilisateur externe, mais la stratégie de partage affecté au demandeur spécifie que le domaine de l’utilisateur externe n’est pas répertorié dans la stratégie.  <br/> |
|ErrorPermissionNotAllowedByPolicy  <br/> |Spécifie que le demandeur a tenté pour accorder des autorisations de son dossier calendrier ou les contacts à un utilisateur externe, mais la stratégie de partage affecté au demandeur spécifie que le niveau d’autorisation demandée est supérieur à la stratégie de partage permet.  <br/> |
|ErrorOrganizationNotFederated  <br/> |Spécifie qu’organisation du demandeur n’est pas fédérée afin que le demandeur ne peut pas créer le partage de messages pour envoyer à un utilisateur externe ou ne peut pas accepter le partage de messages provenant d’un utilisateur externe. Ce code d’erreur doit être renvoyé si l’organisation du demandeur n’est pas fédérée.  <br/> |
|ErrorMailboxFailover  <br/> |Spécifie que la tentative d’accéder à une boîte aux lettres a échoué, car la boîte aux lettres se trouve dans un processus de basculement.  <br/> |
|ErrorInvalidExternalSharingInitiator  <br/> |Spécifie que l’expéditeur invitation de partage n’a pas créé les métadonnées invitation de partage. Ce code d’erreur doit être renvoyé si l’expéditeur invitation de partage n’a pas créé les métadonnées invitation de partage.  <br/> |
|ErrorMessageTrackingPermanentError  <br/> |Spécifie que le service de suivi de message ne peut pas suivre le message.  <br/> |
|ErrorMessageTrackingTransientError  <br/> |Spécifie que soit le service de suivi des messages est arrêté ou occupé (e). Ce code d’erreur indique une erreur temporaire. Les clients peuvent réessayer de vous connecter au serveur lors de la réception de cette erreur.  <br/> |
|ErrorMessageTrackingNoSuchDomain  <br/> |Spécifie que le domaine spécifié est introuvable.  <br/> |
|ErrorUserWithoutFederatedProxyAddress  <br/> |Spécifie qu’organisation du demandeur dispose d’un ensemble de domaines fédérés mais organisation du demandeur n’a pas d’adresse de proxy SMTP avec l’un des domaines fédérés.  <br/> |
|ErrorInvalidOrganizationRelationshipForFreeBusy  <br/> |Spécifie qu’un appelant a demandé des informations de disponibilité pour un utilisateur d’une autre organisation, mais la relation d’organisation n’a pas activé libre/occupé.  <br/> |
|ErrorInvalidFederatedOrganizationId  <br/> |Spécifie que les objets de fédération du demandeur l’organisation ne sont pas configurés correctement.  <br/> |
|ErrorInvalidExternalSharingSubscriber  <br/> |Spécifie qu’un message de partage n’est pas destiné à l’appelant.  <br/> |
|ErrorInvalidSharingData  <br/> |Spécifie que les métadonnées de partage ne sont pas valide. Cela peut être dû à XML non valide.  <br/> |
|ErrorInvalidSharingMessage  <br/> |Spécifie que le message de partage n’est pas valide. Cela peut être dû à une propriété manquante.  <br/> |
|ErrorNotSupportedSharingMessage  <br/> |Spécifie que le message de partage n’est pas pris en charge.  <br/> |
|ErrorApplyConversationActionFailed  <br/> |Cette erreur doit être renvoyée si une action ne peut pas être appliquée à un ou plusieurs éléments de la conversation.  <br/> |
|ErrorInboxRulesValidationError  <br/> |Cette erreur doit être renvoyée si aucune règle ne valide pas.  <br/> |
|ErrorOutlookRuleBlobExists  <br/> |Cette erreur doit être renvoyée lors de la tentative de gérer les règles de boîte de réception se produit une fois que les règles de boîte de réception a accédé à un autre client.  <br/> |
|ErrorRulesOverQuota  <br/> |Cette erreur doit être renvoyée lorsque le quota de règles d’un utilisateur a été dépassé.  <br/> |
|ErrorNewEventStreamConnectionOpened  <br/> |Cette erreur doit être renvoyée à la première connexion abonnement si une deuxième connexion abonnement est ouvert.  <br/> |
|ErrorMissedNotificationEvents  <br/> |Cette erreur doit être renvoyée lorsque les notifications d’événements sont ignorées.  <br/> |
|ErrorDuplicateLegacyDistinguishedName  <br/> |Cette erreur est renvoyée lorsqu’il existe des noms uniques hérités en double dans les Services de domaine Active Directory (AD DS). Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorInvalidClientAccessTokenRequest  <br/> |Cette erreur indique qu’une demande pour obtenir un accès au client jeton n’était pas valide. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorNoSpeechDetected  <br/> |Cette erreur est destinée à une utilisation interne uniquement. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorUMServerUnavailable  <br/> |Cette erreur est destinée à une utilisation interne uniquement. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorRecipientNotFound  <br/> |Cette erreur est destinée à une utilisation interne uniquement. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorRecognizerNotInstalled  <br/> |Cette erreur est destinée à une utilisation interne uniquement. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorSpeechGrammarError  <br/> |Cette erreur est destinée à une utilisation interne uniquement. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorInvalidManagementRoleHeader  <br/> |Cette erreur est renvoyée si l’en-tête [ManagementRole](managementrole.md) dans l’en-tête SOAP est incorrect. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorLocationServicesDisabled  <br/> |Cette erreur est destinée à une utilisation interne uniquement. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorLocationServicesRequestTimedOut  <br/> |Cette erreur est destinée à une utilisation interne uniquement. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorLocationServicesRequestFailed  <br/> |Cette erreur est destinée à une utilisation interne uniquement. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorLocationServicesInvalidRequest  <br/> |Cette erreur est destinée à une utilisation interne uniquement. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorWeatherServiceDisabled  <br/> |Cette erreur est destinée à une utilisation interne uniquement.  <br/> |
|ErrorMailboxScopeNotAllowedWithoutQueryString  <br/> |Cette erreur est renvoyée lorsqu’une tentative de recherche à étendue définie est exécutée sans l’aide d’un élément de la [chaîne de requête (chaîne)](querystring-string.md) pour une recherche d’indexation de contenu. Cela concerne les opérations **SearchMailboxes** et **FindConversation** . Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorArchiveMailboxSearchFailed  <br/> |Cette erreur est renvoyée lorsqu’une recherche de boîte aux lettres d’archive a échoué. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorArchiveMailboxServiceDiscoveryFailed  <br/> |Cette erreur est renvoyée lorsque l’URL d’une boîte aux lettres d’archivage n’est pas accessible. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorGetRemoteArchiveFolderFailed  <br/> |Cette erreur se produit lorsque l’opération pour obtenir le dossier de boîte aux lettres d’archivage à distance a échoué.  <br/> |
|ErrorFindRemoteArchiveFolderFailed  <br/> |Cette erreur se produit lorsque l’opération pour rechercher le dossier de boîte aux lettres d’archivage à distance a échoué.  <br/> |
|ErrorGetRemoteArchiveItemFailed  <br/> |Cette erreur se produit lorsque l’opération pour obtenir l’élément de boîte aux lettres d’archivage à distance a échoué.  <br/> |
|ErrorExportRemoteArchiveItemsFailed  <br/> |Cette erreur se produit lorsque l’opération pour exporter les éléments de boîte aux lettres d’archivage à distance a échoué.  <br/> |
|ErrorInvalidPhotoSize  <br/> |Cette erreur est renvoyée si une taille de photo non valide est requise à partir du serveur. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorSearchQueryHasTooManyKeywords  <br/> |Cette erreur est renvoyée si une taille de photo inattendue est demandée dans une requête d’opération **GetUserPhoto** . Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorSearchTooManyMailboxes  <br/> |Cette erreur est renvoyée lorsqu’une demande d’opération **SearchMailboxes** contient trop de boîtes aux lettres à rechercher. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorInvalidRetentionTagNone  <br/> |Cette erreur indique qu’aucune des balises de rétention a été trouvés pour cet utilisateur. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorDiscoverySearchesDisabled  <br/> |Cette erreur est renvoyée lorsque les recherches de découverte sont désactivés sur un serveur ou client. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorCalendarSeekToConditionNotSupported  <br/> |Cette erreur se produit lorsque vous essayez d’appeler l' [opération FindItem](finditem-operation.md) avec un [SeekToConditionPageItemView](seektoconditionpageitemview.md) pour l’extraction des éléments de calendrier, qui n’est pas pris en charge.  <br/> |
|ErrorCalendarIsGroupMailboxForAccept  <br/> |Cette erreur est destinée à une utilisation interne uniquement.  <br/> |
|ErrorCalendarIsGroupMailboxForDecline  <br/> |Cette erreur est destinée à une utilisation interne uniquement.  <br/> |
|ErrorCalendarIsGroupMailboxForTentative  <br/> |Cette erreur est destinée à une utilisation interne uniquement.  <br/> |
|ErrorCalendarIsGroupMailboxForSuppressReadReceipt  <br/> |Cette erreur est destinée à une utilisation interne uniquement.  <br/> |
|ErrorOrganizationAccessBlocked  <br/> |Le client est marqué pour suppression.  <br/> |
|ErrorInvalidLicense  <br/> |L’utilisateur n’est pas une licence valide.  <br/> |
|ErrorMessagePerFolderCountReceiveQuotaExceeded  <br/> |Recevoir les messages par dossier de quota a été dépassé.  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément n’est pas obligatoire et n’est pas inclus dans toutes les réponses. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

