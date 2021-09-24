---
title: PushSubscriptionRequest
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- PushSubscriptionRequest
api_type:
- schema
ms.assetid: 70caa0ca-40a1-421f-b4e6-0658f22d0b8e
description: L’élément PushSubscriptionRequest représente un abonnement à un abonnement de notification d’événements push.
ms.openlocfilehash: 6eb76bba92e78e048ae97dbec5fc6c4d698a815f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523726"
---
# <a name="pushsubscriptionrequest"></a>PushSubscriptionRequest

**L’élément PushSubscriptionRequest** représente un abonnement à un abonnement de notification d’événements push. 
  
[Subscribe](subscribe.md)
  
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
|[Watermark](watermark.md) <br/> |Représente un signet d’événement dans la table des événements de boîte aux lettres. Il est utilisé pour créer un abonnement à partir d’un événement représenté par le filigrane. Si le filigrane d’une demande d’abonnement est in trouvé, une réponse d’erreur est renvoyée au client. Cela peut se produire si le filigrane a plus de 30 jours ou s’il n’a jamais été présent dans la boîte aux lettres.  <br/> |
|[StatusFrequency](statusfrequency.md) <br/> |Représente la fréquence, spécifiée en minutes, à laquelle les messages de notification sont envoyés au client lorsqu’aucun événement ne s’est produit.  <br/> |
|[URL ](url-ex15websvcsotherref.md) <br/> |Représente l’emplacement du service Web client pour les notifications Push.  <br/> |
   
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



[Opération d'abonnement](subscribe-operation.md)
  
[Opération de GetEvents](getevents-operation.md)
  
[Opération de résiliation d'abonnement](unsubscribe-operation.md)

