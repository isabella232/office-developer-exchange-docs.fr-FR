---
title: ResponseType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ResponseType
api_type:
- schema
ms.assetid: cdc09dda-ce20-4504-880d-9da6025ca812
description: L’élément ResponseType représente le type de réponse du destinataire reçu pour une réunion.
ms.openlocfilehash: d986eff544dc55d257903a2114e87af16eefea97
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518966"
---
# <a name="responsetype"></a>ResponseType

**L’élément ResponseType** représente le type de réponse du destinataire reçu pour une réunion. 
  
```xml
<ResponseType/>
```

 **ResponseTypeType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Attendee](attendee.md) <br/> |Représente les participants et les ressources d’une réunion.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Représente une annulation de réunion dans le magasin Exchange de réunion  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Représente un message de réunion dans le magasin Exchange de réunion.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Représente une demande de réunion dans la banque d'informations Exchange.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Représente une réponse à une réunion dans la banque d'informations Exchange.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte est requise. Voici les valeurs de texte possibles pour cet élément :
  
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
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

