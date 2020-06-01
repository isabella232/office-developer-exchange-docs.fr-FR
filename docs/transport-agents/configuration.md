---
title: Configuration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- configuration
api_type:
- schema
ms.assetid: 6fc04e4d-657a-4999-9431-186ccb7832b5
description: 'Dernière modification : 17 septembre 2015'
ms.openlocfilehash: b886851b9a0c17d58428f49281d664930d0e4070
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461561"
---
# <a name="configuration"></a>Configuration
  
**S’applique à :** Exchange Server 2013
  
L’élément **configuration** est l’élément racine du fichier de configuration des agents. 
  
- [configuration](configuration.md) 
- [mexRuntime](mexruntime.md)
  
```XML
<configuration>
      <mexRuntime/>
</configuration>
```

**configurationType (complexType)**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[mexRuntime](mexruntime.md) <br/> |Contient des éléments qui définissent les informations de configuration des informations de configuration et de surveillance de l’agent pour les agents SMTP et de routage installés.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |Ce fichier ne définit pas d’espace de noms.  <br/> |
|Nom du schéma  <br/> |Non disponible.  <br/> |
|Fichier de validation  <br/> |Non disponible.  <br/> |
|Peut être vide  <br/> |Faux.  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments du fichier de configuration des agents pour Exchange 2013](agents-configuration-file-elements-for-exchange-2013.md)

