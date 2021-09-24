---
title: DeleteFromFolderStateDefinition
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 3aba59a0-f12a-48b5-842b-11cf4530dd51
description: L’élément DeleteFromFolderStateDefinition spécifie l’état lorsqu’un élément est supprimé d’un dossier.
ms.openlocfilehash: 270edfc0b7abd70b74ff8c8b4353140ec5fbe27b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510238"
---
# <a name="deletefromfolderstatedefinition"></a>DeleteFromFolderStateDefinition

**L’élément DeleteFromFolderStateDefinition** spécifie l’état lorsqu’un élément est supprimé d’un dossier. 
  
```XML
<DeleteFromFolderStateDefinition>
    <OccurrenceDate></OccurrenceDate>
    <IsOccurrencePresent></IsOccurrencePresent>
</DeleteFromFolderStateDefinition>
```

 **DeleteFromFolderStateDefinitionType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Occurrence (transition de fuseau horaire)](occurrence-time-zone-transition.md) <br/> |Spécifie la date de l’occurrence d’un élément de calendrier.  <br/> |
|[IsOccurrencePresent](isoccurrencepresent.md) <br/> |Spécifie une valeur de booléen qui indique si une occurrence de l’élément de calendrier est présente.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[StateDefinition](statedefinition.md) <br/> |Spécifie une définition d’état.  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma type  <br/> |
|Validation File  <br/> |types.xsd  <br/> |
|Peut être vide  <br/> ||
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

