---
title: SharingEffectiveRights (CalendarPermissionReadAccessType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SharingEffectiveRights
api_type:
- schema
ms.assetid: b519f642-a9ef-4300-92e6-ed8202855fde
description: L’élément SharingEffectiveRights indique les autorisations dont dispose l’utilisateur pour les données de calendrier en cours de partage.
ms.openlocfilehash: d1e669b70ad816cc24e34554a116159025e267e6
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59547070"
---
# <a name="sharingeffectiverights-calendarpermissionreadaccesstype"></a>SharingEffectiveRights (CalendarPermissionReadAccessType)

**L’élément SharingEffectiveRights** indique les autorisations dont dispose l’utilisateur pour les données de calendrier en cours de partage. 
  
```XML
<SharingEffectiveRights>None | TimeOnly | TimeAndSubjectAndLocation | FullDetails</SharingEffectiveRights>
```

 **CalendarPermissionReadAccessType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[CalendarFolder](calendarfolder.md) <br/> |Représente un dossier qui contient principalement des éléments de calendrier.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Le tableau suivant répertorie les valeurs possibles pour **l’élément SharingEffectiveRights.** 
  
|**Valeur**|**Description**|
|:-----|:-----|
|Aucun  <br/> |Indique que l’utilisateur n’est pas autorisé à afficher les éléments du calendrier.  <br/> |
|TimeOnly  <br/> |Indique que l’utilisateur est autorisé à afficher uniquement les heures de libre/occupé dans le calendrier.  <br/> |
|TimeAndSubjectAndLocation  <br/> |Indique que l’utilisateur est autorisé à afficher les heures de libre/occupé dans le calendrier, ainsi que l’objet et l’emplacement des rendez-vous.  <br/> |
|FullDetails  <br/> |Indique que l’utilisateur est autorisé à afficher tous les éléments du calendrier, y compris les heures de libre/occupé et l’objet, l’emplacement et les détails des rendez-vous.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

