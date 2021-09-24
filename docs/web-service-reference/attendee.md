---
title: Participant
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Attendee
api_type:
- schema
ms.assetid: 393c3d7e-7416-458a-b976-270b88eaaa03
description: L’élément Attendee représente les participants et les ressources d’une réunion.
ms.openlocfilehash: d48dcee42292b045ffc7cdcc5fd02f70109b1853
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59531193"
---
# <a name="attendee"></a>Participant

**L’élément Attendee** représente les participants et les ressources d’une réunion. 
  
```xml
<Attendee>
   <Mailbox/>
   <ResponseType/>
   <LastResponseTime/>
</Attendee>
```

 **AttendeeType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Boîte aux lettres](mailbox.md) <br/> |Identifie une adresse de messagerie entièrement résolue.  <br/> |
|[ResponseType](responsetype.md) <br/> |Représente le type de réponse du destinataire reçu pour une réunion. Cette propriété est uniquement pertinente pour l’élément de calendrier d’un organisateur de réunion.  <br/> |
|[LastResponseTime](lastresponsetime.md) <br/> |Représente la date et l’heure de la dernière réponse reçue.  <br/> |
|[ProposedStart](proposedstart-attendeetype.md) <br/> |Représente l’heure de début proposée par un participant pour une réunion. <br/> |
|[ProposedEnd](proposedend-attendeetype.md) <br/> |Représente l’heure de fin proposée par un participant pour une réunion. <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[RequiredAttendees](requiredattendees.md) <br/> |Représente les participants requis pour participer à une réunion.  <br/> |
|[OptionalAttendees](optionalattendees.md) <br/> |Représente les participants qui ne sont pas tenus de participer à une réunion.  <br/> |
|[Ressources](resources.md) <br/> |Représente une ressource programmée pour une réunion.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

