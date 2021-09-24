---
title: Watermark
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Watermark
api_type:
- schema
ms.assetid: e1545046-94f9-4ac7-af1c-ea81dfb6822c
description: L’élément Watermark représente un signet d’événement dans la file d’attente d’événements de boîte aux lettres.
ms.openlocfilehash: 959ae7369195a164d257b8805a8c985f1fdca53b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59524398"
---
# <a name="watermark"></a>Watermark

**L’élément Watermark** représente un signet d’événement dans la file d’attente d’événements de boîte aux lettres. 
  
```xml
<Watermark/>
```

 **WatermarkType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[PullSubscriptionRequest](pullsubscriptionrequest.md) <br/> |Représente un abonnement à un abonnement de notification d’événement basé sur un pull.  <br/> |
|[PushSubscriptionRequest](pushsubscriptionrequest.md) <br/> |Représente un abonnement à un abonnement de notification d’événements push.  <br/> |
|[GetEvents](getevents.md) <br/> |Représente l’opération utilisée par les clients pull pour demander des notifications au serveur.  <br/> |
|[CopiedEvent](copiedevent.md) <br/> |Représente un événement dans lequel un élément ou un dossier est copié.  <br/> |
|[CreatedEvent](createdevent.md) <br/> |Représente un événement dans lequel un élément ou un dossier est créé.  <br/> |
|[DeletedEvent](deletedevent.md) <br/> |Représente un événement dans lequel un élément ou un dossier est supprimé.  <br/> |
|[ModifiedEvent](modifiedevent.md) <br/> |Représente un événement dans lequel un élément ou un dossier est modifié.  <br/> |
|[MovedEvent](movedevent.md) <br/> |Représente un événement dans lequel un élément ou un dossier est déplacé d’un dossier parent vers un autre dossier parent.  <br/> |
|[NewMailEvent](newmailevent.md) <br/> |Représente un événement déclenché par un nouvel élément de courrier dans une boîte aux lettres.  <br/> |
|[StatusEvent](statusevent.md) <br/> |Représente une notification vous avertissant qu’aucune nouvelle activité n’a eu lieu dans la boîte aux lettres.  <br/> |
|[SubscribeResponseMessage](subscriberesponsemessage.md) <br/> |Contient l’état et le résultat d’une demande d’abonnement.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte peut être requise ou facultative en fonction de la façon dont cet élément est utilisé.
  
## <a name="remarks"></a>Remarques

Si une demande d’abonnement contient un filigrane, l’abonnement est créé à partir du filigrane avant. Si la demande d’abonnement contient un filigrane qui n’est pas trouvé dans la table des événements de boîte aux lettres, une erreur est renvoyée  `ErrorInvalidWatermark` à l’application cliente. Cela peut se produire si le filigrane est trop ancien et a été supprimé de la fenêtre de 30 jours de la table d’événements ou si le filigrane n’a jamais été présent dans la table d’événements. Cela peut se produire, par exemple, si un filigrane est obtenu à partir d’un abonnement différent pour une boîte aux lettres dans une autre base de données. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération d'abonnement](subscribe-operation.md)
  
[Opération de GetEvents](getevents-operation.md)
  
[Opération de résiliation d'abonnement](unsubscribe-operation.md)

