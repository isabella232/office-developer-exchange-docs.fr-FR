---
title: ChangeHighlights
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f9bd7323-44db-4d2f-aaaa-94c2dfdeead6
description: L’élément ChangeHighlights spécifie les modifications apportées entre deux versions d’un message de demande de réunion.
ms.openlocfilehash: 6c78d2c96449ee41032859f90bf51d6e0faa92ae
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463278"
---
# <a name="changehighlights"></a>ChangeHighlights

L’élément **ChangeHighlights** spécifie les modifications apportées entre deux versions d’un message de demande de réunion. 
  
```XML
<ChangeHighlights>
    <HasLocationChanged></HasLocationChanged>
    <Location></Location>
    <HasStartTimeChanged></HasStartTimeChanged>
    <Start></Start>
    <HasEndTimeChanged></HasEndTimeChanged>
    <End></End>
</ChangeHighlights>
```

 **ChangeHighlightsType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[HasLocationChanged](haslocationchanged.md) <br/> |Indique si la propriété Location d’une réunion a été modifiée.  <br/> |
|[Emplacement](location.md) <br/> |Représente l’emplacement d’une réunion ou d’un rendez-vous.  <br/> |
|[HasStartTimeChanged](hasstarttimechanged.md) <br/> |Indique si l’heure de début d’une réunion a changé.  <br/> |
|[Démarrage](start.md) <br/> |Représente le début d’une durée.  <br/> |
|[HasEndTimeChanged](hasendtimechanged.md) <br/> |Indique si l’heure de fin d’une réunion a changé.  <br/> |
|[Fin](end-ex15websvcsotherref.md) <br/> |Représente la fin d’une durée.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Propriété meetingrequest](meetingrequest.md) <br/> |Représente une demande de réunion dans la banque d'informations Exchange.  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma type  <br/> |
|Validation File  <br/> |types. xsd  <br/> |
|Peut être vide  <br/> ||
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

