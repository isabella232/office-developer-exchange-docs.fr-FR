---
title: RetentionPolicyType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: abce5b3e-971d-42fc-aeea-caa7202214de
description: L’élément RetentionPolicyType Spécifie le type de stratégie de rétention appliqué aux éléments d’une conversation.
ms.openlocfilehash: dacb3fa75611cbd6e6e29eab7c791dfd8964c9ec
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829229"
---
# <a name="retentionpolicytype"></a>RetentionPolicyType

L’élément **RetentionPolicyType** Spécifie le type de stratégie de rétention appliqué aux éléments d’une conversation. 
  
```XML
<RetentionPolicyType> Delete | Archive </RetentionPolicyType>
```

 **RetentionType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[ConversationAction](conversationaction.md)
  
## <a name="text-value"></a>Valeur de texte

La valeur de texte de l’élément **RetentionPolicyType** est le type de rétention appliqué aux éléments d’une conversation. La valeur de texte de **suppression** indique que les éléments de la conversation sont supprimés lorsque le blocage de rétention arrive à expiration. La valeur de texte de **l’Archive** indique que les éléments de la conversation sont déplacés vers la boîte aux lettres d’archive lorsque le blocage de rétention arrive à expiration. 
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> ||
   

