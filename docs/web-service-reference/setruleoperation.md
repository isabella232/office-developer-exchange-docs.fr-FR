---
title: SetRuleOperation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SetRuleOperation
api_type:
- schema
ms.assetid: 2106a85b-58fe-49be-b71d-4ca6aa66e060
description: L’élément SetRuleOperation représente une opération de mise à jour d’une règle existante.
ms.openlocfilehash: 96fba2f229003b8c729c36614e69655852a3aa8c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526332"
---
# <a name="setruleoperation"></a>SetRuleOperation

L’élément **SetRuleOperation** représente une opération de mise à jour d’une règle existante. 
  
[UpdateInboxRules](updateinboxrules.md)
  
[Operations](operations.md)
  
```XML
<SetRuleOperation>
    <Rule/>
</SetRuleOperation>
```

 **SetRuleOperationType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Règle (RuleType)](rule-ruletype.md) <br/> |Représente une règle dans la boîte aux lettres d’un utilisateur.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Opérations](operations.md) <br/> |Contient un tableau des opérations de règle qui peuvent être effectuées sur une boîte de réception.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
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



[UpdateInboxRules](updateinboxrules.md)
  
[DeleteRuleOperation](deleteruleoperation.md)
  
[CreateRuleOperation](createruleoperation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

