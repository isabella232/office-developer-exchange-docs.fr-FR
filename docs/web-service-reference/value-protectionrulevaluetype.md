---
title: Value (ProtectionRuleValueType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Value
api_type:
- schema
ms.assetid: b039bd6e-2198-47cf-9c78-a5e8b9d51c98
description: L’élément Value identifie un seul service de destinataire ou d’expéditeur.
ms.openlocfilehash: 2c4bbdcb3364f0ef8f608469f0dc1b289c4eeaf6
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541622"
---
# <a name="value-protectionrulevaluetype"></a>Value (ProtectionRuleValueType)

**L’élément Value** identifie un seul service de destinataire ou d’expéditeur. 
  
```XML
<Value/>
```

**ProtectionRuleValueType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[RecipientIs](recipientis.md) <br/> |Spécifie que tout destinataire du message électronique correspond à l’un des destinataires spécifiés dans les éléments **Value** enfants.  <br/> |
|[SenderDepartments](senderdepartments.md) <br/> |Spécifie que le service de l’expéditeur correspond à l’un des services spécifiés dans les éléments **Value** enfants.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Cet élément doit contenir une valeur de chaîne nonempty.
  
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

