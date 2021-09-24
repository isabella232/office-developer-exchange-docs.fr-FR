---
title: ResponseCode
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ResponseCode
api_type:
- schema
ms.assetid: 4b84d670-74c9-4d6d-84e7-f0a9f76f0d93
description: L’élément ResponseCode fournit des informations d’état sur la demande.
ms.openlocfilehash: 9d662ee93870c2aabe045d801222deb881d0a28b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59512386"
---
# <a name="responsecode"></a>ResponseCode

**L’élément ResponseCode** fournit des informations d’état sur la demande. 
  
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
|[ResponseMessage](responsemessage.md) <br/> | Fournit des informations descriptives sur l’état de la réponse.<br/><br/>  Voici les expressions XPath possibles pour cet élément :<br/><br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/ResponseMessage` <br/><br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/ResponseMessage` <br/><br/>  `/SetUserOofSettingsResponse/ResponseMessage` <br/><br/>  `/GetUserOofSettingsResponse/ResponseMessage` <br/> |
|[DeleteItemResponseMessage](deleteitemresponsemessage.md) <br/> |Contient l’état et le résultat d’une demande [d’opération DeleteItem](deleteitem-operation.md) unique.  <br/> |
|[SendItemResponseMessage](senditemresponsemessage.md) <br/> |Contient l’état et le résultat d’une demande [d’opération SendItem](senditem-operation.md) unique.  <br/> |
|[DeleteFolderResponseMessage](deletefolderresponsemessage.md) <br/> |Contient l’état et le résultat d’une demande [d’opération DeleteFolder](deletefolder-operation.md) unique.  <br/> |
|[DeleteAttachmentResponseMessage](deleteattachmentresponsemessage.md) <br/> |Contient l’état et le résultat d’une demande [d’opération DeleteAttachment](deleteattachment-operation.md) unique.  <br/> |
|[UnsubscribeResponseMessage](unsubscriberesponsemessage.md) <br/> |Contient l’état et le résultat d’une demande [d’opération de désabonnement](unsubscribe-operation.md) unique.  <br/> |
|[CreateFolderResponseMessage](createfolderresponsemessage.md) <br/> |Contient l’état et le résultat d’une [demande d’opération CreateFolder](createfolder-operation.md) unique.  <br/> |
|[GetFolderResponseMessage](getfolderresponsemessage.md) <br/> |Contient l’état et le résultat d’une demande [d’opération GetFolder](getfolder-operation.md) unique.  <br/> |
|[UpdateFolderResponseMessage](updatefolderresponsemessage.md) <br/> |Contient l’état et le résultat d’une demande [d’opération UpdateFolder](updatefolder-operation.md) unique.  <br/> |
|[MoveFolderResponseMessage](movefolderresponsemessage.md) <br/> |Contient l’état et le résultat d’une [demande d’opération MoveFolder](movefolder-operation.md) unique.  <br/> |
|[CopyFolderResponseMessage](copyfolderresponsemessage.md) <br/> |Contient l’état et le résultat d’une demande [d’opération CopyFolder](copyfolder-operation.md)unique.  <br/> |
|[CreateManagedFolderResponseMessage](createmanagedfolderresponsemessage.md) <br/> |Contient l’état et le résultat d’une [demande d’opération CreateManagedFolder](createmanagedfolder-operation.md) unique.  <br/> |
|[FindFolderResponseMessage](findfolderresponsemessage.md) <br/> |Contient l’état et le résultat d’une demande [d’opération FindFolder](findfolder-operation.md) unique.  <br/> |
|[CreateItemResponseMessage](createitemresponsemessage.md) <br/> |Contient l’état et le résultat d’une [demande d’opération CreateItem](createitem-operation.md) unique.  <br/> |
|[GetItemResponseMessage](getitemresponsemessage.md) <br/> |Contient l’état et le résultat d’une demande [d’opération GetItem](getitem-operation.md) unique.  <br/> |
|[UpdateItemResponseMessage](updateitemresponsemessage.md) <br/> |Contient l’état et le résultat d’une demande [d’opération UpdateItem](updateitem-operation.md) unique.  <br/> |
|[MoveItemResponseMessage](moveitemresponsemessage.md) <br/> |Contient l’état et le résultat d’une [demande d’opération MoveItem](moveitem-operation.md) unique.  <br/> |
|[CopyItemResponseMessage](copyitemresponsemessage.md) <br/> |Contient l’état et le résultat d’une demande [d’opération CopyItem](copyitem-operation.md) unique.  <br/> |
|[CreateAttachmentResponseMessage](createattachmentresponsemessage.md) <br/> |Contient l’état et le résultat d’une demande [d’opération CreateAttachment](createattachment-operation.md) unique.  <br/> |
|[GetAttachmentResponseMessage](getattachmentresponsemessage.md) <br/> |Contient l’état et le résultat d’une [demande d’opération GetAttachment](getattachment-operation.md) unique.  <br/> |
|[FindItemResponseMessage](finditemresponsemessage.md) <br/> |Contient l’état et le résultat d’une demande [d’opération FindItem](finditem-operation.md) unique.  <br/> |
|[ResolveNamesResponseMessage](resolvenamesresponsemessage.md) <br/> |Contient l’état et le résultat [d’une demande d’opération ResolveNames.](resolvenames-operation.md)  <br/> |
|[ExpandDLResponseMessage](expanddlresponsemessage.md) <br/> |Contient l’état et le résultat d’une demande [d’opération ExpandDL](expanddl-operation.md) unique.  <br/> |
|[SubscribeResponseMessage](subscriberesponsemessage.md) <br/> |Contient l’état et le résultat d’une demande [d’opération d’abonnement](subscribe-operation.md) unique.  <br/> |
|[GetEventsResponseMessage](geteventsresponsemessage.md) <br/> |Contient l’état et le résultat d’une demande [d’opération GetEvents](getevents-operation.md) unique.  <br/> |
|[SendNotificationResponseMessage](sendnotificationresponsemessage.md) <br/> |Contient l’état et le résultat d’une demande d’opération SendNotification unique.  <br/> |
|[SyncFolderHierarchyResponseMessage](syncfolderhierarchyresponsemessage.md) <br/> |Contient l’état et le résultat [d’une demande d’opération SyncFolderHierarchy.](syncfolderhierarchy-operation.md)  <br/> |
|[SyncFolderItemsResponseMessage](syncfolderitemsresponsemessage.md) <br/> |Contient l’état et le résultat [d’une demande d’opération SyncFolderItems.](syncfolderitems-operation.md)  <br/> |
|[ConvertIdResponseMessage](convertidresponsemessage.md) <br/> |Contient l’état et le résultat d’une [demande d’opération ConvertId.](convertid-operation.md)  <br/> |
|[AddDelegateResponse](adddelegateresponse.md) <br/> |Contient l’état et le résultat d’une [demande d’opération AddDelegate.](adddelegate-operation.md)  <br/> |
|[GetDelegateResponse](getdelegateresponse.md) <br/> |Contient l’état et le résultat d’une [demande d’opération GetDelegate.](getdelegate-operation.md)  <br/> |
|[RemoveDelegateResponse](removedelegateresponse.md) <br/> |Contient l’état et le résultat [d’une demande d’opération RemoveDelegate.](removedelegate-operation.md)  <br/> |
|[UpdateDelegateResponse](updatedelegateresponse.md) <br/> |Contient l’état et le résultat d’une [demande d’opération UpdateDelegate.](updatedelegate-operation.md)  <br/> |
|[GetServerTimeZonesResponseMessage](getservertimezonesresponsemessage.md) <br/> |Contient l’état et le résultat [d’une demande d’opération GetServerTimeZones.](getservertimezones-operation.md)  <br/> |
|[GetSharingFolderResponseMessage](getsharingfolderresponsemessage.md) <br/> |Contient l’état et le résultat [d’une demande d’opération GetSharingFolder.](getsharingfolder-operation.md)  <br/> |
|[GetSharingFolderResponse](getsharingfolderresponse.md) <br/> |Définit une réponse à une [demande d’opération GetSharingFolder.](getsharingfolder-operation.md)  <br/> |
|[GetSharingMetadataResponseMessage](getsharingmetadataresponsemessage.md) <br/> |Contient l’état et le résultat [d’une demande d’opération GetSharingMetadata.](getsharingmetadata-operation.md)  <br/> |
|[GetSharingMetadataResponse](getsharingmetadataresponse.md) <br/> |Définit une réponse à une demande de [Opération de GetSharingMetadata](getsharingmetadata-operation.md) .  <br/> |
|[RefreshSharingFolderResponseMessage](refreshsharingfolderresponsemessage.md) <br/> |Contient l’état et le résultat [d’une demande d’opération RefreshSharingFolder.](refreshsharingfolder-operation.md)  <br/> |
|[RefreshSharingFolderResponse](refreshsharingfolderresponse.md) <br/> |Définit une réponse à une [demande d’opération RefreshSharingFolder.](refreshsharingfolder-operation.md)  <br/> |
|[FindConversationResponse](findconversationresponse.md) <br/> |Contient l’état et les résultats [d’une réponse d’opération FindConversation.](findconversation-operation.md)  <br/> |
|[ApplyConversationActionResponseMessage](applyconversationactionresponsemessage.md) <br/> |Contient l’état et les résultats [d’une demande d’opération ApplyConversationAction.](applyconversationaction-operation.md)  <br/> |
|[EmptyFolderResponseMessage](emptyfolderresponsemessage.md) <br/> |Contient l’état et le résultat d’une demande [d’opération EmptyFolder](emptyfolder-operation.md) unique.  <br/> |
|[UpdateInboxRulesResponse](updateinboxrulesresponse.md) <br/> |Contient un état et le résultat d’une [demande d’opération UpdateInboxRules.](updateinboxrules-operation.md)  <br/> |
|[UploadItemsResponseMessage](uploaditemsresponsemessage.md) <br/> |Contient un état et le résultat d’une [demande d’opération UploadItems.](uploaditems-operation.md)  <br/> |
|[GetInboxRulesResponse](getinboxrulesresponse.md) <br/> |Contient une réponse à une [demande d’opération GetInboxRules](getinboxrules-operation.md) ****.  <br/> |
|[GetServiceConfigurationResponse](getserviceconfigurationresponse.md) <br/> |Contient une réponse à une [demande d’opération GetServiceConfiguration.](getserviceconfiguration-operation.md)  <br/> |
|[ServiceConfigurationResponseMessageType](serviceconfigurationresponsemessagetype.md) <br/> |Contient les paramètres de configuration du service.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte est requise si cet élément est utilisé. Le tableau suivant décrit les valeurs renvoyées avec cet élément.
  
