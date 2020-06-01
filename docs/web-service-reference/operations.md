---
title: Opérations
manager: sethgros
ms.date: 09/17/2015
ms.audience: ITPro
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Operations
api_type:
- schema
ms.assetid: d8cd41b1-28ae-4c95-9ff6-8b25c8e18306
description: L’élément Operations contient un tableau d’opérations de règle qui peuvent être effectuées sur une boîte de réception.
ms.openlocfilehash: 4bbec4ad6424f802bb6781a870d65f23705e88c4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462485"
---
# <a name="operations"></a>Opérations

L’élément **Operations** contient un tableau d’opérations de règle qui peuvent être effectuées sur une boîte de réception. 
  
[UpdateInboxRules](updateinboxrules.md)
  
```XML
<Operations>
    <CreateRuleOperation/>
    <SetRuleOperation/>
    <DeleteRuleOperation/>
</Operations>
```

 **ArrayOfRuleOperationsType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[CreateRuleOperation](createruleoperation.md) <br/> |Représente une opération de création d’une nouvelle règle de boîte de réception.  <br/> |
|[SetRuleOperation](setruleoperation.md) <br/> |Représente une opération de mise à jour d’une règle de boîte de réception.  <br/> |
|[DeleteRuleOperation](deleteruleoperation.md) <br/> |Représente une opération de suppression d’une règle de boîte de réception.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[UpdateInboxRules](updateinboxrules.md) <br/> |Définit une demande de mise à jour des règles de boîte de réception dans une boîte aux lettres dans le magasin du serveur.  <br/> |
   
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



[Opération de UpdateInboxRules](updateinboxrules-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

