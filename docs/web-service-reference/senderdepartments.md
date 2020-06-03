---
title: SenderDepartments
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SenderDepartments
api_type:
- schema
ms.assetid: b016cdde-d597-40ac-87c4-63ca68bd539d
description: L’élément SenderDepartments spécifie que le service de l’expéditeur correspond à l’un des services spécifiés dans les éléments de valeur enfant (ProtectionRuleValueType).
ms.openlocfilehash: cf15b974b9c0cfb09767661f17334defc4041e43
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530344"
---
# <a name="senderdepartments"></a>SenderDepartments

L’élément **SenderDepartments** spécifie que le service de l’expéditeur correspond à l’un des services spécifiés dans les éléments de [valeur enfant (ProtectionRuleValueType)](value-protectionrulevaluetype.md) . 
  
```XML
<SenderDepartments>
   <Value/>
</SenderDepartments>
```

 **ProtectionRuleSenderDepartmentsType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Valeur (ProtectionRuleValueType)](value-protectionrulevaluetype.md) <br/> |Identifie un service d’expéditeur unique.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Condition](condition.md) <br/> |Identifie la condition qui doit être remplie pour que la partie action de la règle soit exécutée.  <br/> |
|[Et (ProtectionRuleAndType)](and-protectionruleandtype.md) <br/> |Spécifie que tous les éléments enfants doivent correspondre pour avoir la **valeur true**. Spécifie qu’il doit y avoir plus d’une condition de règle de protection enfant.  <br/> |
   
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

