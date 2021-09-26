---
title: InboxRules
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- InboxRules
api_type:
- schema
ms.assetid: 7bb9896c-bd12-49ae-842a-a10b5f9a2ef6
description: L'élément InboxRules représente un tableau de règles de boîte aux lettres de l'utilisateur.
ms.openlocfilehash: 6b6b399f685accca90fbaffd3ed461aa43a3c2b3
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59547231"
---
# <a name="inboxrules"></a>InboxRules

Ce document peut contenir des informations liées aux fonctionnalités ou produits préliminaires qui sont sujettes à modifications avant la sortie de la version définitive. Ce document est fourni "tel quel" à titre indicatif et Microsoft exclut toute garantie, expresse ou implicite, en ce qui concerne ce document. L'élément **InboxRules** représente un tableau de règles de boîte aux lettres de l'utilisateur. 
  
[GetInboxRulesResponse](getinboxrulesresponse.md)
  
[InboxRules](inboxrules.md)
  
```XML
<InboxRules>
   <Rule/>
</InboxRules>
```

 **ArrayOfRulesType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Règle (RuleType)](rule-ruletype.md) <br/> |Contient une règle unique et représente une règle de boîte aux lettres de l'utilisateur.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetInboxRulesResponse](getinboxrulesresponse.md) <br/> |Définit une réponse à une demande de [Opération de GetInboxRules](getinboxrules-operation.md) .  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi



[GetInboxRules](getinboxrules.md)
  
[Opération de GetInboxRules](getinboxrules-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

