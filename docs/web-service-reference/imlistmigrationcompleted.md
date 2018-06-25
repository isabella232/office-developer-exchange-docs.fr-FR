---
title: ImListMigrationCompleted
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 6eed9502-5d9e-4345-ba23-3582ff487147
description: L’élément ImListMigrationCompleted indique si la banque d’informations Exchange contient les éléments de messagerie instantanées utilisés par les clients de messagerie instantanée.
ms.openlocfilehash: 25f1b583b354a71958fbc8052c492726dc0eb7db
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827893"
---
# <a name="imlistmigrationcompleted"></a>ImListMigrationCompleted

L’élément **ImListMigrationCompleted** indique si la banque d’informations Exchange contient les éléments utilisés par les clients de messagerie instantanée de la messagerie instantanée. 
  
```XML
<ImListMigrationCompleted>true | false</ImListMigrationCompleted>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[SetImListMigrationCompleted](setimlistmigrationcompleted.md)
  
## <a name="text-value"></a>Valeur de texte

Une valeur de texte de **la valeur true** pour l’élément **ImListMigrationCompleted** indique que les contacts de messagerie instantanée store a été migré vers la version d’Exchange stockent. La valeur **false** indique que le magasin de contacts de messagerie instantanée n’a pas été migré. 
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> ||
   

