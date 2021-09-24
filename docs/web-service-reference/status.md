---
title: Statut
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Status
api_type:
- schema
ms.assetid: 80121e41-291b-4fc0-a55e-6f677d4b5fb5
description: L’élément Status représente l’état d’un élément de tâche.
ms.openlocfilehash: 5ec50e3f0c06ad3ec8301ddbe8e7bd249b1e8fe9
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59525539"
---
# <a name="status"></a>Statut

**L’élément Status** représente l’état d’un élément de tâche. 
  
```xml
<Status/>
```

 **TaskStatusType**
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

Une valeur de texte est requise. Voici les valeurs de texte possibles pour cet élément :
  
- NotStarted
    
- InProgress
    
- Terminé
    
- WaitingOnOthers
    
- Différé
    
## <a name="remarks"></a>Remarques

La [définition de CompleteDate](completedate.md) a le même effet que la définition de [PercentComplete](percentcomplete.md) sur 100 ou **d’état** **sur Terminé**. Dans une requête qui définit au moins deux de ces propriétés, la dernière propriété traitée détermine la valeur définie pour ces éléments. Par exemple, si **PercentComplete** a la valeur 100, **CompleteDate** est 1/1/2007 et **status** is NotStarted et  que les propriétés sont diffusées dans cet ordre, l’effet est de définir l’état de la tâche sur NotStarted, **CompleteDate** sur **null** et **percentComplete** sur 0. 
  
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

