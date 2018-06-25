---
title: Notifications
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Notifications
api_type:
- schema
ms.assetid: 153cc420-d2fe-42f1-afb2-9a31ee09a750
description: L’élément de Notifications contient un tableau d’informations sur l’abonnement et les événements qui se sont produites depuis la dernière notification.
ms.openlocfilehash: f576bf579c91b77dcde8646a6af7fdc47145aef7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828550"
---
# <a name="notifications"></a>Notifications

L’élément de **Notifications** contient un tableau d’informations sur l’abonnement et les événements qui se sont produites depuis la dernière notification. 
  
```xml
<Notifications>
   <Notification/>
</Notifications>
```

 **NonEmptyArrayOfNotificationsType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Notification](notification-ex15websvcsotherref.md) <br/> |Contient des informations sur l’abonnement et les événements qui se sont produites depuis la dernière notification.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetStreamingEventsResponseMessage](getstreamingeventsresponsemessage.md) <br/> |Contient l’état et les résultats d’une seule demande [d’opération GetStreamingEvents](getstreamingevents-operation.md) .  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages et http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma des messages ; Schéma de types  <br/> |
|Fichier de validation  <br/> |Messages.xsd ; Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetFolder](getfolder-operation.md)
  
[Opération DeleteFolder](deletefolder-operation.md)
  
[Opération MoveFolder](movefolder-operation.md)
  
[Opération CopyFolder](copyfolder-operation.md)
  
[Opération d'abonnement](subscribe-operation.md)

