---
title: AttendeeType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- AttendeeType
api_type:
- schema
ms.assetid: 048043a8-dbad-45a0-97c8-4cad63d8898b
description: L’élément AttendeeType représente le type de participant identifié dans l’élément Email (EmailAddressType). Cet élément est utilisé dans les demandes de suggestions de réunion.
ms.openlocfilehash: 5bcec50fe6cccc3df48ca9615dbd0d9418211b4b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59533933"
---
# <a name="attendeetype"></a>AttendeeType

**L’élément AttendeeType** représente le type de participant identifié dans l’élément [Email (EmailAddressType).](email-emailaddresstype.md) Cet élément est utilisé dans les demandes de suggestions de réunion. 
  
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
|[MailboxData](mailboxdata.md) <br/> |Représente un utilisateur de boîte aux lettres individuel et des options pour le type de données à retourner sur l’utilisateur de la boîte aux lettres.  <br/> Voici le chemin d’accès XPath à cet élément :  <br/>  `/GetUserAvailabilityRequest/MailboxDataArray[i]/MailboxData` <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte est requise pour cet élément. Le tableau suivant répertorie les valeurs possibles pour cet élément.
  
|**Valeur**|**Description**|
|:-----|:-----|
|Organisateur  <br/> |Utilisateur de boîte aux lettres et participant qui a créé l’élément de calendrier.  <br/> |
|Obligatoire  <br/> |Utilisateur de boîte aux lettres qui est un participant requis à la réunion.  <br/> |
|Facultatif  <br/> |Un utilisateur de boîte aux lettres qui est un participant facultatif à la réunion.  <br/> |
|Room  <br/> |Entité de boîte aux lettres qui représente une ressource de salle utilisée pour la réunion.  <br/> |
|Ressource  <br/> |Ressource telle qu’un téléviseur ou un projecteur qui est prévu pour être utilisé dans la réunion.  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est un élément enfant requis de [l’élément MailboxData.](mailboxdata.md) Cet élément ne peut se produire qu’une seule fois dans [l’élément MailboxData.](mailboxdata.md) Le schéma qui décrit cet élément se trouve dans le répertoire /EWS/ de l’ordinateur qui exécute MicrosoftExchange Server 2007 sur qui le rôle serveur d’accès au client est installé. 
  
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

