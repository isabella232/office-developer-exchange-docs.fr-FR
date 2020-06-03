---
title: Auxquelles
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
description: L’élément d’heure représente la date et l’heure auxquelles le temps passe de l’heure standard à l’heure d’été.
ms.openlocfilehash: bf2041cb4677f837ddb5b399041f1c19a7b5f577
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457458"
---
# <a name="daylight"></a>Auxquelles

L’élément d' **heure** représente la date et l’heure auxquelles le temps passe de l’heure standard à l’heure d’été. 
  
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

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**TimeZoneName** <br/> |Décrit le nom du fuseau horaire.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Offset](offset.md) <br/> |Décrit le décalage par rapport à l' [BaseOffset](baseoffset.md). Le décalage de base en plus de ce décalage identifie le temps en fonction de l’heure standard ou de l’heure d’été.  <br/> |
|[RelativeYearlyRecurrence](relativeyearlyrecurrence.md) <br/> |Décrit un modèle de périodicité annuelle relative pour un modèle de date de transition de fuseau horaire.  <br/> |
|[AbsoluteDate](absolutedate.md) <br/> |Représente la date à laquelle le temps passe de standard ou de l’heure d’été.  <br/> |
|[Heure (TimeChangeType)](time-timechangetype.md) <br/> |Décrit le moment où l’heure change entre l’heure standard et l’heure d’été.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[MeetingTimeZone](meetingtimezone.md) <br/> |Représente le fuseau horaire de l’emplacement où la réunion est hébergée.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

