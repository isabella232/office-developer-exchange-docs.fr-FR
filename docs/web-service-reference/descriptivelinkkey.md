---
title: DescriptiveLinkKey
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DescriptiveLinkKey
api_type:
- schema
ms.assetid: f7f36749-00f3-4915-b17c-e3caa0af6e67
description: L’élément DescriptiveLinkKey est actuellement inutilisé et est réservé à une utilisation ultérieure. Il contient la valeur 0.
ms.openlocfilehash: fe646275bae3c533ee68d5137b019ea7a715c762
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59519806"
---
# <a name="descriptivelinkkey"></a>DescriptiveLinkKey

**L’élément DescriptiveLinkKey** est actuellement inutilisé et est réservé à une utilisation ultérieure. Il contient la valeur 0. 
  
```XML
<DescriptiveLinkKey/>
```

 **int**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ResponseMessage](responsemessage.md) <br/> | Fournit des informations descriptives sur l’état de la réponse.  <br/><br/>Voici quelques expressions XPath possibles pour cet élément :<br/><br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/ResponseMessage` <br/><br/>`/GetUserAvailabilityResponse/SuggestionsResponse/ResponseMessage` <br/><br/>`/SetUserOofSettingsResponse/ResponseMessage` <br/><br/>`/GetUserOofSettingsResponse/ResponseMessage` <br/> |
|[DeleteItemResponseMessage](deleteitemresponsemessage.md) <br/> |Contient l’état et le résultat d’une demande **DeleteItem** unique.  <br/> |
|[SendItemResponseMessage](senditemresponsemessage.md) <br/> |Contient l’état et le résultat d’une demande **SendItem** unique.  <br/> |
|[DeleteFolderResponseMessage](deletefolderresponsemessage.md) <br/> |Contient l’état et le résultat d’une demande **DeleteFolder** unique.  <br/> |
|[DeleteAttachmentResponseMessage](deleteattachmentresponsemessage.md) <br/> |Contient l’état et le résultat d’une demande **DeleteAttachment** unique.  <br/> |
|[UnsubscribeResponseMessage](unsubscriberesponsemessage.md) <br/> |Contient l’état et le résultat d’une demande **de désabonnement** unique.  <br/> |
|[CreateFolderResponseMessage](createfolderresponsemessage.md) <br/> |Contient l’état et le résultat d’une **demande CreateFolder** unique.  <br/> |
|[GetFolderResponseMessage](getfolderresponsemessage.md) <br/> |Contient l’état et le résultat d’une **demande GetFolder** unique.  <br/> |
|[UpdateFolderResponseMessage](updatefolderresponsemessage.md) <br/> |Contient l’état et le résultat d’une demande **UpdateFolder** unique.  <br/> |
|[MoveFolderResponseMessage](movefolderresponsemessage.md) <br/> |Contient l’état et le résultat d’une **demande MoveFolder** unique.  <br/> |
|[CopyFolderResponseMessage](copyfolderresponsemessage.md) <br/> |Contient l’état et le résultat d’une **demande CopyFolder** unique.  <br/> |
|[CreateManagedFolderResponseMessage](createmanagedfolderresponsemessage.md) <br/> |Contient l’état et le résultat d’une **demande CreateManagedFolder** unique.  <br/> |
|[FindFolderResponseMessage](findfolderresponsemessage.md) <br/> |Contient l’état et le résultat d’une **demande FindFolder** unique.  <br/> |
|[CreateItemResponseMessage](createitemresponsemessage.md) <br/> |Contient l’état et le résultat d’une **demande CreateItem** unique.  <br/> |
|[GetItemResponseMessage](getitemresponsemessage.md) <br/> |Contient l’état et le résultat d’une **demande GetItem** unique.  <br/> |
|[UpdateItemResponseMessage](updateitemresponsemessage.md) <br/> |Contient l’état et le résultat d’une demande **UpdateItem** unique.  <br/> |
|[MoveItemResponseMessage](moveitemresponsemessage.md) <br/> |Contient l’état et le résultat d’une **demande MoveItem** unique.  <br/> |
|[CopyItemResponseMessage](copyitemresponsemessage.md) <br/> |Contient l’état et le résultat d’une **demande CopyItem** unique.  <br/> |
|[CreateAttachmentResponseMessage](createattachmentresponsemessage.md) <br/> |Contient l’état et le résultat d’une **demande CreateAttachment** unique.  <br/> |
|[GetAttachmentResponseMessage](getattachmentresponsemessage.md) <br/> |Contient l’état et le résultat d’une **demande GetAttachment** unique.  <br/> |
|[FindItemResponseMessage](finditemresponsemessage.md) <br/> |Contient l’état et le résultat d’une demande **FindItem** unique.  <br/> |
|[ResolveNamesResponseMessage](resolvenamesresponsemessage.md) <br/> |Contient l’état et le résultat **d’une demande ResolveNames.**  <br/> |
|[ExpandDLResponseMessage](expanddlresponsemessage.md) <br/> |Contient l’état et le résultat d’une **demande ExpandDL** unique.  <br/> |
|[SubscribeResponseMessage](subscriberesponsemessage.md) <br/> |Contient l’état et le résultat d’une demande **d’abonnement** unique.  <br/> |
|[GetEventsResponseMessage](geteventsresponsemessage.md) <br/> |Contient l’état et le résultat d’une **demande GetEvents** unique.  <br/> |
|[SendNotificationResponseMessage](sendnotificationresponsemessage.md) <br/> |Contient l’état et le résultat d’une demande **SendNotification** unique.  <br/> |
|[SyncFolderHierarchyResponseMessage](syncfolderhierarchyresponsemessage.md) <br/> |Contient l’état et le résultat **d’une demande SyncFolderHierarchy.**  <br/> |
|[SyncFolderItemsResponseMessage](syncfolderitemsresponsemessage.md) <br/> |Contient l’état et le résultat **d’une demande SyncFolderItems.**  <br/> |
|[ConvertIdResponseMessage](convertidresponsemessage.md) <br/> |Contient l’état et le résultat **d’une demande ConvertId.**  <br/> |
|[AddDelegateResponse](adddelegateresponse.md) <br/> |Contient l’état et le résultat **d’une demande AddDelegate.**  <br/> |
|[GetServerTimeZonesResponseMessage](getservertimezonesresponsemessage.md) <br/> |Contient l’état et le résultat **d’une demande GetServerTimeZones.**  <br/> |
|[GetSharingFolderResponseMessage](getsharingfolderresponsemessage.md) <br/> |Contient l’état et le résultat **d’une demande GetSharingFolder.**  <br/> |
|[GetSharingFolderResponse](getsharingfolderresponse.md) <br/> |Définit une réponse à une **demande GetSharingFolder.**  <br/> |
|[GetSharingMetadataResponseMessage](getsharingmetadataresponsemessage.md) <br/> |Contient l’état et le résultat **d’une demande GetSharingMetadata.**  <br/> |
|[GetSharingMetadataResponse](getsharingmetadataresponse.md) <br/> |Définit une réponse à une **demande GetSharingMetadata.**  <br/> |
|[RefreshSharingFolderResponseMessage](refreshsharingfolderresponsemessage.md) <br/> |Contient l’état et le résultat **d’une demande RefreshSharingFolder.**  <br/> |
|[RefreshSharingFolderResponse](refreshsharingfolderresponse.md) <br/> |Définit une réponse à **une demande RefreshSharingFolder.**  <br/> |
|[FindConversationResponse](findconversationresponse.md) <br/> |Contient l’état et les résultats **d’une réponse FindConversation.**  <br/> |
|[EmptyFolderResponseMessage](emptyfolderresponsemessage.md) <br/> |Contient l’état et le résultat d’une **demande EmptyFolder** unique.  <br/> |
|[UpdateInboxRulesResponse](updateinboxrulesresponse.md) <br/> |Contient l’état et le résultat **d’une demande UpdateInboxRules.**  <br/> |
|[UploadItemsResponseMessage](uploaditemsresponsemessage.md) <br/> |Contient un état et le résultat **d’une demande UploadItemsResponse.**  <br/> |
|[GetInboxRulesResponse](getinboxrulesresponse.md) <br/> |Contient une réponse à **une demande GetInboxRules.**  <br/> |
|GetServiceConfigurationResponse  <br/> |Contient une réponse à **une demande GetServiceConfiguration.**  <br/> |
|[ServiceConfigurationResponseMessageType](serviceconfigurationresponsemessagetype.md) <br/> |Contient les paramètres de configuration du service.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte est requise si cet élément est utilisé. Cet élément est en lecture seule.
  
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

- [Référence EWS pour Exchange](ews-reference-for-exchange.md) 
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

