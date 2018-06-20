---
title: AttendeeType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AttendeeType
api_type:
- schema
ms.assetid: 048043a8-dbad-45a0-97c8-4cad63d8898b
description: L’élément AttendeeType représente le type de participant est identifié dans l’élément de courrier électronique (EmailAddressType). Cet élément est utilisé dans les requêtes de suggestions de réunion.
ms.openlocfilehash: a08532ed78296102ee252c1e0c40beee7ca8ea5d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755346"
---
# <a name="attendeetype"></a>AttendeeType

L’élément **AttendeeType** représente le type de participant est identifié dans l’élément de [courrier électronique (EmailAddressType)](email-emailaddresstype.md) . Cet élément est utilisé dans les requêtes de suggestions de réunion. 
  
- [GetUserAvailabilityRequest](getuseravailabilityrequest.md)
  
- [MailboxDataArray](mailboxdataarray.md)
  
- [MailboxData](mailboxdata.md)
  
- [AttendeeType](attendeetype.md)
  
```xml
<AttendeeType>Organizer or Required or Optional or Room or Resource</AttendeeType>
```

 **MeetingAttendeeType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[MailboxData](mailboxdata.md) <br/> |Représente un utilisateur de boîte aux lettres et les options pour le type de données à renvoyer sur l’utilisateur de boîte aux lettres.  <br/> Vous trouverez ci-dessous le XPath pour cet élément :  <br/>  `/GetUserAvailabilityRequest/MailboxDataArray[i]/MailboxData` <br/> |
   
## <a name="text-value"></a>Valeur de texte

Une valeur de texte est nécessaire pour cet élément. Le tableau suivant répertorie les valeurs possibles de cet élément.
  
|**Valeur**|**Description**|
|:-----|:-----|
|Organisateur  <br/> |L’utilisateur de boîte aux lettres et les participants qui a créé l’élément de calendrier.  <br/> |
|Obligatoire  <br/> |Un utilisateur de boîte aux lettres qui est un participant obligatoire à la réunion.  <br/> |
|Facultatif  <br/> |Un utilisateur de boîte aux lettres qui est un participant facultatif à la réunion.  <br/> |
|Salle  <br/> |Une entité de boîte aux lettres qui représente une ressource de l’espace utilisée pour la réunion.  <br/> |
|Ressource  <br/> |Une ressource comme une télévision ou un projecteur qui est prévue pour une utilisation dans la réunion.  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est un élément enfant requis de l’élément [MailboxData](mailboxdata.md) . Cet élément ne peut apparaître qu’une seule fois dans l’élément [MailboxData](mailboxdata.md) . Le schéma qui décrit cet élément se trouve dans le répertoire /EWS/ de l’ordinateur qui exécute MicrosoftExchange Server 2007 ayant le rôle de serveur d’accès au Client est installé. 
  
> [!NOTE]
> Le type de schéma AttendeeType est utilisé pour représenter les participants à un élément de calendrier. Ne confondez pas cet élément avec des éléments du type de schéma AttendeeType. 
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération GetUserAvailability](getuseravailability-operation.md)
- [GetUserAvailabilityRequest](getuseravailabilityrequest.md)
- [Obtention de disponibilité de l’utilisateur](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

