---
title: DateTimeCreated
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DateTimeCreated
api_type:
- schema
ms.assetid: 42ae0067-4688-49d9-93c5-c4dbeb54cee1
description: L’élément DateTimeCreated représente la date et l’heure auxquelles un élément de la boîte aux lettres a été créé.
ms.openlocfilehash: c79fe4f9288a5b636d7a85412f2410fe388272fc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461414"
---
# <a name="datetimecreated"></a>DateTimeCreated

L’élément **DateTimeCreated** représente la date et l’heure auxquelles un élément de la boîte aux lettres a été créé. 
  
```xml
<DateTimeCreated/>
```

**DateTime**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[CalendarItem](calendaritem.md) <br/> |Représente un élément de calendrier Exchange.  <br/> |
|[Contact](contact.md) <br/> |Représente un élément de contact Exchange.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Représente une liste de distribution.  <br/> |
|[Élément](item.md) <br/> |Représente un élément dans la banque d'informations Exchange.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Représente une annulation de réunion dans la banque d'informations Exchange.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Représente une réunion dans la banque d'informations Exchange.  <br/> |
|[Propriété meetingrequest](meetingrequest.md) <br/> |Représente une demande de réunion dans la banque d'informations Exchange.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Représente une réponse à une réunion dans la banque d'informations Exchange.  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Représente un message électronique Exchange.  <br/> |
|[RemoveItem](removeitem.md) <br/> |Supprime un élément de la banque d'informations Exchange.  <br/> |
|[Tâche](task.md) <br/> |Représente une tâche dans la banque d'informations Exchange.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur de texte représente la date et l’heure auxquelles un élément de la boîte aux lettres a été créé.
  
## <a name="remarks"></a>Remarques

L’utilisation d’objets de réponse de calendrier met à jour la propriété [DateTimeCreated](datetimecreated.md) sur l’élément de calendrier associé. Le comportement attendu est que la propriété **DateTimeCreated** reste inchangée. Par exemple, l’utilisateur A envoie une demande de réunion à l’utilisateur B. l’utilisateur B accepte la demande de réunion avec l’identificateur de la demande de réunion. La propriété **DateTimeCreated** de l’élément de calendrier associé est modifiée. 
  
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

