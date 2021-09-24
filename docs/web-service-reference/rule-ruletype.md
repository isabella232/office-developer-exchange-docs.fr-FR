---
title: Règle (RuleType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Rule
api_type:
- schema
ms.assetid: 259a1f62-b235-4964-88bf-2d1f1c05a563
description: L’élément Rule contient une seule règle et représente une règle dans la boîte aux lettres d’un utilisateur.
ms.openlocfilehash: 0e7d7284d561ea374f66106072df0c4f850c590c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59527515"
---
# <a name="rule-ruletype"></a>Règle (RuleType)

**L’élément Rule** contient une seule règle et représente une règle dans la boîte aux lettres d’un utilisateur. 
  
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
|[RuleId](ruleid.md) <br/> |Spécifie l’identificateur de règle.  <br/> |
|[DisplayName (chaîne)](displayname-string.md) <br/> |Contient le nom complet d’une règle.  <br/> |
|[Priorité](priority.md) <br/> |Indique l’ordre dans lequel une règle doit être exécuté.  <br/> |
|[IsEnabled](isenabled.md) <br/> |Indique si la règle est activée.  <br/> |
|[IsNotSupported](isnotsupported.md) <br/> |Indique si la règle ne peut pas être modifiée avec les API de code géré.  <br/> |
|[IsInError](isinerror.md) <br/> |Indique si la règle se trouve dans une condition d’erreur.  <br/> |
|[Conditions](conditions.md) <br/> |Identifie les conditions qui, lorsqu’elles sont remplies, déclenchent les actions de règle pour une règle.  <br/> |
|[Exceptions](exceptions.md) <br/> |Identifie les exceptions qui représentent toutes les conditions d’exception de règle disponibles pour la règle de boîte de réception.  <br/> |
|[Actions](actions.md) <br/> |Représente les actions à prendre sur un message lorsque les conditions sont remplies.  <br/> |
   
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

