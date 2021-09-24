---
title: monitoring
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- monitoring
api_type:
- schema
ms.assetid: 350d7b46-9260-41a7-8613-3cb8cc1b29a5
description: 'Last modified: September 17, 2015'
ms.openlocfilehash: 215737fb43e1dbef9b7dd11baea1d3f922df7d34
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540364"
---
# <a name="monitoring"></a>monitoring
  
**S’applique à :** Exchange Server 2013
  
**L’élément de** surveillance contient des informations de configuration qui définissent comment et quand le service de transport frontal ou le service de transport surveille les agents installés. 
  
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
|[agentExecution](agentexecution.md) <br/> |Définit le temps, en millisecondes, pendant que le serveur d’accès au client ou de boîtes aux lettres attend le retour d’un agent d’un événement avant d’écrire dans le journal des événements.  <br/> |
|[messageSnapshot](messagesnapshot.md) <br/> |Contient un attribut qui spécifie si la fonctionnalité de suivi du pipeline est activée pour l’accès au client ou le serveur de boîtes aux lettres.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[mexRuntime](mexruntime.md) <br/> |Contient des éléments qui définissent les informations de configuration pour la surveillance des agents et les informations de configuration pour SMTP et les agents de routage installés.  <br/> |
   
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |Ce fichier ne définit pas d’espace de noms.  <br/> |
|Nom du schéma  <br/> |Non disponible.  <br/> |
|Fichier de validation  <br/> |Non disponible.  <br/> |
|Peut être vide  <br/> |Faux.  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments de fichier de configuration des agents Exchange 2013](agents-configuration-file-elements-for-exchange-2013.md)

