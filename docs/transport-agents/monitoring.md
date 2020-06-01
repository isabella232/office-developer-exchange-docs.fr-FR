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
ms.openlocfilehash: 5614ac2c6428da9b6845769a9335486d3ded5754
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455827"
---
# <a name="monitoring"></a>surveillance
  
**S’applique à :** Exchange Server 2013
  
L’élément **Monitoring** contient des informations de configuration qui définissent comment et quand le service de transport frontal ou le service de transport surveille les agents installés. 
  
- [configuration](configuration.md)  
- [mexRuntime](mexruntime.md)  
- [surveillance](monitoring.md)
  
```XML
<monitoring>
   <agentExecution/>
   <messageSnapshot/>
</monitoring>
```

**monitoringType (complexType)**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[agentExecution](agentexecution.md) <br/> |Définit le temps, en millisecondes, au-delà duquel le serveur d’accès au client ou de boîtes aux lettres doit attendre qu’un agent renvoie à partir d’un événement avant d’écrire dans le journal des événements.  <br/> |
|[messageSnapshot](messagesnapshot.md) <br/> |Contient un attribut qui indique si la fonctionnalité de suivi de pipeline est activée pour le serveur d’accès au client ou de boîtes aux lettres.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[mexRuntime](mexruntime.md) <br/> |Contient des éléments qui définissent les informations de configuration des informations de configuration et de surveillance de l’agent pour les agents SMTP et de routage installés.  <br/> |
   
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |Ce fichier ne définit pas d’espace de noms.  <br/> |
|Nom du schéma  <br/> |Non disponible.  <br/> |
|Fichier de validation  <br/> |Non disponible.  <br/> |
|Peut être vide  <br/> |Faux.  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments du fichier de configuration des agents pour Exchange 2013](agents-configuration-file-elements-for-exchange-2013.md)

