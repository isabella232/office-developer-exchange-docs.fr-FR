---
title: ExceptionFieldURI
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ExceptionFieldURI
api_type:
- schema
ms.assetid: 7afda93a-0f8c-4c9e-8e09-f1b0bfc928bf
description: L’élément ExceptionFieldURI identifie des erreurs particulières dans une demande. Cet élément est utilisé uniquement dans le cadre d’une réponse d’erreur dans le nœud MessageXml.
ms.openlocfilehash: 7368fd51e8eca2081b1fd50c86bce9ffa469c6b1
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59524328"
---
# <a name="exceptionfielduri"></a>ExceptionFieldURI

**L’élément ExceptionFieldURI** identifie des erreurs particulières dans une demande. Cet élément est utilisé uniquement dans le cadre d’une réponse d’erreur dans le [nœud MessageXml.](messagexml.md) 
  
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
|attachment:Name  <br/> |Identifie le nom de la pièce jointe comme contenant une erreur.  <br/> |
|attachment:ContentType  <br/> |Identifie le type de contenu comme contenant une erreur.  <br/> |
|attachment:Content  <br/> |Identifie le contenu comme contenant une erreur.  <br/> |
|recurrence:Month  <br/> |Identifie le champ mois comme contenant une erreur.  <br/> |
|recurrence:DayOfWeekIndex  <br/> |Identifie l’index du jour de la semaine comme contenant une erreur.  <br/> |
|recurrence:DaysOfWeek  <br/> |Identifie la propriété DaysOfWeek comme contenant une erreur.  <br/> |
|recurrence:DayOfMonth  <br/> |Identifie dayOfMonth comme contenant une erreur.  <br/> |
|recurrence:Interval  <br/> |Identifie l’intervalle comme contenant une erreur.  <br/> |
|recurrence:NumberOfOccurrences  <br/> |Identifie le nombre d’occurrences comme contenant une erreur.  <br/> |
   
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

