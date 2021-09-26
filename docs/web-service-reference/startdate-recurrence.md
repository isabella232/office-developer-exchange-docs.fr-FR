---
title: StartDate (périodicité)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- StartDate
api_type:
- schema
ms.assetid: bd65ac06-b3ac-4c9b-9568-3e4dc94378e7
description: L’élément StartDate représente la date de début d’une tâche périodique ou d’un élément de calendrier.
ms.openlocfilehash: 50f83e5c97d346cc3f7dfced1ee71aa3f9f38ed5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59545866"
---
# <a name="startdate-recurrence"></a>StartDate (périodicité)

**L’élément StartDate** représente la date de début d’une tâche périodique ou d’un élément de calendrier. 
  
```xml
<StartDate/>
```

**Date**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[EndDateRecurrence](enddaterecurrence.md) <br/> |Décrit la date de début et la date de fin d’une récurrence d’élément.  <br/> |
|[NoEndRecurrence](noendrecurrence.md) <br/> |Décrit la date de début d’une récurrence d’élément qui n’a pas de date de fin définie.  <br/> |
|[NumberedRecurrence](numberedrecurrence.md) <br/> |Décrit la date de début et le nombre d’occurrences d’un élément périodique.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte qui représente une date est requise si cet élément est utilisé. La valeur ne peut pas être inférieure à avr, 1, 1601 00:00:00.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

