---
title: ResponseMessages
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ResponseMessages
api_type:
- schema
ms.assetid: 2071bed8-ea66-4627-aa4f-a1d9a025cf3d
description: L’élément ResponseMessages contient les messages de réponse pour une demande Exchange services Web.
ms.openlocfilehash: 23fa25b29cec0377d83ecf56a094da86af6c5213
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516389"
---
# <a name="responsemessages"></a>ResponseMessages

**L’élément ResponseMessages** contient les messages de réponse pour une demande Exchange services Web. 
  
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
|[CopyFolderResponseMessage](copyfolderresponsemessage.md) <br/> |Contient l’état et le résultat d’une demande CopyFolder unique.  <br/> |
|[CopyItemResponseMessage](copyitemresponsemessage.md) <br/> |Contient l’état et le résultat d’une demande CopyItem unique.  <br/> |
|[CreateAttachmentResponseMessage](createattachmentresponsemessage.md) <br/> |Contient l’état et le résultat d’une demande CreateAttachment unique.  <br/> |
|[CreateFolderResponseMessage](createfolderresponsemessage.md) <br/> |Contient l’état et le résultat d’une demande CreateFolder unique.  <br/> |
|[CreateItemResponseMessage](createitemresponsemessage.md) <br/> |Contient l’état et le résultat d’une demande CreateItem unique.  <br/> |
|[CreateManagedFolderResponseMessage](createmanagedfolderresponsemessage.md) <br/> |Contient l’état et le résultat d’une demande CreateManagedFolder unique.  <br/> |
|[DeleteAttachmentResponseMessage](deleteattachmentresponsemessage.md) <br/> |Contient l’état et le résultat d’une demande DeleteAttachment unique.  <br/> |
|[DeleteFolderResponseMessage](deletefolderresponsemessage.md) <br/> |Contient l’état et le résultat d’une demande DeleteFolder unique.  <br/> |
|[DeleteItemResponseMessage](deleteitemresponsemessage.md) <br/> |Contient l’état et le résultat d’une demande DeleteItem unique.  <br/> |
|[EmptyFolderResponseMessage](emptyfolderresponsemessage.md) <br/> |Contient l’état et le résultat d’une [demande EmptyFolder](emptyfolder.md) unique.  <br/> |
|[ExpandDLResponseMessage](expanddlresponsemessage.md) <br/> |Contient l’état et le résultat d’une demande ExpandDL unique.  <br/> |
|[FindFolderResponseMessage](findfolderresponsemessage.md) <br/> |Contient l’état et le résultat d’une demande FindFolder unique.  <br/> |
|[FindItemResponseMessage](finditemresponsemessage.md) <br/> |Contient l’état et le résultat d’une demande FindItem unique.  <br/> |
|[GetAttachmentResponseMessage](getattachmentresponsemessage.md) <br/> |Contient l’état et le résultat d’une demande GetAttachment unique.  <br/> |
|[UploadItemsResponseMessage](uploaditemsresponsemessage.md) <br/> |Contient l’état et les résultats d’une seule demande UploadItems.  <br/> |
|[ExportItemsResponseMessage](exportitemsresponsemessage.md) <br/> |Contient l’état et les résultats d’une demande ExportItems unique.  <br/> |
|[GetEventsResponseMessage](geteventsresponsemessage.md) <br/> |Contient l’état et le résultat d’une demande GetEvents unique.  <br/> |
|[GetStreamingEventsResponseMessage](getstreamingeventsresponsemessage.md) <br/> |Contient l’état et le résultat d’une demande GetStreamingEvents unique.  <br/> |
|[GetFolderResponseMessage](getfolderresponsemessage.md) <br/> |Contient l’état et le résultat d’une demande GetFolder unique.  <br/> |
|[GetItemResponseMessage](getitemresponsemessage.md) <br/> |Contient l’état et le résultat d’une demande GetItem unique.  <br/> |
|[MoveFolderResponseMessage](movefolderresponsemessage.md) <br/> |Contient l’état et le résultat d’une demande MoveFolder unique.  <br/> |
|[MoveItemResponseMessage](moveitemresponsemessage.md) <br/> |Contient l’état et le résultat d’une demande MoveItem unique.  <br/> |
|[ResolveNamesResponseMessage](resolvenamesresponsemessage.md) <br/> |Contient l’état et le résultat d’une demande ResolveNames.  <br/> |
|[SendItemResponseMessage](senditemresponsemessage.md) <br/> |Contient l’état et le résultat d’une demande SendItem unique.  <br/> |
|[SendNotificationResponseMessage](sendnotificationresponsemessage.md) <br/> |Contient l’état et le résultat d’une demande SendNotification unique.  <br/> |
|[SubscribeResponseMessage](subscriberesponsemessage.md) <br/> |Contient l’état et le résultat d’une demande d’abonnement unique.  <br/> |
|[SyncFolderHierarchyResponseMessage](syncfolderhierarchyresponsemessage.md) <br/> |Contient l’état et le résultat d’une demande SyncFolderHierarchy.  <br/> |
|[SyncFolderItemsResponseMessage](syncfolderitemsresponsemessage.md) <br/> |Contient l’état et le résultat d’une demande SyncFolderItems.  <br/> |
|[UnsubscribeResponseMessage](unsubscriberesponsemessage.md) <br/> |Contient l’état et le résultat d’une demande de désabonnement unique.  <br/> |
|[UpdateFolderResponseMessage](updatefolderresponsemessage.md) <br/> |Contient l’état et le résultat d’une demande UpdateFolder unique.  <br/> |
|[UpdateItemResponseMessage](updateitemresponsemessage.md) <br/> |Contient l’état et le résultat d’une demande UpdateItem unique.  <br/> |
|[ConvertIdResponseMessage](convertidresponsemessage.md) <br/> |Contient l’état et le résultat d’une demande ConvertId.  <br/> |
|[GetSharingMetadataResponseMessage](getsharingmetadataresponsemessage.md) <br/> |Contient l’état et les résultats d’une demande GetSharingMetadata.  <br/> |
|[RefreshSharingFolderResponseMessage](refreshsharingfolderresponsemessage.md) <br/> |Contient l’état et les résultats d’une demande RefreshSharingFolder.  <br/> |
|[GetSharingFolderResponseMessage](getsharingfolderresponsemessage.md) <br/> |Contient l’état et les résultats d’une demande GetSharingFolder.  <br/> |
|[CreateUserConfigurationResponseMessage](createuserconfigurationresponsemessage.md) <br/> |Contient l’état et les résultats d’une demande CreateUserConfiguration.  <br/> |
|[DeleteUserConfigurationResponseMessage](deleteuserconfigurationresponsemessage.md) <br/> |Contient l’état et les résultats d’une demande DeleteUserConfiguration.  <br/> |
|[GetUserConfigurationResponseMessage](getuserconfigurationresponsemessage.md) <br/> |Contient l’état et les résultats d’une demande GetUserConfiguration.  <br/> |
|[UpdateUserConfigurationResponseMessage](updateuserconfigurationresponsemessage.md) <br/> |Contient l’état et les résultats d’une demande UpdateUserConfiguration.  <br/> |
|[GetRoomListsResponse](getroomlistsresponse.md) <br/> |Contient l’état et les résultats d’une demande GetRoomLists.  <br/> |
|[GetRoomsResponse](getroomsresponse.md) <br/> |Contient l’état et les résultats d’une demande GetRooms.  <br/> |
|[GetRemindersResponse](getremindersresponse.md) <br/> |Contient l’état et les résultats d’une demande GetReminders.  <br/> |
|[PerformReminderActionResponse](performreminderactionresponse.md) <br/> |Contient l’état et les résultats d’une demande PerformReminderAction.  <br/> |
|[GetServerTimeZonesResponseMessage](getservertimezonesresponsemessage.md) <br/> |Contient l’état et le résultat d’une demande GetServerTimeZones unique.  <br/> |
|[ApplyConversationActionResponseMessage](applyconversationactionresponsemessage.md) <br/> |Contient l’état et les résultats [d’une demande d’opération ApplyConversationAction.](applyconversationaction-operation.md)  <br/> |
   
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
|[DeleteItemResponse](deleteitemresponse.md) <br/> |Définit une réponse à une demande DeleteItem.  <br/> |
|[EmptyFolderResponse](emptyfolderresponse.md) <br/> |Définit une réponse à une demande EmptyFolder.  <br/> |
|[ExpandDLResponse](expanddlresponse.md) <br/> |Définit une réponse à une demande ExpandDL.  <br/> |
|[ExportItemsResponse](exportitemsresponse.md) <br/> |Représente la réponse à une seule demande ExportItems.  <br/> |
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
|[SubscribeResponse](subscriberesponse.md) <br/> |Définit une réponse à une demande d’abonnement.  <br/> |
|[SyncFolderHierarchyResponse](syncfolderhierarchyresponse.md) <br/> |Définit une réponse à une demande SyncFolderHierarchy.  <br/> |
|[SyncFolderItemsResponse](syncfolderitemsresponse.md) <br/> |Définit une réponse à une demande SyncFolderItems.  <br/> |
|[UnsubscribeResponse](unsubscriberesponse.md) <br/> |Définit une réponse à une demande de désabonnement.  <br/> |
|[UpdateFolderResponse](updatefolderresponse.md) <br/> |Définit une réponse à une demande UpdateFolder.  <br/> |
|[UpdateItemResponse](updateitemresponse.md) <br/> |Définit une réponse à une demande UpdateItem.  <br/> |
|[ConvertIdResponse](convertidresponse.md) <br/> |Contient une réponse à une demande ConvertId.  <br/> |
|[GetServerTimeZonesResponse](getservertimezonesresponse.md) <br/> |Définit une réponse à une demande GetServerTimeZones.  <br/> |
|[CreateUserConfigurationResponse](createuserconfigurationresponse.md) <br/> |Définit une réponse à une demande CreateUserConfiuration.  <br/> |
|[DeleteUserConfigurationResponse](deleteuserconfigurationresponse.md) <br/> |Définit une réponse à une demande DeleteUserConfiguration.  <br/> |
|[GetUserConfigurationResponse](getuserconfigurationresponse.md) <br/> |Définit une réponse à une demande GetUserConfiguration.  <br/> |
|[UpdateUserConfigurationResponse](updateuserconfigurationresponse.md) <br/> |Définit une réponse à une demande UpdateUserConfiguration.  <br/> |
|[ApplyConversationActionResponse](applyconversationactionresponse.md) <br/> |Définit une réponse à une [demande d’opération ApplyConversationAction.](applyconversationaction-operation.md)  <br/> |
|[GetPasswordExpirationDateResponse](getpasswordexpirationdateresponse.md) <br/> |Définit une réponse à une demande d’opération [GetPasswordExpirationDate.](getpasswordexpirationdate-operation.md)  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération ExportItems](exportitems-operation.md) 
- [Opération UploadItems](uploaditems-operation.md)
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

