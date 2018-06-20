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
description: L’élément de règle contient une règle unique et représente une règle de boîte aux lettres d’un utilisateur.
ms.openlocfilehash: b1f9f058213543633335db11f03729964baf98ad
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829259"
---
# <a name="rule-ruletype"></a>Règle (RuleType)

L’élément de **règle** contient une règle unique et représente une règle de boîte aux lettres d’un utilisateur. 
  
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

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[ID de la règle](ruleid.md) <br/> |Spécifie l’identificateur de la règle.  <br/> |
|[DisplayName (chaîne)](displayname-string.md) <br/> |Contient le nom complet d’une règle.  <br/> |
|[Priority](priority.md) <br/> |Indique l’ordre dans lequel une règle doit être exécutée.  <br/> |
|[IsEnabled](isenabled.md) <br/> |Indique si la règle est activée.  <br/> |
|[IsNotSupported](isnotsupported.md) <br/> |Indique si la règle ne peut pas être modifiée avec l’API du code managé.  <br/> |
|[IsInError](isinerror.md) <br/> |Indique si la règle se trouve dans une condition d’erreur.  <br/> |
|[Conditions](conditions.md) <br/> |Identifie les conditions qui, lorsque remplies, déclenchent des actions de règle d’une règle.  <br/> |
|[Exceptions](exceptions.md) <br/> |Identifie les exceptions qui représentent toutes les conditions d’exception de règle disponibles pour la règle de boîte de réception.  <br/> |
|[Actions](actions.md) <br/> |Représente les actions à entreprendre sur un message lorsque les conditions sont remplies.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[CreateRuleOperation](createruleoperation.md) <br/> |Représente une opération pour créer une nouvelle règle.  <br/> |
|[InboxRules](inboxrules.md) <br/> |Représente un tableau de règles de boîte aux lettres de l’utilisateur.  <br/> |
|[SetRuleOperation](setruleoperation.md) <br/> |Représente une opération de mise à jour d’une règle existante.  <br/> |
   
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
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi



[UpdateInboxRules](updateinboxrules.md)
  
[SetRuleOperation](setruleoperation.md)
  
[CreateRuleOperation](createruleoperation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

