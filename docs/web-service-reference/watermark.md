---
title: Watermark
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Watermark
api_type:
- schema
ms.assetid: e1545046-94f9-4ac7-af1c-ea81dfb6822c
description: L’élément Watermark représente un signet d’événement dans la file d’attente d’événements de boîte aux lettres.
ms.openlocfilehash: a717196101fea698b0b8c66f92a3d420fda9a421
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459762"
---
# <a name="watermark"></a>Watermark

L’élément **Watermark** représente un signet d’événement dans la file d’attente d’événements de boîte aux lettres. 
  
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
|[PullSubscriptionRequest](pullsubscriptionrequest.md) <br/> |Représente un abonnement à un abonnement de notification d’événement basé sur l’extraction.  <br/> |
|[PushSubscriptionRequest](pushsubscriptionrequest.md) <br/> |Représente un abonnement à un abonnement de notification d’événement basé sur un type de message.  <br/> |
|[GetEvents](getevents.md) <br/> |Représente l’opération utilisée par les clients de type pull pour demander des notifications à partir du serveur.  <br/> |
|[CopiedEvent](copiedevent.md) <br/> |Représente un événement dans lequel un élément ou un dossier est copié.  <br/> |
|[CreatedEvent](createdevent.md) <br/> |Représente un événement dans lequel un élément ou un dossier est créé.  <br/> |
|[DeletedEvent](deletedevent.md) <br/> |Représente un événement dans lequel un élément ou un dossier est supprimé.  <br/> |
|[ModifiedEvent](modifiedevent.md) <br/> |Représente un événement dans lequel un élément ou un dossier est modifié.  <br/> |
|[MovedEvent](movedevent.md) <br/> |Représente un événement dans lequel un élément ou un dossier est déplacé d’un dossier parent vers un autre dossier parent.  <br/> |
|[NewMailEvent](newmailevent.md) <br/> |Représente un événement déclenché par un nouvel élément de courrier dans une boîte aux lettres.  <br/> |
|[StatusEvent](statusevent.md) <br/> |Représente une notification indiquant qu’aucune nouvelle activité n’a eu lieu dans la boîte aux lettres.  <br/> |
|[SubscribeResponseMessage](subscriberesponsemessage.md) <br/> |Contient l’État et le résultat d’une demande subscribe.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte peut être obligatoire ou facultative en fonction de la façon dont cet élément est utilisé.
  
## <a name="remarks"></a>Remarques

Si une demande subscribe contient un filigrane, l’abonnement est créé à partir du filigrane avant. Si la demande subscribe contient un filigrane qui est introuvable dans la table des événements de boîte aux lettres, une `ErrorInvalidWatermark` erreur est renvoyée à l’application cliente. Cela peut se produire si le filigrane est trop ancien et a été supprimé de la fenêtre de 30 jours de la table des événements ou si le filigrane n’était jamais présent dans la table des événements. Cela peut se produire, par exemple, si un filigrane est obtenu à partir d’un autre abonnement pour une boîte aux lettres dans une autre base de données. 
  
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

