---
title: ReturnNewItemIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: aeef79e4-31e1-4213-b627-9bac676be018
description: L’élément ReturnNewItemIds indique si les identificateurs d’élément de nouveaux éléments sont renvoyés dans la réponse.
ms.openlocfilehash: 6d3bc83c05a82d6e448041167676f41c2620dcd4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829232"
---
# <a name="returnnewitemids"></a>ReturnNewItemIds

L’élément **ReturnNewItemIds** indique si les identificateurs d’élément de nouveaux éléments sont renvoyés dans la réponse. 
  
```XML
<ReturnNewItemIds/>
```

 **xs : Boolean**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[CopyItem](copyitem.md) <br/> |Définit une demande pour copier un élément dans une boîte aux lettres dans la banque d’informations Exchange.  <br/> |
|[MoveItem](moveitem.md) <br/> |Définit une demande de déplacement d’un élément dans la banque d’informations Exchange.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Une valeur de texte de **la valeur true** pour l’élément **ReturnNewItemIds** indique que les nouveaux identificateurs d’élément sont retournés dans la réponse. La valeur **false** indique que les nouveaux identificateurs d’élément ne sont pas renvoyées dans la réponse. 
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma des messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   

