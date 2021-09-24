---
title: PullSubscriptionRequest
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- PullSubscriptionRequest
api_type:
- schema
ms.assetid: 145c5cc7-a894-4f0b-a6ea-358cddfb5c33
description: L’élément PullSubscriptionRequest représente un abonnement à un abonnement de notification d’événement basé sur un pull.
ms.openlocfilehash: f1a527dff0c81262cac01a905293af1155acbf1c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540600"
---
# <a name="pullsubscriptionrequest"></a>PullSubscriptionRequest

**L’élément PullSubscriptionRequest** représente un abonnement à un abonnement de notification d’événement basé sur un pull. 
  
[Subscribe](subscribe.md)
  
[PullSubscriptionRequest](pullsubscriptionrequest.md)
  
```XML
<PullSubscriptionRequest SubscribeToAllFolders="">
   <FolderIds/>
   <EventTypes/>
   <Watermark/>
   <Timeout/>
</PullSubscriptionRequest>
```

 **PullSubscriptionRequestType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**SubscribeToAllFolders** <br/> |Indique s’il faut s’abonner à tous les dossiers disponibles. Cet attribut est facultatif.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[FolderIds](folderids.md) <br/> |Contient un tableau d’identificateurs de dossiers utilisés pour identifier les dossiers à surveiller pour les notifications d’événement.  <br/> |
|[EventTypes](eventtypes.md) <br/> |Contient une collection de notifications d’événements utilisées pour créer un abonnement.  <br/> |
|[Watermark](watermark.md) <br/> |Représente un signet d’événement dans la table des événements de boîte aux lettres. Il est utilisé pour créer un abonnement qui commence à un événement représenté par le filigrane. Si le filigrane d’une demande d’abonnement est in trouvé, une réponse d’erreur est renvoyée au client. Cette erreur peut se produire si le filigrane a plus de 30 jours ou s’il n’a jamais été présent dans la boîte aux lettres.  <br/> |
|[Timeout](timeout.md) <br/> |Représente la durée, en minutes, pendant qui l’abonnement peut rester inactif sans demande GetEvents du client.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Subscribe](subscribe.md) <br/> |Contient les propriétés utilisées pour créer des abonnements.  <br/> |
   
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



[PushSubscriptionRequest](pushsubscriptionrequest.md)
  
[Opération d'abonnement](subscribe-operation.md)
  
[Opération de GetEvents](getevents-operation.md)
  
[Opération de résiliation d'abonnement](unsubscribe-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

