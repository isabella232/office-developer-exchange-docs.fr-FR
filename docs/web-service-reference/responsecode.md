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
description: L’élément ResponseCode fournit des informations sur l’état de la demande.
ms.openlocfilehash: 6481272c61aab3dc9aeb2fd988e3544169306f06
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457465"
---
# <a name="responsecode"></a>ResponseCode

L’élément **ResponseCode** fournit des informations sur l’état de la demande. 
  
- [ResponseMessage](responsemessage.md) 
- [ResponseCode](responsecode.md)
  
```XML
<ResponseCode/>
```

**ResponseCodeType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|Élément|Description|
|:-----|:-----|
|[ResponseMessage](responsemessage.md) <br/> | Fournit des informations descriptives sur l’état de la réponse.<br/><br/>  Voici les expressions XPath possibles pour cet élément :<br/><br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/ResponseMessage` <br/><br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/ResponseMessage` <br/><br/>  `/SetUserOofSettingsResponse/ResponseMessage` <br/><br/>  `/GetUserOofSettingsResponse/ResponseMessage` <br/> |
|[DeleteItemResponseMessage](deleteitemresponsemessage.md) <br/> |Contient l’État et le résultat d’une seule demande d' [opération DeleteItem](deleteitem-operation.md) .  <br/> |
|[SendItemResponseMessage](senditemresponsemessage.md) <br/> |Contient l’État et le résultat d’une seule demande d' [opération SendItem](senditem-operation.md) .  <br/> |
|[DeleteFolderResponseMessage](deletefolderresponsemessage.md) <br/> |Contient l’État et le résultat d’une seule demande d' [opération DeleteFolder](deletefolder-operation.md) .  <br/> |
|[DeleteAttachmentResponseMessage](deleteattachmentresponsemessage.md) <br/> |Contient l’État et le résultat d’une seule demande d' [opération DeleteAttachment](deleteattachment-operation.md) .  <br/> |
|[UnsubscribeResponseMessage](unsubscriberesponsemessage.md) <br/> |Contient l’État et le résultat d’une demande d' [opération de désinscription](unsubscribe-operation.md) unique.  <br/> |
|[CreateFolderResponseMessage](createfolderresponsemessage.md) <br/> |Contient l’État et le résultat d’une seule demande d' [opération CreateFolder](createfolder-operation.md) .  <br/> |
|[GetFolderResponseMessage](getfolderresponsemessage.md) <br/> |Contient l’État et le résultat d’une seule demande d' [opération GetFolder](getfolder-operation.md) .  <br/> |
|[UpdateFolderResponseMessage](updatefolderresponsemessage.md) <br/> |Contient l’État et le résultat d’une seule demande d' [opération UpdateFolder](updatefolder-operation.md) .  <br/> |
|[MoveFolderResponseMessage](movefolderresponsemessage.md) <br/> |Contient l’État et le résultat d’une seule demande d' [opération MoveFolder](movefolder-operation.md) .  <br/> |
|[CopyFolderResponseMessage](copyfolderresponsemessage.md) <br/> |Contient l’État et le résultat d’une seule demande d' [opération CopyFolder](copyfolder-operation.md).  <br/> |
|[CreateManagedFolderResponseMessage](createmanagedfolderresponsemessage.md) <br/> |Contient l’État et le résultat d’une seule demande d' [opération CreateManagedFolder](createmanagedfolder-operation.md) .  <br/> |
|[FindFolderResponseMessage](findfolderresponsemessage.md) <br/> |Contient l’État et le résultat d’une seule demande d' [opération FindFolder](findfolder-operation.md) .  <br/> |
|[CreateItemResponseMessage](createitemresponsemessage.md) <br/> |Contient l’État et le résultat d’une seule demande d' [opération CreateItem](createitem-operation.md) .  <br/> |
|[GetItemResponseMessage](getitemresponsemessage.md) <br/> |Contient l’État et le résultat d’une demande d' [opération GetItem](getitem-operation.md) unique.  <br/> |
|[UpdateItemResponseMessage](updateitemresponsemessage.md) <br/> |Contient l’État et le résultat d’une seule demande d' [opération UpdateItem](updateitem-operation.md) .  <br/> |
|[MoveItemResponseMessage](moveitemresponsemessage.md) <br/> |Contient l’État et le résultat d’une seule demande d' [opération MoveItem](moveitem-operation.md) .  <br/> |
|[CopyItemResponseMessage](copyitemresponsemessage.md) <br/> |Contient l’État et le résultat d’une demande d' [opération CopyItem](copyitem-operation.md) unique.  <br/> |
|[CreateAttachmentResponseMessage](createattachmentresponsemessage.md) <br/> |Contient l’État et le résultat d’une seule demande d' [opération CreateAttachment](createattachment-operation.md) .  <br/> |
|[GetAttachmentResponseMessage](getattachmentresponsemessage.md) <br/> |Contient l’État et le résultat d’une seule demande d' [opération GetAttachment](getattachment-operation.md) .  <br/> |
|[FindItemResponseMessage](finditemresponsemessage.md) <br/> |Contient l’État et le résultat d’une seule demande d' [opération FindItem](finditem-operation.md) .  <br/> |
|[ResolveNamesResponseMessage](resolvenamesresponsemessage.md) <br/> |Contient l’État et le résultat d’une demande d' [opération ResolveNames](resolvenames-operation.md) .  <br/> |
|[ExpandDLResponseMessage](expanddlresponsemessage.md) <br/> |Contient l’État et le résultat d’une seule demande d' [opération ExpandDL](expanddl-operation.md) .  <br/> |
|[SubscribeResponseMessage](subscriberesponsemessage.md) <br/> |Contient l’État et le résultat d’une demande d' [opération subscribe](subscribe-operation.md) unique.  <br/> |
|[GetEventsResponseMessage](geteventsresponsemessage.md) <br/> |Contient l’État et le résultat d’une seule demande d' [opération GetEvents](getevents-operation.md) .  <br/> |
|[SendNotificationResponseMessage](sendnotificationresponsemessage.md) <br/> |Contient l’État et le résultat d’une seule demande d’opération SendNotification.  <br/> |
|[SyncFolderHierarchyResponseMessage](syncfolderhierarchyresponsemessage.md) <br/> |Contient l’État et le résultat d’une demande d' [opération opérationsyncfolderhierarchy](syncfolderhierarchy-operation.md) .  <br/> |
|[SyncFolderItemsResponseMessage](syncfolderitemsresponsemessage.md) <br/> |Contient l’État et le résultat d’une demande d' [opération SyncFolderItems](syncfolderitems-operation.md) .  <br/> |
|[ConvertIdResponseMessage](convertidresponsemessage.md) <br/> |Contient l’État et le résultat d’une demande d' [opération ConvertId](convertid-operation.md) .  <br/> |
|[AddDelegateResponse](adddelegateresponse.md) <br/> |Contient l’État et le résultat d’une demande d' [opération AddDelegate](adddelegate-operation.md) .  <br/> |
|[GetDelegateResponse](getdelegateresponse.md) <br/> |Contient l’État et le résultat d’une demande d' [opération GetDelegate](getdelegate-operation.md) .  <br/> |
|[RemoveDelegateResponse](removedelegateresponse.md) <br/> |Contient l’État et le résultat d’une demande d' [opération RemoveDelegate](removedelegate-operation.md) .  <br/> |
|[UpdateDelegateResponse](updatedelegateresponse.md) <br/> |Contient l’État et le résultat d’une demande d' [opération UpdateDelegate](updatedelegate-operation.md) .  <br/> |
|[GetServerTimeZonesResponseMessage](getservertimezonesresponsemessage.md) <br/> |Contient l’État et le résultat d’une demande d' [opération GetServerTimeZones](getservertimezones-operation.md) .  <br/> |
|[GetSharingFolderResponseMessage](getsharingfolderresponsemessage.md) <br/> |Contient l’État et le résultat d’une demande d' [opération GetSharingFolder](getsharingfolder-operation.md) .  <br/> |
|[GetSharingFolderResponse](getsharingfolderresponse.md) <br/> |Définit une réponse à une demande d' [opération GetSharingFolder](getsharingfolder-operation.md) .  <br/> |
|[GetSharingMetadataResponseMessage](getsharingmetadataresponsemessage.md) <br/> |Contient l’État et le résultat d’une demande d' [opération GetSharingMetadata](getsharingmetadata-operation.md) .  <br/> |
|[GetSharingMetadataResponse](getsharingmetadataresponse.md) <br/> |Définit une réponse à une demande de [Opération de GetSharingMetadata](getsharingmetadata-operation.md) .  <br/> |
|[RefreshSharingFolderResponseMessage](refreshsharingfolderresponsemessage.md) <br/> |Contient l’État et le résultat d’une demande d' [opération RefreshSharingFolder](refreshsharingfolder-operation.md) .  <br/> |
|[RefreshSharingFolderResponse](refreshsharingfolderresponse.md) <br/> |Définit une réponse à une demande d' [opération RefreshSharingFolder](refreshsharingfolder-operation.md) .  <br/> |
|[FindConversationResponse](findconversationresponse.md) <br/> |Contient l’État et les résultats d’une réponse d' [opération FindConversation](findconversation-operation.md) .  <br/> |
|[ApplyConversationActionResponseMessage](applyconversationactionresponsemessage.md) <br/> |Contient l’État et les résultats d’une demande d' [opération ApplyConversationAction](applyconversationaction-operation.md) .  <br/> |
|[EmptyFolderResponseMessage](emptyfolderresponsemessage.md) <br/> |Contient l’État et le résultat d’une seule demande d' [opération EmptyFolder](emptyfolder-operation.md) .  <br/> |
|[UpdateInboxRulesResponse](updateinboxrulesresponse.md) <br/> |Contient l’État et le résultat d’une demande d' [opération UpdateInboxRules](updateinboxrules-operation.md) .  <br/> |
|[UploadItemsResponseMessage](uploaditemsresponsemessage.md) <br/> |Contient l’État et le résultat d’une demande d' [opération UploadItems](uploaditems-operation.md) .  <br/> |
|[GetInboxRulesResponse](getinboxrulesresponse.md) <br/> |Contient une réponse à une [opération GetInboxRules](getinboxrules-operation.md) * * * * Request.  <br/> |
|[GetServiceConfigurationResponse](getserviceconfigurationresponse.md) <br/> |Contient une réponse à une demande d' [opération GetServiceConfiguration](getserviceconfiguration-operation.md) .  <br/> |
|[ServiceConfigurationResponseMessageType](serviceconfigurationresponsemessagetype.md) <br/> |Contient les paramètres de configuration du service.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte est requise si cet élément est utilisé. Le tableau suivant décrit les valeurs renvoyées avec cet élément.
  