|Valeur|Description|
|:-----|:-----|
|NoError  <br/> |Aucune erreur ne s’est produite pour la demande.  <br/> |
|ErrorAccessDenied  <br/> |Cette erreur se produit lorsque le compte appelant ne peut pas effectuer l’action demandée.  <br/> |
|ErrorAccessModeSpecified  <br/> |Cette erreur est uniquement à usage interne. Cette erreur n’est pas renvoyée.  <br/> |
|ErrorAccountDisabled  <br/> |Cette erreur se produit lorsque le compte en question a été désactivé.  <br/> |
|ErrorAddDelegatesFailed  <br/> |Cette erreur se produit lorsqu’une liste avec des délégués ajoutés ne peut pas être enregistrée.  <br/> |
|ErrorAddressSpaceNotFound  <br/> |Cette erreur se produit lorsque l’enregistrement d’espace d’adressaie ou le nom de domaine DNS (Domain Name System) pour la disponibilité entre forêts est in trouvé dans la base de données Active Directory.  <br/> |
|ErrorADOperation  <br/> |Cette erreur se produit lorsque l’opération a échoué en raison de problèmes de communication avec les services de domaine Active Directory (AD DS).  <br/> |
|ErrorADSessionFilter  <br/> |Cette erreur est renvoyée lorsqu’une **demande d’opération ResolveNames** spécifie un nom non valide.  <br/> |
|ErrorADUnavailable  <br/> |Cette erreur se produit lorsqu’AD DS n’est pas disponible. Essayez à nouveau votre demande ultérieurement.  <br/> |
|ErrorAffectedTaskOccurrencesRequired  <br/> |Cette erreur indique que **l’attribut AffectedTaskOccurrences** n’a pas été spécifié. Lorsque l’élément [DeleteItem](deleteitem.md) est utilisé pour supprimer au moins un élément qui est une tâche et que cette tâche soit périodique ou non, l’attribut **AffectedTaskOccurrences** doit être spécifié afin que **DeleteItem** puisse déterminer s’il faut supprimer l’occurrence actuelle ou la série entière.  <br/> |
|ErrorArchiveFolderPathCreation  <br/> |Indique une erreur lors de la création du chemin d’accès du dossier d’archivage.  <br/> |
|ErrorArchiveMailboxNotEnabled  <br/> |Indique que la boîte aux lettres d’archivage n’a pas été activée.  <br/> |
|ErrorArchiveMailboxServiceDiscoveryFailed  <br/> |Indique que la découverte du service de boîte aux lettres d’archivage a échoué.  <br/> |
|ErrorAttachmentNestLevelLimitExceeded  <br/> |Spécifie qu’une tentative de création d’un élément avec plus de 10 pièces jointes imbrmbrées a été tentée. Cette valeur a été introduite dans Exchange Server 2010 Service Pack 2 (SP2).  <br/> |
|ErrorAttachmentSizeLimitExceeded  <br/> |[L’élément CreateAttachment](createattachment.md) renvoie cette erreur si une tentative de création d’une pièce jointe dont la taille dépasse int32.MaxValue, en octets.  <br/> [L’élément GetAttachment](getattachment.md) renvoie cette erreur si une tentative de récupération d’une pièce jointe existante dont la taille dépasse int32.MaxValue, en octets.  <br/> |
|ErrorAutoDiscoverFailed  <br/> |Cette erreur indique que les services web Exchange ont tenté de déterminer l’emplacement d’un ordinateur entre forêts exécutant Exchange 2010 sur qui le rôle serveur d’accès au client est installé à l’aide du service de découverte automatique, mais que l’appel au service de découverte automatique a échoué.  <br/> |
|ErrorAvailabilityConfigNotFound  <br/> |Cette erreur indique que les informations de configuration de disponibilité pour la forêt locale sont manquantes dans AD DS.  <br/> |
|ErrorBatchProcessingStopped  <br/> | Cette erreur indique qu’une exception s’est produite lors du traitement d’un élément et que cette exception est susceptible de se produire pour les éléments qui suivent. Les demandes peuvent inclure plusieurs éléments ; Par exemple, une demande d’opération GetItem peut inclure plusieurs identificateurs. En règle générale, les éléments sont traitées un par un. Si une exception se produit lors du traitement d’un élément et que cette exception est susceptible de se produire pour les éléments qui suivent, les éléments qui suivent ne sont pas traitées.  <br/><br/>  Voici quelques exemples d’erreurs qui arrêteront le traitement des éléments qui suivent :<br/>  <br/>- ErrorAccessDenied  <br/>- ErrorAccountDisabled  <br/>- ErrorADUnavailable  <br/>- ErrorADOperation  <br/>- ErrorConnectionFailed  <br/>- ErrorMailboxStoreUnavailable  <br/>- ErrorMailboxMoveInProgress  <br/>- ErrorPasswordChangeRequired  <br/>- ErrorPasswordExpired  <br/>- ErrorQuotaExceeded  <br/>- ErrorInsufficientResources  <br/> |
|ErrorCalendarCannotMoveOrCopyOccurrence  <br/> |Cette erreur se produit lorsqu’une tentative de déplacement ou de copie d’une occurrence d’un élément de calendrier périodique est tentée.  <br/> |
|ErrorCalendarCannotUpdateDeletedItem  <br/> | Cette erreur se produit lorsqu’une tentative de mise à jour d’un élément de calendrier se trouve dans le dossier Éléments supprimés et lorsque des mises à jour ou des annulations de réunion doivent être envoyées en fonction de la valeur de l’attribut **SendMeetingInvitationsOrCancellations.** <br/><br/>Les valeurs possibles pour cet attribut sont les suivantes :  <br/><br/>- SendToAllAndSaveCopy  <br/>- SendToChangedAndSaveCopy  <br/>- SendOnlyToAll  <br/>- SendOnlyToChanged  <br/>  <br/>Toutefois, une telle mise à jour est autorisée uniquement lorsque la valeur de cet attribut est définie sur SendToNone.  <br/> |
|ErrorCalendarCannotUseIdForOccurrenceId  <br/> |Cette erreur se produit lorsque l’opération UpdateItem, GetItem, DeleteItem, MoveItem, CopyItem ou SendItem est appelée et que l’ID spécifié n’est pas un ID d’occurrence d’un élément de calendrier périodique.  <br/> |
|ErrorCalendarCannotUseIdForRecurringMasterId  <br/> |Cette erreur se produit lorsque l’opération **UpdateItem**, **GetItem**, **DeleteItem**, **MoveItem**, **CopyItem** ou **SendItem** est appelée et que l’ID spécifié n’est pas un ID d’élément maître périodique.  <br/> |
|ErrorCalendarDurationIsTooLong  <br/> |Cette erreur se produit lors d’une opération **CreateItem** ou **UpdateItem** lorsqu’une durée d’élément de calendrier est plus longue que la durée maximale autorisée, qui est actuellement de 5 ans.  <br/> |
|ErrorCalendarEndDateIsEarlierThanStartDate  <br/> |Cette erreur se produit lorsqu’une heure de fin du calendrier est définie sur la même heure ou après l’heure de début.  <br/> |
|ErrorCalendarFolderIsInvalidForCalendarView  <br/> |Cette erreur se produit lorsque le dossier spécifié pour une **opération FindItem** avec un [élément CalendarView](calendarview.md) n’est pas de type dossier calendrier.  <br/> |
|ErrorCalendarInvalidAttributeValue  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorCalendarInvalidDayForTimeChangePattern  <br/> |Cette erreur se produit lors d’une opération **CreateItem** ou **UpdateItem** lorsque des valeurs non valides de Day, WeekendDay et Weekday sont utilisées pour définir le modèle de changement d’heure.  <br/> |
|ErrorCalendarInvalidDayForWeeklyRecurrence  <br/> |Cette erreur se produit lors d’une opération **CreateItem** ou **UpdateItem** lorsque des valeurs non valides de Day, WeekDay et WeekendDay sont utilisées pour spécifier la récurrence hebdomadaire.  <br/> |
|ErrorCalendarInvalidPropertyState  <br/> |Cette erreur se produit lorsque l’état d’un objet BLOB (Binary Large Object) de récurrence d’élément de calendrier dans le magasin Exchange n’est pas valide.  <br/> |
|ErrorCalendarInvalidPropertyValue  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorCalendarInvalidRecurrence  <br/> |Cette erreur se produit lorsque la récurrence spécifiée ne peut pas être créée.  <br/> |
|ErrorCalendarInvalidTimeZone  <br/> |Cette erreur se produit lorsqu’un fuseau horaire non valide est rencontré.  <br/> |
|ErrorCalendarIsCancelledForAccept  <br/> |Cette erreur indique qu’un élément de calendrier a été annulé.  <br/> |
|ErrorCalendarIsCancelledForDecline  <br/> |Cette erreur indique qu’un élément de calendrier a été annulé.  <br/> |
|ErrorCalendarIsCancelledForRemove  <br/> |Cette erreur indique qu’un élément de calendrier a été annulé.  <br/> |
|ErrorCalendarIsCancelledForTentative  <br/> |Cette erreur indique qu’un élément de calendrier a été annulé.  <br/> |
|ErrorCalendarIsDelegatedForAccept  <br/> |Cette erreur indique que [l’élément AcceptItem](acceptitem.md) n’est pas valide pour un élément de calendrier ou une demande de réunion dans un scénario délégué.  <br/> |
|ErrorCalendarIsDelegatedForDecline  <br/> |Cette erreur indique que l’élément [DeclineItem](declineitem.md) n’est pas valide pour un élément de calendrier ou une demande de réunion dans un scénario délégué.  <br/> |
|ErrorCalendarIsDelegatedForRemove  <br/> |Cette erreur indique que [l’élément RemoveItem](removeitem.md) n’est pas valide pour une annulation de réunion dans un scénario délégué.  <br/> |
|ErrorCalendarIsDelegatedForTentative  <br/> |Cette erreur indique que [l’élément TentativelyAcceptItem](tentativelyacceptitem.md) n’est pas valide pour un élément de calendrier ou une demande de réunion dans un scénario délégué.  <br/> |
|ErrorCalendarIsNotOrganizer  <br/> |Cette erreur indique que l’opération (actuellement CancelItem) sur l’élément de calendrier n’est pas valide pour un participant. Seul l’organisateur de la réunion peut annuler la réunion.  <br/> |
|ErrorCalendarIsOrganizerForAccept  <br/> |Cette erreur indique que [AcceptItem](acceptitem.md) n’est pas valide pour l’élément de calendrier de l’organisateur.  <br/> |
|ErrorCalendarIsOrganizerForDecline  <br/> |Cette erreur indique que [DeclineItem](declineitem.md) n’est pas valide pour l’élément de calendrier de l’organisateur.  <br/> |
|ErrorCalendarIsOrganizerForRemove  <br/> |Cette erreur indique que [RemoveItem n’est](removeitem.md) pas valide pour l’élément de calendrier de l’organisateur. Pour supprimer une réunion du calendrier, l’organisateur doit utiliser CancelCalendarItem.  <br/> |
|ErrorCalendarIsOrganizerForTentative  <br/> |Cette erreur indique que [TentativelyAcceptItem n’est](tentativelyacceptitem.md) pas valide pour l’élément de calendrier de l’organisateur.  <br/> |
|ErrorCalendarMeetingRequestIsOutOfDate  <br/> |Cette erreur indique qu’une demande de réunion n’est pas à jour et qu’elle ne peut pas être mise à jour.  <br/> |
|ErrorCalendarOccurrenceIndexIsOutOfRecurrenceRange  <br/> |Cette erreur indique que l’index d’occurrence ne pointe pas vers une occurrence dans la récurrence actuelle. Par exemple, si votre modèle de récurrence définit un ensemble de trois occurrences de réunion et que vous essayez d’accéder à la cinquième occurrence, ce code de réponse se produit.  <br/> |
|ErrorCalendarOccurrenceIsDeletedFromRecurrence  <br/> |Cette erreur indique que toute opération sur une occurrence supprimée (adressée via l’ID maître périodique et l’index d’occurrence) n’est pas valide.  <br/> |
|ErrorCalendarOutOfRange  <br/> |Cette erreur est signalée dans les opérations CreateItem et UpdateItem pour les éléments de calendrier ou les propriétés de récurrence des tâches lorsque la valeur de la propriété est en dehors de la plage. Par exemple, la spécification de la quinzième semaine du mois entraîne ce code de réponse.  <br/> |
|ErrorCalendarViewRangeTooBig  <br/> |Cette erreur se produit lorsque la plage de début à fin de l’élément [CalendarView](calendarview.md) est plus que la valeur maximale autorisée, actuellement de 2 ans.  <br/> |
|ErrorCallerIsInvalidADAccount  <br/> |Cette erreur indique que le compte demandeur n’est pas un compte valide dans la base de données d’annuaire.  <br/> |
|ErrorCannotArchiveCalendarContactTaskFolderException  <br/> |Indique qu’une tentative d’archivage d’un dossier de tâches de contact de calendrier a été réalisée.  <br/> |
|ErrorCannotArchiveItemsInPublicFolders  <br/> |Indique qu’une tentative d’archivage des éléments des dossiers publics a été réalisée.  <br/> |
|ErrorCannotArchiveItemsInArchiveMailbox  <br/> |Indique que la tentative d’archivage des éléments de la boîte aux lettres d’archivage a eu lieu.  <br/> |
|ErrorCannotCreateCalendarItemInNonCalendarFolder  <br/> |Cette erreur se produit lorsqu’un élément de calendrier est créé et que l’attribut **SavedItemFolderId** fait référence à un dossier autre que calendrier.  <br/> |
|ErrorCannotCreateContactInNonContactFolder  <br/> |Cette erreur se produit lorsqu’un contact est créé et que l’attribut **SavedItemFolderId** fait référence à un dossier sans contact.  <br/> |
|ErrorCannotCreatePostItemInNonMailFolder  <br/> |Cette erreur indique qu’un élément de publication ne peut pas être créé dans un dossier autre qu’un dossier de messagerie, tel que Calendrier, Contact, Tâches, Notes, etc.  <br/> |
|ErrorCannotCreateTaskInNonTaskFolder  <br/> |Cette erreur se produit lorsqu’une tâche est créée et que l’attribut **SavedItemFolderId** fait référence à un dossier autre qu’une tâche.  <br/> |
|ErrorCannotDeleteObject  <br/> |Cette erreur se produit lorsque l’élément ou le dossier à supprimer ne peut pas être supprimé.  <br/> |
|ErrorCannotDeleteTaskOccurrence  <br/> |[L’opération DeleteItem renvoie](deleteitem-operation.md) cette erreur lorsqu’elle ne parvient pas à supprimer l’occurrence actuelle d’une tâche périodique. Cela ne peut se produire que si l’attribut **AffectedTaskOccurrences** a la valeur SpecifiedOccurrenceOnly.  <br/> |
|ErrorCannotDisableMandatoryExtension  <br/> |Indique qu’une tentative de désactivation d’une extension obligatoire a été réalisée.  <br/> |
|ErrorCannotEmptyFolder  <br/> |Cette erreur doit être renvoyée lorsque le serveur ne peut pas vider un dossier.  <br/> |
|ErrorCannotGetSourceFolderPath  <br/> |Indique que le chemin d’accès du dossier source n’a pas pu être récupéré.  <br/> |
|ErrorCannotGetExternalEcpUrl  <br/> |Spécifie que le serveur n’a pas pu récupérer l’URL externe Outlook Options Web App.  <br/> |
|ErrorCannotOpenFileAttachment  <br/> |**L’opération GetAttachment** renvoie cette erreur si elle ne peut pas récupérer le corps d’une pièce jointe.  <br/> |
|ErrorCannotSetCalendarPermissionOnNonCalendarFolder  <br/> |Cette erreur indique que l’appelant a tenté de définir des autorisations de calendrier sur un dossier autre que calendrier.  <br/> |
|ErrorCannotSetNonCalendarPermissionOnCalendarFolder  <br/> |Cette erreur indique que l’appelant a tenté de définir des autorisations non-calendrier sur un dossier de calendrier.  <br/> |
|ErrorCannotSetPermissionUnknownEntries  <br/> |Cette erreur indique que vous ne pouvez pas définir d’autorisations inconnues dans un jeu d’autorisations.  <br/> |
|ErrorCannotSpecifySearchFolderAsSourceFolder  <br/> |Indique qu’une tentative a été réalisée pour spécifier le dossier de recherche comme dossier source.  <br/> |
|ErrorCannotUseFolderIdForItemId  <br/> |Cette erreur se produit lorsqu’un identificateur de dossier est attribué à une demande nécessitant un identificateur d’élément.  <br/> |
|ErrorCannotUseItemIdForFolderId  <br/> |Cette erreur se produit lorsqu’un identificateur d’élément est attribué à une demande nécessitant un identificateur de dossier.  <br/> |
|ErrorChangeKeyRequired  <br/> |Ce code de réponse a été remplacé par **ErrorChangeKeyRequiredForWriteOperations** <br/> |
|ErrorChangeKeyRequiredForWriteOperations  <br/> |Cette erreur est renvoyée lorsque la touche de modification d’un élément est manquante ou obsolète. <br/><br/>Pour les opérations SendItem, UpdateItem et UpdateFolder, l’appelant doit transmettre une touche de modification correcte et actuelle pour l’élément. Notez que c’est le cas avec UpdateItem même lorsque la résolution des conflits est définie sur toujours overwrite.  <br/> |
|ErrorClientDisconnected  <br/> |Spécifie que le client a été déconnecté.  <br/> |
|ErrorClientIntentInvalidStateDefinition  <br/> |Cette erreur est destinée à un usage interne uniquement.  <br/> |
|ErrorClientIntentNotFound  <br/> |Cette erreur est destinée à un usage interne uniquement.  <br/> |
|ErrorConnectionFailed  <br/> |Cette erreur se produit lorsque les Exchange Web Ne peuvent pas se connecter à la boîte aux lettres.  <br/> |
|ErrorContainsFilterWrongType  <br/> |Cette erreur indique que la propriété qui a été inspectée pour un filtre Contient n’est pas un type de chaîne.  <br/> |
|ErrorContentConversionFailed  <br/> |**L’opération GetItem** renvoie cette erreur lorsque Exchange Web Services n’est pas en mesure de récupérer le contenu MIME de l’élément demandé. <br/><br/>**L’opération CreateItem** renvoie cette erreur lorsque Exchange Web Services n’est pas en mesure de créer l’élément à partir du contenu MIME fourni. Il s’agit généralement d’une indication que la propriété d’élément est endommagée ou tronquée.  <br/> |
|ErrorContentIndexingNotEnabled  <br/> |Cette erreur se produit lorsqu’une demande de recherche est faite à l’aide de l’option QueryString et que l’indexation de contenu n’est pas activée pour la boîte aux lettres cible.  <br/> |
|ErrorCorruptData  <br/> |Cette erreur se produit lorsque les données sont endommagées et ne peuvent pas être traitées.  <br/> |
|ErrorCreateItemAccessDenied  <br/> |Cette erreur se produit lorsque l’appelant n’est pas autorisé à créer l’élément.  <br/> |
|ErrorCreateManagedFolderPartialCompletion  <br/> |Cette erreur se produit lorsqu’un ou plusieurs des dossiers gérés spécifiés dans la demande d’opération CreateManagedFolder n’ont pas pu être créés. Recherchez chaque dossier pour déterminer quels dossiers ont été créés et quels dossiers n’existent pas.  <br/> |
|ErrorCreateSubfolderAccessDenied  <br/> |Cette erreur se produit lorsque le compte appelant n’a pas les autorisations requises pour créer le sous-folder.  <br/> |
|ErrorCrossMailboxMoveCopy  <br/> |Cette erreur se produit lorsqu’une tentative de déplacement d’un élément ou d’un dossier d’une boîte aux lettres à une autre est tentée. Si la boîte aux lettres source et la boîte aux lettres de destination sont différentes, vous obtenez cette erreur.  <br/> |
|ErrorCrossSiteRequest  <br/> |Cette erreur indique que la demande n’est pas autorisée, car le serveur d’accès au client qui doit la prendre en compte se trouve sur un autre site.  <br/> |
|ErrorDataSizeLimitExceeded  <br/> |Cette erreur peut se produire dans les scénarios suivants :<br/>  <br/>- Une tentative d’accès ou d’écriture d’une propriété sur un élément est tentée et la valeur de la propriété est trop grande.<br/>- La longueur du contenu MIME codé en base 64 dans le code XML de la demande dépasse la limite.<br/>- La taille du corps d’un corps d’élément existant dépasse la limite.<br/>- Le consommateur tente de définir un corps de texte ou HTML dont la longueur (ou la longueur combinée dans le cas de l’annexe) dépasse la limite. |
|ErrorDataSourceOperation  <br/> |Cette erreur se produit lorsque le fournisseur de données sous-jacent ne parvient pas à terminer l’opération.  <br/> |
|ErrorDelegateAlreadyExists  <br/> |Cette erreur se produit dans une **opération AddDelegate** lorsque l’utilisateur spécifié existe déjà dans la liste des délégués.  <br/> |
|ErrorDelegateCannotAddOwner  <br/> |Cette erreur se produit lors d’une **opération AddDelegate** lorsque l’utilisateur spécifié à ajouter est le propriétaire de la boîte aux lettres.  <br/> |
|ErrorDelegateMissingConfiguration  <br/> |Cette erreur se produit dans une opération **GetDelegate** lorsqu’il n’existe aucune information de délégué sur le message FreeBusy local ou aucun délégué public Active Directory (pas de délégué public ou d’entrée « Envoyer de la part de » dans AD DS).  <br/> |
|ErrorDelegateNoUser  <br/> |Cette erreur se produit lorsqu’un utilisateur spécifié ne peut pas être mappé à un utilisateur dans AD DS.  <br/> |
|ErrorDelegateValidationFailed  <br/> |Cette erreur se produit dans **l’opération AddDelegate** lorsqu’un utilisateur délégué ajouté n’est pas valide.  <br/> |
|ErrorDeleteDistinguishedFolder  <br/> |Cette erreur se produit lorsqu’une tentative de suppression d’un dossier est réalisée.  <br/> |
|ErrorDeleteItemsFailed  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorDeleteUnifiedMessagingPromptFailed  <br/> |Cette erreur est destinée à un usage interne uniquement.  <br/> |
|ErrorDistinguishedUserNotSupported  <br/> |Cette erreur indique qu’un ID d’utilisateur n’est pas valide pour l’opération. **DistinguishedUserType** ne doit pas être présent dans la demande.  <br/> |
|ErrorDistributionListMemberNotExist  <br/> |Cette erreur indique qu’un membre de liste de distribution de demande n’existe pas dans la liste de distribution.  <br/> |
|ErrorDuplicateInputFolderNames  <br/> |Cette erreur se produit lorsque des noms de dossiers en double sont spécifiés dans l’élément [FolderNames](foldernames.md) de la demande d’opération **CreateManagedFolder.**  <br/> |
|ErrorDuplicateSOAPHeader  <br/> |Cette erreur indique qu’il existe des en-têtes SOAP en double.  <br/> |
|ErrorDuplicateUserIdsSpecified  <br/> |Cette erreur indique qu’un ID utilisateur en double a été trouvé dans un jeu d’autorisations, par défaut ou anonyme sont définies plusieurs fois, ou qu’il existe des SID ou des destinataires en double.  <br/> |
|ErrorEmailAddressMismatch  <br/> |Cette erreur se produit lorsqu’une demande tente de créer/mettre à jour les paramètres de recherche d’un dossier de recherche. Par exemple, cela peut se produire lorsqu’un dossier de recherche est créé dans la boîte aux lettres, mais que le dossier de recherche est dirigé vers une autre boîte aux lettres.  <br/> |
|ErrorEventNotFound  <br/> |Cette erreur se produit lorsque l’événement associé à un filigrane est supprimé avant que l’événement soit renvoyé. Lorsque cette erreur est renvoyée, l’abonnement est également supprimé.  <br/> |
|ErrorExceededConnectionCount  <br/> |Cette erreur -iIndicates qu’il y a plus de demandes simultanées sur le serveur que ce qui est autorisé par la stratégie d’un utilisateur.  <br/> |
|ErrorExceededSubscriptionCount  <br/> |Cette erreur indique que le nombre maximal d’abonnements de la stratégie de limitation d’un utilisateur a été dépassé.  <br/> |
|ErrorExceededFindCountLimit  <br/> |Cette erreur indique qu’un appel d’opération de recherche a dépassé le nombre total d’éléments qui peuvent être renvoyés.  <br/> |
|ErrorExpiredSubscription  <br/> |Cette erreur se produit si [l’opération GetEvents](getevents-operation.md) est appelée en tant qu’abonnement en cours de suppression car elle a expiré.  <br/> |
|ErrorExtensionNotFound  <br/> |Indique que l’extension n’a pas été trouvée.  <br/> |
|ErrorFolderCorrupt  <br/> |Cette erreur se produit lorsque le dossier est endommagé et ne peut pas être enregistré.  <br/> |
|ErrorFolderExists  <br/> |Cette erreur se produit lorsqu’une tentative de création d’un dossier qui a le même nom qu’un autre dossier du même parent est tentée. Les noms de dossiers en double ne sont pas autorisés.  <br/> |
|ErrorFolderNotFound  <br/> |Cette erreur indique que l’ID de dossier spécifié ne correspond pas à un dossier valide ou que le délégué n’est pas autorisé à accéder au dossier.  <br/> |
|ErrorFolderPropertRequestFailed  <br/> |Cette erreur indique que la propriété demandée n’a pas pu être récupérée. Cela n’indique pas que la propriété n’existe pas, mais que la propriété a été endommagée d’une certaine façon afin que la récupération échoue.  <br/> |
|ErrorFolderSave  <br/> |Cette erreur indique que le dossier n’a pas pu être créé ou mis à jour en raison d’un état non valide.  <br/> |
|ErrorFolderSaveFailed  <br/> |Cette erreur indique que le dossier n’a pas pu être créé ou mis à jour en raison d’un état non valide.  <br/> |
|ErrorFolderSavePropertyError  <br/> |Cette erreur indique que le dossier n’a pas pu être créé ou mis à jour en raison de valeurs de propriété non valides. Le code de réponse répertorie les propriétés à l’origine du problème.  <br/> |
|ErrorFreeBusyDLLimitReached  <br/> |Cette erreur indique que le nombre maximal de membres du groupe a été atteint pour obtenir des informations de libre/occupé pour une liste de distribution.  <br/> |
|ErrorFreeBusyGenerationFailed  <br/> |Cette erreur est renvoyée lorsque les informations de libre/occupé ne peuvent pas être récupérées en raison d’une défaillance intermédiaire.  <br/> |
|ErrorGetServerSecurityDescriptorFailed  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorImContactLimitReached  <br/> |Cette erreur est renvoyée lorsque de nouveaux contacts de messagerie instantanée ne peuvent pas être ajoutés car le nombre maximal de contacts a été atteint. Cette erreur a été introduite dans Exchange Server 2013.  <br/> |
|ErrorImGroupDisplayNameAlreadyExists  <br/> |Cette erreur est renvoyée lorsqu’une tentative d’ajout d’un nom complet de groupe est réalisée lorsqu’un groupe existant a déjà le même nom complet. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorImGroupLimitReached  <br/> |Cette erreur est renvoyée lorsque de nouveaux groupes de messagerie instantanée ne peuvent pas être ajoutés car le nombre maximal de groupes a été atteint. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorImpersonateUserDenied  <br/> |L’erreur est renvoyée dans le cas d’autorisation de serveur à serveur pour l’emprunt d’identité Exchange lorsque l’appelant ne Exchange pas les droits appropriés pour usurper l’identité de l’utilisateur en question. Cette erreur est ms-Exch-MAPS-May-Impersonate extended Active Directory right.  <br/> |
|ErrorImpersonationDenied  <br/> |Cette erreur est renvoyée dans l’autorisation de serveur à serveur pour l’emprunt d’identité Exchange lorsque l’appelant ne Exchange pas les droits appropriés pour usurper l’identité via le serveur d’accès au client sur qui il fait la demande. Cette carte est ms-Exch-CAS-Impersonation étendue Active Directory droite.  <br/> |
|ErrorImpersonationFailed  <br/> |Cette erreur indique qu’une erreur inattendue s’est produite lors d’une tentative d’authentification de serveur à serveur. Ce code de réponse indique généralement que le compte de service qui exécute le pool d’applications des services web Exchange est configuré de manière incorrecte, que les services Web Exchange ne peuvent pas parler à l’annuaire ou qu’une relation d’confiance entre les forêts n’est pas correctement configurée.  <br/> |
|ErrorIncorrectSchemaVersion  <br/> |Cette erreur indique que la demande était valide pour la version Exchange Server actuelle, mais qu’elle n’était pas valide pour la version du serveur de demande spécifiée.  <br/> |
|ErrorIncorrectUpdatePropertyCount  <br/> |Cette erreur indique que chaque description de modification dans les éléments [UpdateItem](updateitem.md) ou [UpdateFolder](updatefolder.md) ne doit lister qu’une seule propriété à mettre à jour.  <br/> |
|ErrorIndividualMailboxLimitReached  <br/> |Cette erreur se produit lorsque la demande contient trop de participants à résoudre. Par défaut, le nombre maximal de participants à résoudre est de 100.  <br/> |
|ErrorInsufficientResources  <br/> |Cette erreur se produit lorsque le serveur de boîtes aux lettres est surchargé. Essayez à nouveau votre demande ultérieurement.  <br/> |
|ErrorInternalServerError  <br/> |Cette erreur indique que Exchange Web Services a rencontré une erreur dont il n’a pas pu récupérer et qu’un code de réponse plus spécifique associé à l’erreur qui s’est produite n’existe pas.  <br/> |
|ErrorInternalServerTransientError  <br/> |Cette erreur indique qu’une erreur de serveur interne s’est produite et que vous devriez essayer à nouveau votre demande ultérieurement.  <br/> |
|ErrorInvalidAccessLevel  <br/> |Cette erreur indique que le niveau d’accès de l’appelant sur les données de libre/occupé n’est pas valide.  <br/> |
|ErrorInvalidArgument  <br/> |Cette erreur indique une erreur causée par tous les arguments non valides transmis à [l’opération GetMessageTrackingReport](getmessagetrackingreport-operation.md).<br/><br/> Cette erreur est renvoyée dans les scénarios suivants : <br/><br/>- L’utilisateur spécifié dans le paramètre  _sending-as_ n’existe pas dans l’annuaire. <br/>- L’utilisateur spécifié dans le paramètre  _sending-as_ n’est pas unique dans l’annuaire. <br/>-  _L’adresse d’envoi en tant_ que est vide.<br/>-  _L’adresse d’envoi en tant_ qu’adresse de messagerie n’est pas valide.  <br/> |
|ErrorInvalidAttachmentId  <br/> |Cette erreur est renvoyée par l’opération [GetAttachment](getattachment-operation.md) ou [DeleteAttachment](deleteattachment-operation.md) lorsqu’une pièce jointe correspondant à l’ID spécifié est in trouvée.  <br/> |
|ErrorInvalidAttachmentSubfilter  <br/> |Cette erreur se produit lorsque vous essayez de lier un dossier de recherche existant à l’aide d’une restriction de table de pièces jointes complexe. Exchange Les services web ne prend en charge que les filtres simples dans la table des pièces jointes. Si vous essayez de lier un dossier de recherche existant qui présente une restriction de table de pièces jointes plus complexe (un sous-filtre), les services web Exchange ne peuvent pas restituer le code XML pour ce filtre et renvoient ce code de réponse. <br/><br/>Notez que vous pouvez toujours appeler l’opération GetFolder sur le dossier, mais ne demandez pas [l’élément SearchParameters.](searchparameters.md)  <br/> |
|ErrorInvalidAttachmentSubfilterTextFilter  <br/> |Cette erreur se produit lorsque vous essayez de lier un dossier de recherche existant à l’aide d’une restriction de table de pièces jointes complexe. Exchange Les services web ne prend en charge que les filtres simples dans la table des pièces jointes. <br/><br/>Si vous essayez de lier un dossier de recherche existant qui présente une restriction de table de pièces jointes plus complexe, Exchange Web Services ne peut pas restituer le XML pour ce filtre. Dans ce cas, le sous-filtre de pièce jointe contient un filtre de texte, mais il ne recherche pas le nom complet de la pièce jointe.<br/><br/> Notez que vous pouvez toujours appeler l’opération GetFolder sur le dossier, mais ne demandez pas [l’élément SearchParameters.](searchparameters.md)  <br/> |
|ErrorInvalidAuthorizationContext  <br/> | Cette erreur indique que la procédure d’autorisation du demandeur a échoué.  <br/> |
|ErrorInvalidChangeKey  <br/> |Cette erreur se produit lorsqu’un consommateur passe un identificateur de dossier ou d’élément avec une clé de modification qui ne peut pas être l’objet d’une recherche. Par exemple, il peut s’agit d’un contenu base64 non valide ou d’une chaîne vide.  <br/> |
|ErrorInvalidClientSecurityContext  <br/> |Cette erreur indique qu’une erreur interne s’est produite lors de la tentative de résolution de l’identité de l’appelant.  <br/> |
|ErrorInvalidCompleteDate  <br/> |Cette erreur est renvoyée lorsqu’une tentative est réalisée pour définir la valeur de l’élément [CompleteDate](completedate.md) d’une tâche sur une heure ultérieure. Lorsqu’elle est convertie en heure locale du serveur d’accès au client, la valeur [CompleteDate](completedate.md) d’une tâche ne peut pas être définie sur une valeur ultérieure à l’heure locale sur le serveur d’accès au client.  <br/> |
|ErrorInvalidContactEmailAddress  <br/> |Cette erreur indique qu’une adresse de messagerie non valide a été fournie pour un contact.  <br/> |
|ErrorInvalidContactEmailIndex  <br/> |Cette erreur indique qu’une valeur d’index de messagerie non valide a été fournie pour une entrée de courrier électronique.  <br/> |
|ErrorInvalidCrossForestCredentials  <br/> |Cette erreur se produit lorsque les informations d’identification utilisées pour proxyer une demande vers une autre forêt de service d’annuaire échouent à l’authentification.  <br/> |
|ErrorInvalidDelegatePermission  <br/> |Cette erreur indique que les autorisations de dossier spécifiées ne sont pas valides.  <br/> |
|ErrorInvalidDelegateUserId  <br/> |Cette erreur indique que l’ID d’utilisateur délégué spécifié n’est pas valide.  <br/> |
|ErrorInvalidExchangeImpersonationHeaderData  <br/> |Cette erreur se produit lors Exchange emprunt d’identité lorsqu’un appelant ne spécifie pas de NOM D’UTILISATEUR, d’adresse de messagerie ou de SID d’utilisateur. Cela se produit également si l’appelant spécifie une ou plusieurs de ces valeurs et que les valeurs sont vides.  <br/> |
|ErrorInvalidExcludesRestriction  <br/> |Cette erreur se produit lorsque le masque de bits qui a été passé dans une restriction d’élément [Excludes](excludes.md) ne peut pas être interrogé.  <br/> |
|ErrorInvalidExpressionTypeForSubFilter  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorInvalidExtendedProperty  <br/> | Cette erreur se produit lorsque les événements suivants se produisent : <br/> <br/>- L’appelant tente d’utiliser une propriété étendue qui n’est pas prise en charge par Exchange Web Services.  <br/>- L’appelant transmet une combinaison non valide de valeurs d’attribut pour une propriété étendue. Cela se produit également si aucun attribut n’est transmis. Seules certaines combinaisons sont autorisées.  <br/> |
|ErrorInvalidExtendedPropertyValue  <br/> |Cette erreur se produit lorsque la section valeur d’une propriété étendue ne correspond pas au type de la propriété. <br/><br/>Par exemple, la définition d’une propriété étendue avec PropertyType="String » sur un tableau d’nombres integers entraîne cette erreur. Toute représentation de chaîne qui n’est pas forable dans le type spécifié pour la propriété étendue donnera cette erreur.  <br/> |
|ErrorInvalidExternalSharingInitiator  <br/> |Cette erreur indique que l’expéditeur de l’invitation de partage n’a pas créé les métadonnées d’invitation de partage.  <br/> |
|ErrorInvalidExternalSharingSubscriber  <br/> |Cette erreur indique qu’un message de partage n’est pas destiné à l’appelant.  <br/> |
|ErrorInvalidFederatedOrganizationId  <br/> |Cette erreur indique que les objets de fédération de l’organisation du demandeur ne sont pas correctement configurés.  <br/> |
|ErrorInvalidFolderId  <br/> |Cette erreur se produit lorsque l’ID du dossier est endommagé.  <br/> |
|ErrorInvalidFolderTypeForOperation  <br/> |Cette erreur indique que le type de dossier spécifié n’est pas valide pour l’opération en cours. Par exemple, vous ne pouvez pas créer un dossier de recherche dans un dossier public.  <br/> |
|ErrorInvalidFractionalPagingParameters  <br/> | Cette erreur se produit lors de la pagination fractionnaire lorsque l’utilisateur a spécifié l’une des erreurs suivantes : <br/> <br/>- Numérateur supérieur au dénominateur  <br/>- Numérateur inférieur à zéro  <br/>- Dénominateur inférieur ou égal à zéro  <br/> |
|ErrorInvalidGetSharingFolderRequest  <br/> |Cette erreur indique que les éléments [DataType](datatype.md) et ShareFolderId sont tous deux présents dans une demande.  <br/> |
|ErrorInvalidFreeBusyViewType  <br/> |Cette erreur se produit lorsque [l’opération GetUserAvailability](getuseravailability-operation.md) est appelée avec [un FreeBusyViewType](freebusyviewtype.md) de None.  <br/> |
|ErrorInvalidId  <br/> |Cette erreur indique que l’ID et/ou la touche de modification sont malformés.  <br/> |
|ErrorInvalidIdEmpty  <br/> |Cette erreur se produit lorsque l’appelant spécifie un **attribut ID** vide.  <br/> |
|ErrorInvalidLikeRequest  <br/> |Cette erreur se produit lorsque l’élément ne peut pas être aimé. Les versions Exchange à partir du numéro de build 15.00.0913.09 incluent cette valeur.  <br/> |
|ErrorInvalidIdMalformed  <br/> |Cette erreur se produit lorsque l’appelant spécifie un **attribut ID** qui est malformé.  <br/> |
|ErrorInvalidIdMalformedEwsLegacyIdFormat  <br/> |Cette erreur indique qu’un ID de dossier ou d’élément qui utilise le format Exchange 2007 a été spécifié pour une demande avec une version de Exchange 2007 SP1 ou version ultérieure. Vous ne pouvez pas utiliser Exchange ID 2007 dans Exchange 2007 SP1 ou des requêtes ultérieures. Vous devez d’abord utiliser [l’opération ConvertId](convertid-operation.md) pour les convertir.  <br/> |
|ErrorInvalidIdMonikerTooLong  <br/> |Cette erreur se produit lorsque l’appelant spécifie un **attribut ID** trop long.  <br/> |
|ErrorInvalidIdNotAnItemAttachmentId  <br/> |Cette erreur est renvoyée chaque fois qu’un ID qui n’est pas un ID de pièce jointe d’élément est transmis à une méthode de service Web qui attend un ID de pièce jointe.  <br/> |
|ErrorInvalidIdReturnedByResolveNames  <br/> |Cette erreur se produit lorsqu’un contact de votre boîte aux lettres est endommagé.  <br/> |
|ErrorInvalidIdStoreObjectIdTooLong  <br/> |Cette erreur se produit lorsque l’appelant spécifie un **attribut ID** trop long.  <br/> |
|ErrorInvalidIdTooManyAttachmentLevels  <br/> |Cette erreur est renvoyée lorsque la hiérarchie des pièces jointes d’un élément dépasse la profondeur maximale de 255 niveaux.  <br/> |
|ErrorInvalidIdXml  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorInvalidImContactId  <br/> |Cette erreur est renvoyée lorsque l’identificateur de contact de messagerie instantanée spécifié ne représente pas un identificateur valide. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorInvalidImDistributionGroupSmtpAddress  <br/> |Cette erreur est renvoyée lorsque l’identificateur d’adresse SMTP du groupe de distribution de messagerie instantanée spécifié ne représente pas un identificateur valide. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorInvalidImGroupId  <br/> |Cette erreur est renvoyée lorsque l’identificateur de groupe de messagerie instantanée spécifié ne représente pas un identificateur valide. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorInvalidIndexedPagingParameters  <br/> |Cette erreur se produit si le décalage de la pagination indexée est négatif.  <br/> |
|ErrorInvalidInternetHeaderChildNodes  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorInvalidItemForOperationArchiveItem  <br/> |Indique que l’élément n’était pas valide pour **une opération ArchiveItem.**  <br/> |
|ErrorInvalidItemForOperationAcceptItem  <br/> |Cette erreur se produit lorsqu’une tentative d’utilisation d’un objet de réponse AcceptItem est réalisée pour un type d’élément autre qu’une demande de réunion ou un élément de calendrier, ou lorsqu’une tentative d’acceptation d’une occurrence d’élément de calendrier se trouve dans le dossier Éléments supprimés.  <br/> |
|ErrorInvalidItemForOperationCancelItem  <br/> |Cette erreur se produit lorsqu’une tentative d’utilisation d’un objet de réponse CancelItem est réalisée sur un type d’élément autre qu’un élément de calendrier.  <br/> |
|ErrorInvalidItemForOperationCreateItemAttachment  <br/> | Cette erreur est renvoyée lorsqu’une tentative de création d’une pièce jointe d’élément d’un type non pris en place est tentée.  <br/><br/>  Les types d’éléments pris en charge pour les pièces jointes d’élément incluent les objets suivants :  <br/><br/>- [Élément](item.md) <br/>- [Message](message-ex15websvcsotherref.md) <br/>- [CalendarItem](calendaritem.md) <br/>- [Tâche](task.md) <br/>- [Contact](contact.md) <br/> <br/> Par exemple, si vous essayez de créer une pièce [jointe MeetingMessage,](meetingmessage.md) vous rencontrerez ce code de réponse.  <br/> |
|ErrorInvalidItemForOperationCreateItem  <br/> | Cette erreur est renvoyée par une [opération CreateItem](createitem-operation.md) si la demande contient un type d’élément non pris en compte. <br/><br/>Les éléments pris en charge incluent les objets suivants :<br/>  <br/>- [Élément](item.md) <br/>- [Message](message-ex15websvcsotherref.md) <br/>- [CalendarItem](calendaritem.md) <br/>- [Tâche](task.md) <br/>- [Contact](contact.md) <br/><br/>  Certains types sont créés en tant qu’effet secondaire d’une autre chose. Les messages de réunion, par exemple, sont créés lorsque vous envoyez un élément de calendrier aux participants ; ils ne sont pas créés explicitement.  <br/> |
|ErrorInvalidItemForOperationDeclineItem  <br/> |Cette erreur se produit lorsqu’une tentative d’utilisation d’un objet de réponse DeclineItem est réalisée pour un type d’élément autre qu’une demande de réunion ou un élément de calendrier, ou lorsqu’une tentative de refus d’une occurrence d’élément de calendrier se trouve dans le dossier Éléments supprimés.  <br/> |
|ErrorInvalidItemForOperationExpandDL  <br/> |Cette erreur indique que [l’opération ExpandDL](expanddl-operation.md) est valide uniquement pour les listes de distribution privées.  <br/> |
|ErrorInvalidItemForOperationRemoveItem  <br/> |Cette erreur est renvoyée à partir d’un objet de réponse RemoveItem si la demande spécifie un élément qui n’est pas un élément d’annulation de réunion.  <br/> |
|ErrorInvalidItemForOperationSendItem  <br/> |Cette erreur est renvoyée par une [opération SendItem](senditem-operation.md) si la demande spécifie un élément qui n’est pas un élément de message.  <br/> |
|ErrorInvalidItemForOperationTentative  <br/> |Cette erreur se produit lorsqu’une tentative d’utilisation de [TentativelyAcceptItem](tentativelyacceptitem.md) est réalisée pour un type d’élément autre qu’une demande de réunion ou un élément de calendrier, ou lorsqu’une tentative d’acceptation d’une occurrence d’élément de calendrier qui se trouve dans le dossier Éléments supprimés est tentée.  <br/> |
|ErrorInvalidLogonType  <br/> |Cette erreur est uniquement à usage interne. Cette erreur n’est pas renvoyée.  <br/> |
|ErrorInvalidMailbox  <br/> |Cette erreur indique que l’opération [CreateItem](createitem-operation.md) ou [UpdateItem](updateitem-operation.md) a échoué lors de la création ou de la mise à jour d’une liste de distribution personnelle.  <br/> |
|ErrorInvalidManagedFolderProperty  <br/> |Cette erreur se produit lorsque la structure du dossier géré est endommagée et ne peut pas être rendue.  <br/> |
|ErrorInvalidManagedFolderQuota  <br/> |Cette erreur se produit lorsque le quota qui est définie sur le dossier géré est inférieur à zéro, ce qui indique un dossier géré endommagé.  <br/> |
|ErrorInvalidManagedFolderSize  <br/> |Cette erreur se produit lorsque la taille définie sur le dossier géré est inférieure à zéro, ce qui indique un dossier géré endommagé.  <br/> |
|ErrorInvalidMergedFreeBusyInterval  <br/> |Cette erreur se produit lorsque la valeur interne de la période de libre/occupé fusionnée fournie n’est pas valide. La valeur minimale par défaut est 5 minutes. La valeur maximale par défaut est 1 440 minutes.  <br/> |
|ErrorInvalidNameForNameResolution  <br/> |Cette erreur se produit lorsque le nom n’est pas valide pour [l’opération ResolveNames](resolvenames-operation.md). Par exemple, une chaîne de longueur nulle, un espace unique, une virgule et un tiret sont tous des noms non valides.  <br/> |
|ErrorInvalidNetworkServiceContext  <br/> |Cette erreur indique une erreur dans le compte service réseau sur le serveur d’accès au client.  <br/> |
|ErrorInvalidOofParameter  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorInvalidOperation  <br/> | Il s’agit d’une erreur générale qui est utilisée lorsque l’opération demandée n’est pas valide. <br/><br/>Par exemple, vous ne pouvez pas : <br/> <br/>- Effectuez une traversée « profonde » à l’aide de [l’opération FindFolder](findfolder-operation.md) sur un dossier public.  <br/>- Déplacer ou copier la racine du dossier public.  <br/>- Supprimez un élément associé en utilisant n’importe quel mode à l’exception de la suppression « dur ».  <br/>- Déplacer ou copier un élément associé.  <br/> |
|ErrorInvalidOrganizationRelationshipForFreeBusy  <br/> |Cette erreur indique qu’un appelant a demandé des informations de libre/occupé pour un utilisateur d’une autre organisation, mais que la relation organisationnelle n’a pas la libre/occupé activée.  <br/> |
|ErrorInvalidPagingMaxRows  <br/> |Cette erreur se produit lorsqu’un consommateur passe un zéro ou une valeur négative pour le nombre maximal de lignes à retourner.  <br/> |
|ErrorInvalidParentFolder  <br/> |Cette erreur se produit lorsqu’un consommateur passe dans un dossier parent non valide pour une opération. Par exemple, cette erreur est renvoyée si vous essayez de créer un dossier dans un dossier de recherche.  <br/> |
|ErrorInvalidPercentCompleteValue  <br/> |Cette erreur est renvoyée lorsqu’une tentative est réalisée pour définir un pourcentage d’achèvement de tâche sur une valeur non valide. La valeur doit être entre 0 et 100 (inclus).  <br/> |
|ErrorInvalidPermissionSettings  <br/> |Cette erreur indique que le niveau d’autorisation est incohérent avec les paramètres d’autorisation.  <br/> |
|ErrorInvalidPhoneCallId  <br/> |Cette erreur indique que l’identificateur de l’appelant n’est pas valide.  <br/> |
|ErrorInvalidPhoneNumber  <br/> |Cette erreur indique que le numéro de téléphone n’est pas correct ou ne correspond pas aux règles du plan de numérotation.  <br/> |
|ErrorInvalidPropertyAppend  <br/> | Cette erreur se produit lorsque la propriété à qui vous essayez d’appender ne prend pas en charge l’attente. <br/><br/>Les propriétés suivantes sont les seules à la prise en charge de l’attente : <br/> <br/>- Collections de destinataires (ToRecipients, CcRecipients, BccRecipients)  <br/>- Collections attendee (RequiredAttendees, OptionalAttendees, Resources)  <br/>- Corps  <br/>- ReplyTo  <br/><br/>  En outre, cette erreur se produit lorsqu’un corps de message est envoyé si le format spécifié dans la demande ne correspond pas au format de l’élément dans la boutique.  <br/> |
|ErrorInvalidPropertyDelete  <br/> |Cette erreur se produit si l’opération de suppression est spécifiée dans une opération [UpdateItem](updateitem-operation.md) ou un appel d’opération [UpdateFolder](updatefolder-operation.md) pour une propriété qui ne prend pas en charge l’opération de suppression. Par exemple, vous ne pouvez pas supprimer [l’élément ItemId](itemid.md) de [l’objet Item.](item.md)  <br/> |
|ErrorInvalidPropertyForExists  <br/> |Cette erreur se produit si le consommateur transmet l’une des propriétés d’indicateur dans un [filtre Exists.](exists.md) Par exemple, cette erreur se produit si les indicateurs [IsRead](isread.md) ou [IsFromMe](isfromme.md) sont spécifiés dans [l’élément Exists.](exists.md) La demande doit utiliser [l’élément IsEqualTo](isequalto.md) à la place pour ceux-ci, car il s’agit d’indicateurs et donc d’une seule propriété.  <br/> |
|ErrorInvalidPropertyForOperation  <br/> |Cette erreur se produit lorsque la propriété que vous essayez de manipuler ne prend pas en charge l’opération en cours sur celle-ci.  <br/> |
|ErrorInvalidPropertyRequest  <br/> | Cette erreur se produit si une propriété spécifiée dans la demande n’est pas disponible pour le type d’élément. Par exemple, cette erreur est renvoyée si une propriété disponible uniquement sur les éléments de calendrier est demandée dans un appel d’opération [GetItem](getitem-operation.md) pour un message ou est mise à jour dans un appel d’opération [UpdateItem](updateitem-operation.md) pour un message. <br/> <br/>  Cela se produit dans les opérations suivantes : <br/> <br/>- [Opération GetItem](getitem-operation.md) <br/>- [Opération GetFolder](getfolder-operation.md) <br/>- [Opération UpdateItem](updateitem-operation.md) <br/>- [Opération UpdateFolder](updatefolder-operation.md) <br/> |
|ErrorInvalidPropertySet  <br/> |Cette erreur indique que la propriété que vous essayez de manipuler ne prend pas en charge l’opération en cours sur celle-ci. Par exemple, cette erreur est renvoyée si la propriété que vous essayez de définir est en lecture seule.  <br/> |
|ErrorInvalidPropertyUpdateSentMessage  <br/> | Cette erreur se produit lors d’une [opération UpdateItem](updateitem-operation.md) lorsqu’un client tente de mettre à jour certaines propriétés d’un message qui a déjà été envoyé.<br/><br/> Par exemple, les propriétés suivantes ne peuvent pas être mises à jour sur un message envoyé : <br/> <br/>- [IsReadReceiptRequested](isreadreceiptrequested.md) <br/>- [IsDeliveryReceiptRequested](isdeliveryreceiptrequested.md) <br/> |
|ErrorInvalidProxySecurityContext  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorInvalidPullSubscriptionId  <br/> |Cette erreur se produit si vous appelez l’opération [GetEvents](getevents-operation.md) ou [l’opération Desubscribe](unsubscribe-operation.md) à l’aide d’un ID d’abonnement Push. Pour vous désabonner d’un abonnement Push, vous devez répondre à une demande Push avec une réponse de désabonnement, ou déconnecter votre service Web et attendre le délai d’attente des notifications Push.  <br/> |
|ErrorInvalidPushSubscriptionUrl  <br/> | Cette erreur est renvoyée par l’opération [Subscribe](subscribe-operation.md) lorsqu’elle crée un abonnement « push » et indique que l’URL incluse dans la demande n’est pas valide.<br/><br/>Les conditions suivantes doivent être remplies pour que Exchange Web Services accepte l’URL : <br/> <br/>- Longueur de \> chaîne 0 et \< 2083.  <br/> - Protocole http ou https.  <br/>- L’URL peut être parée par l’URI Microsoft .NET Framework classe.  <br/> |
|ErrorInvalidRecipients  <br/> |Cette erreur indique que la collection de destinataires sur votre message ou la collection de participants sur votre élément de calendrier n’est pas valide. Par exemple, cette erreur est renvoyée lorsqu’une tentative d’envoi d’un élément sans destinataire est réalisée.  <br/> |
|ErrorInvalidRecipientSubfilter  <br/> |Cette erreur indique que le dossier de recherche possède un filtre de table de destinataires Exchange que les services Web ne peuvent pas représenter. Pour contourner cette erreur, récupérez le dossier sans demander les paramètres de recherche.  <br/> |
|ErrorInvalidRecipientSubfilterComparison  <br/> |Cette erreur indique que le dossier de recherche possède un filtre de table de destinataires Exchange que les services Web ne peuvent pas représenter. Pour contourner cette erreur, récupérez le dossier sans demander les paramètres de recherche.  <br/> |
|ErrorInvalidRecipientSubfilterOrder  <br/> |Cette erreur indique que le dossier de recherche possède un filtre de table de destinataires Exchange que les services Web ne peuvent pas représenter. Pour contourner cette erreur, récupérez le dossier sans demander les paramètres de recherche.  <br/> |
|ErrorInvalidRecipientSubfilterTextFilter  <br/> |Cette erreur indique que le dossier de recherche possède un filtre de table de destinataires Exchange que les services Web ne peuvent pas représenter. Pour contourner cette erreur, récupérez le dossier sans demander les paramètres de recherche.  <br/> |
|ErrorInvalidReferenceItem  <br/> | Cette erreur est renvoyée par [l’opération CreateItem](createitem-operation.md) pour les objets de réponse forward et reply dans les scénarios suivants :<br/>  <br/>- L’identificateur de l’élément référencé n’est pas un [Message,](message-ex15websvcsotherref.md)un [CalendarItem](calendaritem.md)ou un descendant d’un **Message** ou **CalendarItem**.  <br/>- L’identificateur de l’élément de référence est pour un **CalendarItem** et l’organisateur tente de répondre à lui-même ou ReplyAll.  <br/>- Le message est un brouillon et Reply ou ReplyAll est sélectionné.  <br/>- L’élément de référence, pour [SuppressReadReceipt,](suppressreadreceipt.md)n’est pas un **message** ou un descendant d’un **message**.  <br/> |
|ErrorInvalidRequest  <br/> |Cette erreur se produit lorsque la requête SOAP a un en-tête d’action SOAP, mais rien dans le corps SOAP. Notez que l’en-tête d’action SOAP n’est pas requis car Exchange Web Services peut déterminer la méthode à appeler à partir du nom local de l’élément racine dans le corps SOAP.  <br/> |
|ErrorInvalidRestriction  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorInvalidRetentionTagTypeMismatch  <br/> |Cette erreur est renvoyée lorsque la balise de rétention spécifiée est associée à une action incorrecte. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorInvalidRetentionTagInvisible  <br/> |Cette erreur est renvoyée lorsqu’une tentative de définir une balise invisible ou inexistante sur une **propriété PolicyTag** est tentée. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorInvalidRetentionTagInheritance  <br/> |Cette erreur est renvoyée lorsqu’une tentative de définir une balise implicite sur la **propriété PolicyTag** est tentée. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorInvalidRetentionTagIdGuid  <br/> |Indique que le GUID de la balise de rétention n’était pas valide.  <br/> |
|ErrorInvalidRoutingType  <br/> |Cette erreur se produit si le type de routage transmis pour un élément [RoutingType (EmailAddressType)](routingtype-emailaddresstype.md) n’est pas valide. En règle générale, le type de routage est définie sur SMTP (Simple Mail Transfer Protocol).  <br/> |
|ErrorInvalidScheduledOofDuration  <br/> |Cette erreur se produit si l’heure de fin spécifiée n’est pas supérieure à l’heure de début ou si l’heure de fin ne se produit pas à l’avenir.  <br/> |
|ErrorInvalidSchemaVersionForMailboxVersion  <br/> |Cette erreur indique qu’une demande de proxy qui a été envoyée à un autre serveur n’est pas en mesure de la mettre en service en raison d’une inaltérée de gestion des versions.  <br/> |
|ErrorInvalidSecurityDescriptor  <br/> |Cette erreur indique que le descripteur de sécurité Exchange dans le dossier Calendrier de la boutique est endommagé.  <br/> |
|ErrorInvalidSendItemSaveSettings  <br/> |Cette erreur se produit lors d’une tentative d’envoi d’un élément où [savedItemFolderId](saveditemfolderid.md) est spécifié dans la demande, mais la propriété **SaveItemToFolder** est définie sur **false**.  <br/> |
|ErrorInvalidSerializedAccessToken  <br/> |Cette erreur indique que le jeton qui a été transmis dans l’en-tête est malformé, qu’il ne fait pas référence à un compte valide dans l’annuaire ou qu’il manque le groupe principal **ConnectingSID**.  <br/> |
|ErrorInvalidSharingData  <br/> |Cette erreur indique que les métadonnées de partage ne sont pas valides. Cela peut être dû à un XML non valide.  <br/> |
|ErrorInvalidSharingMessage  <br/> |Cette erreur indique que le message de partage n’est pas valide. Cela peut être dû à une propriété manquante.  <br/> |
|ErrorInvalidSid  <br/> |Cette erreur se produit lorsqu’un SID non valide est transmis dans une demande.  <br/> |
|ErrorInvalidSIPUri  <br/> |Cette erreur indique que le nom SIP, le plan de numérotation ou le numéro de téléphone ne sont pas valides.  <br/> |
|ErrorInvalidServerVersion  <br/> |Cette erreur indique qu’une version du serveur de demande non valide a été spécifiée dans la demande.  <br/> |
|ErrorInvalidSmtpAddress  <br/> |Cette erreur se produit lorsque l’adresse SMTP ne peut pas être interrogée.  <br/> |
|ErrorInvalidSubfilterType  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorInvalidSubfilterTypeNotAttendeeType  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorInvalidSubfilterTypeNotRecipientType  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorInvalidSubscription  <br/> |Cette erreur indique que l’abonnement n’est plus valide. Cela peut être dû au redémarrage du serveur d’accès au client ou à l’expiration de l’abonnement.  <br/> |
|ErrorInvalidSubscriptionRequest  <br/> |Cette erreur indique que la demande d’abonnement incluait plusieurs ID de dossier public. Un abonnement peut inclure plusieurs dossiers de la même boîte aux lettres ou d’un ID de dossier public.  <br/> |
|ErrorInvalidSyncStateData  <br/> |Cette erreur est renvoyée par [SyncFolderItems](syncfolderitems.md) ou [SyncFolderHierarchy](syncfolderhierarchy.md) si les données [SyncState](syncstate-ex15websvcsotherref.md) transmises ne sont pas valides. Pour corriger cette erreur, vous devez resynchroniser sans l’état de synchronisation. Assurez-vous que si vous persistez les objets BLOB d’état de synchronisation, vous ne tronqués pas accidentellement l’objet BLOB.  <br/> |
|ErrorInvalidTimeInterval  <br/> |Cette erreur indique que l’intervalle de temps spécifié n’est pas valide. L’heure de début doit être supérieure ou égale à l’heure de fin.  <br/> |
|ErrorInvalidUserInfo  <br/> |Cette erreur indique qu’un [UserId](userid.md) incohérent en interne a été spécifié pour une opération d’autorisations. Par exemple, si un ID d’utilisateur spécifique est spécifié (par défaut ou anonyme), cette erreur est renvoyée si vous essayez également de spécifier un SID, une adresse SMTP principale ou un nom complet pour cet utilisateur.  <br/> |
|ErrorInvalidUserOofSettings  <br/> |Cette erreur indique que les paramètres d’absence du Office utilisateur ne sont pas valides en raison d’une réponse interne ou externe manquante.  <br/> |
|ErrorInvalidUserPrincipalName  <br/> |Cette erreur se produit pendant l Exchange emprunt d’identité. L’appelant a transmis un UPN non valide dans l’en-tête SOAP qui n’était pas accessible dans l’annuaire.  <br/> |
|ErrorInvalidUserSid  <br/> |Cette erreur se produit lorsqu’un SID non valide est transmis dans une demande.  <br/> |
|ErrorInvalidUserSidMissingUPN  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorInvalidValueForProperty  <br/> |Cette erreur indique que la valeur de comparaison dans la restriction n’est pas valide pour la propriété que vous comparez.<br/><br/> Par exemple, la valeur de comparaison [DateTimeCreated](datetimecreated.md)  >  **true** ren retournerait ce code de réponse. <br/><br/>Ce code de réponse est également renvoyé si vous spécifiez une propriété d’éumération dans la comparaison, mais la valeur que vous comparez n’est pas une valeur valide pour cette éumération.  <br/> |
|ErrorInvalidMark  <br/> |Cette erreur est due à un filigrane non valide.  <br/> |
|ErrorIPGatewayNotFound  <br/> |Cette erreur indique qu’une passerelle VoIP valide n’est pas disponible.  <br/> |
|ErrorIrresolvableConflict  <br/> |Cette erreur indique que la résolution des conflits n’a pas pu résoudre les modifications des propriétés. Les éléments de la boutique ont peut-être été modifiés et doivent être mis à jour. Récupérez la touche de modification mise à jour et recommencez.  <br/> |
|ErrorItemCorrupt  <br/> |Cette erreur indique que l’état de l’objet est endommagé et ne peut pas être récupéré. Lorsque vous récupérez un élément, seuls certains éléments seront dans cet état, tels que [Body](body.md) et [MimeContent](mimecontent.md). Omettez ces éléments et réessayez l’opération.  <br/> |
|ErrorItemNotFound  <br/> |Cette erreur se produit lorsque l’élément est in trouvé ou que vous n’êtes pas autorisé à accéder à l’élément.  <br/> |
|ErrorItemPropertyRequestFailed  <br/> |Cette erreur se produit en cas d’échec d’une demande de propriété sur un élément. La propriété peut exister, mais elle n’a pas pu être récupérée.  <br/> |
|ErrorItemSave  <br/> |Cette erreur se produit lorsque les tentatives d’enregistrer l’élément ou le dossier échouent.  <br/> |
|ErrorItemSavePropertyError  <br/> |Cette erreur se produit lorsque les tentatives d’enregistrer l’élément ou le dossier échouent en raison de valeurs de propriété non valides. Le code de réponse inclut le chemin d’accès des propriétés non valides.  <br/> |
|ErrorLegacyMailboxFreeBusyViewTypeNotMerged  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorLocalServerObjectNotFound  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorLogonAsNetworkServiceFailed  <br/> |Cette erreur indique que le service de disponibilité n’a pas pu se connecter en tant que service réseau pour proxyer les demandes aux sites ou forêts appropriés. Cette réponse indique généralement une erreur de configuration.  <br/> |
|ErrorMailboxConfiguration  <br/> |Cette erreur indique que les informations de boîte aux lettres dans AD DS sont configurées de manière incorrecte.  <br/> |
|ErrorMailboxDataArrayEmpty  <br/> |Cette erreur indique que [l’élément MailboxDataArray](mailboxdataarray.md) dans la demande est vide. Vous devez fournir au moins un identificateur de boîte aux lettres.  <br/> |
|ErrorMailboxDataArrayTooBig  <br/> |Cette erreur se produit lorsque plus de 100 entrées sont fournies dans un élément [MailboxDataArray.](mailboxdataarray.md)  <br/> |
|ErrorMailboxFailover  <br/> |Cette erreur indique qu’une tentative d’accès à une boîte aux lettres a échoué car la boîte aux lettres est en cours de processus deover.  <br/> |
|ErrorMailboxHoldNotFound  <br/> |Indique que la boîte aux lettres est in trouvée.  <br/> |
|ErrorMailboxLogonFailed  <br/> |Cette erreur se produit lorsque la connexion à la boîte aux lettres pour obtenir les informations de l’affichage Calendrier a échoué.  <br/> |
|ErrorMailboxMoveInProgress  <br/> | Cette erreur indique que la boîte aux lettres est déplacée vers un autre magasin ou serveur de boîtes aux lettres. Cette erreur peut également indiquer que la boîte aux lettres se trouve sur un autre serveur ou base de données de boîtes aux lettres.  <br/> |
|ErrorMailboxStoreUnavailable  <br/> | Cette erreur indique que l’une des conditions d’erreur suivantes s’est produite :  <br/><br/>- La boîte aux lettres est endommagée.  <br/>- La boîte aux lettres est en cours d’arrêt.  <br/>- La boîte aux lettres est hors connexion.  <br/>- Une erreur réseau s’est produite lors d’une tentative d’accès à la boîte aux lettres.  <br/>- La boîte aux lettres est surchargée et ne peut plus accepter de connexions.  <br/>- La boîte aux lettres a été suspendue.  <br/> |
|ErrorMailRecipientNotFound  <br/> |Cette erreur se produit si les informations de l’élément [MailboxData](mailboxdata.md) ne peuvent pas être mappées sur un compte de boîte aux lettres valide.  <br/> |
|ErrorMailTipsDisabled  <br/> |Cette erreur indique que les infos-courrier sont désactivées.  <br/> |
|ErrorManagedFolderAlreadyExists  <br/> |Cette erreur se produit si le dossier géré que vous essayez de créer existe déjà dans une boîte aux lettres.  <br/> |
|ErrorManagedFolderNotFound  <br/> |Cette erreur se produit lorsque le nom du dossier spécifié dans la demande n’est pas map marqué sur une définition de dossier géré dans AD DS. Vous pouvez uniquement créer des instances de dossiers gérés pour les dossiers définis dans AD DS. Vérifiez le nom et recommencez.  <br/> |
|ErrorManagedFoldersRootFailure  <br/> |Cette erreur indique que la racine des dossiers gérés a été supprimée de la boîte aux lettres ou qu’un dossier existe dans le même dossier parent qui porte le nom de la racine du dossier géré. Cela se produit également si la tentative de création du dossier géré racine échoue.  <br/> |
|ErrorMeetingSuggestionGenerationFailed  <br/> |Cette erreur indique que le moteur de suggestions a rencontré un problème lors de la tentative de générer les suggestions.  <br/> |
|ErrorMessageDispositionRequired  <br/> | Cette erreur se produit si **l’attribut MessageDisposition** n’est pas définie.<br/><br/> Cet attribut est requis pour les éléments suivants : <br/> <br/>- [L’opération CreateItem et](createitem-operation.md) [l’opération UpdateItem](updateitem-operation.md) lorsque l’élément en cours de création ou de mise à jour est un [message](message-ex15websvcsotherref.md).  <br/>- Objets de réponse [CancelCalendarItem,](cancelcalendaritem.md) [AcceptItem,](acceptitem.md) [DeclineItem](declineitem.md)ou [TentativelyAcceptItem.](tentativelyacceptitem.md)  <br/> |
|ErrorMessageSizeExceeded  <br/> |Cette erreur indique que le message que vous essayez d’envoyer dépasse les limites autorisées.  <br/> |
|ErrorMessageTrackingNoSuchDomain  <br/> |Cette erreur indique que le domaine donné est in trouver.  <br/> |
|ErrorMessageTrackingPermanentError  <br/> |Cette erreur indique que le service de suivi des messages ne peut pas suivre le message.  <br/> |
| ErrorMessageTrackingTransientError  <br/> |Cette erreur indique que le service de suivi des messages est en panne ou occupé. Ce code d’erreur indique une erreur passagère. Les clients peuvent réessayer de se connecter au serveur lorsque cette erreur est reçue.  <br/> |
|ErrorMimeContentConversionFailed  <br/> |Cette erreur se produit lorsque le contenu MIME n’est pas un iCal valide pour une [opération CreateItem](createitem-operation.md). Pour une [opération GetItem,](getitem-operation.md)cette réponse indique que le contenu MIME n’a pas pu être généré.  <br/> |
|ErrorMimeContentInvalid  <br/> |Cette erreur se produit lorsque le contenu MIME n’est pas valide.  <br/> |
|ErrorMimeContentInvalidBase64String  <br/> |Cette erreur se produit lorsque le contenu MIME dans la demande n’est pas une chaîne de base 64 valide.  <br/> |
|ErrorMissingArgument  <br/> |Cette erreur indique qu’un argument obligatoire était absent de la demande. Le texte du message de réponse indique l’argument à vérifier.  <br/> |
|ErrorMissingEmailAddress  <br/> |Cette erreur indique que vous avez spécifié un ID de dossier spécifique dans la demande, mais que le compte qui a effectué la demande n’a pas de boîte aux lettres sur le système. Dans ce cas, vous devez fournir un sous-élément [Mailbox](mailbox.md) sous [DistinguishedFolderId](distinguishedfolderid.md).  <br/> |
|ErrorMissingEmailAddressForManagedFolder  <br/> |Cette erreur indique que vous avez spécifié un ID de dossier spécifique dans la demande, mais que le compte qui a effectué la demande n’a pas de boîte aux lettres sur le système. Dans ce cas, vous devez fournir un sous-élément [Mailbox](mailbox.md) sous [DistinguishedFolderId](distinguishedfolderid.md). Cette réponse est renvoyée par [l’opération CreateManagedFolder](createmanagedfolder-operation.md).  <br/> |
|ErrorMissingInformationEmailAddress  <br/> |Cette erreur se produit si [l’élément EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) est manquant.  <br/> |
|ErrorMissingInformationReferenceItemId  <br/> |Cette erreur se produit si [le ReferenceItemId](referenceitemid.md) est manquant.  <br/> |
|ErrorMissingInformationSharingFolderId  <br/> |Ce code d’erreur n’est jamais renvoyé.  <br/> |
|ErrorMissingItemForCreateItemAttachment  <br/> |Cette erreur est renvoyée lorsqu’une tentative est faite de ne pas inclure l’élément d’élément dans l’élément **ItemAttachment** d’une [demande d’opération CreateAttachment.](createattachment-operation.md)  <br/> |
|ErrorMissingManagedFolderId  <br/> |Cette erreur se produit lorsque la propriété ID de stratégie, balise de 0x6732, pour le dossier est manquante. Vous devez considérer qu’il s’agit d’un dossier endommagé.  <br/> |
|ErrorMissingRecipients  <br/> |Cette erreur indique que vous avez essayé d’envoyer un élément sans inclure de destinataires. Notez que si vous appelez l’opération [CreateItem](createitem-operation.md) avec une disposition de message qui entraîne l’envoi du message, vous obtenez le code de réponse suivant : **ErrorInvalidRecipients**.  <br/> |
|ErrorMissingUserIdInformation  <br/> |Cette erreur indique qu’un [UserId](userid.md) n’a pas été entièrement spécifié dans un jeu d’autorisations.  <br/> |
|ErrorMoreThanOneAccessModeSpecified  <br/> |Cette erreur indique que vous avez spécifié plusieurs valeurs d’élément [ExchangeImpersonation](exchangeimpersonation.md) dans une demande.  <br/> |
|ErrorMoveCopyFailed  <br/> |Cette erreur indique que l’opération de déplacement ou de copie a échoué. Le déplacement se produit dans [l’opération CreateItem](createitem-operation.md) lorsque vous acceptez une demande de réunion qui se trouve dans le dossier Éléments supprimés. En outre, si vous refusez une demande de réunion, annulez un élément de calendrier ou supprimez une réunion de votre calendrier, elle est déplacée vers le dossier Éléments supprimés.  <br/> |
|ErrorMoveDistinguishedFolder  <br/> |Cette erreur se produit si vous essayez de déplacer un dossier spécifique.  <br/> |
|ErrorMultiLegacyMailboxAccess  <br/> |Cette erreur se produit lorsqu’une demande tente d’accéder à plusieurs serveurs de boîtes aux lettres. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorNameResolutionMultipleResults  <br/> |Cette erreur se produit si [l’opération ResolveNames](resolvenames-operation.md) renvoie plusieurs résultats ou si le nom ambigu que vous avez spécifié correspond à plusieurs objets dans le répertoire. Le code de réponse inclut les noms de correspondance dans les données de réponse.  <br/> |
|ErrorNameResolutionNoMailbox  <br/> |Cette erreur indique que l’appelant n’a pas de boîte aux lettres sur le système. [L’opération ResolveNames ou](resolvenames-operation.md) [ExpandDL n’est](expanddl-operation.md) pas valide pour connecter un utilisateur sans boîte aux lettres.  <br/> |
|ErrorNameResolutionNoResults  <br/> |Cette erreur indique que [l’opération ResolveNames ne](resolvenames-operation.md) renvoie aucun résultat.  <br/> |
|ErrorNoApplicableProxyCASServersAvailable  <br/> |Ce code d’erreur DOIT être renvoyé lorsque le service Web ne peut pas trouver de serveur pour gérer la demande.  <br/> |
|ErrorNoCalendar  <br/> |Cette erreur se produit s’il n’existe aucun dossier Calendrier pour la boîte aux lettres.  <br/> |
|ErrorNoDestinationCASDueToKerberosRequirements  <br/> |Cette erreur indique que la demande a fait référence à une boîte aux lettres dans un autre site Active Directory, mais qu’aucun serveur d’accès au client dans le site de destination n’a été configuré pour l’authentification Windows et que la demande n’a pas pu être proxyée.  <br/> |
|ErrorNoDestinationCASDueToSSLRequirements  <br/> |Cette erreur indique que la demande a fait référence à une boîte aux lettres dans un autre site Active Directory, mais qu’aucun serveur d’accès au client du site de destination n’a été configuré pour les connexions SSL et que la demande n’a pas pu être proxyée.  <br/> |
|ErrorNoDestinationCASDueToVersionMismatch  <br/> |Cette erreur indique que la demande a fait référence à une boîte aux lettres dans un autre site Active Directory, mais qu’aucun serveur d’accès au client dans le site de destination n’était d’une version acceptable du produit pour recevoir la demande, et par conséquent, la demande n’a pas pu être proxyée.  <br/> |
|ErrorNoFolderClassOverride  <br/> |Cette erreur se produit si vous définissez l’élément [FolderClass](folderclass.md) lorsque vous créez un élément autre qu’un dossier générique. Pour les dossiers typés tels que [CalendarFolder](calendarfolder.md) et [TasksFolder,](tasksfolder.md)la classe de dossier est implicite. La définition de la classe de dossier sur un autre type de dossier à l’aide de l’opération [UpdateFolder](updatefolder-operation.md) entraîne la réponse **ErrorObjectTypeChanged.** Utilisez plutôt un type de dossier générique, mais définissez la classe de dossier sur la valeur dont vous avez besoin. Exchange Les services web créent le dossier correctement fortement typé.  <br/> |
|ErrorNoFreeBusyAccess  <br/> |Cette erreur indique que l’appelant n’a pas de droits d’affichage de libre/occupé sur le dossier Calendrier en question.  <br/> |
|ErrorNonExistentMailbox  <br/> | Cette erreur se produit dans les scénarios suivants : <br/> <br/>- L’adresse de messagerie est vide dans [CreateManagedFolder](createmanagedfolder.md).  <br/>- L’adresse de messagerie ne fait pas référence à un compte valide dans une demande qui prend une adresse de messagerie dans le corps ou dans l’en-tête SOAP, comme dans un appel d’emprunt d’identité Exchange.  <br/> |
|ErrorNonPrimarySmtpAddress  <br/> |Cette erreur se produit lorsqu’un appelant passe à une adresse SMTP non principale. La réponse inclut l’adresse SMTP correcte à utiliser.  <br/> |
|ErrorNoPropertyTagForCustomProperties  <br/> |Cette erreur indique que les propriétés MAPI de la plage personnalisée, 0x8000 et supérieure, ne peuvent pas être référencés par des balises de propriété. Vous devez utiliser la propriété [PropertySetId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.extendedpropertydefinition.propertysetid%28v=exchg.80%29.aspx)de l’API gérée EWS ou l’élément EWS [ExtendedFieldURI](extendedfielduri.md) avec l’attribut PropertySetId.  <br/> |
|ErrorNoPublicFolderReplicaAvailable  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorNoPublicFolderServerAvailable  <br/> |Ce code d’erreur DOIT être renvoyé si aucun serveur de dossiers publics n’est disponible ou si l’appelant ne dispose pas d’un serveur public à domicile.  <br/> |
|ErrorNoRespondingCASInDestinationSite  <br/> |Cette erreur indique que la demande a fait référence à une boîte aux lettres dans un autre site Active Directory, mais qu’aucun des serveurs d’accès au client de ce site n’a répondu et que la demande n’a pas pu être proxyée.  <br/> |
|ErrorNotAllowedExternalSharingByPolicy  <br/> |Cette erreur indique que l’appelant a tenté d’accorder des autorisations dans son calendrier ou son dossier de contacts à un utilisateur d’une autre organisation, et que la tentative a échoué.  <br/> |
|ErrorNotDelegate  <br/> |Cette erreur indique que l’utilisateur n’est pas délégué pour la boîte aux lettres. Elle est renvoyée par l’opération [GetDelegate,](getdelegate-operation.md) [l’opération RemoveDelegate](removedelegate-operation.md)et l’opération [UpdateDelegate](updatedelegate-operation.md) lorsque l’utilisateur délégué spécifié est in trouvé dans la liste des délégués.  <br/> |
|ErrorNotEnoughMemory  <br/> |Cette erreur indique que l’opération n’a pas pu être achevée en raison d’une mémoire insuffisante.  <br/> |
|ErrorNotSupportedSharingMessage  <br/> |Cette erreur indique que le message de partage n’est pas pris en charge.  <br/> |
|ErrorObjectTypeChanged  <br/> |Cette erreur se produit si le type d’objet a changé.  <br/> |
|ErrorOccurrenceCrossingBoundary  <br/> |Cette erreur se [](start.md) produit [](end-ex15websvcsotherref.md) lorsque l’heure de début ou de fin d’une occurrence est mise à jour afin que l’occurrence soit programmée pour se produire plus tôt ou plus tard que l’occurrence précédente ou suivante correspondante.  <br/> |
|ErrorOccurrenceTimeSpanTooBig  <br/> |Cette erreur indique que l’allotment de temps pour une occurrence donnée chevauche une autre occurrence du même élément périodique. Cette réponse se produit également lorsque la longueur en minutes d’une occurrence donnée est supérieure à Int32.MaxValue.  <br/> |
|ErrorOperationNotAllowedWithPublicFolderRoot  <br/> |Cette erreur indique que l’opération en cours n’est pas valide pour la racine du dossier public.  <br/> |
|ErrorOrganizationNotFederated  <br/> |Cette erreur indique que l’organisation du demandeur n’est pas fédérée de sorte que le demandeur ne peut pas créer de messages de partage à envoyer à un utilisateur externe ou ne peut pas accepter le partage de messages reçus d’un utilisateur externe.  <br/> |
|ErrorParentFolderIdRequired  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorParentFolderNotFound  <br/> |Cette erreur se produit dans [l’opération CreateFolder](createfolder-operation.md) lorsque le dossier parent est in trouvé.  <br/> |
|ErrorPasswordChangeRequired  <br/> |Cette erreur indique que vous devez modifier votre mot de passe avant de pouvoir accéder à cette boîte aux lettres. Cela se produit lorsqu’un nouveau compte a été créé et que l’administrateur a indiqué que l’utilisateur doit modifier le mot de passe lors de la première logonisation. Vous ne pouvez pas mettre à jour le mot de passe en utilisant Exchange Web Services. Vous devez utiliser un outil tel que Microsoft Office Outlook Web App pour modifier votre mot de passe.  <br/> |
|ErrorPasswordExpired  <br/> |Cette erreur indique que le mot de passe a expiré. Vous ne pouvez pas modifier le mot de passe à l’aide Exchange Web Services. Vous devez utiliser un outil tel que Outlook Web App pour modifier votre mot de passe.  <br/> |
|ErrorPermissionNotAllowedByPolicy  <br/> |Cette erreur indique que le demandeur a tenté d’accorder des autorisations dans son calendrier ou son dossier de contacts à un utilisateur externe, mais que la stratégie de partage attribuée au demandeur indique que le niveau d’autorisation demandé est supérieur à ce que la stratégie de partage autorise.  <br/> |
|ErrorPhoneNumberNotDialable  <br/> |Cette erreur indique que le numéro de téléphone n’était pas au bon état.  <br/> |
|ErrorPropertyUpdate  <br/> |Cette erreur indique que la mise à jour a échoué en raison de valeurs de propriété non valides. Le message de réponse inclut les chemins de propriété non valides.  <br/> |
|ErrorPromptPublishingOperationFailed  <br/> |Cette erreur est destinée à un usage interne uniquement. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorPropertyValidationFailure  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorProxiedSubscriptionCallFailure  <br/> |Cette erreur indique que la demande fait référence à un abonnement qui existe sur un autre serveur d’accès au client, mais qu’une tentative de proxy de la demande vers ce serveur d’accès au client a échoué.  <br/> |
|ErrorProxyCallFailed  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorProxyGroupSidLimitExceeded  <br/> |Cette erreur indique que la demande a fait référence à une boîte aux lettres dans un autre site Active Directory et que l’appelant d’origine est membre de plus de 3 000 groupes.  <br/> |
|ErrorProxyRequestNotAllowed  <br/> |Cette erreur indique que la demande envoyée par Exchange Web Services à un autre serveur d’accès au client lors de la tentative de réalisation d’une demande [GetUserAvailabilityRequest](getuseravailabilityrequest.md) n’était pas valide. Ce code de réponse indique généralement qu’une erreur de configuration ou de droits s’est produite ou qu’une personne a tenté sans succès d’imiter une demande de proxy de disponibilité.  <br/> |
|ErrorProxyRequestProcessingFailed  <br/> |Cette erreur indique que les services web Exchange tenté de proxyer une demande de disponibilité vers un autre serveur d’accès au client pour l’accomplir, mais que la demande a échoué. Cette réponse peut être causée par des problèmes de connectivité réseau ou des problèmes de délai d’accès aux demandes.  <br/> |
|ErrorProxyServiceDiscoveryFailed  <br/> |Ce code d’erreur doit être renvoyé si le service Web ne peut pas déterminer si la demande doit s’exécuter sur le serveur cible ou si elle sera dirigée par proxy vers un autre serveur.  <br/> |
|ErrorProxyTokenExpired  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorPublicFolderMailboxDiscoveryFailed  <br/> |Cette erreur se produit lorsque l’URL de la boîte aux lettres de dossiers publics est in trouvée. Cette erreur est destinée à un usage interne uniquement. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorPublicFolderOperationFailed  <br/> |Cette erreur se produit lorsqu’une tentative d’accès à un dossier public est tentée et que la tentative échoue. Cette erreur a été introduite dans Exchange 2013Exchange Server 2013.  <br/> |
|ErrorPublicFolderRequestProcessingFailed  <br/> |Cette erreur se produit lorsque le destinataire transmis à l’opération [GetUserAvailability](getuseravailability-operation.md) se trouve sur un ordinateur exécutant une version de Exchange Server antérieure à Exchange 2007 et que la demande de récupération des informations de disponibilité du destinataire à partir du serveur de dossiers publics a échoué.  <br/> |
|ErrorPublicFolderServerNotFound  <br/> |Cette erreur se produit lorsque le destinataire qui a été transmis à l’opération [GetUserAvailability](getuseravailability-operation.md) se trouve sur un ordinateur exécutant une version de Exchange Server antérieure à Exchange 2007 et que la demande de récupération des informations de disponibilité du destinataire à partir du serveur de dossiers publics a échoué car l’unité d’organisation n’avait pas de serveur de dossiers publics associé.  <br/> |
|ErrorPublicFolderSyncException  <br/> |Cette erreur se produit lorsqu’une opération de synchronisation aboutie sur la boîte aux lettres de dossiers publics principale, mais pas sur la boîte aux lettres de dossiers publics secondaire. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorQueryFilterTooLong  <br/> |Cette erreur indique que la restriction de dossier de recherche est peut-être valide, mais qu’elle n’est pas prise en charge par EWS. Exchange Les services web limitent les restrictions pour contenir un maximum de 255 expressions de filtre. Si vous essayez de lier un dossier de recherche existant qui dépasse 255, ce code de réponse est renvoyé.  <br/> |
|ErrorQuotaExceeded  <br/> |Cette erreur se produit lorsque le quota de boîte aux lettres est dépassé.  <br/> |
|ErrorReadEventsFailed  <br/> |Cette erreur est renvoyée par l’opération [GetEvents](getevents-operation.md) ou les notifications Push lorsqu’un échec se produit lors de la récupération des informations d’événement. Lorsque cette erreur est renvoyée, l’abonnement est supprimé. Re-créez la synchronisation d’événements en fonction d’un dernier filigrane connu.  <br/> |
|ErrorReadReceiptNotPending  <br/> |Cette erreur est renvoyée par l’opération [CreateItem](createitem-operation.md) si une tentative de suppression d’une réception de lecture a été réalisée lorsque l’expéditeur du message n’a pas demandé de accusé de réception de lecture sur le message ou si le message se trouve dans le dossier Courrier indésirable.  <br/> |
|ErrorRecurrenceEndDateTooBig  <br/> |Cette erreur se produit lorsque la date de fin de la récurrence se trouve après le 01/09/4500.  <br/> |
|ErrorRecurrenceHasNoOccurrence  <br/> |Cette erreur se produit lorsque la récurrence spécifiée n’a aucune instance d’occurrence dans la plage spécifiée.  <br/> |
|ErrorRemoveDelegatesFailed  <br/> |Cette erreur indique que la liste des délégués n’a pas pu être enregistrée après la suppression des délégués.  <br/> |
|ErrorRequestAborted  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorRequestStreamTooBig  <br/> | Cette erreur se produit lorsque le flux de demande est supérieur à 400 Ko.  <br/> |
|ErrorRequiredPropertyMissing  <br/> |Cette erreur est renvoyée lorsqu’une propriété requise est manquante dans une [demande d’opération CreateAttachment.](createattachment-operation.md) L’URI de propriété manquante est inclus dans la réponse.  <br/> |
|ErrorResolveNamesInvalidFolderType  <br/> |Cette erreur indique que l’appelant a spécifié un dossier qui n’est pas un dossier de contacts à [l’opération ResolveNames](resolvenames-operation.md).  <br/> |
|ErrorResolveNamesOnlyOneContactsFolderAllowed  <br/> |Cette erreur indique que l’appelant a spécifié plusieurs dossiers de contacts à [l’opération ResolveNames](resolvenames-operation.md).  <br/> |
|ErrorResponseSchemaValidation  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorRestrictionTooLong  <br/> |Cette erreur se produit si la restriction contient plus de 255 nodes.  <br/> |
|ErrorRestrictionTooComplex  <br/> |Cette erreur se produit lorsque la restriction ne peut pas être évaluée par Exchange Web Services.  <br/> |
|ErrorResultSetTooBig  <br/> |Cette erreur indique que le nombre d’entrées de calendrier pour un destinataire donné dépasse la limite autorisée de 1 000. Réduisez la fenêtre et recommencez.  <br/> |
|ErrorSavedItemFolderNotFound  <br/> |Cette erreur se produit lorsque [l’savedItemFolderId](saveditemfolderid.md) est in trouvé.  <br/> |
|ErrorSchemaValidation  <br/> | Cette erreur se produit lorsque la demande ne peut pas être validée par rapport au schéma.  <br/> |
|ErrorSearchFolderNotInitialized  <br/> |Cette erreur indique que le dossier de recherche a été créé, mais que les critères de recherche n’ont jamais été définis sur le dossier. Cela se produit uniquement lorsque vous accédez à des dossiers de recherche endommagés qui ont été créés à l’aide d’une autre API ou client. Pour corriger cette erreur, utilisez l’opération [UpdateFolder](updatefolder-operation.md) pour définir l’élément [SearchParameters](searchparameters.md) afin d’inclure la restriction qui doit se trouver sur le dossier.  <br/> |
|ErrorSendAsDenied  <br/> | Cette erreur se produit lorsque les deux conditions suivantes se produisent : <br/> <br/>- Un utilisateur a reçu des autorisations CanActAsOwner, mais ne dispose pas des droits de délégué sur la boîte aux lettres du principal.  <br/>- Le même utilisateur tente de créer et d’envoyer un message électronique dans la boîte aux lettres du principal à l’aide de l’option SendAndSaveCopy.<br/>  <br/>  Le résultat est une erreur ErrorSendAsDenied et la création du message électronique dans le dossier Brouillons du principal.  <br/> |
|ErrorSendMeetingCancellationsRequired  <br/> |Cette erreur est renvoyée par l’opération [DeleteItem](deleteitem-operation.md) si l’attribut **SendMeetingCancellations** est absent de la demande et si l’élément à supprimer est un élément de calendrier.  <br/> |
|ErrorSendMeetingInvitationsOrCancellationsRequired  <br/> |Cette erreur est renvoyée par l’opération [UpdateItem](updateitem-operation.md) si l’attribut **SendMeetingInvitationsOrCancellations** est absent de la demande et si l’élément à mettre à jour est un élément de calendrier.  <br/> |
|ErrorSendMeetingInvitationsRequired  <br/> |Cette erreur est renvoyée par l’opération [CreateItem](createitem-operation.md) si l’attribut **SendMeetingInvitations** est absent de la demande et si l’élément à créer est un élément de calendrier.  <br/> |
|ErrorSentMeetingRequestUpdate  <br/> |Cette erreur indique qu’une fois que l’organisateur a envoyé une demande de réunion, la demande ne peut pas être mise à jour. Pour modifier la réunion, modifiez l’élément de calendrier, et non la demande de réunion.  <br/> |
|ErrorSentTaskRequestUpdate  <br/> |Cette erreur indique qu’une fois que l’initiateur de la tâche a envoyé une demande de tâche, cette demande ne peut pas être mise à jour.  <br/> |
|ErrorServerBusy  <br/> |Cette erreur se produit lorsque le serveur est occupé.  <br/> |
|ErrorServiceDiscoveryFailed  <br/> |Cette erreur indique que les services web Exchange essayé de transmettre par proxy une demande de disponibilité utilisateur à la forêt appropriée pour le destinataire, mais qu’ils n’ont pas pu déterminer où envoyer la demande en raison d’un échec de découverte de service.  <br/> |
|ErrorSharingNoExternalEwsAvailable  <br/> |Cette erreur indique que la propriété d’URL externe n’a pas été définie dans la base de données Active Directory.  <br/> |
|ErrorSharingSynchronizationFailed  <br/> |Cette erreur indique qu’une tentative de synchronisation d’un dossier de partage a échoué. <br/><br/>Ce code d’erreur est renvoyé lorsque les erreurs suivantes se produisent :<br/><br/>- L’abonnement pour un dossier de partage est in trouvé.<br/>- Le dossier de partage est in trouvé.<br/>- L’utilisateur d’annuaire correspondant est in trouvé.<br/>- L’utilisateur n’existe plus.<br/>- Le rendez-vous n’est pas valide.<br/>- L’élément de contact n’est pas valide.<br/>- Échec de communication avec le serveur distant.  <br/> |
|ErrorStaleObject  <br/> |Cette erreur se produit dans une [opération UpdateItem](updateitem-operation.md) ou [SendItem](senditem-operation.md) lorsque la touche de modification n’est pas à jour ou n’a pas été fournie. Appelez [l’opération GetItem](getitem-operation.md) pour récupérer une touche de modification mise à jour, puis tentez à nouveau l’opération.  <br/> |
|ErrorSubmissionQuotaExceeded  <br/> |Cette erreur indique qu’un utilisateur ne peut pas envoyer immédiatement plus de demandes, car le quota de soumission a été atteint.  <br/> |
|ErrorSubscriptionAccessDenied  <br/> |Cette erreur se produit lorsque vous essayez d’accéder à un abonnement à l’aide d’un compte qui n’a pas créé cet abonnement. Chaque abonnement est accessible uniquement par le créateur de l’abonnement.  <br/> |
|ErrorSubscriptionDelegateAccessNotSupported  <br/> |Cette erreur indique que vous ne pouvez pas créer d’abonnement si vous n’êtes pas le propriétaire ou si vous n’avez pas accès à la boîte aux lettres.  <br/> |
|ErrorSubscriptionNotFound  <br/> |Cette erreur se produit si l’abonnement correspondant à [l’subscriptionId spécifié (GetEvents)](subscriptionid-getevents.md) est in trouvé. L’abonnement a peut-être expiré, le processus Exchange services web a peut-être été redémarré ou un abonnement non valide a été transmis. Si l’abonnement était valide, re-créez l’abonnement avec le filigrane le plus récent. Cette opération est renvoyée par [l’opération Unsubscribe ou](unsubscribe-operation.md) [les réponses de l’opération GetEvents.](getevents-operation.md)  <br/> |
|ErrorSubscriptionUnsubsribed  <br/> |Ce code d’erreur doit être renvoyé lorsqu’une demande d’abonnement n’a pas été inscrite.  <br/> |
|ErrorSyncFolderNotFound  <br/> |Cette erreur est renvoyée par [l’opération SyncFolderItems](syncfolderitems-operation.md) si le dossier parent spécifié est inaltérable.  <br/> |
|ErrorTeamMailboxNotFound  <br/> |Cette erreur indique qu’une boîte aux lettres d’équipe est in trouvée. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorTeamMailboxNotLinkedToSharePoint  <br/> |Cette erreur indique qu’une boîte aux lettres d’équipe a été trouvée, mais qu’elle n’est pas liée à SharePoint Server. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorTeamMailboxUrlValidationFailed  <br/> |Cette erreur indique qu’une boîte aux lettres d’équipe a été trouvée, mais que le lien vers SharePoint Server n’est pas valide. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorTeamMailboxNotAuthorizedOwner  <br/> |Ce code d’erreur n’est pas utilisé. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorTeamMailboxActiveToPendingDelete  <br/> |Ce code d’erreur n’est pas utilisé. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorTeamMailboxFailedSendingNotifications  <br/> |Cette erreur indique qu’une tentative d’envoi d’une notification aux propriétaires de boîtes aux lettres d’équipe a échoué. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorTeamMailboxErrorUnknown  <br/> |Cette erreur indique une erreur générale qui peut se produire lors de la tentative d’accès à une boîte aux lettres d’équipe. Essayez d’envoyer la demande ultérieurement. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorTimeIntervalTooBig  <br/> |Cette erreur indique que la période spécifiée est supérieure à la limite autorisée. Par défaut, la limite autorisée est 42.  <br/> |
|ErrorTimeoutExpired  <br/> | Cette erreur se produit lorsqu’il n’y a pas suffisamment de temps pour terminer le traitement de la demande.  <br/> |
|ErrorTimeZone  <br/> |Cette erreur indique qu’il existe une erreur de fuseau horaire.  <br/> |
|ErrorToFolderNotFound  <br/> |Cette erreur indique que le dossier de destination n’existe pas.  <br/> |
|ErrorTokenSerializationDenied  <br/> |Cette erreur se produit si l’appelant tente d’obtenir une demande de sérialisation de jeton, mais qu’il n’a pas le droit ms-Exch-PROXY-TokenSerialization sur le serveur d’accès au client.  <br/> |
|ErrorTooManyObjectsOpened  <br/> |Cette erreur se produit lorsque la limite interne sur les objets ouverts est dépassée.  <br/> |
|ErrorUnifiedMessagingDialPlanNotFound  <br/> |Cette erreur indique que le plan de numérotation d’un utilisateur n’est pas disponible.  <br/> |
|ErrorUnifiedMessagingReportDataNotFound  <br/> |Cette erreur est destinée à un usage interne uniquement. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorUnifiedMessagingPromptNotFound  <br/> |Cette erreur est destinée à un usage interne uniquement. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorUnifiedMessagingRequestFailed  <br/> |Cette erreur indique que l’utilisateur est in retrouve.  <br/> |
|ErrorUnifiedMessagingServerNotFound  <br/> |Cette erreur indique qu’un serveur valide pour le plan de numérotation est trouvé pour gérer la demande.  <br/> |
|ErrorUnableToGetUserOofSettings  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorUnableToRemoveImContactFromGroup  <br/> |Cette erreur se produit lorsqu’une tentative infructueuse de suppression d’un contact de messagerie instantanée d’un groupe est tentée. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorUnsupportedCulture  <br/> |Cette erreur se produit lorsque vous essayez de définir la propriété **Culture** sur une valeur qui n’est pas utilisable par la classe **System.Globalization.CultureInfo.**  <br/> |
|ErrorUnsupportedMapiPropertyType  <br/> |Cette erreur se produit lorsqu’un appelant tente d’utiliser des propriétés étendues de types objet, tableau d’objets, erreur ou null.  <br/> |
|ErrorUnsupportedMimeConversion  <br/> |Cette erreur se produit lorsque vous essayez de récupérer ou de définir le contenu MIME d’un élément autre qu’un objet [PostItem,](postitem.md) [Message](message-ex15websvcsotherref.md)ou [CalendarItem.](calendaritem.md)  <br/> |
|ErrorUnsupportedPathForQuery  <br/> |Cette erreur se produit lorsque l’appelant transmet une propriété non valide pour une requête. Cela peut se produire lorsque des propriétés calculées sont utilisées.  <br/> |
|ErrorUnsupportedPathForSortGroup  <br/> |Cette erreur se produit lorsque l’appelant transmet une propriété non valide pour un tri ou un groupe par propriété. Cela peut se produire lorsque des propriétés calculées sont utilisées.  <br/> |
|ErrorUnsupportedPropertyDefinition  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorUnsupportedQueryFilter  <br/> |Cette erreur indique que la restriction de dossier de recherche est peut-être valide, mais qu’elle n’est pas prise en charge par EWS.  <br/> |
|ErrorUnsupportedRecurrence  <br/> |Cette erreur indique que la récurrence spécifiée n’est pas prise en charge pour les tâches.  <br/> |
|ErrorUnsupportedSubFilter  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorUnsupportedTypeForConversion  <br/> |Cette erreur indique que les Exchange web ont trouvé un type de propriété dans la boutique, mais qu’ils ne peuvent pas générer de données XML pour le type de propriété.  <br/> |
|ErrorUpdateDelegatesFailed  <br/> |Cette erreur indique que la liste des délégués n’a pas pu être enregistrée après la mise à jour des délégués.  <br/> |
|ErrorUpdatePropertyMismatch  <br/> |Cette erreur se produit lorsque le chemin de propriété unique répertorié dans une description de modification ne correspond pas à la propriété unique définie dans l’objet [Item](item.md) ou [Folder](folder.md) réel.  <br/> |
|ErrorUserNotUnifiedMessagingEnabled  <br/> |Cette erreur indique que le demandeur n’est pas activé.  <br/> |
|ErrorUserNotAllowedByPolicy  <br/> |Cette erreur indique que le demandeur a tenté d’accorder des autorisations dans son dossier de calendrier ou de contacts à un utilisateur externe, mais que la stratégie de partage attribuée au demandeur indique que le domaine de l’utilisateur externe n’est pas répertorié dans la stratégie.  <br/> |
|ErrorUserWithoutFederatedProxyAddress  <br/> |Indique que l’organisation du demandeur dispose d’un ensemble de domaines fédérés, mais qu’elle n’a pas d’adresses proxy SMTP avec l’un des domaines fédérés.  <br/> |
|ErrorValueOutOfRange  <br/> |Cette erreur indique qu’une date de début ou de fin d’affichage Calendrier a été définie sur 1/1/0001 12:00:00 AM ou 31/12/9999 11:59:59 PM.  <br/> |
|ErrorVirusDetected  <br/> |Cette erreur indique que la Exchange a détecté un virus dans le message.  <br/> |
|ErrorVirusMessageDeleted  <br/> |Cette erreur indique que la Exchange a détecté un virus dans le message et l’a supprimé.  <br/> |
|ErrorVoiceMailNotImplemented  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorWebRequestInInvalidState  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorWin32InteropError  <br/> |Cette erreur indique qu’une défaillance interne s’est produite lors de la communication avec du code nonmanaté.  <br/> |
|ErrorWorkingHoursSaveFailed  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorWorkingHoursXmlMalformed  <br/> |Ce code de réponse n’est pas utilisé.  <br/> |
|ErrorWrongServerVersion  <br/> |Cette erreur indique qu’une demande peut uniquement être faite vers un serveur de la même version que le serveur de boîtes aux lettres.  <br/> |
|ErrorWrongServerVersionDelegate  <br/> |Cette erreur indique qu’une demande a été faite par un délégué dont la version du serveur est différente de celle du serveur de boîtes aux lettres du principal.  <br/> |
|ErrorMissingInformationSharingFolderId  <br/> |Ce code d’erreur n’est jamais renvoyé.  <br/> |
|ErrorDuplicateSOAPHeader  <br/> |Spécifie qu’il existe des en-têtes SOAP en double.  <br/> |
|ErrorSharingSynchronizationFailed  <br/> | Spécifie qu’une tentative de synchronisation d’un dossier de partage a échoué.<br/><br/> Ce code d’erreur DOIT être renvoyé dans les cas ci-après :<br/><br/>- L’abonnement pour un dossier de partage est in trouvé.  <br/>- Le dossier de partage est in trouvé.  <br/>- L’utilisateur d’annuaire correspondant est in trouvé.  <br/>- L’utilisateur n’existe plus.  <br/>- Le rendez-vous n’est pas valide.  <br/>- L’élément de contact n’est pas valide.  <br/>- Échec de communication avec le serveur distant.  <br/> |
|ErrorSharingNoExternalEwsAvailable  <br/> |Spécifie que la propriété d’URL externe n’a pas été définie dans la base de données Active Directory. Ce code d’erreur DOIT être renvoyé si la propriété d’URL externe n’a pas été définie dans la base de données Active Directory.  <br/> |
|ErrorFreeBusyDLLimitReached  <br/> |Spécifie que le nombre maximal de membres du groupe a été atteint pour obtenir des informations de libre/occupé pour une liste de distribution. Cette erreur DOIT être renvoyée lorsque le nombre maximal de membres du groupe a été atteint pour obtenir des informations de libre/occupé pour une liste de distribution.  <br/> |
|ErrorInvalidGetSharingFolderRequest  <br/> |Spécifie que les éléments DataType et ShareFolderId sont tous deux présents dans une demande. Ce code d’erreur DOIT être renvoyé si l’élément DataType et l’élément ShareFolderId sont tous deux présents dans une demande.  <br/> |
|ErrorNotAllowedExternalSharingByPolicy  <br/> |Spécifie que l’appelant a tenté d’accorder des autorisations dans son calendrier ou son dossier de contacts à un utilisateur d’une autre organisation et que la tentative a échoué. Ce code d’erreur DOIT être renvoyé lorsque la stratégie de partage est désactivée pour l’appelant ou lorsque la stratégie de partage attribuée à l’appelant désactive le partage pour le niveau demandé ou le type de dossier demandé.  <br/> |
|ErrorUserNotAllowedByPolicy  <br/> |Spécifie que le demandeur a tenté d’accorder des autorisations dans son dossier de calendrier ou de contacts à un utilisateur externe, mais que la stratégie de partage affectée au demandeur spécifie que le domaine de l’utilisateur externe n’est pas répertorié dans la stratégie.  <br/> |
|ErrorPermissionNotAllowedByPolicy  <br/> |Spécifie que le demandeur a tenté d’accorder des autorisations dans son calendrier ou son dossier de contacts à un utilisateur externe, mais que la stratégie de partage attribuée au demandeur spécifie que le niveau d’autorisation demandé est supérieur à ce que la stratégie de partage autorise.  <br/> |
|ErrorOrganizationNotFederated  <br/> |Spécifie que l’organisation du demandeur n’est pas fédérée de sorte que le demandeur ne peut pas créer de messages de partage à envoyer à un utilisateur externe ou ne peut pas accepter le partage de messages reçus d’un utilisateur externe. Ce code d’erreur DOIT être renvoyé si l’organisation du demandeur n’est pas fédérée.  <br/> |
|ErrorMailboxFailover  <br/> |Spécifie qu’une tentative d’accès à une boîte aux lettres a échoué car la boîte aux lettres est en cours de processus deover.  <br/> |
|ErrorInvalidExternalSharingInitiator  <br/> |Spécifie que l’expéditeur de l’invitation de partage n’a pas créé les métadonnées d’invitation de partage. Ce code d’erreur DOIT être renvoyé si l’expéditeur de l’invitation de partage n’a pas créé les métadonnées d’invitation de partage.  <br/> |
|ErrorMessageTrackingPermanentError  <br/> |Spécifie que le service de suivi des messages ne peut pas suivre le message.  <br/> |
|ErrorMessageTrackingTransientError  <br/> |Spécifie que le service de suivi des messages est en panne ou occupé. Ce code d’erreur spécifie une erreur passagère. Les clients peuvent réessayer de se connecter au serveur lorsque cette erreur est reçue.  <br/> |
|ErrorMessageTrackingNoSuchDomain  <br/> |Spécifie que le domaine donné est in trouver.  <br/> |
|ErrorUserWithoutFederatedProxyAddress  <br/> |Spécifie que l’organisation du demandeur possède un ensemble de domaines fédérés, mais que l’organisation du demandeur n’a pas d’adresses proxy SMTP avec l’un des domaines fédérés.  <br/> |
|ErrorInvalidOrganizationRelationshipForFreeBusy  <br/> |Spécifie qu’un appelant a demandé des informations de libre/occupé pour un utilisateur d’une autre organisation, mais que la relation organisationnelle n’est pas activée.  <br/> |
|ErrorInvalidFederatedOrganizationId  <br/> |Spécifie que les objets de fédération de l’organisation du demandeur ne sont pas correctement configurés.  <br/> |
|ErrorInvalidExternalSharingSubscriber  <br/> |Spécifie qu’un message de partage n’est pas destiné à l’appelant.  <br/> |
|ErrorInvalidSharingData  <br/> |Spécifie que les métadonnées de partage ne sont pas valides. Cela peut être dû à un XML non valide.  <br/> |
|ErrorInvalidSharingMessage  <br/> |Spécifie que le message de partage n’est pas valide. Cela peut être dû à une propriété manquante.  <br/> |
|ErrorNotSupportedSharingMessage  <br/> |Spécifie que le message de partage n’est pas pris en charge.  <br/> |
|ErrorApplyConversationActionFailed  <br/> |Cette erreur DOIT être renvoyée si une action ne peut pas être appliquée à un ou plusieurs éléments de la conversation.  <br/> |
|ErrorInboxRulesValidationError  <br/> |Cette erreur DOIT être renvoyée si une règle n’est pas validée.  <br/> |
|ErrorOutlookRuleBlobExists  <br/> |Cette erreur DOIT être renvoyée lorsqu’une tentative de gestion des règles de boîte de réception se produit après qu’un autre client a accédé aux règles de boîte de réception.  <br/> |
|ErrorRulesOverQuota  <br/> |Cette erreur DOIT être renvoyée lorsque le quota de règle d’un utilisateur est dépassé.  <br/> |
|ErrorNewEventStreamConnectionOpened  <br/> |Cette erreur DOIT être renvoyée à la première connexion d’abonnement si une deuxième connexion d’abonnement est ouverte.  <br/> |
|ErrorMissedNotificationEvents  <br/> |Cette erreur DOIT être renvoyée lorsque les notifications d’événement sont manquées.  <br/> |
|ErrorDuplicateLegacyDistinguishedName  <br/> |Cette erreur est renvoyée lorsqu’il existe des noms hérités dupliqués dans les services de domaine Active Directory (AD DS). Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorInvalidClientAccessTokenRequest  <br/> |Cette erreur indique qu’une demande d’obtenir un jeton d’accès client n’était pas valide. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorNoSpeechDetected  <br/> |Cette erreur est destinée à un usage interne uniquement. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorUMServerUnavailable  <br/> |Cette erreur est destinée à un usage interne uniquement. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorRecipientNotFound  <br/> |Cette erreur est destinée à un usage interne uniquement. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorRecognizerNotInstalled  <br/> |Cette erreur est destinée à un usage interne uniquement. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorSpeechGrammarError  <br/> |Cette erreur est destinée à un usage interne uniquement. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorInvalidManagementRoleHeader  <br/> |Cette erreur est renvoyée si [l’en-tête ManagementRole](managementrole.md) dans l’en-tête SOAP est incorrect. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorLocationServicesDisabled  <br/> |Cette erreur est destinée à un usage interne uniquement. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorLocationServicesRequestTimedOut  <br/> |Cette erreur est destinée à un usage interne uniquement. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorLocationServicesRequestFailed  <br/> |Cette erreur est destinée à un usage interne uniquement. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorLocationServicesInvalidRequest  <br/> |Cette erreur est destinée à un usage interne uniquement. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorWeatherServiceDisabled  <br/> |Cette erreur est destinée à un usage interne uniquement.  <br/> |
|ErrorMailboxScopeNotAllowedWithoutQueryString  <br/> |Cette erreur est renvoyée lorsqu’une tentative de recherche étendue est effectuée sans utiliser d’élément [QueryString (String)](querystring-string.md) pour une recherche d’indexation de contenu. Ceci s’applique aux **opérations SearchMailboxes et** **FindConversation.** Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorArchiveMailboxSearchFailed  <br/> |Cette erreur est renvoyée lorsqu’une recherche de boîte aux lettres d’archivage échoue. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorArchiveMailboxServiceDiscoveryFailed  <br/> |Cette erreur est renvoyée lorsque l’URL d’une boîte aux lettres d’archivage n’est pas découvrable. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorGetRemoteArchiveFolderFailed  <br/> |Cette erreur se produit en cas d’échec de l’opération d’accès au dossier de boîte aux lettres d’archivage à distance.  <br/> |
|ErrorFindRemoteArchiveFolderFailed  <br/> |Cette erreur se produit lorsque l’opération de recherche du dossier de boîte aux lettres d’archivage à distance a échoué.  <br/> |
|ErrorGetRemoteArchiveItemFailed  <br/> |Cette erreur se produit lorsque l’opération d’accès à l’élément de boîte aux lettres d’archivage à distance a échoué.  <br/> |
|ErrorExportRemoteArchiveItemsFailed  <br/> |Cette erreur se produit en cas d’échec de l’opération d’exportation des éléments de boîte aux lettres d’archivage à distance.  <br/> |
|ErrorInvalidPhotoSize  <br/> |Cette erreur est renvoyée si une taille de photo non valide est demandée au serveur. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorSearchQueryHasTooManyKeywords  <br/> |Cette erreur est renvoyée lorsqu’une taille de photo inattendue est demandée dans une **demande d’opération GetUserPhoto.** Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorSearchTooManyMailboxes  <br/> |Cette erreur est renvoyée lorsqu’une **demande d’opération SearchMailboxes** contient trop de boîtes aux lettres à rechercher. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorInvalidRetentionTagNone  <br/> |Cette erreur indique qu’aucune balise de rétention n’a été trouvée pour cet utilisateur. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorDiscoverySearchesDisabled  <br/> |Cette erreur est renvoyée lorsque les recherches de découverte sont désactivées sur un client ou un serveur. Cette erreur a été introduite dans Exchange 2013.  <br/> |
|ErrorCalendarSeekToConditionNotSupported  <br/> |Cette erreur se produit lorsque vous tentez d’appeler l’opération [FindItem](finditem-operation.md) avec [un objet SeekToConditionPageItemView](seektoconditionpageitemview.md) pour récupérer des éléments de calendrier, ce qui n’est pas pris en charge.  <br/> |
|ErrorCalendarIsGroupMailboxForAccept  <br/> |Cette erreur est destinée à un usage interne uniquement.  <br/> |
|ErrorCalendarIsGroupMailboxForDecline  <br/> |Cette erreur est destinée à un usage interne uniquement.  <br/> |
|ErrorCalendarIsGroupMailboxForTentative  <br/> |Cette erreur est destinée à un usage interne uniquement.  <br/> |
|ErrorCalendarIsGroupMailboxForSuppressReadReceipt  <br/> |Cette erreur est destinée à un usage interne uniquement.  <br/> |
|ErrorOrganizationAccessBlocked  <br/> |Le client est marqué pour suppression.  <br/> |
|ErrorInvalidLicense  <br/> |L’utilisateur n’a pas de licence valide.  <br/> |
|ErrorMessagePerFolderCountReceiveQuotaExceeded  <br/> |Le quota de réception du message par dossier a été dépassé.  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément n’est pas obligatoire et n’est pas inclus dans toutes les réponses. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

