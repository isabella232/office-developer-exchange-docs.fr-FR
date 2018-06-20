---
title: Règle
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Rule
api_type:
- schema
ms.assetid: c30f3851-bd56-4473-9106-dc85e9619486
description: L’élément de règle contient une règle de protection unique.
ms.openlocfilehash: 9abbb70381c214211172d2d5ba1ed43ee4797f17
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829263"
---
# <a name="rule"></a>Règle

L’élément de **règle** contient une règle de protection unique. 
  
```XML
<Rule Name="" UserOverridable=="" Priority="">
   <Condition/>
   <Action/>
</Rule>
```

 **ProtectionRuleType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**Name** <br/> |Identifie le nom de la règle. Un attribut obligatoire de type chaîne avec une longueur minimale de 1.  <br/> |
|**UserOverridable** <br/> |Indique si la règle est obligatoire. Si la règle est obligatoire, cette valeur d’attribut doit avoir la **valeur false**. Attribut de type Boolean obligatoire.  <br/> |
|**Priority** <br/> |Spécifie la priorité de la règle. Un attribut obligatoire de type int avec une valeur minimale de 1.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Condition](condition.md) <br/> |Identifie la condition qui doit être remplie pour la partie de l’action de la règle doit être exécutée.  <br/> |
|[Action (ProtectionRuleActionType)](action-protectionruleactiontype.md) <br/> |Identifie l’action qui doit être exécutée si correspond à la partie de la condition de la règle.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Règles](rules-ex15websvcsotherref.md) <br/> |Contient un tableau des règles de protection.  <br/> |
   
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



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

