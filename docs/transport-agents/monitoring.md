---
title: surveillance
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- monitoring
api_type:
- schema
ms.assetid: 350d7b46-9260-41a7-8613-3cb8cc1b29a5
description: 'Dernière modification : 17 septembre 2015'
ms.openlocfilehash: 1b5484467def0bf3d22ba0707357977d5ed461ff
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755139"
---
# <a name="monitoring"></a>surveillance
  
**S’applique à :** Exchange Server 2013
  
L’élément de **surveillance** contient des informations de configuration qui définit comment et quand le service de transport frontal ou le service de Transport analyse les agents qui sont installés. 
  
- [configuration](configuration.md)  
- [mexRuntime](mexruntime.md)  
- [surveillance](monitoring.md)
  
```XML
<monitoring>
   <agentExecution/>
   <messageSnapshot/>
</monitoring>
```

**monitoringType (type complexe)**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[agentExecution](agentexecution.md) <br/> |Définit la durée, en millisecondes, pour l’accès au Client ou le serveur de boîtes aux lettres d’attente d’un agent renvoyer à partir d’un événement avant de les écrire dans le journal des événements.  <br/> |
|[messageSnapshot](messagesnapshot.md) <br/> |Contient un attribut qui spécifie si la fonctionnalité de suivi du pipeline est activée pour l’accès au Client ou le serveur de boîtes aux lettres.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[mexRuntime](mexruntime.md) <br/> |Contient des éléments qui définissent les informations de configuration pour l’agent de surveillance et les informations de configuration pour SMTP et les agents de routage qui sont installés.  <br/> |
   
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |Ce fichier ne définit pas un espace de noms.  <br/> |
|Nom du schéma  <br/> |N’est pas disponible.  <br/> |
|Fichier de validation  <br/> |N’est pas disponible.  <br/> |
|Peut être vide  <br/> |Faux  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments du fichier de configuration agents pour Exchange 2013](agents-configuration-file-elements-for-exchange-2013.md)

