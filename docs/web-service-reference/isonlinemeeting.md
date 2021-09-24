---
title: IsOnlineMeeting
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- IsOnlineMeeting
api_type:
- schema
ms.assetid: c29df676-0f3a-4694-a42f-522c6d16872f
description: L’élément IsOnlineMeeting indique si la réunion est en ligne.
ms.openlocfilehash: 3521cf82f2b6b2b2514b82478fc4e1e5c6edb563
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59514514"
---
# <a name="isonlinemeeting"></a>IsOnlineMeeting

**L’élément IsOnlineMeeting** indique si la réunion est en ligne. 
  
```xml
<IsOnlineMeeting/>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[MeetingRequest](meetingrequest.md) <br/> |Représente une réunion dans la banque d'informations Exchange.  <br/> |
|[CalendarItem](calendaritem.md) <br/> |Représente un élément de calendrier Exchange.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte qui représente une valeur boolé américaine est requise si cet élément est utilisé. La valeur **true indique** que la réunion est en ligne. La valeur **false indique** que la réunion n’est pas en ligne. 
  
## <a name="remarks"></a>Remarques

La propriété IsOnlineMeeting est accessible en lecture et en lecture pour l’élément de calendrier de l’organisateur. Il est en lecture seule pour les demandes de réunion et les éléments de calendrier des participants.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur exécutant MicrosoftExchange 2007 sur qui le rôle serveur d’accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

