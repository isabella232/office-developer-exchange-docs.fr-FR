---
title: GetEvents
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- GetEvents
api_type:
- schema
ms.assetid: 22d4da6b-d8a8-484f-82c4-3e4b8f5431cd
description: L’élément GetEvents représente l’opération utilisée par les clients pull pour demander des notifications au serveur.
ms.openlocfilehash: c76672baf05efce0ce9c8221f4f2965a9bc922fc
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59547490"
---
# <a name="getevents"></a>GetEvents

**L’élément GetEvents** représente l’opération utilisée par les clients pull pour demander des notifications au serveur. 
  
[GetEvents](getevents.md)
  
```xml
<GetEvents>
   <SubscriptionId/>
   <Watermark/>
</GetEvents>
```

 **GetEventsType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[SubscriptionId (GetEvents)](subscriptionid-getevents.md) <br/> |Représente l’identificateur d’un abonnement interrogé pour les événements.  <br/> |
|[Watermark](watermark.md) <br/> |Représente le dernier filigrane renvoyé au client. Si GetEvents n’a pas été appelé pour cet abonnement, le client utilise le filigrane renvoyé par la demande d’abonnement. Sinon, le filigrane du dernier événement de la dernière réponse GetEvents est utilisé.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |false  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération d'abonnement](subscribe-operation.md)
  
[Opération de GetEvents](getevents-operation.md)
  
[Opération de résiliation d'abonnement](unsubscribe-operation.md)

