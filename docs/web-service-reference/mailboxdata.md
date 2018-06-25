---
title: MailboxData
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailboxData
api_type:
- schema
ms.assetid: e9e3f50c-5a7b-49c7-a9ea-117959c08352
description: L’élément MailboxData représente un utilisateur de boîte aux lettres et les options pour le type de données à renvoyer sur l’utilisateur de boîte aux lettres.
ms.openlocfilehash: df60294e7d83b1459e5cca7d75c2b6b4bb9d931d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828281"
---
# <a name="mailboxdata"></a>MailboxData

L’élément **MailboxData** représente un utilisateur de boîte aux lettres et les options pour le type de données à renvoyer sur l’utilisateur de boîte aux lettres. 
  
- [GetUserAvailabilityRequest](getuseravailabilityrequest.md)
  
- [MailboxDataArray](mailboxdataarray.md)
  
- [MailboxData](mailboxdata.md)
  
```xml
<MailboxData>
   <Email>...</Email>
   <AttendeeType>...</AttendeeType>
   <ExcludeConflicts>...</ExcludeConflicts>
<MailboxData>
```

**MailboxData**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Courrier électronique (EmailAddressType)](email-emailaddresstype.md) <br/> |Représente l’utilisateur de boîte aux lettres pour une requête GetUserAvailability.  <br/> |
|[AttendeeType](attendeetype.md) <br/> |Représente le type de participant identifié dans l’élément de [courrier électronique (EmailAddressType)](email-emailaddresstype.md) . Il est utilisé dans les requêtes de suggestions de réunion.  <br/> |
|[ExcludeConflicts](excludeconflicts.md) <br/> |Spécifie s’il faut renvoyer suggérées heures de temps de calendrier en conflit entre les participants.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[MailboxDataArray](mailboxdataarray.md) <br/> |Contient une liste des boîtes aux lettres pour interroger des informations de disponibilité.  <br/> Vous trouverez ci-dessous le XPath pour cet élément :  <br/>  `/GetUserAvailabilityRequest/MailboxDataArray[i]` <br/> |
   
## <a name="remarks"></a>Remarques

Une application cliente peut en définir une à de nombreux éléments **MailboxData** . 
  
> [!NOTE]
> Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Exchange Server 2007 ayant le rôle de serveur d’accès au Client est installé. 
  
## <a name="example"></a>Exemple

```xml
<MailboxDataArray>
  <MailboxData xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
    <Email>
      <Name></Name>
      <Address>someone@ExServer.example.com</Address>
      <RoutingType>SMTP</RoutingType>
    </Email>
    <AttendeeType>Organizer</AttendeeType>
    <ExcludeConflicts>false</ExcludeConflicts>
  </MailboxData>
</MailboxDataArray>
```

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

