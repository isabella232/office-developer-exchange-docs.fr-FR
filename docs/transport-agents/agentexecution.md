---
title: agentExecution
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- agentExecution
api_type:
- schema
ms.assetid: 600c4690-941c-45af-a906-5528748d09cd
description: 'Last modified: September 17, 2015'
ms.openlocfilehash: 04a53e2698c66326943bcd083c775b53f5c6d5d5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513058"
---
# <a name="agentexecution"></a>agentExecution
  
**S’applique à :** Exchange Server 2013 
  
**L’élément agentExecution** définit le temps, en millisecondes, pendant que le serveur d’accès au client ou de boîtes aux lettres attend le retour d’un agent d’un événement avant d’écrire dans le journal des événements. 
  
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
|**timeLimitInMilliseconds** <br/> |Valeur d’un nombre réel positif qui spécifie le temps, en millisecondes, pendant que le serveur attend le retour d’un agent à partir d’un événement avant d’écrire un avertissement dans le journal des événements. Les performances peuvent diminuer si cette valeur est trop petite. La valeur suggérée pour cet attribut est 300 000, ce qui équivaut à 5 minutes.  <br/> |
   
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

- [Éléments de fichier de configuration des agents Exchange 2013](agents-configuration-file-elements-for-exchange-2013.md)

