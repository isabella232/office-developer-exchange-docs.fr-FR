---
title: EndDate (périodicité)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EndDate
api_type:
- schema
ms.assetid: 16026595-26f8-4770-8a6d-0d3e4157effd
description: L’élément EndDate représente la date de fin d’une tâche périodique ou un élément de calendrier dont le type de motif EndDateRecurrence.
ms.openlocfilehash: b8570a069fc0a2d05044a9c85ab2d5c39d70ccdf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756163"
---
# <a name="enddate-recurrence"></a>EndDate (périodicité)

L’élément **EndDate** représente la date de fin d’une tâche périodique ou un élément de calendrier dont le type de motif EndDateRecurrence. 
  
```xml
<EndDate/>
```

 **date**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[EndDateRecurrence](enddaterecurrence.md) <br/> |Décrit la date de début et date de fin de périodicité d’un élément.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Une valeur de texte qui représente une date est obligatoire si cet élément est utilisé. La valeur ne peut pas dépasser 1 septembre, 4500 00:00:00.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

