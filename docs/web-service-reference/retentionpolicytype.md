---
title: RetentionPolicyType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: abce5b3e-971d-42fc-aeea-caa7202214de
description: L’élément RetentionPolicyType spécifie le type de stratégie de rétention appliqué aux éléments d’une conversation.
ms.openlocfilehash: 3900718f10e1e11d5864ebf7e64a3e1e22aa45c7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462870"
---
# <a name="retentionpolicytype"></a>RetentionPolicyType

L’élément **RetentionPolicyType** spécifie le type de stratégie de rétention appliqué aux éléments d’une conversation. 
  
```XML
<RetentionPolicyType> Delete | Archive </RetentionPolicyType>
```

 **RetentionType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[ConversationAction](conversationaction.md)
  
## <a name="text-value"></a>Valeur texte

La valeur de texte de l’élément **RetentionPolicyType** est le type de rétention appliqué aux éléments d’une conversation. La valeur texte de **Delete** indique que les éléments de la conversation sont supprimés lorsque le blocage de rétention expire. La valeur texte d' **Archive** indique que les éléments de la conversation sont déplacés vers la boîte aux lettres d’archivage lorsque le blocage de rétention expire. 
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> ||
   

