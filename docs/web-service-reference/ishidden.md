---
title: IsHidden
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 2377b584-bd1e-49fc-b80a-a6634721a297
description: L’élément IsHidden contient une valeur booléen qui indique si le contact sous-jacent doit être masqué ou affiché dans le cadre du personnage.
ms.openlocfilehash: 7ff24eaa5e8e7b25c87af0bf299fcca0d88dc0b6
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59532787"
---
# <a name="ishidden"></a>IsHidden

**L’élément IsHidden** contient une valeur booléen qui indique si le contact sous-jacent doit être masqué ou affiché dans le cadre du personnage. 
  
```XML
<IsHidden>true | false</IsHidden>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Attribution (PersonaAttributionType)](attribution-personaattributiontype.md) <br/> |Spécifie une instance d'un tableau d'attributs pour un élément **Persona**.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte **true** pour l’élément **IsHidden** indique que le contact sous-jacent doit être masqué ou affiché dans le cadre du personnage. La valeur **false indique** que le contact sous-jacent ne doit pas être masqué ou affiché dans le cadre du personnage. 
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma type  <br/> |
|Validation File  <br/> |types.xsd  <br/> |
|Peut être vide  <br/> ||
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

