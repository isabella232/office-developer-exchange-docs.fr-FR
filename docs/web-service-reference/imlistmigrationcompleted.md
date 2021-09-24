---
title: ImListMigrationCompleted
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 6eed9502-5d9e-4345-ba23-3582ff487147
description: L’élément ImListMigrationCompleted indique si la Exchange contient les éléments de messagerie instantanée utilisés par les clients de messagerie instantanée.
ms.openlocfilehash: b55f3d72259897d7bdf46b351421b0148a41b93e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59514612"
---
# <a name="imlistmigrationcompleted"></a>ImListMigrationCompleted

**L’élément ImListMigrationCompleted** indique si le magasin Exchange contient les éléments de messagerie instantanée utilisés par les clients de messagerie instantanée. 
  
```XML
<ImListMigrationCompleted>true | false</ImListMigrationCompleted>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[SetImListMigrationCompleted](setimlistmigrationcompleted.md)
  
## <a name="text-value"></a>Valeur texte

Une valeur de texte **true** pour l’élément **ImListMigrationCompleted** indique que le magasin de contacts de messagerie instantanée a été migré vers le magasin Exchange messagerie instantanée. La valeur **false indique** que le magasin de contacts de message instantané n’a pas été migré. 
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> ||
   

