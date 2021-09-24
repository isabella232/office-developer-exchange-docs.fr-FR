---
title: EndDate (Recurrence)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- EndDate
api_type:
- schema
ms.assetid: 16026595-26f8-4770-8a6d-0d3e4157effd
description: L’élément EndDate représente la date de fin d’une tâche périodique ou d’un élément de calendrier qui a le type de modèle EndDateRecurrence.
ms.openlocfilehash: c53d83a3fb2f3a6a841d7e16c94d20dd3c7a92a4
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540091"
---
# <a name="enddate-recurrence"></a>EndDate (Recurrence)

**L’élément EndDate** représente la date de fin d’une tâche périodique ou d’un élément de calendrier qui a le type de modèle EndDateRecurrence. 
  
```xml
<EndDate/>
```

 **date**
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
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte qui représente une date est requise si cet élément est utilisé. La valeur ne peut pas être supérieure au 1er septembre 4500 00:00:00.
  
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

