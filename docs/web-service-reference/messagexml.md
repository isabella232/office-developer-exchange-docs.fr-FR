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
description: L’élément MessageXml fournit des informations supplémentaires sur la réponse aux erreurs.
ms.openlocfilehash: 180b447874523742a1d29d457c4ef020e4124f7c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466275"
---
# <a name="messagexml"></a>MessageXml

L’élément **messagexml** fournit des informations supplémentaires sur la réponse aux erreurs. 
  
- [ResponseMessage](responsemessage.md)  
- [MessageXml](messagexml.md)
  
```XML
<MessageXml/>
```

 **XS : any**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ResponseMessage](responsemessage.md) <br/> | Fournit des informations descriptives sur l’état de la réponse. <br/> <br/>  Voici quelques-unes des expressions XPath possibles pour cet élément : <br/> <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/ResponseMessage` <br/> <br/> `/GetUserAvailabilityResponse/SuggestionsResponse/ResponseMessage` <br/><br/>  `/SetUserOofSettingsResponse/ResponseMessage` <br/><br/>  `/GetUserOofSettingsResponse/ResponseMessage` <br/> |
|[DeleteItemResponseMessage](deleteitemresponsemessage.md) <br/> |Contient l’État et le résultat d’une seule demande DeleteItem.  <br/> |
|[SendItemResponseMessage](senditemresponsemessage.md) <br/> |Contient l’État et le résultat d’une seule demande SendItem.  <br/> |
|[DeleteFolderResponseMessage](deletefolderresponsemessage.md) <br/> |Contient l’État et le résultat d’une seule demande DeleteFolder.  <br/> |
|[DeleteAttachmentResponseMessage](deleteattachmentresponsemessage.md) <br/> |Contient l’État et le résultat d’une seule demande DeleteAttachment.  <br/> |
|[UnsubscribeResponseMessage](unsubscriberesponsemessage.md) <br/> |Contient l’État et le résultat d’une demande d’annulation d’abonnement unique.  <br/> |
|[CreateFolderResponseMessage](createfolderresponsemessage.md) <br/> |Contient l’État et le résultat d’une seule demande CreateFolder.  <br/> |
|[GetFolderResponseMessage](getfolderresponsemessage.md) <br/> |Contient l’État et le résultat d’une demande GetFolder unique.  <br/> |
|[UpdateFolderResponseMessage](updatefolderresponsemessage.md) <br/> |Contient l’État et le résultat d’une seule demande UpdateFolder.  <br/> |
|[MoveFolderResponseMessage](movefolderresponsemessage.md) <br/> |Contient l’État et le résultat d’une seule demande MoveFolder.  <br/> |
|[CopyFolderResponseMessage](copyfolderresponsemessage.md) <br/> |Contient l’État et le résultat d’une seule demande CopyFolder.  <br/> |
|[CreateManagedFolderResponseMessage](createmanagedfolderresponsemessage.md) <br/> |Contient l’État et le résultat d’une seule demande CreateManagedFolder.  <br/> |
|[FindFolderResponseMessage](findfolderresponsemessage.md) <br/> |Contient l’État et le résultat d’une seule demande FindFolder.  <br/> |
|[CreateItemResponseMessage](createitemresponsemessage.md) <br/> |Contient l’État et le résultat d’une seule demande CreateItem.  <br/> |
|[GetItemResponseMessage](getitemresponsemessage.md) <br/> |Contient l’État et le résultat d’une seule demande GetItem.  <br/> |
|[UpdateItemResponseMessage](updateitemresponsemessage.md) <br/> |Contient l’État et le résultat d’une seule demande UpdateItem.  <br/> |
|[MoveItemResponseMessage](moveitemresponsemessage.md) <br/> |Contient l’État et le résultat d’une seule demande MoveItem.  <br/> |
|[CopyItemResponseMessage](copyitemresponsemessage.md) <br/> |Contient l’État et le résultat d’une demande CopyItem unique.  <br/> |
|[CreateAttachmentResponseMessage](createattachmentresponsemessage.md) <br/> |Contient l’État et le résultat d’une seule demande CreateAttachment.  <br/> |
|[GetAttachmentResponseMessage](getattachmentresponsemessage.md) <br/> |Contient l’État et le résultat d’une seule demande GetAttachment.  <br/> |
|[FindItemResponseMessage](finditemresponsemessage.md) <br/> |Contient l’État et le résultat d’une seule demande FindItem.  <br/> |
|[ResolveNamesResponseMessage](resolvenamesresponsemessage.md) <br/> |Contient l’État et le résultat d’une demande ResolveNames.  <br/> |
|[ExpandDLResponseMessage](expanddlresponsemessage.md) <br/> |Contient l’État et le résultat d’une seule demande ExpandDL.  <br/> |
|[SubscribeResponseMessage](subscriberesponsemessage.md) <br/> |Contient l’État et le résultat d’une demande d’abonnement unique.  <br/> |
|[GetEventsResponseMessage](geteventsresponsemessage.md) <br/> |Contient l’État et le résultat d’une demande GetEvents unique.  <br/> |
|[SendNotificationResponseMessage](sendnotificationresponsemessage.md) <br/> |Contient l’État et le résultat d’une seule demande SendNotification.  <br/> |
|[SyncFolderHierarchyResponseMessage](syncfolderhierarchyresponsemessage.md) <br/> |Contient l’État et le résultat d’une demande Opérationsyncfolderhierarchy.  <br/> |
|[SyncFolderItemsResponseMessage](syncfolderitemsresponsemessage.md) <br/> |Contient l’État et le résultat d’une demande SyncFolderItems.  <br/> |
|[ConvertIdResponseMessage](convertidresponsemessage.md) <br/> |Contient l’État et le résultat d’une demande ConvertId.  <br/> |
|[AddDelegateResponse](adddelegateresponse.md) <br/> |Contient l’État et le résultat d’une demande AddDelegate.  <br/> |
|[GetServerTimeZonesResponseMessage](getservertimezonesresponsemessage.md) <br/> |Contient l’État et le résultat d’une demande GetServerTimeZones.  <br/> |
|[GetSharingFolderResponseMessage](getsharingfolderresponsemessage.md) <br/> |Contient l’État et le résultat d’une demande GetSharingFolder.  <br/> |
|[GetSharingFolderResponse](getsharingfolderresponse.md) <br/> |Définit une réponse à une demande GetSharingFolder.  <br/> |
|[GetSharingMetadataResponseMessage](getsharingmetadataresponsemessage.md) <br/> |Contient l’État et le résultat d’une demande GetSharingMetadata.  <br/> |
|[GetSharingMetadataResponse](getsharingmetadataresponse.md) <br/> |Définit une réponse à une demande GetSharingMetadata.  <br/> |
|[RefreshSharingFolderResponseMessage](refreshsharingfolderresponsemessage.md) <br/> |Contient l’État et le résultat d’une demande RefreshSharingFolder.  <br/> |
|[RefreshSharingFolderResponse](refreshsharingfolderresponse.md) <br/> |Définit une réponse à une demande RefreshSharingFolder.  <br/> |
|[FindConversationResponse](findconversationresponse.md) <br/> |Contient l’État et les résultats d’une réponse **FindConversation** .  <br/> |
|[EmptyFolderResponseMessage](emptyfolderresponsemessage.md) <br/> |Contient l’État et le résultat d’une demande **EmptyFolder** .  <br/> |
|[UpdateInboxRulesResponse](updateinboxrulesresponse.md) <br/> |Contient l’État et le résultat d’une demande **UpdateInboxRules** .  <br/> |
|[UploadItemsResponseMessage](uploaditemsresponsemessage.md) <br/> |Contient l’État et le résultat d’une demande **UploadItemsResponse** .  <br/> |
|[GetInboxRulesResponse](getinboxrulesresponse.md) <br/> |Contient une réponse à une demande **GetInboxRules** .  <br/> |
|[GetServiceConfigurationResponse](getserviceconfigurationresponse.md) <br/> |Contient une réponse à une demande **GetServiceConfiguration** .  <br/> |
|[ServiceConfigurationResponseMessageType](serviceconfigurationresponsemessagetype.md) <br/> |Contient les paramètres de configuration du service.  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément n’est pas obligatoire et n’est pas inclus dans toutes les réponses. Elle est incluse pour les messages d’erreur. Dans les demandes qui impliquent des dossiers ou des éléments, l’élément **messagexml** contient un ou plusieurs éléments qui contiennent les URI vers les propriétés ayant provoqué l’erreur. Voici un exemple de l’élément [FieldURI](fielduri.md) . 
  
L’élément **messagexml** est de type **XS : any**, ce qui signifie que tout code XML bien formé est un contenu valide pour l’élément This.
  
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

