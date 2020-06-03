---
title: ResponseMessages
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResponseMessages
api_type:
- schema
ms.assetid: 2071bed8-ea66-4627-aa4f-a1d9a025cf3d
description: L’élément ResponseMessages contient les messages de réponse pour une demande des services Web Exchange.
ms.openlocfilehash: 93d83fbba3ea4bfe33f574eea7991157a4f10b88
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465400"
---
# <a name="responsemessages"></a>ResponseMessages

L’élément **ResponseMessages** contient les messages de réponse pour une demande des services Web Exchange. 
  
```XML
<ResponseMessages>
   <CreateItemResponseMessage/>
</ResponseMessages>
```

```xml
<ResponseMessages>
   <DeleteItemResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <GetItemResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <UpdateItemResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <SendItemResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <DeleteFolderResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <EmptyFolderResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <CreateFolderResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <GetFolderResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <FindFolderResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <UpdateFolderResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <MoveFolderResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <CopyFolderResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <CreateAttachmentResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <DeleteAttachmentResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <GetAttachmentResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <UploadItemsResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <ExportItemsResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <FindItemResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <MoveItemResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <CopyItemResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <ResolveNamesResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <ExpandDLResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <GetServerTimeZonesResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <GetEventsResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <GetStreamingEventsResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <SubscribeResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <UnsubscribeResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <SendNotificationResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <SyncFolderHierarchyResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <SyncFolderItemsResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <CreateManagedFolderResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <ConvertIdResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <GetSharingMetadataResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <RefreshSharingFolderResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <GetSharingFolderResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <CreateUserConfigurationResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <DeleteUserConfigurationResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <GetUserConfigurationResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <UpdateUserConfigurationResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <GetRoomListsResponse/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <GetRoomsResponse/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <GetRemindersResponse/>
</ResponseMessages
```

```xml 
<ResponseMessages>
   <PerformReminderActionResponse/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <ApplyConversationActionResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <GetPasswordExpirationDateResponse />
</ResponseMessages>
```


