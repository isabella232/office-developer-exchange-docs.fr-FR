---
title: CompleteDate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CompleteDate
api_type:
- schema
ms.assetid: b2b53b87-6a0b-4a55-bcfc-3bf67d3c1700
description: L’élément CompleteDate représente la date à laquelle un élément a été effectué.
ms.openlocfilehash: 00a1ec25be737ec0a5cc874063e1bce19a96cee0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755519"
---
# <a name="completedate"></a>CompleteDate

L’élément **CompleteDate** représente la date à laquelle un élément a été effectué. 
  
```xml
<CompleteDate/>
```

 **DateTime**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Tâche](task.md) <br/> |Représente une tâche dans la banque d'informations Exchange.  <br/> |
|[Flag](flag.md) <br/> |Spécifie un indicateur sur un élément de boîte aux lettres.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Une valeur de texte qui représente la date et l’heure est obligatoire si cet élément est utilisé.
  
## <a name="remarks"></a>Remarques

Définition de **CompleteDate** a le même effet que la définition [PercentComplete](percentcomplete.md) à 100 ou [état](status.md) sur **terminée**. Dans une demande qu’au moins deux jeux de ces propriétés, la dernière propriété traitée détermine la valeur est définie pour ces éléments. Par exemple, si [PercentComplete](percentcomplete.md) est 100, **CompleteDate** est le 1er janvier 2007, [l’état](status.md) est **NotStarted**et les propriétés sont transmises dans l’ordre, l’effet sera pour définir l' [état](status.md) de la tâche à **NotStarted **, le [CompleteDate](completedate.md) à **null**et [PercentComplete](percentcomplete.md) à 0. 
  
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


[Création de tâches](http://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
  
[Suppression de tâches](http://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

