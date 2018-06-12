---
title: Participant
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Attendee
api_type:
- schema
ms.assetid: 393c3d7e-7416-458a-b976-270b88eaaa03
description: L’élément Attendee représente les participants et les ressources pour une réunion.
ms.openlocfilehash: 60cb0839c2f6de69b833c11f4594d40c14cd8887
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755341"
---
# <a name="attendee"></a>Participant

L’élément **Attendee** représente les participants et les ressources pour une réunion. 
  
```xml
<Attendee>
   <Mailbox/>
   <ResponseType/>
   <LastResponseTime/>
</Attendee>
```

 **AttendeeType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Boîte aux lettres](mailbox.md) <br/> |Identifie une adresse de messagerie entièrement résolu.  <br/> |
|[ResponseType](responsetype.md) <br/> |Représente le type de destinataire réponse reçue pour une réunion. Cette propriété n’est pas pertinente pour l’élément de calendrier de l’organisateur d’une réunion.  <br/> |
|[LastResponseTime](lastresponsetime.md) <br/> |Représente la date et l’heure de la dernière réponse reçue.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[RequiredAttendees](requiredattendees.md) <br/> |Représente les participants qui sont nécessaires pour participer à une réunion.  <br/> |
|[OptionalAttendees](optionalattendees.md) <br/> |Représente les participants qui ne sont pas indispensables à participer à une réunion.  <br/> |
|[Ressources](resources.md) <br/> |Représente une ressource pour une réunion planifiée.  <br/> |
   
## <a name="remarks"></a>Note

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

