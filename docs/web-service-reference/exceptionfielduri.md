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
description: L’élément ExceptionFieldURI identifie les erreurs particulières dans une demande. Cet élément est utilisé uniquement dans le cadre d’une réponse d’erreur dans le nœud MessageXml.
ms.openlocfilehash: a47d44098f85d8bacb1e7a2c48a33e478e56c7ac
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44454343"
---
# <a name="exceptionfielduri"></a>ExceptionFieldURI

L’élément **ExceptionFieldURI** identifie les erreurs particulières dans une demande. Cet élément est utilisé uniquement dans le cadre d’une réponse d’erreur dans le nœud [messagexml](messagexml.md) . 
  
```xml
<ExceptionFieldURI FieldURI="" />
```

 **ExceptionPropertyURIType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**FieldURI** <br/> |Identifie une propriété d’une occurrence d’un élément périodique. Cet attribut est obligatoire.  <br/> |
   
#### <a name="fielduri-attribute"></a>Attribut FieldURI

|**Valeur**|**Description**|
|:-----|:-----|
|pièce jointe : nom  <br/> |Identifie le nom de la pièce jointe comme contenant une erreur.  <br/> |
|pièce jointe : ContentType  <br/> |Identifie le type de contenu comme contenant une erreur.  <br/> |
|pièce jointe : contenu  <br/> |Identifie le contenu comme contenant une erreur.  <br/> |
|Périodicité : mois  <br/> |Identifie le champ de mois comme contenant une erreur.  <br/> |
|Périodicité : DayOfWeekIndex  <br/> |Identifie l’index du jour de la semaine comme contenant une erreur.  <br/> |
|Périodicité : DaysOfWeek  <br/> |Identifie la propriété DaysOfWeek comme contenant une erreur.  <br/> |
|Périodicité : DayOfMonth  <br/> |Identifie le DayOfMonth comme contenant une erreur.  <br/> |
|Périodicité : intervalle  <br/> |Identifie l’intervalle comme contenant une erreur.  <br/> |
|Périodicité : NumberOfOccurrences  <br/> |Identifie le nombre d’occurrences contenant une erreur.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[MessageXml](messagexml.md) <br/> |Fournit des informations supplémentaires sur la réponse aux erreurs.  <br/> |
   
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

