---
title: IsArchive
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b89d8a78-5c18-4547-aaf4-4b16a93190a7
description: L’élément IsArchive indique une valeur de type Boolean qui indique si la boîte aux lettres est une boîte aux lettres d’archive.
ms.openlocfilehash: 417afd1afc25e5872d1f511feff34494fe6b7b62
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827990"
---
# <a name="isarchive"></a>IsArchive

L’élément **IsArchive** indique une valeur de type Boolean qui indique si la boîte aux lettres est une boîte aux lettres d’archive. 
  
```XML
<IsArchive>true | false</IsArchive>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[FailedMailbox](failedmailbox.md) | [RetentionPolicyTag](retentionpolicytag.md)
  
## <a name="text-value"></a>Valeur de texte

Une valeur de texte de **la valeur true** pour l’élément **IsArchive** indique que la boîte aux lettres cible est une boîte aux lettres d’archive. La valeur **false** indique que la boîte aux lettres cible n’est pas une boîte aux lettres d’archive. 
  
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

