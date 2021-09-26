---
title: Standard
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Standard
api_type:
- schema
ms.assetid: d598f0a6-e296-423f-8ce5-3da57cfd8189
description: L’élément Standard représente la date et l’heure de passage de l’heure d’été à l’heure standard.
ms.openlocfilehash: 8e44bc458f109975acd3d48c80726654b70373e8
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544667"
---
# <a name="standard"></a>Standard

**L’élément Standard** représente la date et l’heure de passage de l’heure d’été à l’heure standard. 
  
```xml
<Standard TimeZoneName="">
   <Offset/>
   <RelativeYearlyRecurrence/>
   <Time/>
</Standard>
```

```xml
<Standard TimeZoneName="">
   <Offset/>
   <AbsoluteDate/>
   <Time/>
</Standard>
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
|[Offset](offset.md) <br/> |Décrit le décalage par rapport à [baseOffset](baseoffset.md). Avec **l’élément BaseOffset,** l’élément **Offset** identifie si l’heure est l’heure standard ou l’heure d’été.  <br/> |
|[RelativeYearlyRecurrence](relativeyearlyrecurrence.md) <br/> |Décrit une récurrence relative de l’année pour une date de transition de fuseau horaire.  <br/> |
|[AbsoluteDate](absolutedate.md) <br/> |Représente la date à laquelle l’heure change à partir de l’heure standard ou de l’heure d’été.  <br/> |
|[Time (TimeChangeType)](time-timechangetype.md) <br/> |Décrit l’heure à quel moment l’heure change entre l’heure standard et l’heure d’été.  <br/> |
   
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

