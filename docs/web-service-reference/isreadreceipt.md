---
title: IsReadReceipt
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsReadReceipt
api_type:
- schema
ms.assetid: e60e525f-c136-469a-b68b-b3dc01f400a6
description: L’élément IsReadReceipt indique si les messages entrants doivent être des confirmations de lecture afin que l’exception ou la condition à appliquer.
ms.openlocfilehash: 78714aafb116a609a69d77b3b4f0fd15695bda34
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828094"
---
# <a name="isreadreceipt"></a>IsReadReceipt

L’élément **IsReadReceipt** indique si les messages entrants doivent être des confirmations de lecture afin que l’exception ou la condition à appliquer. 
  
```XML
<IsReadReceipt> true | false</IsReadReceipt>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Conditions](conditions.md) <br/> |Représente les conditions qui, une fois traité, déclenche les actions de règle associée à cette règle.  <br/> |
|[Exceptions](exceptions.md) <br/> |Représente toutes les conditions d'exception de règle disponibles pour la règle de boîte de réception.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Texte la valeur **true** indique que le message doit être une confirmation de lecture afin que l’exception ou la condition à appliquer. Si le message n’a pas à une confirmation de lecture pour la condition ou une exception à appliquer, la valeur est **false**.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

