---
title: agentExecution
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- agentExecution
api_type:
- schema
ms.assetid: 600c4690-941c-45af-a906-5528748d09cd
description: 'Dernière modification : 17 septembre 2015'
ms.openlocfilehash: 457257e59fb37659daf2f91b0fa5dfced5c48c03
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44446489"
---
# <a name="agentexecution"></a>agentExecution
  
**S’applique à :** Exchange Server 2013 
  
L’élément **agentExecution** définit le temps, en millisecondes, pendant lequel le serveur d’accès au client ou de boîtes aux lettres doit attendre qu’un agent renvoie à partir d’un événement avant d’écrire dans le journal des événements. 
  
- [configuration](configuration.md)  
- [surveillance](monitoring.md)
- [agentExecution](agentexecution.md)
  
```XML
<agentExecution timeLimitInMilliseconds="" />
```

**agentExecutionType (complexType)**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**timeLimitInMilliseconds** <br/> |Valeur entière positive qui spécifie le temps, en millisecondes, pendant lequel le serveur doit attendre qu’un agent renvoie à partir d’un événement avant d’écrire un avertissement dans le journal des événements. Les performances peuvent diminuer si cette valeur est trop petite. La valeur suggérée pour cet attribut est 300 000, ce qui équivaut à 5 minutes.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[surveillance](monitoring.md) <br/> |Contient des informations de configuration qui définissent comment et quand le service de transport frontal ou le service de transport surveille les agents installés.  <br/> |
   
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |Ce fichier ne définit pas d’espace de noms.  <br/> |
|Nom du schéma  <br/> |Non disponible.  <br/> |
|Fichier de validation  <br/> |Non disponible.  <br/> |
|Peut être vide  <br/> |Faux.  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments du fichier de configuration des agents pour Exchange 2013](agents-configuration-file-elements-for-exchange-2013.md)

