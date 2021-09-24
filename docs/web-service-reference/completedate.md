---
title: CompleteDate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CompleteDate
api_type:
- schema
ms.assetid: b2b53b87-6a0b-4a55-bcfc-3bf67d3c1700
description: L’élément CompleteDate représente la date à laquelle un élément a été terminé.
ms.openlocfilehash: 07f6034b4fd91d22ad07167d931bcd02a74782f9
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518777"
---
# <a name="completedate"></a>CompleteDate

**L’élément CompleteDate** représente la date à laquelle un élément a été terminé. 
  
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

La **définition de CompleteDate** a le même effet que la définition de [PercentComplete](percentcomplete.md) sur 100 ou [d’état](status.md) **sur Terminé**. Dans une requête qui définit au moins deux de ces propriétés, la dernière propriété traitée détermine la valeur définie pour ces éléments. Par exemple, si [PercentComplete](percentcomplete.md) a la valeur 100, **CompleteDate** est le 1er janvier 2007 et [que l’état](status.md) [](status.md) est **NotStarted** et que les propriétés sont diffusées dans cet ordre, l’effet sera de définir l’état de la tâche sur **NotStarted,** [CompleteDate](completedate.md) sur **null** et [PercentComplete](percentcomplete.md) sur 0. 
  
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

