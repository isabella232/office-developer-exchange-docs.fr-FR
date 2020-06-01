---
title: AllInternal
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AllInternal
api_type:
- schema
ms.assetid: b7e5072f-5d9f-4ee0-b58b-4d75d878ea1c
description: L’élément AllInternal renvoie la valeur true si tous les destinataires d’un message électronique sont internes à l’organisation de l’expéditeur.
ms.openlocfilehash: c5ffe15eca5d680994acb62913ebf5effacce214
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464832"
---
# <a name="allinternal"></a>AllInternal

L’élément **AllInternal** renvoie la **valeur true** si tous les destinataires d’un message électronique sont internes à l’organisation de l’expéditeur. 
  
```xml
<AllInternal/>
```

 **ProtectionRuleAllInternalType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Condition](condition.md) <br/> |Identifie la condition qui doit être remplie pour que la partie action de la règle soit exécutée.  <br/> |
|[Et (ProtectionRuleAndType)](and-protectionruleandtype.md) <br/> |Spécifie que tous les éléments enfants doivent correspondre pour avoir la **valeur true**.  <br/> |
   
## <a name="text-value"></a>Valeur texte

L’élément **AllInternal** doit être vide. 
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

