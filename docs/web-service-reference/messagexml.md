---
title: MessageXml
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MessageXml
api_type:
- schema
ms.assetid: bcaf9e35-d351-48f3-baad-f90c633cba8a
description: L’élément MessageXml fournit des informations de réponse d’erreur supplémentaires.
ms.openlocfilehash: 8b6d201fe35c99a65f920ed7f60c33a2271fbd2e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828470"
---
# <a name="messagexml"></a>MessageXml

L’élément **MessageXml** fournit des informations de réponse d’erreur supplémentaires. 
  
- [ResponseMessage](responsemessage.md)  
- [MessageXml](messagexml.md)
  
```XML
<MessageXml/>
```

 **xs : tout**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ResponseMessage](responsemessage.md) <br/> | Fournit des informations descriptives concernant l’état de réponse. <br/> <br/>  Voici quelques-unes des expressions XPath possibles pour cet élément : <br/> <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/ResponseMessage` <br/> <br/> `/GetUserAvailabilityResponse/SuggestionsResponse/ResponseMessage` <br/><br/>  `/SetUserOofSettingsResponse/ResponseMessage` <br/><br/>  `/GetUserOofSettingsResponse/ResponseMessage` <br/> |
|[DeleteItemResponseMessage](deleteitemresponsemessage.md) <br/> |Contient l’état et les résultats d’une seule demande DeleteItem.  <br/> |
|[SendItemResponseMessage](senditemresponsemessage.md) <br/> |Contient l’état et les résultats d’une seule demande SendItem.  <br/> |
|[DeleteFolderResponseMessage](deletefolderresponsemessage.md) <br/> |Contient l’état et les résultats d’une seule demande DeleteFolder.  <br/> |
|[DeleteAttachmentResponseMessage](deleteattachmentresponsemessage.md) <br/> |Contient l’état et les résultats d’une seule demande DeleteAttachment.  <br/> |
|[UnsubscribeResponseMessage](unsubscriberesponsemessage.md) <br/> |Contient l’état et les résultats d’une demande de désabonnement unique.  <br/> |
|[CreateFolderResponseMessage](createfolderresponsemessage.md) <br/> |Contient l’état et les résultats d’une seule demande CreateFolder.  <br/> |
|[GetFolderResponseMessage](getfolderresponsemessage.md) <br/> |Contient l’état et les résultats d’une seule demande GetFolder.  <br/> |
|[UpdateFolderResponseMessage](updatefolderresponsemessage.md) <br/> |Contient l’état et les résultats d’une seule demande UpdateFolder.  <br/> |
|[MoveFolderResponseMessage](movefolderresponsemessage.md) <br/> |Contient l’état et les résultats d’une seule demande MoveFolder.  <br/> |
|[CopyFolderResponseMessage](copyfolderresponsemessage.md) <br/> |Contient l’état et les résultats d’une seule demande CopyFolder.  <br/> |
|[CreateManagedFolderResponseMessage](createmanagedfolderresponsemessage.md) <br/> |Contient l’état et les résultats d’une seule demande CreateManagedFolder.  <br/> |
|[FindFolderResponseMessage](findfolderresponsemessage.md) <br/> |Contient l’état et les résultats d’une seule demande FindFolder.  <br/> |
|[CreateItemResponseMessage](createitemresponsemessage.md) <br/> |Contient l’état et les résultats d’une demande CreateItem unique.  <br/> |
|[GetItemResponseMessage](getitemresponsemessage.md) <br/> |Contient l’état et les résultats d’une demande de GetItem unique.  <br/> |
|[UpdateItemResponseMessage](updateitemresponsemessage.md) <br/> |Contient l’état et les résultats d’une seule demande UpdateItem.  <br/> |
|[MoveItemResponseMessage](moveitemresponsemessage.md) <br/> |Contient l’état et les résultats d’une seule demande MoveItem.  <br/> |
|[CopyItemResponseMessage](copyitemresponsemessage.md) <br/> |Contient l’état et les résultats d’une seule demande CopyItem.  <br/> |
|[CreateAttachmentResponseMessage](createattachmentresponsemessage.md) <br/> |Contient l’état et les résultats d’une seule demande CreateAttachment.  <br/> |
|[GetAttachmentResponseMessage](getattachmentresponsemessage.md) <br/> |Contient l’état et les résultats d’une seule demande GetAttachment.  <br/> |
|[FindItemResponseMessage](finditemresponsemessage.md) <br/> |Contient l’état et les résultats d’une seule demande FindItem.  <br/> |
|[ResolveNamesResponseMessage](resolvenamesresponsemessage.md) <br/> |Contient l’état et les résultats d’une demande ResolveNames.  <br/> |
|[ExpandDLResponseMessage](expanddlresponsemessage.md) <br/> |Contient l’état et les résultats d’une seule demande ExpandDL.  <br/> |
|[SubscribeResponseMessage](subscriberesponsemessage.md) <br/> |Contient l’état et les résultats d’une seule demande Subscribe.  <br/> |
|[GetEventsResponseMessage](geteventsresponsemessage.md) <br/> |Contient l’état et les résultats d’une seule demande GetEvents.  <br/> |
|[SendNotificationResponseMessage](sendnotificationresponsemessage.md) <br/> |Contient l’état et les résultats d’une requête SendNotification.  <br/> |
|[SyncFolderHierarchyResponseMessage](syncfolderhierarchyresponsemessage.md) <br/> |Contient l’état et les résultats d’une demande SyncFolderHierarchy.  <br/> |
|[SyncFolderItemsResponseMessage](syncfolderitemsresponsemessage.md) <br/> |Contient l’état et les résultats d’une demande SyncFolderItems.  <br/> |
|[ConvertIdResponseMessage](convertidresponsemessage.md) <br/> |Contient l’état et les résultats d’une demande ConvertId.  <br/> |
|[AddDelegateResponse](adddelegateresponse.md) <br/> |Contient l’état et les résultats d’une requête AddDelegate.  <br/> |
|[GetServerTimeZonesResponseMessage](getservertimezonesresponsemessage.md) <br/> |Contient l’état et les résultats d’une demande GetServerTimeZones.  <br/> |
|[GetSharingFolderResponseMessage](getsharingfolderresponsemessage.md) <br/> |Contient l’état et les résultats d’une demande GetSharingFolder.  <br/> |
|[GetSharingFolderResponse](getsharingfolderresponse.md) <br/> |Définit une réponse à une demande de GetSharingFolder.  <br/> |
|[GetSharingMetadataResponseMessage](getsharingmetadataresponsemessage.md) <br/> |Contient l’état et les résultats d’une demande GetSharingMetadata.  <br/> |
|[GetSharingMetadataResponse](getsharingmetadataresponse.md) <br/> |Définit une réponse à une demande de GetSharingMetadata.  <br/> |
|[RefreshSharingFolderResponseMessage](refreshsharingfolderresponsemessage.md) <br/> |Contient l’état et les résultats d’une demande RefreshSharingFolder.  <br/> |
|[RefreshSharingFolderResponse](refreshsharingfolderresponse.md) <br/> |Définit une réponse à une demande de RefreshSharingFolder.  <br/> |
|[FindConversationResponse](findconversationresponse.md) <br/> |Contient l’état et les résultats d’une réponse **FindConversation** .  <br/> |
|[EmptyFolderResponseMessage](emptyfolderresponsemessage.md) <br/> |Contient l’état et le résultat d’une demande **EmptyFolder** .  <br/> |
|[UpdateInboxRulesResponse](updateinboxrulesresponse.md) <br/> |Contient un état et les résultats d’une requête **UpdateInboxRules** .  <br/> |
|[UploadItemsResponseMessage](uploaditemsresponsemessage.md) <br/> |Contient un état et les résultats d’une requête **UploadItemsResponse** .  <br/> |
|[GetInboxRulesResponse](getinboxrulesresponse.md) <br/> |Contient une réponse à une demande de **GetInboxRules** .  <br/> |
|[GetServiceConfigurationResponse](getserviceconfigurationresponse.md) <br/> |Contient une réponse à une demande de **GetServiceConfiguration** .  <br/> |
|[ServiceConfigurationResponseMessageType](serviceconfigurationresponsemessagetype.md) <br/> |Contient les paramètres de configuration de service.  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément n’est pas obligatoire et n’est pas inclus dans toutes les réponses. Il est inclus pour les messages d’erreur. Dans les requêtes qui impliquent des dossiers ou des éléments, l’élément **MessageXML** contient un ou plusieurs éléments qui contiennent les URI pour les propriétés qui a provoqué l’erreur. Un exemple est l’élément [FieldURI](fielduri.md) . 
  
L’élément **MessageXML** est de type **xs : tout**, ce qui signifie que n’importe quel code XML bien formé est contenu valide pour cet élément.
  
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

