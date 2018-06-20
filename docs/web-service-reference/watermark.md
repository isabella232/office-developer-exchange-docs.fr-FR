---
title: Filigrane
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
description: L’élément filigrane représente un signet d’événements dans la file d’attente des événements de boîte aux lettres.
ms.openlocfilehash: 1867aa781bc24f5eb3bdb4648fa494a2a7ea396a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839023"
---
# <a name="watermark"></a>Filigrane

L’élément **filigrane** représente un signet d’événements dans la file d’attente des événements de boîte aux lettres. 
  
```xml
<Watermark/>
```

 **WatermarkType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[PullSubscriptionRequest](pullsubscriptionrequest.md) <br/> |Représente un abonnement à un abonnement de notification d’événement de type pull.  <br/> |
|[PushSubscriptionRequest](pushsubscriptionrequest.md) <br/> |Représente un abonnement à un abonnement de notification push d’événements.  <br/> |
|[GetEvents](getevents.md) <br/> |Représente l’opération utilisée par les clients de l’extraction pour demander des notifications à partir du serveur.  <br/> |
|[CopiedEvent](copiedevent.md) <br/> |Représente un événement où un élément ou un dossier est copié.  <br/> |
|[CreatedEvent](createdevent.md) <br/> |Représente un événement dans lequel un élément ou un dossier est créé.  <br/> |
|[DeletedEvent](deletedevent.md) <br/> |Représente un événement de suppression d’un élément ou un dossier.  <br/> |
|[ModifiedEvent](modifiedevent.md) <br/> |Représente un événement où un élément ou un dossier est modifié.  <br/> |
|[MovedEvent](movedevent.md) <br/> |Représente un événement où un élément ou un dossier est déplacé à partir du dossier parent d’un vers un autre dossier parent.  <br/> |
|[NewMailEvent](newmailevent.md) <br/> |Représente un événement déclenché par un nouvel élément de messagerie dans une boîte aux lettres.  <br/> |
|[StatusEvent](statusevent.md) <br/> |Représente une notification qu’aucune nouvelle activité se n’est produite dans la boîte aux lettres.  <br/> |
|[SubscribeResponseMessage](subscriberesponsemessage.md) <br/> |Contient l’état et les résultats d’une demande Subscribe.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Une valeur de texte peut être obligatoire ou facultatif selon la façon dont cet élément est utilisé.
  
## <a name="remarks"></a>Remarques

Si une demande Subscribe contient un filigrane, l’abonnement est créé à partir de la limite de transférer. Si la demande Subscribe contient un filigrane qui ne figure pas dans la table d’événements de boîte aux lettres, un `ErrorInvalidWatermark` erreur est renvoyée à l’application cliente. Cela peut se produire si le filigrane est obsolète et a été supprimé de la fenêtre de 30 jours de la table d’événements ou si celui-ci n’a pas déjà présents dans la table des événements. Cela peut se produire, par exemple, si un filigrane est obtenu à partir d’un autre abonnement pour une boîte aux lettres dans une autre base de données. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération d'abonnement](subscribe-operation.md)
  
[Opération de GetEvents](getevents-operation.md)
  
[Opération de résiliation d'abonnement](unsubscribe-operation.md)

