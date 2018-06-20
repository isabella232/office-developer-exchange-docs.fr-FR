---
title: PushSubscriptionRequest
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PushSubscriptionRequest
api_type:
- schema
ms.assetid: 70caa0ca-40a1-421f-b4e6-0658f22d0b8e
description: L’élément PushSubscriptionRequest représente un abonnement à un abonnement de notification push d’événements.
ms.openlocfilehash: 34717d37b8e5bb50c927e57088299fbcb18a2514
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828929"
---
# <a name="pushsubscriptionrequest"></a>PushSubscriptionRequest

L’élément **PushSubscriptionRequest** représente un abonnement à un abonnement de notification push d’événements. 
  
[S’abonner](subscribe.md)
  
[PushSubscriptionRequest](pushsubscriptionrequest.md)
  
```XML
<PushSubscriptionRequest SubscribeToAllFolders="">
   <FolderIds/>
   <EventTypes/>
   <Watermark/>
   <StatusFrequency/>
   <URL/>
</PushSubscriptionRequest>
```

 **PushSubscriptionRequestType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**SubscribeToAllFolders** <br/> |Indique s’il s’abonner à tous les dossiers disponibles. Cet attribut est facultatif.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[FolderIds](folderids.md) <br/> |Contient un tableau d’identificateurs de dossier qui sont utilisés pour identifier les dossiers à analyser pour les notifications d’événement.  <br/> |
|[EventTypes](eventtypes.md) <br/> |Contient une collection de notifications d’événements qui sont utilisés pour créer un abonnement.  <br/> |
|[Filigrane](watermark.md) <br/> |Représente un signet d’événements dans la table d’événements de boîte aux lettres. Cela permet de créer un abonnement commençant à un événement représenté par le filigrane. Si la limite d’une demande Subscribe n’est trouvée, une réponse d’erreur est retournée au client. Cela peut se produire si celui-ci est antérieure à 30 jours ou si celui-ci n’a jamais été présent dans la boîte aux lettres.  <br/> |
|[StatusFrequency](statusfrequency.md) <br/> |Représente la fréquence, en minutes, à la notification messages sont envoyées au client lorsqu’aucun événement ne se sont produites.  <br/> |
|[URL](url-ex15websvcsotherref.md) <br/> |Représente l’emplacement du client de service Web pour les notifications push.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[S’abonner](subscribe.md) <br/> |Contient les propriétés utilisées pour créer des abonnements.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération d'abonnement](subscribe-operation.md)
  
[Opération de GetEvents](getevents-operation.md)
  
[Opération de résiliation d'abonnement](unsubscribe-operation.md)

