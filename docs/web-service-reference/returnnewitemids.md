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
ms.openlocfilehash: 003676c4c034454aa551e42bf3af976183117b8c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465113"
---
# <a name="returnnewitemids"></a>ReturnNewItemIds

L’élément **ReturnNewItemIds** indique si les identificateurs d’élément de nouveaux éléments sont renvoyés dans la réponse. 
  
```XML
<ReturnNewItemIds/>
```

 **XS : Boolean**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[CopyItem](copyitem.md) <br/> |Définit une demande de copie d’un élément dans une boîte aux lettres dans la Banque d’Exchange.  <br/> |
|[MoveItem](moveitem.md) <br/> |Définit une demande de déplacement d’un élément dans la Banque d’Exchange.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte de **true** pour l’élément **ReturnNewItemIds** indique que les nouveaux identificateurs d’élément sont renvoyés dans la réponse. La valeur **false** indique que les nouveaux identificateurs d’élément ne sont pas renvoyés dans la réponse. 
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma de message  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   

