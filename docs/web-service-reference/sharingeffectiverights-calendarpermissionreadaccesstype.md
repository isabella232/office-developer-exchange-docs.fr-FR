---
title: SharingEffectiveRights (CalendarPermissionReadAccessType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SharingEffectiveRights
api_type:
- schema
ms.assetid: b519f642-a9ef-4300-92e6-ed8202855fde
description: L’élément SharingEffectiveRights indique les autorisations dont dispose l’utilisateur pour les données de calendrier qui sont partagées.
ms.openlocfilehash: e7d2aa061650c33d27de042ae8a6348f9a7d3430
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829480"
---
# <a name="sharingeffectiverights-calendarpermissionreadaccesstype"></a>SharingEffectiveRights (CalendarPermissionReadAccessType)

L’élément **SharingEffectiveRights** indique les autorisations dont dispose l’utilisateur pour les données de calendrier qui sont partagées. 
  
```XML
<SharingEffectiveRights>None | TimeOnly | TimeAndSubjectAndLocation | FullDetails</SharingEffectiveRights>
```

 **CalendarPermissionReadAccessType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[CalendarFolder](calendarfolder.md) <br/> |Représente un dossier contenant principalement des éléments de calendrier.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Le tableau suivant répertorie les valeurs possibles pour l’élément **SharingEffectiveRights** . 
  
|**Valeur**|**Description**|
|:-----|:-----|
|None  <br/> |Indique que l’utilisateur ne dispose pas d’autorisation d’afficher des éléments dans le calendrier.  <br/> |
|TimeOnly  <br/> |Indique que l’utilisateur est autorisé à afficher uniquement formulées dans le calendrier.  <br/> |
|TimeAndSubjectAndLocation  <br/> |Indique que l’utilisateur est autorisé à afficher le temps de disponibilité dans le calendrier et le sujet et l’emplacement du rendez-vous.  <br/> |
|FullDetails  <br/> |Indique que l’utilisateur est autorisé à afficher tous les éléments dans le calendrier, notamment formulées et subject, emplacement et les détails des rendez-vous.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

