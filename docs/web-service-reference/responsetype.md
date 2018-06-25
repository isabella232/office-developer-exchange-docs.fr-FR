---
title: ResponseType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResponseType
api_type:
- schema
ms.assetid: cdc09dda-ce20-4504-880d-9da6025ca812
description: L’élément ResponseType représente le type de destinataire réponse reçue pour une réunion.
ms.openlocfilehash: fcfd47cb988ee00303b2c4205cb3d058cb6599b2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829200"
---
# <a name="responsetype"></a>ResponseType

L’élément **ResponseType** représente le type de destinataire réponse reçue pour une réunion. 
  
```xml
<ResponseType/>
```

 **ResponseTypeType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Attendee](attendee.md) <br/> |Représente les participants et les ressources pour une réunion.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Représente une annulation de réunion dans la banque d’informations Exchange  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Représente un message de réunion dans la banque d’informations Exchange.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Représente une demande de réunion dans la banque d'informations Exchange.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Représente une réponse à une réunion dans la banque d'informations Exchange.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Une valeur texte est requise. Les valeurs de texte possibles de cet élément sont les suivantes :
  
- Inconnu
    
- Organisateur
    
- Provisoire
    
- Accepter
    
- Refuser
    
- NoResponseReceived
    
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

