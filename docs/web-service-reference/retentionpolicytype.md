---
title: RetentionPolicyType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: abce5b3e-971d-42fc-aeea-caa7202214de
description: L’élément RetentionPolicyType spécifie le type de stratégie de rétention appliqué aux éléments d’une conversation.
ms.openlocfilehash: 961f72c35443e9f265e9313166fa77c8cd93d654
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59509384"
---
# <a name="retentionpolicytype"></a>RetentionPolicyType

**L’élément RetentionPolicyType** spécifie le type de stratégie de rétention appliqué aux éléments d’une conversation. 
  
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

La valeur de texte de **l’élément RetentionPolicyType** est le type de rétention appliqué aux éléments d’une conversation. La valeur de texte **Delete** indique que les éléments de la conversation sont supprimés à l’expiration de la conservation de rétention. La valeur de texte **Archive** indique que les éléments de la conversation sont déplacés vers la boîte aux lettres d’archivage à l’expiration de la conservation de rétention. 
  
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
   

