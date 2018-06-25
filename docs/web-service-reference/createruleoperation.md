---
title: CreateRuleOperation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateRuleOperation
api_type:
- schema
ms.assetid: e9f70726-db08-4089-839e-a41007d0a473
description: L’élément CreateRuleOperation représente une opération pour créer une nouvelle règle de boîte de réception.
ms.openlocfilehash: c531f222ffe886e6ef53a99609cfa27e84fd6107
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755738"
---
# <a name="createruleoperation"></a>CreateRuleOperation

L’élément **CreateRuleOperation** représente une opération pour créer une nouvelle règle de boîte de réception. 
  
[UpdateInboxRules](updateinboxrules.md)
  
[Opérations](operations.md)
  
```xml
<CreateRuleOperation>
    <Rule/>
</CreateRuleOperation>
```

 **CreateRuleOperationType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Règle (RuleType)](rule-ruletype.md) <br/> |Représente une règle à créer dans la boîte aux lettres d’un utilisateur.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Opérations](operations.md) <br/> |Contient les opérations qui peuvent être effectuées sur une boîte de réception.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[UpdateInboxRules](updateinboxrules.md)
  
[SetRuleOperation](setruleoperation.md)
  
[DeleteRuleOperation](deleteruleoperation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