|Valeur|Description|
|:-----|:-----|
|NoError  <br/> |Aucune erreur n’est survenue pour la demande.  <br/> |
|ErrorAccessDenied  <br/> |Cette erreur se produit lorsque le compte appelant ne dispose pas des autorisations nécessaires pour effectuer l’action demandée.  <br/> |
|ErrorAccessModeSpecified  <br/> |Cette erreur est réservée à un usage interne. Cette erreur n’est pas renvoyée.  <br/> |
|ErrorAccountDisabled  <br/> |Cette erreur se produit lorsque le compte en question a été désactivé.  <br/> |
|ErrorAddDelegatesFailed  <br/> |Cette erreur se produit lorsqu’une liste avec des délégués ajoutés ne peut pas être enregistrée.  <br/> |
|ErrorAddressSpaceNotFound  <br/> |Cette erreur se produit lorsque l’enregistrement d’espace d’adressage, ou le nom de domaine DNS (Domain Name System), pour la disponibilité entre forêts est introuvable dans la base de données Active Directory.  <br/> |
|ErrorADOperation  <br/> |Cette erreur se produit lorsque l’opération a échoué en raison de problèmes de communication avec les services de domaine Active Directory (AD DS).  <br/> |
|ErrorADSessionFilter  <br/> |Cette erreur est renvoyée lorsqu’une demande d’opération **ResolveNames** spécifie un nom qui n’est pas valide.  <br/> |
|ErrorADUnavailable  <br/> |Cette erreur se produit lorsque AD DS n’est pas disponible. Renouvelez votre demande ultérieurement.  <br/> |
|ErrorAffectedTaskOccurrencesRequired  <br/> |Cette erreur indique que l’attribut **AffectedTaskOccurrences** n’a pas été spécifié. Lorsque l’élément [DeleteItem](deleteitem.md) est utilisé pour supprimer au moins un élément qui est une tâche, et indépendamment du fait que cette tâche soit périodique ou non, l’attribut **AffectedTaskOccurrences** doit être spécifié afin que **DeleteItem** puisse déterminer s’il faut supprimer l’occurrence actuelle ou toute la série.  <br/> |
|ErrorArchiveFolderPathCreation  <br/> |Indique une erreur lors de la création du chemin d’accès du dossier d’archivage.  <br/> |
|ErrorArchiveMailboxNotEnabled  <br/> |Indique que la boîte aux lettres d’archivage n’a pas été activée.  <br/> |
|ErrorArchiveMailboxServiceDiscoveryFailed  <br/> |Indique que la découverte du service de boîte aux lettres d’archivage a échoué.  <br/> |
|ErrorAttachmentNestLevelLimitExceeded  <br/> |Spécifie qu’une tentative de création d’un élément avec plus de 10 pièces jointes a été effectuée. Cette valeur a été introduite dans Exchange Server 2010 Service Pack 2 (SP2).  <br/> |
|ErrorAttachmentSizeLimitExceeded  <br/> |L’élément [CreateAttachment](createattachment.md) renvoie cette erreur en cas de tentative de création d’une pièce jointe dont la taille dépasse Int32. MaxValue, en octets.  <br/> L’élément [GetAttachment](getattachment.md) renvoie cette erreur en cas de tentative de récupération d’une pièce jointe existante dont la taille dépasse Int32. MaxValue, en octets.  <br/> |
|ErrorAutoDiscoverFailed  <br/> |Cette erreur indique que les services Web Exchange ont tenté de déterminer l’emplacement d’un ordinateur de forêt croisé exécutant Exchange 2010 sur lequel le rôle de serveur d’accès au client est installé à l’aide du service de découverte automatique, mais l’appel au service de découverte automatique a échoué.  <br/> |
|ErrorAvailabilityConfigNotFound  <br/> |Cette erreur indique que les informations de configuration de disponibilité pour la forêt locale sont manquantes dans AD DS.  <br/> |
|ErrorBatchProcessingStopped  <br/> | Cette erreur indique qu’une exception s’est produite lors du traitement d’un élément et que cette exception est susceptible de se produire pour les éléments qui suivent. Les demandes peuvent inclure plusieurs éléments ; par exemple, une demande d’opération GetItem peut inclure plusieurs identificateurs. En règle générale, les éléments sont traités un par un. Si une exception se produit lors du traitement d’un élément et que cette exception est susceptible de se produire pour les éléments qui suivent, les éléments qui suivent ne seront pas traités.  <br/><br/>  Voici des exemples d’erreurs qui vont arrêter le traitement des éléments suivants :<br/>  <br/>- ErrorAccessDenied  <br/>- ErrorAccountDisabled  <br/>- ErrorADUnavailable  <br/>- ErrorADOperation  <br/>- ErrorConnectionFailed  <br/>- ErrorMailboxStoreUnavailable  <br/>- ErrorMailboxMoveInProgress  <br/>- ErrorPasswordChangeRequired  <br/>- ErrorPasswordExpired  <br/>- ErrorQuotaExceeded  <br/>- ErrorInsufficientResources  <br/> |
|ErrorCalendarCannotMoveOrCopyOccurrence  <br/> |Cette erreur se produit lorsqu’une tentative de déplacement ou de copie d’une occurrence d’un élément de calendrier périodique est effectuée.  <br/> |
|ErrorCalendarCannotUpdateDeletedItem  <br/> | Cette erreur se produit lorsqu’une tentative de mise à jour d’un élément de calendrier se trouvant dans le dossier éléments supprimés est effectuée et que les mises à jour ou annulations de réunion doivent être envoyées en fonction de la valeur de l’attribut **SendMeetingInvitationsOrCancellations** . <br/><br/>Les valeurs possibles pour cet attribut sont les suivantes :  <br/><br/>- SendToAllAndSaveCopy  <br/>- SendToChangedAndSaveCopy  <br/>- SendOnlyToAll  <br/>- SendOnlyToChanged  <br/>  <br/>Toutefois, une telle mise à jour est autorisée uniquement lorsque la valeur de cet attribut est définie sur SendToNone.  <br/> |
|ErrorCalendarCannotUseIdForOccurrenceId  <br/> |Cette erreur se produit lorsque l’opération UpdateItem, GetItem, DeleteItem, MoveItem, CopyItem ou SendItem est appelée et que l’ID spécifié n’est pas un ID d’occurrence d’un élément de calendrier périodique.  <br/> |
|ErrorCalendarCannotUseIdForRecurringMasterId  <br/> |Cette erreur se produit lorsque l’opération **UpdateItem**, **GetItem**, **DeleteItem**, **MoveItem**, **CopyItem**ou **SendItem** est appelée et que l’ID spécifié n’est pas un ID d’un élément de gabarit périodique.  <br/> |
|ErrorCalendarDurationIsTooLong  <br/> |Cette erreur se produit lors d’une opération **CreateItem** ou **UpdateItem** lorsque la durée d’un élément de calendrier est supérieure à la durée maximale autorisée, qui est actuellement de 5 ans.  <br/> |
|ErrorCalendarEndDateIsEarlierThanStartDate  <br/> |Cette erreur se produit lorsqu’une heure de fin du calendrier est définie sur la même heure ou après l’heure de début.  <br/> |
|ErrorCalendarFolderIsInvalidForCalendarView  <br/> |Cette erreur se produit lorsque le dossier spécifié pour une opération **FindItem** avec un élément [CalendarView](calendarview.md) n’est pas du type de dossier de calendrier.  <br/> |
|ErrorCalendarInvalidAttributeValue  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorCalendarInvalidDayForTimeChangePattern  <br/> |Cette erreur se produit lors d’une opération **CreateItem** ou **UpdateItem** lorsque des valeurs non valides de Day, WeekendDay et Weekday sont utilisées pour définir le modèle de changement d’heure.  <br/> |
|ErrorCalendarInvalidDayForWeeklyRecurrence  <br/> |Cette erreur se produit lors d’une opération **CreateItem** ou **UpdateItem** lorsque des valeurs non valides de Day, Weekday et WeekendDay sont utilisées pour spécifier la périodicité hebdomadaire.  <br/> |
|ErrorCalendarInvalidPropertyState  <br/> |Cette erreur se produit lorsque l’état d’un objet BLOB de récurrence d’élément de calendrier dans la Banque d’instructions Exchange n’est pas valide.  <br/> |
|ErrorCalendarInvalidPropertyValue  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorCalendarInvalidRecurrence  <br/> |Cette erreur se produit lorsque la périodicité spécifiée ne peut pas être créée.  <br/> |
|ErrorCalendarInvalidTimeZone  <br/> |Cette erreur se produit lorsqu’un fuseau horaire incorrect est rencontré.  <br/> |
|ErrorCalendarIsCancelledForAccept  <br/> |Cette erreur indique qu’un élément de calendrier a été annulé.  <br/> |
|ErrorCalendarIsCancelledForDecline  <br/> |Cette erreur indique qu’un élément de calendrier a été annulé.  <br/> |
|ErrorCalendarIsCancelledForRemove  <br/> |Cette erreur indique qu’un élément de calendrier a été annulé.  <br/> |
|ErrorCalendarIsCancelledForTentative  <br/> |Cette erreur indique qu’un élément de calendrier a été annulé.  <br/> |
|ErrorCalendarIsDelegatedForAccept  <br/> |Cette erreur indique que l’élément [AcceptItem](acceptitem.md) n’est pas valide pour un élément de calendrier ou une demande de réunion dans un scénario délégué.  <br/> |
|ErrorCalendarIsDelegatedForDecline  <br/> |Cette erreur indique que l’élément [DeclineItem](declineitem.md) n’est pas valide pour un élément de calendrier ou une demande de réunion dans un scénario délégué.  <br/> |
|ErrorCalendarIsDelegatedForRemove  <br/> |Cette erreur indique que l’élément [RemoveItem](removeitem.md) n’est pas valide pour une annulation de réunion dans un scénario délégué.  <br/> |
|ErrorCalendarIsDelegatedForTentative  <br/> |Cette erreur indique que l’élément [TentativelyAcceptItem](tentativelyacceptitem.md) n’est pas valide pour un élément de calendrier ou une demande de réunion dans un scénario délégué.  <br/> |
|ErrorCalendarIsNotOrganizer  <br/> |Cette erreur indique que l’opération (actuellement CancelItem) sur l’élément de calendrier n’est pas valide pour un participant. Seul l’organisateur de la réunion peut annuler la réunion.  <br/> |
|ErrorCalendarIsOrganizerForAccept  <br/> |Cette erreur indique qu' [AcceptItem](acceptitem.md) n’est pas valide pour l’élément de calendrier de l’organisateur.  <br/> |
|ErrorCalendarIsOrganizerForDecline  <br/> |Cette erreur indique qu' [DeclineItem](declineitem.md) n’est pas valide pour l’élément de calendrier de l’organisateur.  <br/> |
|ErrorCalendarIsOrganizerForRemove  <br/> |Cette erreur indique que [RemoveItem](removeitem.md) n’est pas valide pour l’élément de calendrier de l’organisateur. Pour supprimer une réunion du calendrier, l’organisateur doit utiliser CancelCalendarItem.  <br/> |
|ErrorCalendarIsOrganizerForTentative  <br/> |Cette erreur indique qu' [TentativelyAcceptItem](tentativelyacceptitem.md) n’est pas valide pour l’élément de calendrier de l’organisateur.  <br/> |
|ErrorCalendarMeetingRequestIsOutOfDate  <br/> |Cette erreur indique qu’une demande de réunion est obsolète et qu’elle ne peut pas être mise à jour.  <br/> |
|ErrorCalendarOccurrenceIndexIsOutOfRecurrenceRange  <br/> |Cette erreur indique que l’index d’occurrence ne pointe pas vers une occurrence dans la périodicité actuelle. Par exemple, si votre périodicité définit un ensemble de trois occurrences de réunion et que vous tentez d’accéder à la cinquième occurrence, ce code de réponse est obtenu.  <br/> |
|ErrorCalendarOccurrenceIsDeletedFromRecurrence  <br/> |Cette erreur indique que toute opération effectuée sur une occurrence supprimée (adressée via un ID de fichier principal périodique et un index d’occurrence) n’est pas valide.  <br/> |
|ErrorCalendarOutOfRange  <br/> |Cette erreur est signalée pour les opérations CreateItem et UpdateItem pour les éléments de calendrier ou les propriétés de récurrence de tâche lorsque la valeur de la propriété est en dehors de la plage. Par exemple, si vous spécifiez le quinzième semaine du mois, ce code de réponse est obtenu.  <br/> |
|ErrorCalendarViewRangeTooBig  <br/> |Cette erreur se produit lorsque la plage de début à fin de l’élément [CalendarView](calendarview.md) est supérieure à la valeur maximale autorisée, actuellement 2 ans.  <br/> |
|ErrorCallerIsInvalidADAccount  <br/> |Cette erreur indique que le compte demandeur n’est pas un compte valide dans la base de données d’annuaire.  <br/> |
|ErrorCannotArchiveCalendarContactTaskFolderException  <br/> |Indique qu’une tentative d’archivage d’un dossier de tâches de contact de calendrier a été effectuée.  <br/> |
|ErrorCannotArchiveItemsInPublicFolders  <br/> |Indique qu’une tentative d’archivage d’éléments dans des dossiers publics a été effectuée.  <br/> |
|ErrorCannotArchiveItemsInArchiveMailbox  <br/> |Indique qu’une tentative d’archivage d’éléments dans la boîte aux lettres d’archivage a été effectuée.  <br/> |
|ErrorCannotCreateCalendarItemInNonCalendarFolder  <br/> |Cette erreur survient lorsqu’un élément de calendrier est créé et que l’attribut **SavedItemFolderId** fait référence à un dossier non-calendrier.  <br/> |
|ErrorCannotCreateContactInNonContactFolder  <br/> |Cette erreur se produit lorsqu’un contact est créé et que l’attribut **SavedItemFolderId** fait référence à un dossier qui n’est pas un contact.  <br/> |
|ErrorCannotCreatePostItemInNonMailFolder  <br/> |Cette erreur indique qu’un élément de publication ne peut pas être créé dans un dossier autre qu’un dossier de messagerie, tel qu’un calendrier, un contact, des tâches, des notes, etc.  <br/> |
|ErrorCannotCreateTaskInNonTaskFolder  <br/> |Cette erreur se produit lorsqu’une tâche est créée et que l’attribut **SavedItemFolderId** fait référence à un dossier non lié à une tâche.  <br/> |
|ErrorCannotDeleteObject  <br/> |Cette erreur se produit lorsque l’élément ou le dossier à supprimer ne peut pas être supprimé.  <br/> |
|ErrorCannotDeleteTaskOccurrence  <br/> |L' [opération DeleteItem](deleteitem-operation.md) renvoie cette erreur lorsqu’elle ne parvient pas à supprimer l’occurrence actuelle d’une tâche périodique. Cela ne peut se produire que si l’attribut **AffectedTaskOccurrences** a été défini sur SpecifiedOccurrenceOnly.  <br/> |
|ErrorCannotDisableMandatoryExtension  <br/> |Indique qu’une tentative de désactivation d’une extension mandatorty a été effectuée.  <br/> |
|ErrorCannotEmptyFolder  <br/> |Cette erreur doit être renvoyée lorsque le serveur ne peut pas vider un dossier.  <br/> |
|ErrorCannotGetSourceFolderPath  <br/> |Indique que le chemin d’accès du dossier source n’a pas pu être récupéré.  <br/> |
|ErrorCannotGetExternalEcpUrl  <br/> |Spécifie que le serveur n’a pas pu récupérer l’URL externe pour les options Outlook Web App.  <br/> |
|ErrorCannotOpenFileAttachment  <br/> |L’opération **GetAttachment** renvoie cette erreur si elle ne peut pas récupérer le corps d’une pièce jointe.  <br/> |
|ErrorCannotSetCalendarPermissionOnNonCalendarFolder  <br/> |Cette erreur indique que l’appelant a essayé de définir des autorisations de calendrier sur un dossier qui n’est pas un calendrier.  <br/> |
|ErrorCannotSetNonCalendarPermissionOnCalendarFolder  <br/> |Cette erreur indique que l’appelant a essayé de définir des autorisations non-calendrier sur un dossier de calendrier.  <br/> |
|ErrorCannotSetPermissionUnknownEntries  <br/> |Cette erreur indique que vous ne pouvez pas définir d’autorisations inconnues dans un jeu d’autorisations.  <br/> |
|ErrorCannotSpecifySearchFolderAsSourceFolder  <br/> |Indique qu’une tentative de spécification du dossier de recherche en tant que dossier source a été effectuée.  <br/> |
|ErrorCannotUseFolderIdForItemId  <br/> |Cette erreur se produit lorsqu’une demande nécessitant un identificateur d’élément reçoit un identificateur de dossier.  <br/> |
|ErrorCannotUseItemIdForFolderId  <br/> |Cette erreur se produit lorsqu’une demande nécessitant un identificateur de dossier reçoit un identificateur d’élément.  <br/> |
|ErrorChangeKeyRequired  <br/> |Ce code de réponse a été remplacé par **ErrorChangeKeyRequiredForWriteOperations** <br/> |
|ErrorChangeKeyRequiredForWriteOperations  <br/> |Cette erreur est renvoyée lorsque la clé de modification d’un élément est manquante ou obsolète. <br/><br/>Pour les opérations SendItem, UpdateItem et UpdateFolder, l’appelant doit transmettre une clé de modification valide et actuelle pour l’élément. Notez que c’est le cas avec UpdateItem même si la résolution des conflits est définie sur toujours remplacer.  <br/> |
|ErrorClientDisconnected  <br/> |Spécifie que le client a été déconnecté.  <br/> |
|ErrorClientIntentInvalidStateDefinition  <br/> |Cette erreur est destinée à un usage interne uniquement.  <br/> |
|ErrorClientIntentNotFound  <br/> |Cette erreur est destinée à un usage interne uniquement.  <br/> |
|ErrorConnectionFailed  <br/> |Cette erreur se produit lorsque les services Web Exchange ne peuvent pas se connecter à la boîte aux lettres.  <br/> |
|ErrorContainsFilterWrongType  <br/> |Cette erreur indique que la propriété qui a été inspectée pour un filtre Contains n’est pas de type chaîne.  <br/> |
|ErrorContentConversionFailed  <br/> |L’opération **GetItem** renvoie cette erreur lorsque les services Web Exchange ne peuvent pas récupérer le contenu MIME de l’élément demandé. <br/><br/>L’opération **CreateItem** renvoie cette erreur lorsque les services Web Exchange ne peuvent pas créer l’élément à partir du contenu MIME fourni. En règle générale, cela indique que la propriété Item est endommagée ou tronquée.  <br/> |
|ErrorContentIndexingNotEnabled  <br/> |Cette erreur se produit lorsqu’une demande de recherche est effectuée à l’aide de l’option QueryString et que l’indexation de contenu n’est pas activée pour la boîte aux lettres cible.  <br/> |
|ErrorCorruptData  <br/> |Cette erreur se produit lorsque les données sont endommagées et ne peuvent pas être traitées.  <br/> |
|ErrorCreateItemAccessDenied  <br/> |Cette erreur se produit lorsque l’appelant n’est pas autorisé à créer l’élément.  <br/> |
|ErrorCreateManagedFolderPartialCompletion  <br/> |Cette erreur se produit lorsqu’un ou plusieurs dossiers gérés qui ont été spécifiés dans la demande d’opération CreateManagedFolder n’ont pas pu être créés. Recherchez chaque dossier pour déterminer les dossiers qui ont été créés et ceux qui n’existent pas.  <br/> |
|ErrorCreateSubfolderAccessDenied  <br/> |Cette erreur se produit lorsque le compte appelant ne dispose pas des autorisations nécessaires pour créer le sous-dossier.  <br/> |
|ErrorCrossMailboxMoveCopy  <br/> |Cette erreur se produit lors d’une tentative de déplacement d’un élément ou d’un dossier d’une boîte aux lettres à une autre. Si la boîte aux lettres source et la boîte aux lettres de destination sont différentes, vous obtiendrez cette erreur.  <br/> |
|ErrorCrossSiteRequest  <br/> |Cette erreur indique que la demande n’est pas autorisée car le serveur d’accès au client qui doit traiter la demande se trouve dans un autre site.  <br/> |
|ErrorDataSizeLimitExceeded  <br/> |Cette erreur peut se produire dans les scénarios suivants :<br/>  <br/>-Une tentative est effectuée pour accéder à une propriété sur un élément ou l’écrire, et la valeur de la propriété est trop grande.<br/>-La longueur du contenu MIME encodé en Base64 dans le code XML de la demande dépasse la limite.<br/>-La taille du corps d’un élément existant dépasse la limite.<br/>-Le consommateur tente de définir un corps de texte ou HTML dont la longueur (ou longueur combinée en cas d’ajout) dépasse la limite. |
|ErrorDataSourceOperation  <br/> |Cette erreur se produit lorsque le fournisseur de données sous-jacent ne parvient pas à terminer l’opération.  <br/> |
|ErrorDelegateAlreadyExists  <br/> |Cette erreur se produit dans une opération **AddDelegate** lorsque l’utilisateur spécifié existe déjà dans la liste des délégués.  <br/> |
|ErrorDelegateCannotAddOwner  <br/> |Cette erreur se produit dans une opération **AddDelegate** lorsque l’utilisateur spécifié à ajouter est le propriétaire de la boîte aux lettres.  <br/> |
|ErrorDelegateMissingConfiguration  <br/> |Cette erreur se produit dans une opération **GetDelegate** lorsqu’il n’y a pas d’informations de délégué sur le message freebusy local ou aucun délégué public Active Directory (aucun « délégué public » ou aucune entrée « envoyer de la part de » dans AD DS).  <br/> |
|ErrorDelegateNoUser  <br/> |Cette erreur se produit lorsqu’un utilisateur spécifié ne peut pas être mappé à un utilisateur dans AD DS.  <br/> |
|ErrorDelegateValidationFailed  <br/> |Cette erreur se produit dans l’opération **AddDelegate** lorsqu’un utilisateur délégué ajouté n’est pas valide.  <br/> |
|ErrorDeleteDistinguishedFolder  <br/> |Cette erreur se produit lorsqu’une tentative de suppression d’un dossier unique est effectuée.  <br/> |
|ErrorDeleteItemsFailed  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorDeleteUnifiedMessagingPromptFailed  <br/> |Cette erreur est destinée à un usage interne uniquement.  <br/> |
|ErrorDistinguishedUserNotSupported  <br/> |Cette erreur indique qu’un ID d’utilisateur unique n’est pas valide pour l’opération. **DistinguishedUserType** ne doit pas être présent dans la demande.  <br/> |
|ErrorDistributionListMemberNotExist  <br/> |Cette erreur indique qu’un membre de la liste de distribution de demande n’existe pas dans la liste de distribution.  <br/> |
|ErrorDuplicateInputFolderNames  <br/> |Cette erreur se produit lorsque des noms de dossier en double sont spécifiés dans l’élément [foldernames](foldernames.md) de la demande d’opération **CreateManagedFolder** .  <br/> |
|ErrorDuplicateSOAPHeader  <br/> |Cette erreur indique qu’il existe des en-têtes SOAP en double.  <br/> |
|ErrorDuplicateUserIdsSpecified  <br/> |Cette erreur indique qu’un ID utilisateur en double a été trouvé dans un jeu d’autorisations, que la valeur par défaut ou anonyme est définie plusieurs fois ou qu’il existe des SID ou des destinataires en double.  <br/> |
|ErrorEmailAddressMismatch  <br/> |Cette erreur se produit lorsqu’une requête tente de créer/mettre à jour les paramètres de recherche d’un dossier de recherche. Par exemple, cela peut se produire lorsqu’un dossier de recherche est créé dans la boîte aux lettres, mais que le dossier de recherche est dirigé vers une autre boîte aux lettres.  <br/> |
|ErrorEventNotFound  <br/> |Cette erreur se produit lorsque l’événement associé à un filigrane est supprimé avant le renvoi de l’événement. Lorsque cette erreur est renvoyée, l’abonnement est également supprimé.  <br/> |
|ErrorExceededConnectionCount  <br/> |Cette erreur-indique qu’il y a plus de demandes simultanées sur le serveur que ce qui est autorisé par la stratégie de l’utilisateur.  <br/> |
|ErrorExceededSubscriptionCount  <br/> |Cette erreur indique que le nombre maximal d’abonnements de stratégie de limitation d’un utilisateur a été dépassé.  <br/> |
|ErrorExceededFindCountLimit  <br/> |Cette erreur indique qu’un appel d’opération de recherche a dépassé le nombre total d’éléments pouvant être renvoyés.  <br/> |
|ErrorExpiredSubscription  <br/> |Cette erreur se produit si l' [opération GetEvents](getevents-operation.md) est appelée alors qu’un abonnement est en cours de suppression car elle a expiré.  <br/> |
|ErrorExtensionNotFound  <br/> |Indique que l’extension est introuvable.  <br/> |
|ErrorFolderCorrupt  <br/> |Cette erreur se produit lorsque le dossier est endommagé et ne peut pas être enregistré.  <br/> |
|ErrorFolderExists  <br/> |Cette erreur se produit lors d’une tentative de création d’un dossier portant le même nom qu’un autre dossier dans le même parent. Les noms de dossier en double ne sont pas autorisés.  <br/> |
|ErrorFolderNotFound  <br/> |Cette erreur indique que l’ID de dossier spécifié ne correspond pas à un dossier valide ou que le délégué n’est pas autorisé à accéder au dossier.  <br/> |
|ErrorFolderPropertRequestFailed  <br/> |Cette erreur indique que la propriété demandée n’a pas pu être récupérée. Cela n’indique pas que la propriété n’existe pas, mais que la propriété a été endommagée de façon à ce que la récupération ait échoué.  <br/> |
|ErrorFolderSave  <br/> |Cette erreur indique que le dossier n’a pas pu être créé ou mis à jour en raison d’un État non valide.  <br/> |
|ErrorFolderSaveFailed  <br/> |Cette erreur indique que le dossier n’a pas pu être créé ou mis à jour en raison d’un État non valide.  <br/> |
|ErrorFolderSavePropertyError  <br/> |Cette erreur indique que le dossier n’a pas pu être créé ou mis à jour en raison de valeurs de propriété non valides. Le code de réponse répertorie les propriétés à l’origine du problème.  <br/> |
|ErrorFreeBusyDLLimitReached  <br/> |Cette erreur indique que le nombre maximal de membres du groupe a été atteint pour obtenir des informations de disponibilité pour une liste de distribution.  <br/> |
|ErrorFreeBusyGenerationFailed  <br/> |Cette erreur est renvoyée lorsque les informations de disponibilité ne peuvent pas être récupérées en raison d’un échec intermédiaire.  <br/> |
|ErrorGetServerSecurityDescriptorFailed  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorImContactLimitReached  <br/> |Cette erreur est renvoyée lorsque les nouveaux contacts de messagerie instantanée ne peuvent pas être ajoutés, car le nombre maximal de contacts a été atteint. Cette erreur a été introduite dans Exchange Server 2013.  <br/> |
|ErrorImGroupDisplayNameAlreadyExists  <br/> |Cette erreur est renvoyée lors d’une tentative d’ajout d’un nom d’affichage de groupe lorsqu’un groupe existant porte déjà le même nom d’affichage. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorImGroupLimitReached  <br/> |Cette erreur est renvoyée lorsque les nouveaux groupes de messagerie instantanée ne peuvent pas être ajoutés car le nombre maximal de groupes a été atteint. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorImpersonateUserDenied  <br/> |L’erreur est renvoyée dans le cas d’autorisation de serveur à serveur pour l’emprunt d’identité Exchange lorsque l’appelant ne dispose pas des droits appropriés pour emprunter l’identité de l’utilisateur spécifique en question. Cette erreur est mappée avec le droit Active Directory étendu ms-Exch-EPI-May-emprunter.  <br/> |
|ErrorImpersonationDenied  <br/> |Cette erreur est renvoyée dans l’autorisation de serveur à serveur pour l’emprunt d’identité Exchange lorsque l’appelant ne dispose pas des droits suffisants pour emprunter l’identité via le serveur d’accès au client auquel il effectue la demande. Ceci est mappé au droit Active Directory étendu ms-Exch-EPI-emprunt d’identité.  <br/> |
|ErrorImpersonationFailed  <br/> |Cette erreur indique qu’une erreur inattendue s’est produite lors d’une tentative d’authentification de serveur à serveur. Ce code de réponse indique généralement que le compte de service qui exécute le pool d’applications des services Web Exchange est configuré de manière incorrecte, que les services Web Exchange ne peuvent pas communiquer avec l’annuaire ou qu’une approbation entre les forêts n’est pas correctement configurée.  <br/> |
|ErrorIncorrectSchemaVersion  <br/> |Cette erreur indique que la demande est valide pour la version actuelle d’Exchange Server mais qu’elle n’était pas valide pour la version du serveur de requêtes qui a été spécifiée.  <br/> |
|ErrorIncorrectUpdatePropertyCount  <br/> |Cette erreur indique que chaque description de modification dans les éléments [UpdateItem](updateitem.md) ou [UpdateFolder](updatefolder.md) doit répertorier une seule propriété à mettre à jour.  <br/> |
|ErrorIndividualMailboxLimitReached  <br/> |Cette erreur se produit lorsque la demande contient trop de participants à résoudre. Par défaut, le nombre maximal de participants à résoudre est de 100.  <br/> |
|ErrorInsufficientResources  <br/> |Cette erreur se produit lorsque le serveur de boîtes aux lettres est surchargé. Renouvelez votre demande ultérieurement.  <br/> |
|ErrorInternalServerError  <br/> |Cette erreur indique que les services Web Exchange ont rencontré une erreur qu’il n’a pas pu récupérer et qu’un code de réponse plus spécifique associé à l’erreur qui s’est produite n’existe pas.  <br/> |
|ErrorInternalServerTransientError  <br/> |Cette erreur indique qu’une erreur de serveur interne s’est produite et que vous devez retenter votre demande plus tard.  <br/> |
|ErrorInvalidAccessLevel  <br/> |Cette erreur indique que le niveau d’accès de l’appelant sur les données de disponibilité n’est pas valide.  <br/> |
|ErrorInvalidArgument  <br/> |Cette erreur indique une erreur causée par tous les arguments non valides transmis à l' [opération GetMessageTrackingReport](getmessagetrackingreport-operation.md).<br/><br/> Cette erreur est renvoyée dans les scénarios suivants : <br/><br/>-L’utilisateur spécifié dans le paramètre _sending As_ n’existe pas dans l’annuaire. <br/>-L’utilisateur spécifié dans le paramètre _sending As_ n’est pas unique dans l’annuaire. <br/>-L’adresse _expéditeur_ est vide.<br/>-L’adresse _expéditeur_ n’est pas une adresse de messagerie valide.  <br/> |
|ErrorInvalidAttachmentId  <br/> |Cette erreur est renvoyée par l' [opération GetAttachment](getattachment-operation.md) ou l' [opération DeleteAttachment](deleteattachment-operation.md) lorsqu’une pièce jointe correspondant à l’ID spécifié est introuvable.  <br/> |
|ErrorInvalidAttachmentSubfilter  <br/> |Cette erreur se produit lorsque vous essayez de lier un dossier de recherche existant à l’aide d’une restriction de tableau de pièces jointes complexe. Les services Web Exchange prennent en charge uniquement les filtres de contenu simple dans le tableau des pièces jointes. Si vous essayez d’établir une liaison avec un dossier de recherche existant dont la restriction de table de pièces jointe est plus complexe (sous-filtre), les services Web Exchange ne peuvent pas restituer le code XML pour ce filtre et renvoyer ce code de réponse. <br/><br/>Notez que vous pouvez toujours appeler l’opération GetFolder sur le dossier, mais ne pas demander l’élément [SearchParameters](searchparameters.md) .  <br/> |
|ErrorInvalidAttachmentSubfilterTextFilter  <br/> |Cette erreur se produit lorsque vous essayez de lier un dossier de recherche existant à l’aide d’une restriction de tableau de pièces jointes complexe. Les services Web Exchange prennent en charge uniquement les filtres de contenu simple dans le tableau des pièces jointes. <br/><br/>Si vous essayez d’établir une liaison avec un dossier de recherche existant dont la restriction de table de pièces jointe est plus complexe, les services Web Exchange ne peuvent pas restituer le code XML pour ce filtre. Dans ce cas, le sous-filtre de pièce jointe contient un filtre de texte, mais il ne recherche pas le nom d’affichage de la pièce jointe.<br/><br/> Notez que vous pouvez toujours appeler l’opération GetFolder sur le dossier, mais ne pas demander l’élément [SearchParameters](searchparameters.md) .  <br/> |
|ErrorInvalidAuthorizationContext  <br/> | Cette erreur indique que la procédure d’autorisation pour le demandeur a échoué.  <br/> |
|ErrorInvalidChangeKey  <br/> |Cette erreur se produit lorsqu’un consommateur passe un identificateur de dossier ou d’élément avec une clé de modification qui ne peut pas être analysée. Par exemple, il peut s’agir d’un contenu base64 non valide ou d’une chaîne vide.  <br/> |
|ErrorInvalidClientSecurityContext  <br/> |Cette erreur indique qu’une erreur interne s’est produite lors d’une tentative de résolution de l’identité de l’appelant.  <br/> |
|ErrorInvalidCompleteDate  <br/> |Cette erreur est renvoyée lors d’une tentative de définition de la valeur de l’élément [terminé](completedate.md) d’une tâche à une heure ultérieure. Lorsqu’elle est convertie en heure locale du serveur d’accès au client, l' [achèvement](completedate.md) d’une tâche ne peut pas être défini sur une valeur qui est postérieure à l’heure locale sur le serveur d’accès au client.  <br/> |
|ErrorInvalidContactEmailAddress  <br/> |Cette erreur indique qu’une adresse de messagerie non valide a été fournie pour un contact.  <br/> |
|ErrorInvalidContactEmailIndex  <br/> |Cette erreur indique qu’une valeur d’index de messagerie non valide a été fournie pour une entrée de courrier électronique.  <br/> |
|ErrorInvalidCrossForestCredentials  <br/> |Cette erreur se produit lorsque les informations d’identification utilisées pour transmettre par proxy une demande à une forêt de service d’annuaire différente ont échoué à l’authentification.  <br/> |
|ErrorInvalidDelegatePermission  <br/> |Cette erreur indique que les autorisations de dossier spécifiées ne sont pas valides.  <br/> |
|ErrorInvalidDelegateUserId  <br/> |Cette erreur indique que l’ID utilisateur du délégué spécifié n’est pas valide.  <br/> |
|ErrorInvalidExchangeImpersonationHeaderData  <br/> |Cette erreur se produit lors de l’emprunt d’identité Exchange lorsqu’un appelant ne spécifie pas de nom d’utilisateur principal, d’adresse de messagerie ou de SID d’utilisateur. Cela se produit également si l’appelant spécifie une ou plusieurs de ces valeurs et que les valeurs sont vides.  <br/> |
|ErrorInvalidExcludesRestriction  <br/> |Cette erreur se produit lorsque le masque de masque qui a été passé dans une restriction d’élément [excludes](excludes.md) ne peut pas être analysé.  <br/> |
|ErrorInvalidExpressionTypeForSubFilter  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorInvalidExtendedProperty  <br/> | Cette erreur se produit lorsque les événements suivants ont lieu : <br/> <br/>-L’appelant tente d’utiliser une propriété étendue qui n’est pas prise en charge par les services Web Exchange.  <br/>-L’appelant transmet une combinaison non valide de valeurs d’attribut pour une propriété étendue. Cela se produit également si aucun attribut n’est passé. Seules certaines combinaisons sont autorisées.  <br/> |
|ErrorInvalidExtendedPropertyValue  <br/> |Cette erreur se produit lorsque la section valeur d’une propriété étendue ne correspond pas au type de la propriété. <br/><br/>Par exemple, la définition d’une propriété étendue dont PropertyType = "String" contient un tableau d’entiers génère cette erreur. Toute représentation sous forme de chaîne qui ne peut pas être convertie en type spécifié pour la propriété étendue génère cette erreur.  <br/> |
|ErrorInvalidExternalSharingInitiator  <br/> |Cette erreur indique que l’expéditeur de l’invitation de partage n’a pas créé les métadonnées de l’invitation de partage.  <br/> |
|ErrorInvalidExternalSharingSubscriber  <br/> |Cette erreur indique qu’un message de partage n’est pas destiné à l’appelant.  <br/> |
|ErrorInvalidFederatedOrganizationId  <br/> |Cette erreur indique que les objets de Fédération de l’organisation du demandeur ne sont pas configurés correctement.  <br/> |
|ErrorInvalidFolderId  <br/> |Cette erreur se produit lorsque l’ID de dossier est endommagé.  <br/> |
|ErrorInvalidFolderTypeForOperation  <br/> |Cette erreur indique que le type de dossier spécifié n’est pas valide pour l’opération en cours. Par exemple, vous ne pouvez pas créer un dossier de recherche dans un dossier public.  <br/> |
|ErrorInvalidFractionalPagingParameters  <br/> | Cette erreur se produit dans la pagination fractionnaire lorsque l’utilisateur a spécifié l’un des éléments suivants : <br/> <br/>-Un numérateur supérieur au dénominateur  <br/>-Un numérateur inférieur à zéro  <br/>-Un dénominateur inférieur ou égal à zéro  <br/> |
|ErrorInvalidGetSharingFolderRequest  <br/> |Cette erreur indique que le [type de données](datatype.md) et les éléments ShareFolderId sont tous les deux présents dans une demande.  <br/> |
|ErrorInvalidFreeBusyViewType  <br/> |Cette erreur se produit lorsque l' [opération GetUserAvailability](getuseravailability-operation.md) est appelée avec un [FreeBusyViewType](freebusyviewtype.md) nul.  <br/> |
|ErrorInvalidId  <br/> |Cette erreur indique que l’ID et/ou la clé de modification est incorrecte.  <br/> |
|ErrorInvalidIdEmpty  <br/> |Cette erreur se produit lorsque l’appelant spécifie un attribut **ID** qui est vide.  <br/> |
|ErrorInvalidLikeRequest  <br/> |Cette erreur se produit lorsque l’élément ne peut pas être aimé. Les versions d’Exchange commençant par le numéro de Build 15.00.0913.09 incluent cette valeur.  <br/> |
|ErrorInvalidIdMalformed  <br/> |Cette erreur se produit lorsque l’appelant spécifie un attribut **ID** qui est incorrect.  <br/> |
|ErrorInvalidIdMalformedEwsLegacyIdFormat  <br/> |Cette erreur indique qu’un dossier ou un ID d’élément qui utilise le format Exchange 2007 a été spécifié pour une demande avec une version d’Exchange 2007 SP1 ou version ultérieure. Vous ne pouvez pas utiliser les ID Exchange 2007 dans les requêtes Exchange 2007 SP1 ou version ultérieure. Vous devez utiliser l' [opération ConvertId](convertid-operation.md) pour les convertir en premier.  <br/> |
|ErrorInvalidIdMonikerTooLong  <br/> |Cette erreur se produit lorsque l’appelant spécifie un attribut **ID** trop long.  <br/> |
|ErrorInvalidIdNotAnItemAttachmentId  <br/> |Cette erreur est renvoyée chaque fois qu’un ID qui n’est pas un ID de pièce jointe d’un élément est transmis à une méthode de service Web qui attend un ID de pièce jointe.  <br/> |
|ErrorInvalidIdReturnedByResolveNames  <br/> |Cette erreur se produit lorsqu’un contact de votre boîte aux lettres est endommagé.  <br/> |
|ErrorInvalidIdStoreObjectIdTooLong  <br/> |Cette erreur se produit lorsque l’appelant spécifie un attribut **ID** trop long.  <br/> |
|ErrorInvalidIdTooManyAttachmentLevels  <br/> |Cette erreur est renvoyée lorsque la hiérarchie des pièces jointes d’un élément dépasse le nombre maximal de 255 niveaux.  <br/> |
|ErrorInvalidIdXml  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorInvalidImContactId  <br/> |Cette erreur est renvoyée lorsque l’identificateur de contact de messagerie instantanée spécifié ne représente pas un identificateur valide. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorInvalidImDistributionGroupSmtpAddress  <br/> |Cette erreur est renvoyée lorsque l’identificateur d’adresse SMTP du groupe de distribution de messagerie instantanée spécifié ne représente pas un identificateur valide. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorInvalidImGroupId  <br/> |Cette erreur est renvoyée lorsque l’identificateur de groupe de messagerie instantanée spécifié ne représente pas un identificateur valide. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorInvalidIndexedPagingParameters  <br/> |Cette erreur se produit si l’offset pour la pagination indexée est négatif.  <br/> |
|ErrorInvalidInternetHeaderChildNodes  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorInvalidItemForOperationArchiveItem  <br/> |Indique que l’élément n’était pas valide pour une opération **ArchiveItem** .  <br/> |
|ErrorInvalidItemForOperationAcceptItem  <br/> |Cette erreur se produit lors d’une tentative d’utilisation d’un objet Response AcceptItem pour un type d’élément autre qu’une demande de réunion ou un élément de calendrier, ou lorsqu’une tentative d’acceptation d’une occurrence d’élément de calendrier se trouve dans le dossier éléments supprimés est effectuée.  <br/> |
|ErrorInvalidItemForOperationCancelItem  <br/> |Cette erreur se produit lors d’une tentative d’utilisation d’un objet de réponse CancelItem sur un type d’élément autre qu’un élément de calendrier.  <br/> |
|ErrorInvalidItemForOperationCreateItemAttachment  <br/> | Cette erreur est renvoyée lorsqu’une tentative de création d’une pièce jointe d’un élément non pris en charge est effectuée.  <br/><br/>  Les types d’éléments pris en charge pour les pièces jointes d’élément incluent les objets suivants :  <br/><br/>- [Complémentaires](item.md) <br/>- [Message](message-ex15websvcsotherref.md) <br/>- [CalendarItem](calendaritem.md) <br/>- [Tâche](task.md) <br/>- [Prenez](contact.md) <br/> <br/> Par exemple, si vous essayez de créer une pièce jointe [MeetingMessage](meetingmessage.md) , vous rencontrerez ce code de réponse.  <br/> |
|ErrorInvalidItemForOperationCreateItem  <br/> | Cette erreur est renvoyée par une [opération CreateItem](createitem-operation.md) si la demande contient un type d’élément non pris en charge. <br/><br/>Les éléments pris en charge incluent les objets suivants :<br/>  <br/>- [Complémentaires](item.md) <br/>- [Message](message-ex15websvcsotherref.md) <br/>- [CalendarItem](calendaritem.md) <br/>- [Tâche](task.md) <br/>- [Prenez](contact.md) <br/><br/>  Certains types sont créés en tant qu’effet secondaire de l’exécution d’autres éléments. Les messages de réunion, par exemple, sont créés lorsque vous envoyez un élément de calendrier aux participants ; elles ne sont pas explicitement créées.  <br/> |
|ErrorInvalidItemForOperationDeclineItem  <br/> |Cette erreur se produit lors d’une tentative d’utilisation d’un objet Response DeclineItem pour un type d’élément autre qu’une demande de réunion ou un élément de calendrier, ou lorsqu’une tentative de refus d’une occurrence d’élément de calendrier dans le dossier éléments supprimés est effectuée.  <br/> |
|ErrorInvalidItemForOperationExpandDL  <br/> |Cette erreur indique que l' [opération ExpandDL](expanddl-operation.md) est valide uniquement pour les listes de distribution privées.  <br/> |
|ErrorInvalidItemForOperationRemoveItem  <br/> |Cette erreur est renvoyée à partir d’un objet de réponse RemoveItem si la requête spécifie un élément qui n’est pas un élément d’annulation de réunion.  <br/> |
|ErrorInvalidItemForOperationSendItem  <br/> |Cette erreur est renvoyée par une [opération SendItem](senditem-operation.md) si la demande spécifie un élément qui n’est pas un élément de message.  <br/> |
|ErrorInvalidItemForOperationTentative  <br/> |Cette erreur se produit lors d’une tentative d’utilisation de [TentativelyAcceptItem](tentativelyacceptitem.md) pour un type d’élément autre qu’une demande de réunion ou un élément de calendrier, ou lorsqu’une tentative d’acceptation provisoire d’une occurrence d’élément de calendrier dans le dossier éléments supprimés est effectuée.  <br/> |
|ErrorInvalidLogonType  <br/> |Cette erreur est réservée à un usage interne. Cette erreur n’est pas renvoyée.  <br/> |
|ErrorInvalidMailbox  <br/> |Cette erreur indique que l' [opération CreateItem](createitem-operation.md) ou l' [opération UpdateItem](updateitem-operation.md) a échoué lors de la création ou de la mise à jour d’une liste de distribution personnelle.  <br/> |
|ErrorInvalidManagedFolderProperty  <br/> |Cette erreur se produit lorsque la structure du dossier géré est endommagée et ne peut pas être rendue.  <br/> |
|ErrorInvalidManagedFolderQuota  <br/> |Cette erreur se produit lorsque le quota défini sur le dossier géré est inférieur à zéro, ce qui indique un dossier géré endommagé.  <br/> |
|ErrorInvalidManagedFolderSize  <br/> |Cette erreur se produit lorsque la taille définie sur le dossier géré est inférieure à zéro, ce qui indique un dossier géré endommagé.  <br/> |
|ErrorInvalidMergedFreeBusyInterval  <br/> |Cette erreur se produit lorsque la valeur interne de disponibilité fusionnée fournie n’est pas valide. La valeur minimale par défaut est de 5 minutes. La valeur maximale par défaut est de 1440 minutes.  <br/> |
|ErrorInvalidNameForNameResolution  <br/> |Cette erreur se produit lorsque le nom n’est pas valide pour l' [opération ResolveNames](resolvenames-operation.md). Par exemple, une chaîne de longueur nulle, un espace, une virgule et un tiret sont tous des noms non valides.  <br/> |
|ErrorInvalidNetworkServiceContext  <br/> |Cette erreur indique une erreur dans le compte de service réseau sur le serveur d’accès au client.  <br/> |
|ErrorInvalidOofParameter  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorInvalidOperation  <br/> | Il s’agit d’une erreur générale qui est utilisée lorsque l’opération demandée n’est pas valide. <br/><br/>Par exemple, vous ne pouvez pas effectuer les opérations suivantes : <br/> <br/>-Effectuer un parcours « approfondi » à l’aide de l' [opération FindFolder](findfolder-operation.md) sur un dossier public.  <br/>-Déplacer ou copier la racine du dossier public.  <br/>-Supprimer un élément associé à l’aide de n’importe quel mode, à l’exception de la suppression « Hard ».  <br/>-Déplacer ou copier un élément associé.  <br/> |
|ErrorInvalidOrganizationRelationshipForFreeBusy  <br/> |Cette erreur indique qu’un appelant a demandé des informations de disponibilité pour un utilisateur d’une autre organisation, mais que la relation organisationnelle n’est pas disponible/occupée.  <br/> |
|ErrorInvalidPagingMaxRows  <br/> |Cette erreur se produit lorsqu’un consommateur passe un zéro ou une valeur négative pour le nombre maximal de lignes à renvoyer.  <br/> |
|ErrorInvalidParentFolder  <br/> |Cette erreur se produit lorsqu’un consommateur passe un dossier parent non valide pour une opération. Par exemple, cette erreur est renvoyée si vous essayez de créer un dossier dans un dossier de recherche.  <br/> |
|ErrorInvalidPercentCompleteValue  <br/> |Cette erreur est renvoyée lorsqu’une tentative de définition d’un pourcentage d’achèvement de tâche sur une valeur non valide est effectuée. La valeur doit être comprise entre 0 et 100 (inclus).  <br/> |
|ErrorInvalidPermissionSettings  <br/> |Cette erreur indique que le niveau d’autorisation n’est pas cohérent avec les paramètres d’autorisation.  <br/> |
|ErrorInvalidPhoneCallId  <br/> |Cette erreur indique que l’identificateur de l’appelant n’est pas valide.  <br/> |
|ErrorInvalidPhoneNumber  <br/> |Cette erreur indique que le numéro de téléphone n’est pas correct ou qu’il ne correspond pas aux règles de plan de numérotation.  <br/> |
|ErrorInvalidPropertyAppend  <br/> | Cette erreur se produit lorsque la propriété à laquelle vous essayez d’ajouter ne prend pas en charge l’ajout. <br/><br/>Les propriétés suivantes sont les seules à prendre en charge l’ajout : <br/> <br/>-Collections de destinataires (ToRecipients, CcRecipients, BccRecipients)  <br/>-Collections de participants (RequiredAttendees, OptionalAttendees, ressources)  <br/>-Body  <br/>-ReplyTo  <br/><br/>  En outre, cette erreur se produit lorsqu’un corps de message est ajouté si le format spécifié dans la demande ne correspond pas au format de l’élément dans la Banque.  <br/> |
|ErrorInvalidPropertyDelete  <br/> |Cette erreur se produit si l’opération de suppression est spécifiée dans une [opération UpdateItem](updateitem-operation.md) ou un appel d' [opération UpdateFolder](updatefolder-operation.md) pour une propriété qui ne prend pas en charge l’opération Delete. Par exemple, vous ne pouvez pas supprimer l’élément [ItemId](itemid.md) de l’objet [Item](item.md) .  <br/> |
|ErrorInvalidPropertyForExists  <br/> |Cette erreur se produit si le consommateur passe l’une des propriétés d’indicateur dans un filtre [Exists](exists.md) . Par exemple, cette erreur se produit si les indicateurs [IsRead](isread.md) ou [IsFromMe](isfromme.md) sont spécifiés dans l’élément [Exists](exists.md) . La demande doit utiliser l’élément [IsEqualTo](isequalto.md) à la place de ces indicateurs, et donc une partie d’une propriété unique.  <br/> |
|ErrorInvalidPropertyForOperation  <br/> |Cette erreur se produit lorsque la propriété que vous essayez de manipuler ne prend pas en charge l’opération qui est en cours d’exécution.  <br/> |
|ErrorInvalidPropertyRequest  <br/> | Cette erreur se produit si une propriété spécifiée dans la demande n’est pas disponible pour le type d’élément. Par exemple, cette erreur est renvoyée si une propriété qui est disponible uniquement pour les éléments de calendrier est demandée dans un appel d' [opération GetItem](getitem-operation.md) pour un message ou si elle est mise à jour dans un appel d' [opération UpdateItem](updateitem-operation.md) pour un message. <br/> <br/>  Cela se produit dans les opérations suivantes : <br/> <br/>- [Opération GetItem](getitem-operation.md) <br/>- [Opération GetFolder](getfolder-operation.md) <br/>- [Opération UpdateItem](updateitem-operation.md) <br/>- [Opération UpdateFolder](updatefolder-operation.md) <br/> |
|ErrorInvalidPropertySet  <br/> |Cette erreur indique que la propriété que vous essayez de manipuler ne prend pas en charge l’opération qui est en cours d’exécution. Par exemple, cette erreur est renvoyée si la propriété que vous essayez de définir est en lecture seule.  <br/> |
|ErrorInvalidPropertyUpdateSentMessage  <br/> | Cette erreur se produit lors d’une [opération UpdateItem](updateitem-operation.md) lorsqu’un client tente de mettre à jour certaines propriétés d’un message qui a déjà été envoyé.<br/><br/> Par exemple, les propriétés suivantes ne peuvent pas être mises à jour sur un message envoyé : <br/> <br/>- [IsReadReceiptRequested](isreadreceiptrequested.md) <br/>- [IsDeliveryReceiptRequested](isdeliveryreceiptrequested.md) <br/> |
|ErrorInvalidProxySecurityContext  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorInvalidPullSubscriptionId  <br/> |Cette erreur se produit si vous appelez l’opération [GetEvents](getevents-operation.md) ou l' [opération d’annulation](unsubscribe-operation.md) d’abonnement à l’aide d’un ID d’abonnement envoyé. Pour annuler l’abonnement à un abonnement envoyé, vous devez répondre à une demande de transmission avec une réponse de désinscription, ou déconnecter votre service Web et attendre que les notifications de type transmission soient Expires.  <br/> |
|ErrorInvalidPushSubscriptionUrl  <br/> | Cette erreur est renvoyée par l' [opération subscribe](subscribe-operation.md) lorsqu’elle crée un abonnement « envoyer » et indique que l’URL incluse dans la demande n’est pas valide.<br/><br/>Les conditions suivantes doivent être remplies pour que les services Web Exchange acceptent l’URL : <br/> <br/>-La longueur de la chaîne \> 0 et \< 2083.  <br/> -Protocol est http ou HTTPS.  <br/>-L’URL peut être analysée par la classe URI Microsoft .NET Framework.  <br/> |
|ErrorInvalidRecipients  <br/> |Cette erreur indique que la collection de destinataires de votre message ou la collection de participants de votre élément de calendrier n’est pas valide. Par exemple, cette erreur est renvoyée lorsqu’une tentative d’envoi d’un élément qui n’a pas de destinataires est effectuée.  <br/> |
|ErrorInvalidRecipientSubfilter  <br/> |Cette erreur indique que le dossier de recherche a un filtre de table de destinataires qui ne peut pas être représenté par les services Web Exchange. Pour résoudre cette erreur, récupérez le dossier sans demander les paramètres de recherche.  <br/> |
|ErrorInvalidRecipientSubfilterComparison  <br/> |Cette erreur indique que le dossier de recherche a un filtre de table de destinataires qui ne peut pas être représenté par les services Web Exchange. Pour résoudre cette erreur, récupérez le dossier sans demander les paramètres de recherche.  <br/> |
|ErrorInvalidRecipientSubfilterOrder  <br/> |Cette erreur indique que le dossier de recherche a un filtre de table de destinataires qui ne peut pas être représenté par les services Web Exchange. Pour résoudre cette erreur, récupérez le dossier sans demander les paramètres de recherche.  <br/> |
|ErrorInvalidRecipientSubfilterTextFilter  <br/> |Cette erreur indique que le dossier de recherche a un filtre de table de destinataires qui ne peut pas être représenté par les services Web Exchange. Pour résoudre cette erreur, récupérez le dossier sans demander les paramètres de recherche.  <br/> |
|ErrorInvalidReferenceItem  <br/> | Cette erreur est renvoyée à partir de l' [opération CreateItem](createitem-operation.md) pour les objets de réponse avant et réponse dans les scénarios suivants :<br/>  <br/>-L’identificateur d’élément référencé n’est pas un [message](message-ex15websvcsotherref.md), un [CalendarItem](calendaritem.md)ou un descendant d’un **message** ou **CalendarItem**.  <br/>-L’identificateur d’élément de référence est destiné à un **CalendarItem** et l’organisateur essaie de répondre ou ReplyAll à lui-même.  <br/>-Le message est un brouillon et réponse ou ReplyAll est sélectionné.  <br/>-L’élément de référence, pour [SuppressReadReceipt](suppressreadreceipt.md), n’est pas un **message** ni un descendant d’un **message**.  <br/> |
|ErrorInvalidRequest  <br/> |Cette erreur se produit lorsque la demande SOAP a un en-tête d’action SOAP, mais rien dans le corps SOAP. Notez que l’en-tête de l’action SOAP n’est pas obligatoire, car les services Web Exchange peuvent déterminer la méthode à appeler à partir du nom local de l’élément racine dans le corps SOAP.  <br/> |
|ErrorInvalidRestriction  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorInvalidRetentionTagTypeMismatch  <br/> |Cette erreur est renvoyée lorsque la balise de rétention spécifiée comporte une action incorrecte. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorInvalidRetentionTagInvisible  <br/> |Cette erreur est renvoyée lorsqu’une tentative de définition d’une balise inexistante ou invisible sur une propriété **PolicyTag** est effectuée. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorInvalidRetentionTagInheritance  <br/> |Cette erreur est renvoyée lorsqu’une tentative de définition d’une balise implicite sur la propriété **PolicyTag** est effectuée. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorInvalidRetentionTagIdGuid  <br/> |Indique que le GUID de balise de rétention n’était pas valide.  <br/> |
|ErrorInvalidRoutingType  <br/> |Cette erreur se produit si le type de routage transmis pour un élément [RoutingType (EmailAddressType)](routingtype-emailaddresstype.md) n’est pas valide. En règle générale, le type de routage est défini sur le protocole SMTP (Simple Mail Transfer Protocol).  <br/> |
|ErrorInvalidScheduledOofDuration  <br/> |Cette erreur se produit si l’heure de fin spécifiée n’est pas postérieure à l’heure de début ou si l’heure de fin ne se produit pas à l’avenir.  <br/> |
|ErrorInvalidSchemaVersionForMailboxVersion  <br/> |Cette erreur indique qu’une demande de proxy qui a été envoyée à un autre serveur ne peut pas traiter la demande en raison d’une incompatibilité de version.  <br/> |
|ErrorInvalidSecurityDescriptor  <br/> |Cette erreur indique que le descripteur de sécurité Exchange du dossier calendrier du magasin est endommagé.  <br/> |
|ErrorInvalidSendItemSaveSettings  <br/> |Cette erreur se produit lors d’une tentative d’envoi d’un élément dans lequel [SavedItemFolderId](saveditemfolderid.md) est spécifié dans la demande, mais que la propriété **SaveItemToFolder** est définie sur **false**.  <br/> |
|ErrorInvalidSerializedAccessToken  <br/> |Cette erreur indique que le jeton qui a été passé dans l’en-tête est incorrect, ne fait pas référence à un compte valide dans le répertoire ou ne dispose pas du groupe principal **ConnectingSID**.  <br/> |
|ErrorInvalidSharingData  <br/> |Cette erreur indique que les métadonnées de partage ne sont pas valides. Cela peut être dû à un code XML non valide.  <br/> |
|ErrorInvalidSharingMessage  <br/> |Cette erreur indique que le message de partage n’est pas valide. Cela peut être dû à une propriété manquante.  <br/> |
|ErrorInvalidSid  <br/> |Cette erreur se produit lorsqu’un SID non valide est transmis dans une demande.  <br/> |
|ErrorInvalidSIPUri  <br/> |Cette erreur indique que le nom SIP, le plan de numérotation ou le numéro de téléphone sont des URI SIP non valides.  <br/> |
|ErrorInvalidServerVersion  <br/> |Cette erreur indique qu’une version de serveur de requête non valide a été spécifiée dans la demande.  <br/> |
|ErrorInvalidSmtpAddress  <br/> |Cette erreur se produit lorsque l’adresse SMTP ne peut pas être analysée.  <br/> |
|ErrorInvalidSubfilterType  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorInvalidSubfilterTypeNotAttendeeType  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorInvalidSubfilterTypeNotRecipientType  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorInvalidSubscription  <br/> |Cette erreur indique que l’abonnement n’est plus valide. Cela peut être dû au fait que le serveur d’accès au client redémarre ou que l’abonnement a expiré.  <br/> |
|ErrorInvalidSubscriptionRequest  <br/> |Cette erreur indique que la demande subscribe inclut plusieurs ID de dossiers publics. Un abonnement peut inclure plusieurs dossiers provenant de la même boîte aux lettres ou d’un même ID de dossier public.  <br/> |
|ErrorInvalidSyncStateData  <br/> |Cette erreur est renvoyée par [SyncFolderItems](syncfolderitems.md) ou [opérationsyncfolderhierarchy](syncfolderhierarchy.md) si les données [SyncState](syncstate-ex15websvcsotherref.md) transmises ne sont pas valides. Pour corriger cette erreur, vous devez resynchroniser sans l’état de synchronisation. Assurez-vous que si vous conservez les BLOBs d’état de synchronisation, vous ne tronquez pas accidentellement le BLOB.  <br/> |
|ErrorInvalidTimeInterval  <br/> |Cette erreur indique que l’intervalle de temps spécifié n’est pas valide. L’heure de début doit être supérieure ou égale à l’heure de fin.  <br/> |
|ErrorInvalidUserInfo  <br/> |Cette erreur indique qu’un [ID utilisateur](userid.md) incohérent de manière interne a été spécifié pour une opération d’autorisation. Par exemple, si un ID d’utilisateur unique est spécifié (par défaut ou anonyme), cette erreur est renvoyée si vous essayez également de spécifier un SID, ou une adresse SMTP principale ou un nom complet pour cet utilisateur.  <br/> |
|ErrorInvalidUserOofSettings  <br/> |Cette erreur indique que les paramètres d’absence du Bureau de l’utilisateur ne sont pas valides en raison d’une réponse interne ou externe manquante.  <br/> |
|ErrorInvalidUserPrincipalName  <br/> |Cette erreur se produit lors de l’emprunt d’identité Exchange. L’appelant a passé un nom d’utilisateur principal non valide dans l’en-tête SOAP qui n’était pas accessible dans l’annuaire.  <br/> |
|ErrorInvalidUserSid  <br/> |Cette erreur se produit lorsqu’un SID non valide est transmis dans une demande.  <br/> |
|ErrorInvalidUserSidMissingUPN  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorInvalidValueForProperty  <br/> |Cette erreur indique que la valeur de comparaison dans la restriction n’est pas valide pour la propriété avec laquelle vous comparez.<br/><br/> Par exemple, la valeur de comparaison de [DateTimeCreated](datetimecreated.md)  >  **true** renvoie ce code de réponse. <br/><br/>Ce code de réponse est également renvoyé si vous spécifiez une propriété d’énumération dans la comparaison, mais que la valeur comparée n’est pas une valeur valide pour cette énumération.  <br/> |
|ErrorInvalidWatermark  <br/> |Cette erreur est due à un filigrane non valide.  <br/> |
|ErrorIPGatewayNotFound  <br/> |Cette erreur indique qu’une passerelle VoIP valide n’est pas disponible.  <br/> |
|ErrorIrresolvableConflict  <br/> |Cette erreur indique que la résolution des conflits n’a pas pu résoudre les modifications apportées aux propriétés. Les éléments du magasin ont peut-être été modifiés et doivent être mis à jour. Récupérez la clé de modification mise à jour, puis réessayez.  <br/> |
|ErrorItemCorrupt  <br/> |Cette erreur indique que l’état de l’objet est endommagé et qu’il ne peut pas être récupéré. Lorsque vous récupérez un élément, seuls certains éléments seront dans cet État, comme [Body](body.md) et [lamimecontent](mimecontent.md). Omettez ces éléments et recommencez l’opération.  <br/> |
|ErrorItemNotFound  <br/> |Cette erreur se produit lorsque l’élément est introuvable ou que vous n’êtes pas autorisé à accéder à l’élément.  <br/> |
|ErrorItemPropertyRequestFailed  <br/> |Cette erreur se produit en cas d’échec d’une demande de propriété sur un élément. La propriété existe peut-être, mais elle n’a pas pu être récupérée.  <br/> |
|ErrorItemSave  <br/> |Cette erreur se produit lorsque l’enregistrement d’un élément ou d’un dossier échoue.  <br/> |
|ErrorItemSavePropertyError  <br/> |Cette erreur se produit lorsque des tentatives d’enregistrement de l’élément ou du dossier échouent en raison de valeurs de propriété non valides. Le code de réponse inclut le chemin d’accès aux propriétés non valides.  <br/> |
|ErrorLegacyMailboxFreeBusyViewTypeNotMerged  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorLocalServerObjectNotFound  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorLogonAsNetworkServiceFailed  <br/> |Cette erreur indique que le service de disponibilité n’a pas pu se connecter en tant que service réseau pour transmettre les requêtes proxy aux sites ou aux forêts appropriés. Cette réponse indique généralement une erreur de configuration.  <br/> |
|ErrorMailboxConfiguration  <br/> |Cette erreur indique que les informations de boîte aux lettres dans AD DS sont configurées de manière incorrecte.  <br/> |
|ErrorMailboxDataArrayEmpty  <br/> |Cette erreur indique que l’élément [MailboxDataArray](mailboxdataarray.md) de la demande est vide. Vous devez fournir au moins un identificateur de boîte aux lettres.  <br/> |
|ErrorMailboxDataArrayTooBig  <br/> |Cette erreur se produit lorsque plus de 100 entrées sont fournies dans un élément [MailboxDataArray](mailboxdataarray.md) ..  <br/> |
|ErrorMailboxFailover  <br/> |Cette erreur indique qu’une tentative d’accès à une boîte aux lettres a échoué car la boîte aux lettres est dans un processus de basculement.  <br/> |
|ErrorMailboxHoldNotFound  <br/> |Indique que la conservation de boîte aux lettres est introuvable.  <br/> |
|ErrorMailboxLogonFailed  <br/> |Cette erreur se produit lorsque la connexion à la boîte aux lettres pour obtenir les informations d’affichage du calendrier a échoué.  <br/> |
|ErrorMailboxMoveInProgress  <br/> | Cette erreur indique que la boîte aux lettres est déplacée vers un autre serveur ou une autre banque de boîtes aux lettres. Cette erreur peut également indiquer que la boîte aux lettres se trouve sur un autre serveur ou une autre base de données de boîtes aux lettres.  <br/> |
|ErrorMailboxStoreUnavailable  <br/> | Cette erreur indique que l’une des conditions d’erreur suivantes s’est produite :  <br/><br/>-La Banque de boîtes aux lettres est endommagée.  <br/>-La Banque de boîtes aux lettres est en cours d’arrêt.  <br/>-La Banque de boîtes aux lettres est hors connexion.  <br/>-Une erreur réseau s’est produite lors d’une tentative d’accès à la Banque de boîtes aux lettres.  <br/>-La Banque de boîtes aux lettres est surchargée et ne peut pas accepter de connexions supplémentaires.  <br/>-La Banque de boîtes aux lettres a été suspendue.  <br/> |
|ErrorMailRecipientNotFound  <br/> |Cette erreur se produit si les informations de l’élément [MailboxData](mailboxdata.md) ne peuvent pas être mappées à un compte de boîte aux lettres valide.  <br/> |
|ErrorMailTipsDisabled  <br/> |Cette erreur indique que les conseils de messagerie sont désactivés.  <br/> |
|ErrorManagedFolderAlreadyExists  <br/> |Cette erreur se produit si le dossier géré que vous essayez de créer existe déjà dans une boîte aux lettres.  <br/> |
|ErrorManagedFolderNotFound  <br/> |Cette erreur se produit lorsque le nom de dossier spécifié dans la demande ne correspond pas à une définition de dossier géré dans AD DS. Vous pouvez uniquement créer des instances de dossiers gérés pour les dossiers définis dans AD DS. Vérifiez le nom, puis réessayez.  <br/> |
|ErrorManagedFoldersRootFailure  <br/> |Cette erreur indique que la racine de dossiers gérés a été supprimée de la boîte aux lettres ou qu’un dossier existe dans le même dossier parent dont le nom est celui de la racine du dossier géré. Cela se produit également si la tentative de création du dossier géré racine échoue.  <br/> |
|ErrorMeetingSuggestionGenerationFailed  <br/> |Cette erreur indique que le moteur de suggestions a rencontré un problème lors de la tentative de génération de suggestions.  <br/> |
|ErrorMessageDispositionRequired  <br/> | Cette erreur se produit si l’attribut **MessageDisposition** n’est pas défini.<br/><br/> Cet attribut est requis pour les éléments suivants : <br/> <br/>-L' [opération CreateItem](createitem-operation.md) et l' [opération UpdateItem](updateitem-operation.md) lorsque l’élément en cours de création ou de mise à jour est un [message](message-ex15websvcsotherref.md).  <br/>- Objets Response [CancelCalendarItem](cancelcalendaritem.md), [AcceptItem](acceptitem.md), [DeclineItem](declineitem.md)ou [TentativelyAcceptItem](tentativelyacceptitem.md) .  <br/> |
|ErrorMessageSizeExceeded  <br/> |Cette erreur indique que le message que vous tentez d’envoyer dépasse les limites autorisées.  <br/> |
|ErrorMessageTrackingNoSuchDomain  <br/> |Cette erreur indique que le domaine donné est introuvable.  <br/> |
|ErrorMessageTrackingPermanentError  <br/> |Cette erreur indique que le service de suivi des messages ne peut pas effectuer le suivi du message.  <br/> |
| ErrorMessageTrackingTransientError  <br/> |Cette erreur indique que le service de suivi des messages est inactif ou occupé. Ce code d’erreur indique une erreur passagère. Les clients peuvent essayer de se connecter au serveur lors de la réception de cette erreur.  <br/> |
|ErrorMimeContentConversionFailed  <br/> |Cette erreur se produit lorsque le contenu MIME n’est pas un iCal valide pour une [opération CreateItem](createitem-operation.md). Pour une [opération GetItem](getitem-operation.md), cette réponse indique que le contenu MIME n’a pas pu être généré.  <br/> |
|ErrorMimeContentInvalid  <br/> |Cette erreur se produit lorsque le contenu MIME n’est pas valide.  <br/> |
|ErrorMimeContentInvalidBase64String  <br/> |Cette erreur se produit lorsque le contenu MIME dans la demande n’est pas une chaîne de base 64 valide.  <br/> |
|ErrorMissingArgument  <br/> |Cette erreur indique qu’un argument obligatoire est manquant dans la demande. Le texte du message de réponse indique l’argument à vérifier.  <br/> |
|ErrorMissingEmailAddress  <br/> |Cette erreur indique que vous avez spécifié un ID de dossier unique dans la demande, mais que le compte qui a effectué la demande n’a pas de boîte aux lettres sur le système. Dans ce cas, vous devez fournir un sous-élément de [boîte aux lettres](mailbox.md) sous [DistinguishedFolderId](distinguishedfolderid.md).  <br/> |
|ErrorMissingEmailAddressForManagedFolder  <br/> |Cette erreur indique que vous avez spécifié un ID de dossier unique dans la demande, mais que le compte qui a effectué la demande n’a pas de boîte aux lettres sur le système. Dans ce cas, vous devez fournir un sous-élément de [boîte aux lettres](mailbox.md) sous [DistinguishedFolderId](distinguishedfolderid.md). Cette réponse est renvoyée par l' [opération CreateManagedFolder](createmanagedfolder-operation.md).  <br/> |
|ErrorMissingInformationEmailAddress  <br/> |Cette erreur se produit si l’élément [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) est manquant.  <br/> |
|ErrorMissingInformationReferenceItemId  <br/> |Cette erreur se produit si le [ReferenceItemId](referenceitemid.md) est manquant.  <br/> |
|ErrorMissingInformationSharingFolderId  <br/> |Ce code d’erreur n’est jamais renvoyé.  <br/> |
|ErrorMissingItemForCreateItemAttachment  <br/> |Cette erreur est renvoyée lorsqu’une tentative d’inclusion de l’élément item dans l’élément **ItemAttachment** d’une demande d' [opération CreateAttachment](createattachment-operation.md) est effectuée.  <br/> |
|ErrorMissingManagedFolderId  <br/> |Cette erreur se produit lorsque la propriété ID de stratégie, balise de propriété 0x6732, pour le dossier est manquante. Vous devez considérer qu’il s’agit d’un dossier endommagé.  <br/> |
|ErrorMissingRecipients  <br/> |Cette erreur indique que vous avez essayé d’envoyer un élément sans inclure de destinataires. Notez que si vous appelez l' [opération CreateItem](createitem-operation.md) avec une disposition de message qui déclenche l’envoi du message, vous obtiendrez le code de réponse suivant : **ErrorInvalidRecipients**.  <br/> |
|ErrorMissingUserIdInformation  <br/> |Cette erreur indique qu’un [userid](userid.md) n’a pas été complètement spécifié dans un jeu d’autorisations.  <br/> |
|ErrorMoreThanOneAccessModeSpecified  <br/> |Cette erreur indique que vous avez spécifié plusieurs valeurs d’élément [ExchangeImpersonation](exchangeimpersonation.md) dans une demande.  <br/> |
|ErrorMoveCopyFailed  <br/> |Cette erreur indique que l’opération de déplacement ou de copie a échoué. Le mouvement se produit dans l' [opération CreateItem](createitem-operation.md) lorsque vous acceptez une demande de réunion qui se trouve dans le dossier éléments supprimés. En outre, si vous refusez une demande de réunion, annulez un élément de calendrier ou supprimez une réunion de votre calendrier, elle est déplacée vers le dossier éléments supprimés.  <br/> |
|ErrorMoveDistinguishedFolder  <br/> |Cette erreur se produit si vous essayez de déplacer un dossier unique.  <br/> |
|ErrorMultiLegacyMailboxAccess  <br/> |Cette erreur se produit lorsqu’une demande tente d’accéder à plusieurs serveurs de boîtes aux lettres. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorNameResolutionMultipleResults  <br/> |Cette erreur se produit si l' [opération ResolveNames](resolvenames-operation.md) renvoie plusieurs résultats ou si le nom ambigu que vous avez spécifié correspond à plusieurs objets de l’annuaire. Le code de réponse inclut les noms correspondants dans les données de réponse.  <br/> |
|ErrorNameResolutionNoMailbox  <br/> |Cette erreur indique que l’appelant n’a pas de boîte aux lettres sur le système. L' [opération ResolveNames](resolvenames-operation.md) ou l' [opération ExpandDL](expanddl-operation.md) n’est pas valide pour la connexion d’un utilisateur sans boîte aux lettres.  <br/> |
|ErrorNameResolutionNoResults  <br/> |Cette erreur indique que l' [opération ResolveNames](resolvenames-operation.md) ne renvoie aucun résultat.  <br/> |
|ErrorNoApplicableProxyCASServersAvailable  <br/> |Ce code d’erreur doit être renvoyé lorsque le service Web ne peut pas trouver de serveur pour traiter la demande.  <br/> |
|ErrorNoCalendar  <br/> |Cette erreur se produit s’il n’existe aucun dossier de calendrier pour la boîte aux lettres.  <br/> |
|ErrorNoDestinationCASDueToKerberosRequirements  <br/> |Cette erreur indique que la demande faisant référence à une boîte aux lettres dans un autre site Active Directory, mais qu’aucun serveur d’accès au client dans le site de destination n’a été configuré pour l’authentification Windows, et que la demande n’a pas pu être transférée par proxy.  <br/> |
|ErrorNoDestinationCASDueToSSLRequirements  <br/> |Cette erreur indique que la demande faisant référence à une boîte aux lettres dans un autre site Active Directory, mais qu’aucun serveur d’accès au client dans le site de destination n’a été configuré pour les connexions SSL, et par conséquent, la demande n’a pas pu être transférée par proxy.  <br/> |
|ErrorNoDestinationCASDueToVersionMismatch  <br/> |Cette erreur indique que la demande faisant référence à une boîte aux lettres dans un autre site Active Directory, mais qu’aucun serveur d’accès au client dans le site de destination ne dispose d’une version de produit acceptable pour recevoir la demande, et par conséquent, la demande n’a pas pu être transférée par proxy.  <br/> |
|ErrorNoFolderClassOverride  <br/> |Cette erreur se produit si vous définissez l’élément [FolderClass](folderclass.md) lorsque vous créez un élément autre qu’un dossier générique. Pour les dossiers typés, tels que [CalendarFolder](calendarfolder.md) et [TasksFolder](tasksfolder.md), la classe Folder est implicite. La définition de la classe de dossier sur un autre type de dossier à l’aide de l' [opération UpdateFolder](updatefolder-operation.md) génère la réponse **ErrorObjectTypeChanged** . À la place, utilisez un type de dossier générique, mais attribuez à la classe Folder la valeur requise. Les services Web Exchange vont créer le dossier fortement typé correct.  <br/> |
|ErrorNoFreeBusyAccess  <br/> |Cette erreur indique que l’appelant ne dispose pas des droits d’affichage de disponibilité sur le dossier de calendrier en question.  <br/> |
|ErrorNonExistentMailbox  <br/> | Cette erreur se produit dans les scénarios suivants : <br/> <br/>-L’adresse de messagerie est vide dans [CreateManagedFolder](createmanagedfolder.md).  <br/>-L’adresse de messagerie ne fait pas référence à un compte valide dans une demande qui prend une adresse de messagerie dans le corps ou dans l’en-tête SOAP, comme dans un appel d’emprunt d’identité Exchange.  <br/> |
|ErrorNonPrimarySmtpAddress  <br/> |Cette erreur se produit lorsqu’un appelant passe une adresse SMTP non principale. La réponse inclut l’adresse SMTP appropriée à utiliser.  <br/> |
|ErrorNoPropertyTagForCustomProperties  <br/> |Cette erreur indique que les propriétés MAPI dans la plage personnalisée, 0x8000 et supérieur, ne peuvent pas être référencées par des balises de propriété. Vous devez utiliser la propriété [PropertySetId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.extendedpropertydefinition.propertysetid%28v=exchg.80%29.aspx)de l’API managée EWS ou l’élément EWS [ExtendedFieldURI](extendedfielduri.md) avec l’attribut PropertySetId.  <br/> |
|ErrorNoPublicFolderReplicaAvailable  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorNoPublicFolderServerAvailable  <br/> |Ce code d’erreur doit être renvoyé si aucun serveur de dossiers publics n’est disponible ou si l’appelant n’a pas de serveur public public.  <br/> |
|ErrorNoRespondingCASInDestinationSite  <br/> |Cette erreur indique que la demande a fait référence à une boîte aux lettres dans un autre site Active Directory, mais qu’aucun des serveurs d’accès au client de ce site n’a répondu, et par conséquent, la demande n’a pas pu être transférée par proxy.  <br/> |
|ErrorNotAllowedExternalSharingByPolicy  <br/> |Cette erreur indique que l’appelant a essayé d’accorder des autorisations dans son calendrier ou un dossier de contacts à un utilisateur d’une autre organisation et que la tentative a échoué.  <br/> |
|ErrorNotDelegate  <br/> |Cette erreur indique que l’utilisateur n’est pas un délégué pour la boîte aux lettres. Elle est renvoyée par l' [opération GetDelegate](getdelegate-operation.md), l' [opération RemoveDelegate](removedelegate-operation.md)et l' [opération UpdateDelegate](updatedelegate-operation.md) lorsque l’utilisateur délégué spécifié est introuvable dans la liste des délégués.  <br/> |
|ErrorNotEnoughMemory  <br/> |Cette erreur indique que l’opération n’a pas pu aboutir en raison d’une mémoire insuffisante.  <br/> |
|ErrorNotSupportedSharingMessage  <br/> |Cette erreur indique que le message de partage n’est pas pris en charge.  <br/> |
|ErrorObjectTypeChanged  <br/> |Cette erreur se produit si le type d’objet a été modifié.  <br/> |
|ErrorOccurrenceCrossingBoundary  <br/> |Cette erreur se produit lorsque l’heure de [début](start.md) ou de [fin](end-ex15websvcsotherref.md) d’une occurrence est mise à jour de manière à ce que l’événement se produise avant ou après l’occurrence précédente ou suivante correspondante.  <br/> |
|ErrorOccurrenceTimeSpanTooBig  <br/> |Cette erreur indique que le temps alloué pour une occurrence donnée chevauche une autre occurrence du même élément périodique. Cette réponse se produit également lorsque la longueur, en minutes, d’une occurrence donnée est supérieure à Int32. MaxValue.  <br/> |
|ErrorOperationNotAllowedWithPublicFolderRoot  <br/> |Cette erreur indique que l’opération en cours n’est pas valide pour la racine de dossier public.  <br/> |
|ErrorOrganizationNotFederated  <br/> |Cette erreur indique que l’organisation du demandeur n’est pas fédérée afin que le demandeur ne puisse pas créer de messages de partage à envoyer à un utilisateur externe ou qu’il ne puisse pas accepter les messages de partage reçus d’un utilisateur externe.  <br/> |
|ErrorParentFolderIdRequired  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorParentFolderNotFound  <br/> |Cette erreur se produit dans l' [opération CreateFolder](createfolder-operation.md) lorsque le dossier parent est introuvable.  <br/> |
|ErrorPasswordChangeRequired  <br/> |Cette erreur indique que vous devez modifier votre mot de passe pour pouvoir accéder à cette boîte aux lettres. Cela se produit lorsqu’un nouveau compte a été créé et que l’administrateur a indiqué que l’utilisateur doit changer le mot de passe à la première ouverture de session. Vous ne pouvez pas mettre à jour le mot de passe à l’aide des services Web Exchange. Vous devez utiliser un outil tel que Microsoft Office Outlook Web App pour modifier votre mot de passe.  <br/> |
|ErrorPasswordExpired  <br/> |Cette erreur indique que le mot de passe a expiré. Vous ne pouvez pas modifier le mot de passe à l’aide des services Web Exchange. Vous devez utiliser un outil tel qu’Outlook Web App pour modifier votre mot de passe.  <br/> |
|ErrorPermissionNotAllowedByPolicy  <br/> |Cette erreur indique que le demandeur a essayé d’accorder des autorisations dans son dossier calendrier ou contacts à un utilisateur externe, mais la stratégie de partage assignée au demandeur indique que le niveau d’autorisation demandé est supérieur à ce que la stratégie de partage autorise.  <br/> |
|ErrorPhoneNumberNotDialable  <br/> |Cette erreur indique que le numéro de téléphone n’était pas de la bonne forme.  <br/> |
|ErrorPropertyUpdate  <br/> |Cette erreur indique que la mise à jour a échoué en raison de valeurs de propriété non valides. Le message de réponse inclut les chemins d’accès aux propriétés non valides.  <br/> |
|ErrorPromptPublishingOperationFailed  <br/> |Cette erreur est destinée à un usage interne uniquement. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorPropertyValidationFailure  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorProxiedSubscriptionCallFailure  <br/> |Cette erreur indique que la demande fait référence à un abonnement qui existe sur un autre serveur d’accès au client, mais qu’une tentative de proxy de la demande vers ce serveur d’accès au client a échoué.  <br/> |
|ErrorProxyCallFailed  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorProxyGroupSidLimitExceeded  <br/> |Cette erreur indique que la demande faisant référence à une boîte aux lettres dans un autre site Active Directory et que l’appelant initial est membre de plus de 3 000 groupes.  <br/> |
|ErrorProxyRequestNotAllowed  <br/> |Cette erreur indique que la demande que les services Web Exchange envoient à un autre serveur d’accès au client lors de la tentative de réponse à une demande [GetUserAvailabilityRequest](getuseravailabilityrequest.md) n’était pas valide. Ce code de réponse indique généralement qu’une erreur de configuration ou de droits s’est produite, ou qu’une personne a tenté de se reproduire une demande de proxy de disponibilité.  <br/> |
|ErrorProxyRequestProcessingFailed  <br/> |Cette erreur indique que les services Web Exchange ont tenté de transmettre une demande de disponibilité à un autre serveur d’accès au client pour y répondre, mais que la demande a échoué. Cette réponse peut être causée par des problèmes de connectivité réseau ou des problèmes de délai d’expiration de la demande.  <br/> |
|ErrorProxyServiceDiscoveryFailed  <br/> |Ce code d’erreur doit être renvoyé si le service Web ne peut pas déterminer si la demande doit être exécutée sur le serveur cible ou si elle sera transférée par proxy vers un autre serveur.  <br/> |
|ErrorProxyTokenExpired  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorPublicFolderMailboxDiscoveryFailed  <br/> |Cette erreur se produit lorsque l’URL de la boîte aux lettres de dossiers publics est introuvable. Cette erreur est destinée à un usage interne uniquement. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorPublicFolderOperationFailed  <br/> |Cette erreur se produit lorsqu’une tentative d’accès à un dossier public est effectuée et que la tentative échoue. Cette erreur a été introduite dans Exchange 2013Boîte Server 2013.  <br/> |
|ErrorPublicFolderRequestProcessingFailed  <br/> |Cette erreur se produit lorsque le destinataire qui a été transmis à l' [opération GetUserAvailability](getuseravailability-operation.md) se trouve sur un ordinateur qui exécute une version d’Exchange Server antérieure à Exchange 2007, et la demande de récupération des informations de disponibilité pour le destinataire à partir du serveur de dossiers publics a échoué.  <br/> |
|ErrorPublicFolderServerNotFound  <br/> |Cette erreur se produit lorsque le destinataire qui a été transmis à l' [opération GetUserAvailability](getuseravailability-operation.md) se trouve sur un ordinateur qui exécute une version d’Exchange Server antérieure à Exchange 2007, et la demande de récupération des informations de disponibilité pour le destinataire à partir du serveur de dossiers publics a échoué car le serveur de dossiers publics de l’unité d’organisation n’est pas associé.  <br/> |
|ErrorPublicFolderSyncException  <br/> |Cette erreur se produit lorsqu’une opération de synchronisation réussit sur la boîte aux lettres de dossiers publics principale, mais n’aboutit pas sur la boîte aux lettres de dossiers publics secondaire. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorQueryFilterTooLong  <br/> |Cette erreur indique que la restriction du dossier de recherche est peut-être valide, mais elle n’est pas prise en charge par EWS. Les services Web Exchange limitent les restrictions pour contenir un maximum de 255 expressions de filtre. Si vous essayez d’effectuer une liaison avec un dossier de recherche qui dépasse 255, ce code de réponse est renvoyé.  <br/> |
|ErrorQuotaExceeded  <br/> |Cette erreur se produit lorsque le quota de boîte aux lettres est dépassé.  <br/> |
|ErrorReadEventsFailed  <br/> |Cette erreur est renvoyée par l' [opération GetEvents](getevents-operation.md) ou les notifications d’envoi lorsqu’un échec se produit lors de la récupération des informations d’événement. Lorsque cette erreur est renvoyée, l’abonnement est supprimé. Recréez la synchronisation d’événement en fonction d’un dernier filigrane connu.  <br/> |
|ErrorReadReceiptNotPending  <br/> |Cette erreur est renvoyée par l' [opération CreateItem](createitem-operation.md) en cas de tentative de suppression d’une confirmation de lecture lorsque l’expéditeur du message n’a pas demandé de confirmation de lecture sur le message ou si le message se trouve dans le dossier courrier indésirable.  <br/> |
|ErrorRecurrenceEndDateTooBig  <br/> |Cette erreur se produit lorsque la date de fin de la périodicité est postérieure à 9/1/4500.  <br/> |
|ErrorRecurrenceHasNoOccurrence  <br/> |Cette erreur se produit lorsque la périodicité spécifiée ne possède aucune instance d’occurrence dans la plage spécifiée.  <br/> |
|ErrorRemoveDelegatesFailed  <br/> |Cette erreur indique que la liste des délégués n’a pas pu être enregistrée après la suppression des délégués.  <br/> |
|ErrorRequestAborted  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorRequestStreamTooBig  <br/> | Cette erreur se produit lorsque le flux de demande est supérieur à 400 Ko.  <br/> |
|ErrorRequiredPropertyMissing  <br/> |Cette erreur est renvoyée lorsqu’une propriété requise est manquante dans une demande d' [opération CreateAttachment](createattachment-operation.md) . L’URI de propriété manquant est inclus dans la réponse.  <br/> |
|ErrorResolveNamesInvalidFolderType  <br/> |Cette erreur indique que l’appelant a spécifié un dossier qui n’est pas un dossier de contacts pour l' [opération ResolveNames](resolvenames-operation.md).  <br/> |
|ErrorResolveNamesOnlyOneContactsFolderAllowed  <br/> |Cette erreur indique que l’appelant a spécifié plusieurs dossiers de contacts à l' [opération ResolveNames](resolvenames-operation.md).  <br/> |
|ErrorResponseSchemaValidation  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorRestrictionTooLong  <br/> |Cette erreur se produit si la restriction contient plus de 255 nœuds.  <br/> |
|ErrorRestrictionTooComplex  <br/> |Cette erreur se produit lorsque la restriction ne peut pas être évaluée par les services Web Exchange.  <br/> |
|ErrorResultSetTooBig  <br/> |Cette erreur indique que le nombre d’entrées de calendrier pour un destinataire donné dépasse la limite autorisée de 1000. Réduisez la fenêtre et recommencez.  <br/> |
|ErrorSavedItemFolderNotFound  <br/> |Cette erreur se produit lorsque le [SavedItemFolderId](saveditemfolderid.md) est introuvable.  <br/> |
|ErrorSchemaValidation  <br/> | Cette erreur se produit lorsque la demande ne peut pas être validée par rapport au schéma.  <br/> |
|ErrorSearchFolderNotInitialized  <br/> |Cette erreur indique que le dossier de recherche a été créé, mais que les critères de recherche n’ont jamais été définis sur le dossier. Cela se produit uniquement lorsque vous accédez à des dossiers de recherche endommagés qui ont été créés à l’aide d’une autre API ou d’un autre client. Pour corriger cette erreur, utilisez l' [opération UpdateFolder](updatefolder-operation.md) pour définir l’élément [SearchParameters](searchparameters.md) de sorte qu’il inclue la restriction qui doit se trouver sur le dossier.  <br/> |
|ErrorSendAsDenied  <br/> | Cette erreur se produit lorsque les deux conditions suivantes sont remplies : <br/> <br/>-Un utilisateur a reçu des autorisations CanActAsOwner, mais ne dispose pas de droits de délégué sur la boîte aux lettres de l’entité.  <br/>-Le même utilisateur tente de créer et d’envoyer un message électronique dans la boîte aux lettres du principal à l’aide de l’option Méthodesendandsavecopy.<br/>  <br/>  Le résultat est une erreur ErrorSendAsDenied et la création du message électronique dans le dossier Brouillons du principal.  <br/> |
|ErrorSendMeetingCancellationsRequired  <br/> |Cette erreur est renvoyée par l' [opération DeleteItem](deleteitem-operation.md) si l’attribut **SendMeetingCancellations** est absent de la demande et que l’élément à supprimer est un élément de calendrier.  <br/> |
|ErrorSendMeetingInvitationsOrCancellationsRequired  <br/> |Cette erreur est renvoyée par l' [opération UpdateItem](updateitem-operation.md) si l’attribut **SendMeetingInvitationsOrCancellations** est absent de la demande et si l’élément à mettre à jour est un élément de calendrier.  <br/> |
|ErrorSendMeetingInvitationsRequired  <br/> |Cette erreur est renvoyée par l' [opération CreateItem](createitem-operation.md) si l’attribut **SendMeetingInvitations** est absent de la demande et que l’élément à créer est un élément de calendrier.  <br/> |
|ErrorSentMeetingRequestUpdate  <br/> |Cette erreur indique qu’après l’envoi d’une demande de réunion par l’organisateur, la demande ne peut pas être mise à jour. Pour modifier la réunion, modifiez l’élément de calendrier, et non la demande de réunion.  <br/> |
|ErrorSentTaskRequestUpdate  <br/> |Cette erreur indique qu’après l’envoi d’une demande de tâche par l’initiateur de la tâche, cette demande ne peut pas être mise à jour.  <br/> |
|ErrorServerBusy  <br/> |Cette erreur se produit lorsque le serveur est occupé.  <br/> |
|ErrorServiceDiscoveryFailed  <br/> |Cette erreur indique que les services Web Exchange ont tenté de transmettre une demande de disponibilité de l’utilisateur à la forêt appropriée pour le destinataire, mais il n’a pas pu déterminer où envoyer la demande en raison d’un échec de la découverte de service.  <br/> |
|ErrorSharingNoExternalEwsAvailable  <br/> |Cette erreur indique que la propriété de l’URL externe n’a pas été définie dans la base de données Active Directory.  <br/> |
|ErrorSharingSynchronizationFailed  <br/> |Cette erreur indique qu’une tentative de synchronisation d’un dossier de partage a échoué. <br/><br/>Ce code d’erreur est renvoyé dans les cas suivants :<br/><br/>-L’abonnement pour un dossier de partage est introuvable.<br/>-Le dossier de partage est introuvable.<br/>-L’utilisateur d’annuaire correspondant est introuvable.<br/>-L’utilisateur n’existe plus.<br/>-Le rendez-vous n’est pas valide.<br/>-L’élément de contact n’est pas valide.<br/>-Il y a un problème de communication avec le serveur distant.  <br/> |
|ErrorStaleObject  <br/> |Cette erreur se produit dans une opération [UpdateItem](updateitem-operation.md) ou [SendItem](senditem-operation.md) lorsque la clé de modification n’est pas à jour ou qu’elle n’a pas été fournie. Appelez l' [opération GetItem](getitem-operation.md) pour récupérer une clé de modification mise à jour, puis tentez à nouveau l’opération.  <br/> |
|ErrorSubmissionQuotaExceeded  <br/> |Cette erreur indique qu’un utilisateur ne peut pas envoyer immédiatement d’autres demandes, car le quota de soumission a été atteint.  <br/> |
|ErrorSubscriptionAccessDenied  <br/> |Cette erreur se produit lorsque vous essayez d’accéder à un abonnement à l’aide d’un compte qui n’a pas créé cet abonnement. Chaque abonnement n’est accessible que par le créateur de l’abonnement.  <br/> |
|ErrorSubscriptionDelegateAccessNotSupported  <br/> |Cette erreur indique que vous ne pouvez pas créer d’abonnement si vous n’êtes pas le propriétaire ou si vous n’avez pas accès au propriétaire de la boîte aux lettres.  <br/> |
|ErrorSubscriptionNotFound  <br/> |Cette erreur se produit si l’abonnement correspondant à l' [SubscriptionId spécifié (GetEvents)](subscriptionid-getevents.md) est introuvable. L’abonnement a peut-être expiré, le processus des services Web Exchange a peut-être été redémarré ou un abonnement non valide a été transmis. Si l’abonnement était valide, recréez l’abonnement avec le dernier filigrane. Cette opération est renvoyée par l' [opération d’annulation d’abonnement](unsubscribe-operation.md) ou par les réponses de l' [opération GetEvents](getevents-operation.md) .  <br/> |
|ErrorSubscriptionUnsubsribed  <br/> |Ce code d’erreur doit être renvoyé lorsqu’une demande est effectuée pour un abonnement qui a été annulé.  <br/> |
|ErrorSyncFolderNotFound  <br/> |Cette erreur est renvoyée par l' [opération SyncFolderItems](syncfolderitems-operation.md) si le dossier parent spécifié est introuvable.  <br/> |
|ErrorTeamMailboxNotFound  <br/> |Cette erreur indique qu’une boîte aux lettres d’équipe est introuvable. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorTeamMailboxNotLinkedToSharePoint  <br/> |Cette erreur indique qu’une boîte aux lettres d’équipe a été trouvée mais qu’elle n’est pas liée à un serveur SharePoint. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorTeamMailboxUrlValidationFailed  <br/> |Cette erreur indique qu’une boîte aux lettres d’équipe a été trouvée mais que le lien vers le serveur SharePoint n’est pas valide. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorTeamMailboxNotAuthorizedOwner  <br/> |Ce code d’erreur n’est pas utilisé. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorTeamMailboxActiveToPendingDelete  <br/> |Ce code d’erreur n’est pas utilisé. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorTeamMailboxFailedSendingNotifications  <br/> |Cette erreur indique qu’une tentative d’envoi d’une notification aux propriétaires de boîtes aux lettres d’équipe a échoué. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorTeamMailboxErrorUnknown  <br/> |Cette erreur indique une erreur générale qui peut se produire lors d’une tentative d’accès à une boîte aux lettres d’équipe. Essayez d’envoyer la demande ultérieurement. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorTimeIntervalTooBig  <br/> |Cette erreur indique que la fenêtre de temps spécifiée est plus grande que la limite autorisée. Par défaut, la limite autorisée est de 42.  <br/> |
|ErrorTimeoutExpired  <br/> | Cette erreur se produit lorsqu’il n’y a pas suffisamment de temps pour terminer le traitement de la demande.  <br/> |
|ErrorTimeZone  <br/> |Cette erreur indique qu’il y a une erreur de fuseau horaire.  <br/> |
|ErrorToFolderNotFound  <br/> |Cette erreur indique que le dossier de destination n’existe pas.  <br/> |
|ErrorTokenSerializationDenied  <br/> |Cette erreur se produit si l’appelant tente d’effectuer une demande de sérialisation de jetons sans avoir le droit ms-Exch-EPI-TokenSerialization sur le serveur d’accès au client.  <br/> |
|ErrorTooManyObjectsOpened  <br/> |Cette erreur se produit lorsque la limite interne sur les objets ouverts a été dépassée.  <br/> |
|ErrorUnifiedMessagingDialPlanNotFound  <br/> |Cette erreur indique que le plan de numérotation d’un utilisateur n’est pas disponible.  <br/> |
|ErrorUnifiedMessagingReportDataNotFound  <br/> |Cette erreur est destinée à un usage interne uniquement. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorUnifiedMessagingPromptNotFound  <br/> |Cette erreur est destinée à un usage interne uniquement. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorUnifiedMessagingRequestFailed  <br/> |Cette erreur indique que l’utilisateur est introuvable.  <br/> |
|ErrorUnifiedMessagingServerNotFound  <br/> |Cette erreur indique qu’un serveur valide pour le plan de numérotation peut être trouvé pour gérer la demande.  <br/> |
|ErrorUnableToGetUserOofSettings  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorUnableToRemoveImContactFromGroup  <br/> |Cette erreur se produit lorsqu’une tentative infructueuse est effectuée pour supprimer un contact de messagerie instantanée d’un groupe. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorUnsupportedCulture  <br/> |Cette erreur se produit lorsque vous essayez de définir la propriété **culture** sur une valeur qui n’est pas analysable par la classe **System. Globalization. CultureInfo** .  <br/> |
|ErrorUnsupportedMapiPropertyType  <br/> |Cette erreur se produit lorsqu’un appelant tente d’utiliser des propriétés étendues de type Object, Array, Object, Error ou null.  <br/> |
|ErrorUnsupportedMimeConversion  <br/> |Cette erreur se produit lorsque vous tentez de récupérer ou de définir du contenu MIME pour un élément autre qu’un objet [PostItem](postitem.md), [message](message-ex15websvcsotherref.md)ou [CalendarItem](calendaritem.md) .  <br/> |
|ErrorUnsupportedPathForQuery  <br/> |Cette erreur se produit lorsque l’appelant transmet une propriété non valide pour une requête. Cela peut se produire lorsque des propriétés calculées sont utilisées.  <br/> |
|ErrorUnsupportedPathForSortGroup  <br/> |Cette erreur se produit lorsque l’appelant transmet une propriété non valide pour une propriété sort ou Group by. Cela peut se produire lorsque des propriétés calculées sont utilisées.  <br/> |
|ErrorUnsupportedPropertyDefinition  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorUnsupportedQueryFilter  <br/> |Cette erreur indique que la restriction du dossier de recherche est peut-être valide, mais elle n’est pas prise en charge par EWS.  <br/> |
|ErrorUnsupportedRecurrence  <br/> |Cette erreur indique que la périodicité spécifiée n’est pas prise en charge pour les tâches.  <br/> |
|ErrorUnsupportedSubFilter  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorUnsupportedTypeForConversion  <br/> |Cette erreur indique que les services Web Exchange ont trouvé un type de propriété dans la Banque, mais il ne peut pas générer de code XML pour le type de propriété.  <br/> |
|ErrorUpdateDelegatesFailed  <br/> |Cette erreur indique que la liste des délégués n’a pas pu être enregistrée après la mise à jour des délégués.  <br/> |
|ErrorUpdatePropertyMismatch  <br/> |Cette erreur se produit lorsque le chemin d’accès à une propriété unique qui est affiché dans une description de modification ne correspond pas à la propriété unique définie dans [l’objet réel ou](item.md) [dossier](folder.md) .  <br/> |
|ErrorUserNotUnifiedMessagingEnabled  <br/> |Cette erreur indique que le demandeur n’est pas activé.  <br/> |
|ErrorUserNotAllowedByPolicy  <br/> |Cette erreur indique que le demandeur a essayé d’accorder des autorisations dans son dossier calendrier ou contacts à un utilisateur externe, mais la stratégie de partage assignée au demandeur indique que le domaine de l’utilisateur externe n’est pas repris dans la stratégie.  <br/> |
|ErrorUserWithoutFederatedProxyAddress  <br/> |Indique que l’organisation du demandeur dispose d’un ensemble de domaines fédérés, mais que l’organisation du demandeur n’a pas d’adresses proxy SMTP avec l’un des domaines fédérés.  <br/> |
|ErrorValueOutOfRange  <br/> |Cette erreur indique qu’une date de début ou une date de fin de mode calendrier a été définie sur 1/1/0001 12:00:00 AM ou 12/31/9999 11:59:59 PM.  <br/> |
|ErrorVirusDetected  <br/> |Cette erreur indique que la banque Exchange a détecté un virus dans le message.  <br/> |
|ErrorVirusMessageDeleted  <br/> |Cette erreur indique que la banque Exchange a détecté un virus dans le message et l’a supprimée.  <br/> |
|ErrorVoiceMailNotImplemented  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorWebRequestInInvalidState  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorWin32InteropError  <br/> |Cette erreur indique qu’une erreur interne s’est produite lors de la communication avec du code non managé.  <br/> |
|ErrorWorkingHoursSaveFailed  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorWorkingHoursXmlMalformed  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorWrongServerVersion  <br/> |Cette erreur indique qu’une requête peut être effectuée uniquement sur un serveur de la même version que le serveur de boîtes aux lettres.  <br/> |
|ErrorWrongServerVersionDelegate  <br/> |Cette erreur indique qu’une demande a été effectuée par un délégué dont la version de serveur est différente de celle du serveur de boîtes aux lettres du principal.  <br/> |
|ErrorMissingInformationSharingFolderId  <br/> |Ce code d’erreur n’est jamais renvoyé.  <br/> |
|ErrorDuplicateSOAPHeader  <br/> |Indique qu’il existe des en-têtes SOAP en double.  <br/> |
|ErrorSharingSynchronizationFailed  <br/> | Indique qu’une tentative de synchronisation d’un dossier de partage a échoué.<br/><br/> Ce code d’erreur doit être renvoyé lorsque :<br/><br/>-L’abonnement pour un dossier de partage est introuvable.  <br/>-Le dossier de partage est introuvable.  <br/>-L’utilisateur d’annuaire correspondant est introuvable.  <br/>-L’utilisateur n’existe plus.  <br/>-Le rendez-vous n’est pas valide.  <br/>-L’élément de contact n’est pas valide.  <br/>-Un échec de communication s’est passé avec le serveur distant.  <br/> |
|ErrorSharingNoExternalEwsAvailable  <br/> |Indique que la propriété de l’URL externe n’a pas été définie dans la base de données Active Directory. Ce code d’erreur doit être renvoyé si la propriété de l’URL externe n’a pas été définie dans la base de données Active Directory.  <br/> |
|ErrorFreeBusyDLLimitReached  <br/> |Indique que le nombre maximal de membres du groupe a été atteint pour obtenir des informations de disponibilité pour une liste de distribution. Cette erreur doit être renvoyée lorsque le nombre maximal de membres du groupe a été atteint pour obtenir des informations de disponibilité pour une liste de distribution.  <br/> |
|ErrorInvalidGetSharingFolderRequest  <br/> |Spécifie que le type de données et l’élément ShareFolderId sont tous deux présents dans une demande. Ce code d’erreur doit être renvoyé si le type de données et l’élément ShareFolderId sont tous deux présents dans une demande.  <br/> |
|ErrorNotAllowedExternalSharingByPolicy  <br/> |Spécifie que l’appelant a tenté d’accorder des autorisations dans son calendrier ou un dossier de contacts à un utilisateur d’une autre organisation et que la tentative a échoué. Ce code d’erreur doit être renvoyé lorsque la stratégie de partage est désactivée pour l’appelant ou lorsque la stratégie de partage attribuée à l’appelant interdit le partage pour le niveau demandé ou le type de dossier demandé.  <br/> |
|ErrorUserNotAllowedByPolicy  <br/> |Spécifie que le demandeur a tenté d’accorder des autorisations dans son dossier calendrier ou contacts à un utilisateur externe, mais que la stratégie de partage assignée au demandeur spécifie que le domaine de l’utilisateur externe n’est pas repris dans la stratégie.  <br/> |
|ErrorPermissionNotAllowedByPolicy  <br/> |Spécifie que le demandeur a tenté d’accorder des autorisations dans son calendrier ou un dossier de contacts à un utilisateur externe, mais la stratégie de partage assignée au demandeur spécifie que le niveau d’autorisation demandé est supérieur à celui autorisé par la stratégie de partage.  <br/> |
|ErrorOrganizationNotFederated  <br/> |Spécifie que l’organisation du demandeur n’est pas fédérée afin que le demandeur ne puisse pas créer de messages de partage à envoyer à un utilisateur externe, ni accepter les messages de partage reçus d’un utilisateur externe. Ce code d’erreur doit être renvoyé si l’organisation du demandeur n’est pas fédérée.  <br/> |
|ErrorMailboxFailover  <br/> |Indique qu’une tentative d’accès à une boîte aux lettres a échoué car la boîte aux lettres est dans un processus de basculement.  <br/> |
|ErrorInvalidExternalSharingInitiator  <br/> |Spécifie que l’expéditeur de l’invitation de partage n’a pas créé les métadonnées de l’invitation de partage. Ce code d’erreur doit être renvoyé si l’expéditeur de l’invitation de partage n’a pas créé les métadonnées de l’invitation de partage.  <br/> |
|ErrorMessageTrackingPermanentError  <br/> |Spécifie que le service de suivi des messages ne peut pas suivre le message.  <br/> |
|ErrorMessageTrackingTransientError  <br/> |Spécifie que le service de suivi des messages est inactif ou occupé. Ce code d’erreur spécifie une erreur passagère. Les clients peuvent essayer de se connecter au serveur lors de la réception de cette erreur.  <br/> |
|ErrorMessageTrackingNoSuchDomain  <br/> |Spécifie que le domaine donné est introuvable.  <br/> |
|ErrorUserWithoutFederatedProxyAddress  <br/> |Spécifie que l’organisation du demandeur a un ensemble de domaines fédérés, mais que l’organisation du demandeur n’a pas d’adresses proxy SMTP avec l’un des domaines fédérés.  <br/> |
|ErrorInvalidOrganizationRelationshipForFreeBusy  <br/> |Spécifie qu’un appelant a demandé des informations de disponibilité pour un utilisateur d’une autre organisation, mais que la relation organisationnelle n’est pas disponible/occupée.  <br/> |
|ErrorInvalidFederatedOrganizationId  <br/> |Spécifie que les objets de Fédération de l’organisation du demandeur ne sont pas configurés correctement.  <br/> |
|ErrorInvalidExternalSharingSubscriber  <br/> |Spécifie qu’un message de partage n’est pas destiné à l’appelant.  <br/> |
|ErrorInvalidSharingData  <br/> |Spécifie que les métadonnées de partage ne sont pas valides. Cela peut être dû à un code XML non valide.  <br/> |
|ErrorInvalidSharingMessage  <br/> |Spécifie que le message de partage n’est pas valide. Cela peut être dû à une propriété manquante.  <br/> |
|ErrorNotSupportedSharingMessage  <br/> |Spécifie que le message de partage n’est pas pris en charge.  <br/> |
|ErrorApplyConversationActionFailed  <br/> |Cette erreur doit être renvoyée si une action ne peut pas être appliquée à un ou plusieurs éléments de la conversation.  <br/> |
|ErrorInboxRulesValidationError  <br/> |Cette erreur doit être renvoyée si une règle ne peut pas être validée.  <br/> |
|ErrorOutlookRuleBlobExists  <br/> |Cette erreur doit être renvoyée lorsqu’une tentative de gestion des règles de boîte de réception a lieu après qu’un autre client a accédé aux règles de boîte de réception.  <br/> |
|ErrorRulesOverQuota  <br/> |Cette erreur doit être renvoyée lorsque le quota d’un utilisateur a été dépassé.  <br/> |
|ErrorNewEventStreamConnectionOpened  <br/> |Cette erreur doit être renvoyée à la première connexion d’abonnement si une seconde connexion d’abonnement est ouverte.  <br/> |
|ErrorMissedNotificationEvents  <br/> |Cette erreur doit être renvoyée lorsque des notifications d’événement sont manquées.  <br/> |
|ErrorDuplicateLegacyDistinguishedName  <br/> |Cette erreur est renvoyée lorsqu’il existe des noms uniques hérités en double dans les services de domaine Active Directory (AD DS). Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorInvalidClientAccessTokenRequest  <br/> |Cette erreur indique qu’une demande d’obtention d’un jeton d’accès au client n’était pas valide. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorNoSpeechDetected  <br/> |Cette erreur est destinée à un usage interne uniquement. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorUMServerUnavailable  <br/> |Cette erreur est destinée à un usage interne uniquement. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorRecipientNotFound  <br/> |Cette erreur est destinée à un usage interne uniquement. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorRecognizerNotInstalled  <br/> |Cette erreur est destinée à un usage interne uniquement. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorSpeechGrammarError  <br/> |Cette erreur est destinée à un usage interne uniquement. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorInvalidManagementRoleHeader  <br/> |Cette erreur est renvoyée si l’en-tête [ManagementRole](managementrole.md) de l’en-tête SOAP est incorrect. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorLocationServicesDisabled  <br/> |Cette erreur est destinée à un usage interne uniquement. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorLocationServicesRequestTimedOut  <br/> |Cette erreur est destinée à un usage interne uniquement. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorLocationServicesRequestFailed  <br/> |Cette erreur est destinée à un usage interne uniquement. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorLocationServicesInvalidRequest  <br/> |Cette erreur est destinée à un usage interne uniquement. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorWeatherServiceDisabled  <br/> |Cette erreur est destinée à un usage interne uniquement.  <br/> |
|ErrorMailboxScopeNotAllowedWithoutQueryString  <br/> |Cette erreur est renvoyée lorsqu’une tentative de recherche dans l’étendue est effectuée sans utiliser d’élément [QueryString (String)](querystring-string.md) pour une recherche d’indexation de contenu. Cela s’applique aux opérations **SearchMailboxes** et **FindConversation** . Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorArchiveMailboxSearchFailed  <br/> |Cette erreur est renvoyée lorsqu’une recherche de boîte aux lettres d’archivage échoue. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorArchiveMailboxServiceDiscoveryFailed  <br/> |Cette erreur est renvoyée lorsque l’URL d’une boîte aux lettres d’archivage n’est pas découvrable. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorGetRemoteArchiveFolderFailed  <br/> |Cette erreur se produit lorsque l’opération d’obtention du dossier de boîte aux lettres d’archivage distant a échoué.  <br/> |
|ErrorFindRemoteArchiveFolderFailed  <br/> |Cette erreur se produit lorsque l’opération de recherche du dossier de boîte aux lettres d’archivage distant a échoué.  <br/> |
|ErrorGetRemoteArchiveItemFailed  <br/> |Cette erreur se produit lorsque l’opération d’obtention de l’élément de boîte aux lettres d’archivage distant a échoué.  <br/> |
|ErrorExportRemoteArchiveItemsFailed  <br/> |Cette erreur se produit lorsque l’opération d’exportation des éléments de boîte aux lettres d’archivage distant a échoué.  <br/> |
|ErrorInvalidPhotoSize  <br/> |Cette erreur est renvoyée si une taille de photo non valide est demandée à partir du serveur. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorSearchQueryHasTooManyKeywords  <br/> |Cette erreur est renvoyée lorsqu’une taille de photo inattendue est demandée dans une demande d’opération **GetUserPhoto** . Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorSearchTooManyMailboxes  <br/> |Cette erreur est renvoyée lorsqu’une demande d’opération **SearchMailboxes** contient trop de boîtes aux lettres à rechercher. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorInvalidRetentionTagNone  <br/> |Cette erreur indique qu’aucune balise de rétention n’a été trouvée pour cet utilisateur. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorDiscoverySearchesDisabled  <br/> |Cette erreur est renvoyée lorsque les recherches de découverte sont désactivées sur un client ou un serveur. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorCalendarSeekToConditionNotSupported  <br/> |Cette erreur se produit lorsque vous tentez d’appeler l' [opération FindItem](finditem-operation.md) avec un [SeekToConditionPageItemView](seektoconditionpageitemview.md) pour extraire des éléments de calendrier, ce qui n’est pas pris en charge.  <br/> |
|ErrorCalendarIsGroupMailboxForAccept  <br/> |Cette erreur est destinée à un usage interne uniquement.  <br/> |
|ErrorCalendarIsGroupMailboxForDecline  <br/> |Cette erreur est destinée à un usage interne uniquement.  <br/> |
|ErrorCalendarIsGroupMailboxForTentative  <br/> |Cette erreur est destinée à un usage interne uniquement.  <br/> |
|ErrorCalendarIsGroupMailboxForSuppressReadReceipt  <br/> |Cette erreur est destinée à un usage interne uniquement.  <br/> |
|ErrorOrganizationAccessBlocked  <br/> |Le client est marqué pour suppression.  <br/> |
|ErrorInvalidLicense  <br/> |L’utilisateur ne dispose pas d’une licence valide.  <br/> |
|ErrorMessagePerFolderCountReceiveQuotaExceeded  <br/> |Le quota de réception du message par dossier a été dépassé.  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément n’est pas obligatoire et n’est pas inclus dans toutes les réponses. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

