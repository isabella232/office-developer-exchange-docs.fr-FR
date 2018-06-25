---
title: CalendarPermissionLevel
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CalendarPermissionLevel
api_type:
- schema
ms.assetid: 6ac2b792-4326-4a3f-b6cb-977bf523b5b2
description: L’élément CalendarPermissionLevel représente le niveau d’autorisation dont dispose un utilisateur sur un dossier de calendrier. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 646e4df3b70350a16cdd1f3e134260c2984a5161
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755480"
---
# <a name="calendarpermissionlevel"></a>CalendarPermissionLevel

L’élément **CalendarPermissionLevel** représente le niveau d’autorisation dont dispose un utilisateur sur un dossier de calendrier. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1). 
  
```xml
<CalendarPermissionLevel>None or Owner or PublishingEditor or Editor or PublishingAuthor or Author or NoneditingAuthor or Reviewer or Contributor or FreeBusyTimeOnly or FreeBusyTimeAndSubjectAndLocation or Custom</CalendarPermissionLevel>
```

 **CalendarPermissionLevelType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[CalendarPermission](calendarpermission.md) <br/> |Définit l'accès dont dispose un utilisateur dans un dossier de calendrier. Cet élément a été introduit dans Exchange 2007 SP1.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Le tableau suivant répertorie les valeurs possibles pour l’élément **CalendarPermissionLevel** . 
  
**Valeurs de texte des éléments CalendarPermissionLevel**

|**Valeur**|**Description**|
|:-----|:-----|
|None  <br/> |Indique que l’utilisateur n’a aucune autorisation sur le dossier.  <br/> |
|Owner  <br/> |Indique que l’utilisateur peut créer, lire, modifier, supprimer tous les éléments dans le dossier et créer des sous-dossiers. L’utilisateur est propriétaire du dossier et contact du dossier.  <br/> |
|Détenir  <br/> |Indique que l’utilisateur peut créer, lire, modifier, supprimer tous les éléments dans le dossier et créer des sous-dossiers.  <br/> |
|Editor  <br/> |Indique que l’utilisateur peut créer, lire, modifier et supprimer tous les éléments dans le dossier.  <br/> |
|PublishingAuthor  <br/> |Indique que l’utilisateur peut créer et lire tous les éléments dans le dossier, modifier et supprimer uniquement les éléments créés par l’utilisateur et créer des sous-dossiers.  <br/> |
|Auteur  <br/> |Indique que l’utilisateur peut créer et lire tous les éléments dans le dossier, modifier et supprimer uniquement les éléments créés par l’utilisateur.  <br/> |
|NoneditingAuthor  <br/> |Indique que l’utilisateur peut créer et lire tous les éléments dans le dossier et supprimer uniquement les éléments créés par l’utilisateur.  <br/> |
|Reviewer  <br/> |Indique que l’utilisateur peut lire tous les éléments dans le dossier.  <br/> |
|Collaborateur  <br/> |Indique que l’utilisateur peut créer des éléments dans le dossier. Le contenu du dossier n’apparaître pas.  <br/> |
|FreeBusyTimeOnly  <br/> |Indique que l’utilisateur peut afficher uniquement formulées dans le calendrier.  <br/> |
|FreeBusyTimeAndSubjectAndLocation  <br/> |Indique que l’utilisateur peut afficher les temps de disponibilité dans le calendrier et le sujet et l’emplacement du rendez-vous.  <br/> |
|Personnalisé  <br/> |Indique que l’utilisateur dispose des autorisations d’accès personnalisées sur le dossier.  <br/> |
   
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


[Setting Folder-Level Permissions](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

