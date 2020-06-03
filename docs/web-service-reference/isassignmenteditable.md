---
title: IsAssignmentEditable
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsAssignmentEditable
api_type:
- schema
ms.assetid: 0ddf9181-f65e-4ad6-ad69-7b074ea0f2e7
description: L’élément IsAssignmentEditable représente le type de tâche.
ms.openlocfilehash: 5eb091b24e2c97f7aa6072044fed998b6c9c1651
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468053"
---
# <a name="isassignmenteditable"></a>IsAssignmentEditable

L’élément **IsAssignmentEditable** représente le type de tâche. 
  
```xml
<IsAssignmentEditable/>
```

 **entier**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Tâche](task.md) <br/> |Représente une tâche dans la banque d'informations Exchange.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Cette propriété est en lecture seule. Le tableau suivant répertorie les valeurs possibles.
  
|**Valeur**|**Description**|
|:-----|:-----|
|0  <br/> |Valeur par défaut pour tous les éléments de tâche.  <br/> |
|1   <br/> |Une demande de tâche.  <br/> |
|n°2  <br/> |Acceptation d’une tâche d’un destinataire d’une demande de tâche.  <br/> |
|3  <br/> |Une tâche de refus d’un destinataire d’une demande de tâche.  <br/> |
|4   <br/> |Mise à jour d’une demande de tâche précédente.  <br/> |
|5   <br/> |Non utilisé.  <br/> |
   
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

