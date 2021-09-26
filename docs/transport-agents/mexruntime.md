---
title: mexRuntime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- mexRuntime
api_type:
- schema
ms.assetid: eabb2f12-10a7-4ce2-ae4b-9c04010c765f
description: 'Last modified: September 17, 2015'
ms.openlocfilehash: c7ae630a01ac0339433a7c78859c06006efab4b5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546909"
---
# <a name="mexruntime"></a>mexRuntime
  
**S’applique à :** Exchange Server 2013
  
**L’élément mexRuntime** contient des éléments qui définissent les informations de configuration pour la surveillance des agents et les informations de configuration pour SMTP et les agents de routage installés. 
  
- [configuration](configuration.md)  
- [mexRuntime](mexruntime.md)
  
```XML
<mexRuntime>
   <monitoring/>
   <agentList/>
</mexRuntime>
```

**mexRuntimeType (complexType)**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[surveillance](monitoring.md) <br/> |Contient des informations de configuration qui définissent comment et quand le transport surveille les agents qui sont installés.  <br/> |
|[agentList](agentlist.md) <br/> |Contient un [élément agent](agent.md) pour chaque agent installé.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[configuration](configuration.md) <br/> |Élément racine du fichier de configuration des agents.  <br/> |
   
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |Ce fichier ne définit pas d’espace de noms.  <br/> |
|Nom du schéma  <br/> |Non disponible.  <br/> |
|Fichier de validation  <br/> |Non disponible.  <br/> |
|Peut être vide  <br/> |Faux.  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments de fichier de configuration des agents Exchange 2013](agents-configuration-file-elements-for-exchange-2013.md)

