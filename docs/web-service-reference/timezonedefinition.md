---
title: TimeZoneDefinition
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- TimeZoneDefinition
api_type:
- schema
ms.assetid: b005a80c-addb-4409-beff-e5162076752c
description: L’élément TimeZoneDefinition spécifie les périodes et les transitions qui définissent un fuseau horaire.
ms.openlocfilehash: 6f2b580d2c3e31826ca74034cfda938cff71ee53
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59538813"
---
# <a name="timezonedefinition"></a>TimeZoneDefinition

**L’élément TimeZoneDefinition** spécifie les périodes et les transitions qui définissent un fuseau horaire. 
  
```XML
<TimeZoneDefinition Id="" Name="">
   <Periods/>
   <TransitionsGroups/>
   <Transitions/>
</TimeZoneDefinition>

```

 **TimeZoneDefinitionType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|ID  <br/> |Représente l’identificateur unique du fuseau horaire.  <br/> |
|Nom  <br/> |Représente le nom descriptif du fuseau horaire.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Periods](periods.md) <br/> |Représente un tableau d’éléments [Period](period.md) qui définissent le décalage horaire à différentes étapes du fuseau horaire.  <br/> |
|[TransitionsGroups](transitionsgroups.md) <br/> |Représente un tableau d’éléments [TransitionsGroup](transitionsgroup.md) qui spécifient les transitions de fuseau horaire.  <br/> |
|[Transitions](transitions.md) <br/> |Représente un tableau de transitions de fuseau horaire.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[TimeZoneDefinitions](timezonedefinitions.md) <br/> |Représente un tableau de définitions de fuseau horaire.  <br/> |
|[TimeZoneContext](timezonecontext.md) <br/> |Représente la définition de fuseau horaire par défaut à utiliser pour l’application des propriétés DateTime des objets créés, mis à jour et récupérés à l’aide des services web Exchange (EWS).  <br/> |
   
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

