---
title: Terminé
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
description: L’élément Completed représente la date à laquelle un élément a été terminé.
ms.openlocfilehash: fff3d5d3105bf63c9cdd34cbcf828d57ca287b86
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461421"
---
# <a name="completedate"></a>Terminé

L’élément **Completed** représente la date à laquelle un élément a été terminé. 
  
```xml
<CompleteDate/>
```

 **DateTime**
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
|[Indicateur](flag.md) <br/> |Spécifie un indicateur sur un élément de boîte aux lettres.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte qui représente la date et l’heure est requise si cet élément est utilisé.
  
## <a name="remarks"></a>Remarques

La définition de l’option **Completed** a le même effet que celle de la valeur de [PourcentageAchevé](percentcomplete.md) sur 100 ou l' [État](status.md) **terminé**. Dans une demande qui définit au moins deux de ces propriétés, la dernière propriété traitée détermine la valeur définie pour ces éléments. Par exemple, si [PercentComplete](percentcomplete.md) est 100, **recompleted** est le 1er janvier 2007 et [Status](status.md) est **NotStarted**, et que les propriétés sont diffusées dans cet ordre, l’effet est de définir l' [État](status.md) de la tâche sur **NotStarted**, la valeur de la propriété [Completed](completedate.md) sur **null**et [PercentComplete](percentcomplete.md) sur 0. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML EWS dans Exchange](ews-xml-elements-in-exchange.md)


[Création de tâches](https://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
  
[Suppression de tâches](https://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

