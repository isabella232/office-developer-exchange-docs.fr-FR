---
title: ExceptionFieldURI
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExceptionFieldURI
api_type:
- schema
ms.assetid: 7afda93a-0f8c-4c9e-8e09-f1b0bfc928bf
description: L’élément ExceptionFieldURI identifie les erreurs spécifiques dans une requête. Cet élément est utilisé uniquement dans le cadre d’une réponse d’erreur dans le nœud MessageXml.
ms.openlocfilehash: 79909405179cec0d0b86ad12bf52031e1daeb790
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756234"
---
# <a name="exceptionfielduri"></a>ExceptionFieldURI

L’élément **ExceptionFieldURI** identifie les erreurs spécifiques dans une requête. Cet élément est utilisé uniquement dans le cadre d’une réponse d’erreur dans le nœud [MessageXml](messagexml.md) . 
  
```xml
<ExceptionFieldURI FieldURI="" />
```

 **ExceptionPropertyURIType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**FieldURI** <br/> |Identifie une propriété d’une occurrence d’un élément périodique. Cet attribut est requis.  <br/> |
   
#### <a name="fielduri-attribute"></a>Attribut FieldURI

|**Valeur**|**Description**|
|:-----|:-----|
|Nom de la pièce jointe :  <br/> |Identifie le nom de la pièce jointe comme contenant une erreur.  <br/> |
|pièce jointe : ContentType  <br/> |Identifie le type de contenu comme contenant une erreur.  <br/> |
|Contenu des pièces jointes :  <br/> |Identifie le contenu comme contenant une erreur.  <br/> |
|Mois de périodicité :  <br/> |Identifie le champ mois comme contenant une erreur.  <br/> |
|Périodicité : DayOfWeekIndex  <br/> |Identifie le jour de l’index de semaine comme contenant une erreur.  <br/> |
|Périodicité : DaysOfWeek  <br/> |Identifie la propriété DaysOfWeek comme contenant une erreur.  <br/> |
|Périodicité : DayOfMonth  <br/> |Identifie le DayOfMonth comme contenant une erreur.  <br/> |
|Intervalle de périodicité :  <br/> |Identifie l’intervalle comme contenant une erreur.  <br/> |
|Périodicité : NumberOfOccurrences  <br/> |Identifie le nombre d’occurrences comme contenant une erreur.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[MessageXml](messagexml.md) <br/> |Fournit des informations de réponse d’erreur.  <br/> |
   
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