**ArrayOfResponseMessagesType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[CopyFolderResponseMessage](copyfolderresponsemessage.md) <br/> |Contient l’État et le résultat d’une seule demande CopyFolder.  <br/> |
|[CopyItemResponseMessage](copyitemresponsemessage.md) <br/> |Contient l’État et le résultat d’une demande CopyItem unique.  <br/> |
|[CreateAttachmentResponseMessage](createattachmentresponsemessage.md) <br/> |Contient l’État et le résultat d’une seule demande CreateAttachment.  <br/> |
|[CreateFolderResponseMessage](createfolderresponsemessage.md) <br/> |Contient l’État et le résultat d’une seule demande CreateFolder.  <br/> |
|[CreateItemResponseMessage](createitemresponsemessage.md) <br/> |Contient l’État et le résultat d’une seule demande CreateItem.  <br/> |
|[CreateManagedFolderResponseMessage](createmanagedfolderresponsemessage.md) <br/> |Contient l’État et le résultat d’une seule demande CreateManagedFolder.  <br/> |
|[DeleteAttachmentResponseMessage](deleteattachmentresponsemessage.md) <br/> |Contient l’État et le résultat d’une seule demande DeleteAttachment.  <br/> |
|[DeleteFolderResponseMessage](deletefolderresponsemessage.md) <br/> |Contient l’État et le résultat d’une seule demande DeleteFolder.  <br/> |
|[DeleteItemResponseMessage](deleteitemresponsemessage.md) <br/> |Contient l’État et le résultat d’une seule demande DeleteItem.  <br/> |
|[EmptyFolderResponseMessage](emptyfolderresponsemessage.md) <br/> |Contient l’État et le résultat d’une seule demande [EmptyFolder](emptyfolder.md) .  <br/> |
|[ExpandDLResponseMessage](expanddlresponsemessage.md) <br/> |Contient l’État et le résultat d’une seule demande ExpandDL.  <br/> |
|[FindFolderResponseMessage](findfolderresponsemessage.md) <br/> |Contient l’État et le résultat d’une seule demande FindFolder.  <br/> |
|[FindItemResponseMessage](finditemresponsemessage.md) <br/> |Contient l’État et le résultat d’une seule demande FindItem.  <br/> |
|[GetAttachmentResponseMessage](getattachmentresponsemessage.md) <br/> |Contient l’État et le résultat d’une seule demande GetAttachment.  <br/> |
|[UploadItemsResponseMessage](uploaditemsresponsemessage.md) <br/> |Contient l’État et les résultats d’une seule demande UploadItems.  <br/> |
|[ExportItemsResponseMessage](exportitemsresponsemessage.md) <br/> |Contient l’État et les résultats d’une seule demande ExportItems.  <br/> |
|[GetEventsResponseMessage](geteventsresponsemessage.md) <br/> |Contient l’État et le résultat d’une demande GetEvents unique.  <br/> |
|[GetStreamingEventsResponseMessage](getstreamingeventsresponsemessage.md) <br/> |Contient l’État et le résultat d’une seule demande GetStreamingEvents.  <br/> |
|[GetFolderResponseMessage](getfolderresponsemessage.md) <br/> |Contient l’État et le résultat d’une demande GetFolder unique.  <br/> |
|[GetItemResponseMessage](getitemresponsemessage.md) <br/> |Contient l’État et le résultat d’une seule demande GetItem.  <br/> |
|[MoveFolderResponseMessage](movefolderresponsemessage.md) <br/> |Contient l’État et le résultat d’une seule demande MoveFolder.  <br/> |
|[MoveItemResponseMessage](moveitemresponsemessage.md) <br/> |Contient l’État et le résultat d’une seule demande MoveItem.  <br/> |
|[ResolveNamesResponseMessage](resolvenamesresponsemessage.md) <br/> |Contient l’État et le résultat d’une demande ResolveNames.  <br/> |
|[SendItemResponseMessage](senditemresponsemessage.md) <br/> |Contient l’État et le résultat d’une seule demande SendItem.  <br/> |
|[SendNotificationResponseMessage](sendnotificationresponsemessage.md) <br/> |Contient l’État et le résultat d’une seule demande SendNotification.  <br/> |
|[SubscribeResponseMessage](subscriberesponsemessage.md) <br/> |Contient l’État et le résultat d’une demande d’abonnement unique.  <br/> |
|[SyncFolderHierarchyResponseMessage](syncfolderhierarchyresponsemessage.md) <br/> |Contient l’État et le résultat d’une demande Opérationsyncfolderhierarchy.  <br/> |
|[SyncFolderItemsResponseMessage](syncfolderitemsresponsemessage.md) <br/> |Contient l’État et le résultat d’une demande SyncFolderItems.  <br/> |
|[UnsubscribeResponseMessage](unsubscriberesponsemessage.md) <br/> |Contient l’État et le résultat d’une demande d’annulation d’abonnement unique.  <br/> |
|[UpdateFolderResponseMessage](updatefolderresponsemessage.md) <br/> |Contient l’État et le résultat d’une seule demande UpdateFolder.  <br/> |
|[UpdateItemResponseMessage](updateitemresponsemessage.md) <br/> |Contient l’État et le résultat d’une seule demande UpdateItem.  <br/> |
|[ConvertIdResponseMessage](convertidresponsemessage.md) <br/> |Contient l’État et le résultat d’une demande ConvertId.  <br/> |
|[GetSharingMetadataResponseMessage](getsharingmetadataresponsemessage.md) <br/> |Contient l’État et les résultats d’une demande GetSharingMetadata.  <br/> |
|[RefreshSharingFolderResponseMessage](refreshsharingfolderresponsemessage.md) <br/> |Contient l’État et les résultats d’une demande RefreshSharingFolder.  <br/> |
|[GetSharingFolderResponseMessage](getsharingfolderresponsemessage.md) <br/> |Contient l’État et les résultats d’une demande GetSharingFolder.  <br/> |
|[CreateUserConfigurationResponseMessage](createuserconfigurationresponsemessage.md) <br/> |Contient l’État et les résultats d’une demande CreateUserConfiguration.  <br/> |
|[DeleteUserConfigurationResponseMessage](deleteuserconfigurationresponsemessage.md) <br/> |Contient l’État et les résultats d’une demande DeleteUserConfiguration.  <br/> |
|[GetUserConfigurationResponseMessage](getuserconfigurationresponsemessage.md) <br/> |Contient l’État et les résultats d’une demande GetUserConfiguration.  <br/> |
|[UpdateUserConfigurationResponseMessage](updateuserconfigurationresponsemessage.md) <br/> |Contient l’État et les résultats d’une demande UpdateUserConfiguration.  <br/> |
|[GetRoomListsResponse](getroomlistsresponse.md) <br/> |Contient l’État et les résultats d’une demande GetRoomLists.  <br/> |
|[GetRoomsResponse](getroomsresponse.md) <br/> |Contient l’État et les résultats d’une demande GetRooms.  <br/> |
|[GetRemindersResponse](getremindersresponse.md) <br/> |Contient l’État et les résultats d’une demande GetReminders.  <br/> |
|[PerformReminderActionResponse](performreminderactionresponse.md) <br/> |Contient l’État et les résultats d’une demande PerformReminderAction.  <br/> |
|[GetServerTimeZonesResponseMessage](getservertimezonesresponsemessage.md) <br/> |Contient l’État et le résultat d’une seule demande GetServerTimeZones.  <br/> |
|[ApplyConversationActionResponseMessage](applyconversationactionresponsemessage.md) <br/> |Contient l’État et les résultats d’une demande d' [opération ApplyConversationAction](applyconversationaction-operation.md) .  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[CopyFolderResponse](copyfolderresponse.md) <br/> |Définit une réponse à une demande CopyFolder.  <br/> |
|[CopyItemResponse](copyitemresponse.md) <br/> |Définit une réponse à une demande CopyItem.  <br/> |
|[CreateAttachmentResponse](createattachmentresponse.md) <br/> |Définit une réponse à une demande CreateAttachment.  <br/> |
|[CreateFolderResponse](createfolderresponse.md) <br/> |Définit une réponse à une demande CreateFolder.  <br/> |
|[CreateItemResponse](createitemresponse.md) <br/> |Définit une réponse à une demande CreateItem.  <br/> |
|[CreateManagedFolderResponse](createmanagedfolderresponse.md) <br/> |Définit une réponse à une demande CreateManagedFolder.  <br/> |
|[DeleteAttachmentResponse](deleteattachmentresponse.md) <br/> |Définit une réponse à une demande DeleteAttachment.  <br/> |
|[DeleteFolderResponse](deletefolderresponse.md) <br/> |Définit une réponse à une demande DeleteFolder.  <br/> |
|[Updateitemresponse](deleteitemresponse.md) <br/> |Définit une réponse à une demande DeleteItem.  <br/> |
|[EmptyFolderResponse](emptyfolderresponse.md) <br/> |Définit une réponse à une demande EmptyFolder.  <br/> |
|[ExpandDLResponse](expanddlresponse.md) <br/> |Définit une réponse à une demande ExpandDL.  <br/> |
|[ExportItemsResponse](exportitemsresponse.md) <br/> |Représente la réponse à une requête ExportItems unique.  <br/> |
|[FindFolderResponse](findfolderresponse.md) <br/> |Définit une réponse à une demande FindFolder.  <br/> |
|[FindItemResponse](finditemresponse.md) <br/> |Définit une réponse à une demande FindItem.  <br/> |
|[GetAttachmentResponse](getattachmentresponse.md) <br/> |Définit une réponse à une demande GetAttachment.  <br/> |
|[GetEventsResponse](geteventsresponse.md) <br/> |Définit une réponse à une demande GetEvents.  <br/> |
|[GetStreamingEventsResponse](getstreamingeventsresponse.md) <br/> |Définit une réponse à une demande GetStreamingEvents.  <br/> |
|[GetFolderResponse](getfolderresponse.md) <br/> |Définit une réponse à une demande GetFolder.  <br/> |
|[GetItemResponse](getitemresponse.md) <br/> |Définit une réponse à une demande GetItem.  <br/> |
|[MoveFolderResponse](movefolderresponse.md) <br/> |Définit une réponse à une demande MoveFolder.  <br/> |
|[MoveItemResponse](moveitemresponse.md) <br/> |Définit une réponse à une demande MoveItem.  <br/> |
|[ResolveNamesResponse](resolvenamesresponse.md) <br/> |Définit une réponse à une demande ResolveNames.  <br/> |
|[SendItemResponse](senditemresponse.md) <br/> |Définit une réponse à une demande SendItem.  <br/> |
|[SendNotificationResult](sendnotificationresult.md) <br/> |Définit une réponse à une demande SendNotification.  <br/> |
|[SubscribeResponse](subscriberesponse.md) <br/> |Définit une réponse à une demande subscribe.  <br/> |
|[SyncFolderHierarchyResponse](syncfolderhierarchyresponse.md) <br/> |Définit une réponse à une demande Opérationsyncfolderhierarchy.  <br/> |
|[SyncFolderItemsResponse](syncfolderitemsresponse.md) <br/> |Définit une réponse à une demande SyncFolderItems.  <br/> |
|[UnsubscribeResponse](unsubscriberesponse.md) <br/> |Définit une réponse à une demande d’annulation d’abonnement.  <br/> |
|[UpdateFolderResponse](updatefolderresponse.md) <br/> |Définit une réponse à une demande UpdateFolder.  <br/> |
|[UpdateItemResponse](updateitemresponse.md) <br/> |Définit une réponse à une demande UpdateItem.  <br/> |
|[ConvertIdResponse](convertidresponse.md) <br/> |Contient une réponse à une demande ConvertId.  <br/> |
|[GetServerTimeZonesResponse](getservertimezonesresponse.md) <br/> |Définit une réponse à une demande GetServerTimeZones.  <br/> |
|[CreateUserConfigurationResponse](createuserconfigurationresponse.md) <br/> |Définit une réponse à une demande CreateUserConfiuration.  <br/> |
|[DeleteUserConfigurationResponse](deleteuserconfigurationresponse.md) <br/> |Définit une réponse à une demande DeleteUserConfiguration.  <br/> |
|[GetUserConfigurationResponse](getuserconfigurationresponse.md) <br/> |Définit une réponse à une demande GetUserConfiguration.  <br/> |
|[UpdateUserConfigurationResponse](updateuserconfigurationresponse.md) <br/> |Définit une réponse à une demande UpdateUserConfiguration.  <br/> |
|[ApplyConversationActionResponse](applyconversationactionresponse.md) <br/> |Définit une réponse à une demande d' [opération ApplyConversationAction](applyconversationaction-operation.md) .  <br/> |
|[GetPasswordExpirationDateResponse](getpasswordexpirationdateresponse.md) <br/> |Définit une réponse à une demande d’opération d' [opération GetPasswordExpirationDate](getpasswordexpirationdate-operation.md) .  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération ExportItems](exportitems-operation.md) 
- [Opération UploadItems](uploaditems-operation.md)
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

