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
ms.openlocfilehash: 5848d52a68c8c3f747614015e49becb34bc4cfd8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755109"
---
# <a name="agentexecution"></a>agentExecution
  
**S’applique à :** Exchange Server 2013 
  
L’élément **agentExecution** définit la durée, en millisecondes, pour le serveur d’accès au Client ou de la boîte aux lettres doit attendre un agent renvoyer à partir d’un événement avant de les écrire dans le journal des événements. 
  
- [configuration](configuration.md)  
- [surveillance](monitoring.md)
- [agentExecution](agentexecution.md)
  
```XML
<agentExecution timeLimitInMilliseconds="" />
```

**agentExecutionType (type complexe)**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**timeLimitInMilliseconds** <br/> |Une valeur entière positive qui spécifie la durée, en millisecondes, pour le serveur doit attendre pour un agent renvoyer à partir d’un événement avant qu’il écrit un message d’avertissement dans le journal des événements. Performances peuvent diminuer si cette valeur est trop petite. La valeur suggérée pour cet attribut est 300 000, ce qui équivaut à 5 minutes.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[surveillance](monitoring.md) <br/> |Contient des informations de configuration qui définit comment et quand le service de Transport frontal ou le service de Transport analyse les agents qui sont installés.  <br/> |
   
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |Ce fichier ne définit pas un espace de noms.  <br/> |
|Nom du schéma  <br/> |N’est pas disponible.  <br/> |
|Fichier de validation  <br/> |N’est pas disponible.  <br/> |
|Peut être vide  <br/> |Faux  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments du fichier de configuration agents pour Exchange 2013](agents-configuration-file-elements-for-exchange-2013.md)

