---
title: IsEncrypted
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsEncrypted
api_type:
- schema
ms.assetid: 68a30e92-c2b1-4af5-bb16-ba38afb80c43
description: L’élément IsEncrypted indique si les messages entrants doivent être chiffré afin que l’exception ou la condition à appliquer S/MIME.
ms.openlocfilehash: 582a1f197d4ee6b60af91b1a178d79163b50052c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828003"
---
# <a name="isencrypted"></a>IsEncrypted

L’élément **IsEncrypted** indique si les messages entrants doivent être chiffré afin que l’exception ou la condition à appliquer S/MIME. 
  
```XML
<IsEncrypted>true | false</IsEncrypted>
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
|[Conditions](conditions.md) <br/> |Représente les conditions qui, lorsqu'elles sont remplies, vont déclencher les actions de règle pour une règle.  <br/> |
|[Exceptions](exceptions.md) <br/> |Représente toutes les conditions d’exception de règle disponibles pour une règle de boîte de réception.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Une valeur de texte de **la valeur true** indique que le message doit être S/MIME chiffré afin que l’exception ou la condition à appliquer. La valeur **false** indique que le message n’a pas être S/MIME afin que l’exception ou la condition à appliquer. 
  
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

