---
title: ReturnNewItemIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: aeef79e4-31e1-4213-b627-9bac676be018
description: L’élément ReturnNewItemIds indique si les identificateurs d’élément des nouveaux éléments sont renvoyés dans la réponse.
ms.openlocfilehash: 93ff4e37c56c3583e81711ba7e3582706d9ef940
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59512379"
---
# <a name="returnnewitemids"></a>ReturnNewItemIds

**L’élément ReturnNewItemIds** indique si les identificateurs d’élément des nouveaux éléments sont renvoyés dans la réponse. 
  
```XML
<ReturnNewItemIds/>
```

 **xs:boolean**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[CopyItem](copyitem.md) <br/> |Définit une demande de copie d’un élément dans une boîte aux lettres dans la Exchange store.  <br/> |
|[MoveItem](moveitem.md) <br/> |Définit une demande de déplacement d’un élément dans la Exchange store.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte **true** pour l’élément **ReturnNewItemIds** indique que les nouveaux identificateurs d’élément sont renvoyés dans la réponse. La valeur **false indique** que les nouveaux identificateurs d’élément ne sont pas renvoyés dans la réponse. 
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma des messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   

