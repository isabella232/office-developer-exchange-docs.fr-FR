---
title: messageSnapshot
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- messageSnapshot
api_type:
- schema
ms.assetid: f157e44c-b950-463f-b086-31d5da94b7ff
description: 'Dernière modification : 17 septembre 2015'
ms.openlocfilehash: 4b814def8eef8fb452d2e754c5f6787d644055f7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755140"
---
# <a name="messagesnapshot"></a>messageSnapshot

**S’applique à :** Exchange Server 2013
  
L’élément **messageSnapshot** contient un attribut qui spécifie si la fonctionnalité de suivi du pipeline est activée pour le serveur Exchange qui a l’accès au Client ou le rôle serveur de boîtes aux lettres. 
  
- [configuration](configuration.md)  
- [mexRuntime](mexruntime.md) 
- [surveillance](monitoring.md) 
- [messageSnapshot](messagesnapshot.md)
  
```XML
<messageSnapshot enabled="" />
```

**messageSnapshotType (Boolean)**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**activé** <br/> |Une valeur de type Boolean qui indique si la fonctionnalité de suivi du pipeline est activée pour l’accès au Client ou le serveur de boîtes aux lettres. La valeur est **true** si le suivi du pipeline est activé ; dans le cas contraire, la valeur est **false** ou l’élément n’est pas présent.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[surveillance](monitoring.md) <br/> |Contient des informations de configuration qui définit comment et quand le service de transport analyse les agents qui sont installés.  <br/> |
   
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |Ce fichier ne définit pas un espace de noms.  <br/> |
|Nom du schéma  <br/> |N’est pas disponible.  <br/> |
|Fichier de validation  <br/> |N’est pas disponible.  <br/> |
|Peut être vide  <br/> |Faux  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments du fichier de configuration agents pour Exchange 2013](agents-configuration-file-elements-for-exchange-2013.md)

