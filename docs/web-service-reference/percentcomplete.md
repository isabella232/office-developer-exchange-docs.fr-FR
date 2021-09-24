---
title: PercentComplete
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- PercentComplete
api_type:
- schema
ms.assetid: 58a67f8a-c4dc-42dc-97ae-a9e5cc672d2d
description: L’élément PercentComplete décrit l’état d’achèvement d’une tâche.
ms.openlocfilehash: 48e6163377d51d64f63e966c525def48f930733e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59519246"
---
# <a name="percentcomplete"></a>PercentComplete

**L’élément PercentComplete** décrit l’état d’achèvement d’une tâche. 
  
```xml
<PercentComplete/>
```

 **double**
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

Une valeur de texte qui représente un integer entre 0 et 100 est requise.
  
## <a name="remarks"></a>Remarques

La **définition de PercentComplete** sur 100 a le même effet que la définition de l’élément [CompleteDate](completedate.md) ou la définition de l’élément [Status](status.md) sur **Completed**. Dans une requête qui définit au moins deux de ces propriétés, la dernière propriété traitée détermine la valeur définie pour ces éléments. Par exemple, si **PercentComplete** a la valeur 100, [CompleteDate](completedate.md) est le 1er janvier 2007 et [que l’état](status.md) [](status.md) est NotStarted et que les propriétés sont diffusées dans cet ordre, l’effet sera de définir l’état de la tâche sur NotStarted, [CompleteDate](completedate.md) sur **null** et **percentComplete** sur 0. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.
  
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

