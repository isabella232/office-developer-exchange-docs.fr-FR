---
title: État
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Status
api_type:
- schema
ms.assetid: 80121e41-291b-4fc0-a55e-6f677d4b5fb5
description: L’élément Status représente l’état d’un élément de tâche.
ms.openlocfilehash: 224b61913a5ae8e5b4aa0d756a9f2488df2741bd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829584"
---
# <a name="status"></a>État

L’élément **Status** représente l’état d’un élément de tâche. 
  
```xml
<Status/>
```

 **TaskStatusType**
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
   
## <a name="text-value"></a>Valeur de texte

Une valeur texte est requise. Les valeurs de texte possibles de cet élément sont les suivantes :
  
- NotStarted
    
- InProgress
    
- Achevé
    
- WaitingOnOthers
    
- Différé
    
## <a name="remarks"></a>Remarques

Définition de [CompleteDate](completedate.md) a le même effet que la définition [PercentComplete](percentcomplete.md) à 100 ou **état** sur **terminée**. Dans une demande qu’au moins deux jeux de ces propriétés, la dernière propriété traitée détermine la valeur est définie pour ces éléments. Par exemple, si **PercentComplete** est 100, **CompleteDate** est 1/1/2007 et **l’état** est NotStarted et les propriétés sont transmises dans l’ordre suivant, l’effet sera pour définir l' **état** de la tâche est NotStarted, la **CompleteDate ** **null**et le **PercentComplete** à 0. 
  
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


[Création de tâches](http://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
  
[Suppression de tâches](http://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

