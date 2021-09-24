---
title: SuppressReadReceipts
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: f0805560-7a2f-455b-94d2-ec4f1e3652c3
description: L’élément SuppressReadReceipts indique si les reçus de lecture doivent être supprimés.
ms.openlocfilehash: 1f63f46f4e74a3123661caba39b737910bc2ef30
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59517650"
---
# <a name="suppressreadreceipts"></a>SuppressReadReceipts

**L’élément SuppressReadReceipts** indique si les reçus de lecture doivent être supprimés. 
  
```XML
<SuppressReadReceipts>true | false</SuppressReadReceipts>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[ConversationAction](conversationaction.md)  |  [MarkAllItemsAsRead](markallitemsasread.md)
  
## <a name="text-value"></a>Valeur texte

Une valeur de texte **true pour** **l’élément SuppressReadReciepts** indique que les reçus de lecture sont supprimés. La valeur **false indique** que les reçus de lecture seront envoyés à l’expéditeur. 
  
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
   

