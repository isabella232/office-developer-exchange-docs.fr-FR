---
title: Règle (RuleType)
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
ms.assetid: 259a1f62-b235-4964-88bf-2d1f1c05a563
description: L’élément rule contient une seule règle et représente une règle dans la boîte aux lettres d’un utilisateur.
ms.openlocfilehash: cdbd21df235a62a9e201e1eaae1d82a8ac10cdd2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/01/2020
ms.locfileid: "44465078"
---
# <a name="rule-ruletype"></a>Règle (RuleType)

L’élément **rule** contient une seule règle et représente une règle dans la boîte aux lettres d’un utilisateur. 
  
```XML
<Rule>
    <RuleId>
    <DisplayName>
    <Priority>
    <IsEnabled>
    <IsNotSupported>
    <IsInError>
    <Conditions>
    <Exceptions>
    <Actions>
</Rule>
```

 **RuleType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[RuleId](ruleid.md) <br/> |Spécifie l’identificateur de la règle.  <br/> |
|[DisplayName (chaîne)](displayname-string.md) <br/> |Contient le nom complet d’une règle.  <br/> |
|[Priorité](priority.md) <br/> |Indique l’ordre dans lequel une règle doit être exécutée.  <br/> |
|[IsEnabled](isenabled.md) <br/> |Indique si la règle est activée.  <br/> |
|[IsNotSupported](isnotsupported.md) <br/> |Indique si la règle ne peut pas être modifiée avec les API avec code managé.  <br/> |
|[IsInError](isinerror.md) <br/> |Indique si la règle se trouve dans une condition d’erreur.  <br/> |
|[Conditions](conditions.md) <br/> |Identifie les conditions qui, lorsqu’elles sont remplies, déclencheront les actions de règle pour une règle.  <br/> |
|[Exceptions](exceptions.md) <br/> |Identifie les exceptions qui représentent toutes les conditions d’exception de règle disponibles pour la règle de boîte de réception.  <br/> |
|[Actions](actions.md) <br/> |Représente les actions à effectuer sur un message lorsque les conditions sont remplies.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[CreateRuleOperation](createruleoperation.md) <br/> |Représente une opération de création d’une règle.  <br/> |
|[InboxRules](inboxrules.md) <br/> |Représente un tableau de règles dans la boîte aux lettres de l’utilisateur.  <br/> |
|[SetRuleOperation](setruleoperation.md) <br/> |Représente une opération de mise à jour d’une règle existante.  <br/> |
   
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
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi



[UpdateInboxRules](updateinboxrules.md)
  
[SetRuleOperation](setruleoperation.md)
  
[CreateRuleOperation](createruleoperation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

