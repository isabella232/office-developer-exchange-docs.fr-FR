---
title: HasAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: de152be6-fc2f-48bc-a05d-1211935da20a
description: L’élément HasAttachment spécifie une valeur booléenne pour indiquer si l’élément a des pièces jointes.
ms.openlocfilehash: dfe163e0850e835784a43984a34c89f14bfbc59b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827798"
---
# <a name="hasattachment"></a>HasAttachment

L’élément **HasAttachment** spécifie une valeur booléenne pour indiquer si l’élément a des pièces jointes. 
  
```XML
<HasAttachment> true | false </HasAttachment
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
|[SearchPreviewItem](searchpreviewitem.md) <br/> |Spécifie les 256 premiers caractères d’un élément de boîte aux lettres pour l’aperçu sans ouvrir l’élément.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Une valeur de texte de **la valeur true** pour l’élément **HasAttachment** indique qu’une pièce jointe à l’élément. La valeur **false** indique que l’élément ne dispose pas d’une pièce jointe. 
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma type  <br/> |
|Validation File  <br/> |types.xsd  <br/> |
|Peut être vide  <br/> ||
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

