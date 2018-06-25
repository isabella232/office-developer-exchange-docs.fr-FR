---
title: Heure d’été
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Daylight
api_type:
- schema
ms.assetid: ea400839-fba8-4a5e-a5d1-9b677afc0ff9
description: L’élément de l’heure d’été représente la date et l’heure de l’heure de modification de l’heure standard à l’heure.
ms.openlocfilehash: cdb6ed305f1d77a73b952f8c659991f3b2a8df7a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755815"
---
# <a name="daylight"></a>Heure d’été

L’élément de **l’heure d’été** représente la date et l’heure de l’heure de modification de l’heure standard à l’heure. 
  
```xml
<Daylight TimeZoneName="">
   <Offset/>
   <RelativeYearlyRecurrence/>
   <Time/>
</Daylight>
```

```xml
<Daylight TimeZoneName="">
   <Offset/>
   <AbsoluteDate/>
   <Time/>
</Daylight>
```

**TimeChangeType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**NomFuseauhoraire** <br/> |Indique le nom du fuseau horaire.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Offset](offset.md) <br/> |Indique le décalage à partir de la [BaseOffset](baseoffset.md). La base de décalage Outre cet offset identifie l’heure selon qu’il soit standard ou de l’heure d’été.  <br/> |
|[RelativeYearlyRecurrence](relativeyearlyrecurrence.md) <br/> |Décrit une périodicité annuelle relative d’un modèle de date de transition de fuseau horaire.  <br/> |
|[AbsoluteDate](absolutedate.md) <br/> |Représente la date à laquelle l’heure passe à partir de standard ou l’heure d’été.  <br/> |
|[Heure (TimeChangeType)](time-timechangetype.md) <br/> |Indique l’heure de l’heure de modification entre heure standard et l’heure d’été.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[MeetingTimeZone](meetingtimezone.md) <br/> |Représente le fuseau horaire de l’emplacement où se trouve la réunion.  <br/> |
   
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

