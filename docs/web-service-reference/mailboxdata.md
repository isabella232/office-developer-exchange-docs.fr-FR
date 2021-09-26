---
title: MailboxData
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- MailboxData
api_type:
- schema
ms.assetid: e9e3f50c-5a7b-49c7-a9ea-117959c08352
description: L’élément MailboxData représente un utilisateur de boîte aux lettres individuel et des options pour le type de données à retourner à propos de l’utilisateur de la boîte aux lettres.
ms.openlocfilehash: 62c8c816fc0b0e0c6831d468d90e7303fb72d9be
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546132"
---
# <a name="mailboxdata"></a>MailboxData

**L’élément MailboxData représente** un utilisateur de boîte aux lettres individuel et des options pour le type de données à retourner à propos de l’utilisateur de la boîte aux lettres. 
  
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

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Email (EmailAddressType)](email-emailaddresstype.md) <br/> |Représente l’utilisateur de boîte aux lettres pour une requête GetUserAvailability.  <br/> |
|[AttendeeType](attendeetype.md) <br/> |Représente le type de participant identifié dans l’élément [Email (EmailAddressType).](email-emailaddresstype.md) Il est utilisé dans les demandes de suggestions de réunion.  <br/> |
|[ExcludeConflicts](excludeconflicts.md) <br/> |Spécifie s’il faut renvoyer les heures suggérées pour les heures de calendrier qui entrent en conflit entre les participants.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[MailboxDataArray](mailboxdataarray.md) <br/> |Contient une liste de boîtes aux lettres à interroger pour obtenir des informations de disponibilité.  <br/> Voici le chemin d’accès XPath à cet élément :  <br/>  `/GetUserAvailabilityRequest/MailboxDataArray[i]` <br/> |
   
## <a name="remarks"></a>Remarques

Une application cliente peut définir un à plusieurs **éléments MailboxData.** 
  
> [!NOTE]
> Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur exécutant Exchange Server 2007 sur qui le rôle serveur d’accès au client est installé. 
  
## <a name="example"></a>Exemple

```xml
<MailboxDataArray>
  <MailboxData xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération GetUserAvailability](getuseravailability-operation.md)
- [GetUserAvailabilityRequest](getuseravailabilityrequest.md)
- [Obtention de la disponibilité des utilisateurs](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

