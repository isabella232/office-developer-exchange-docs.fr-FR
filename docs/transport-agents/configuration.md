---
title: configuration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- configuration
api_type:
- schema
ms.assetid: 6fc04e4d-657a-4999-9431-186ccb7832b5
description: 'Last modified: September 17, 2015'
ms.openlocfilehash: 35fcb131fbe552a38d9f7eb6022eb5fb52db44b7
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516145"
---
# <a name="configuration"></a>configuration
  
**S’applique à :** Exchange Server 2013
  
**L’élément de configuration** est l’élément racine du fichier de configuration des agents. 
  
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
|[mexRuntime](mexruntime.md) <br/> |Contient des éléments qui définissent les informations de configuration pour la surveillance des agents et les informations de configuration pour SMTP et les agents de routage installés.  <br/> |
   
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

- [Éléments de fichier de configuration des agents Exchange 2013](agents-configuration-file-elements-for-exchange-2013.md)

