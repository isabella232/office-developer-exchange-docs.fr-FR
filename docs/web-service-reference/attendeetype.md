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
description: L’élément AttendeeType représente le type de participant identifié dans l’élément email (EmailAddressType). Cet élément est utilisé dans les demandes de suggestions de réunion.
ms.openlocfilehash: 104b9f38cc891310ecb47c0b47837a912ced6ab7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462296"
---
# <a name="attendeetype"></a>AttendeeType

L’élément **AttendeeType** représente le type de participant identifié dans l’élément [email (EmailAddressType)](email-emailaddresstype.md) . Cet élément est utilisé dans les demandes de suggestions de réunion. 
  
- [GetUserAvailabilityRequest](getuseravailabilityrequest.md)
  
- [MailboxDataArray](mailboxdataarray.md)
  
- [MailboxData](mailboxdata.md)
  
- [AttendeeType](attendeetype.md)
  
```xml
<AttendeeType>Organizer or Required or Optional or Room or Resource</AttendeeType>
```

 **MeetingAttendeeType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[MailboxData](mailboxdata.md) <br/> |Représente un utilisateur et des options de boîte aux lettres individuelle pour le type de données à renvoyer à propos de l’utilisateur de boîte aux lettres.  <br/> Voici le XPath de cet élément :  <br/>  `/GetUserAvailabilityRequest/MailboxDataArray[i]/MailboxData` <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte est requise pour cet élément. Le tableau suivant répertorie les valeurs possibles pour cet élément.
  
|**Valeur**|**Description**|
|:-----|:-----|
|Organisateur  <br/> |Utilisateur de boîte aux lettres et participant qui a créé l’élément de calendrier.  <br/> |
|Requis  <br/> |Utilisateur de boîte aux lettres qui est un participant obligatoire de la réunion.  <br/> |
|Facultatif  <br/> |Utilisateur de boîte aux lettres qui est un participant facultatif à la réunion.  <br/> |
|Salle  <br/> |Entité de boîte aux lettres qui représente une ressource de salle utilisée pour la réunion.  <br/> |
|Resource  <br/> |Ressource telle qu’un téléviseur ou un projecteur prévu pour être utilisée lors de la réunion.  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est un élément enfant obligatoire de l’élément [MailboxData](mailboxdata.md) . Cet élément ne peut se produire qu’une seule fois dans l’élément [MailboxData](mailboxdata.md) . Le schéma qui décrit cet élément se trouve dans le répertoire/EWS/de l’ordinateur exécutant MicrosoftExchange Server 2007 sur lequel le rôle de serveur d’accès au client est installé. 
  
> [!NOTE]
> Le type de schéma AttendeeType est utilisé pour représenter les participants à un élément de calendrier. Ne confondez pas cet élément avec des éléments du type de schéma AttendeeType. 
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération GetUserAvailability](getuseravailability-operation.md)
- [GetUserAvailabilityRequest](getuseravailabilityrequest.md)
- [Obtention de la disponibilité des utilisateurs](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

