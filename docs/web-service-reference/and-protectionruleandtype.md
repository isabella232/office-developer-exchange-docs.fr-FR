---
title: Et (ProtectionRuleAndType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- And
api_type:
- schema
ms.assetid: 7fafd1c8-cd29-43a0-b383-f6595f934f48
description: L’élément et spécifie que tous les éléments enfants doivent correspondre pour renvoyer la valeur true.
ms.openlocfilehash: 9e0128ee3fa2b6ffdc5975946694475afec53c25
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755205"
---
# <a name="and-protectionruleandtype"></a>Et (ProtectionRuleAndType)

L’élément **et** Spécifie que tous les éléments enfants doivent correspondre pour prendre la **valeur true**.
  
```xml
<And>
   <AllInternal/>
   <And/>
   <RecipientIs/>
   <SenderDepartments/>
   <True/>
</And>
```

 **ProtectionRuleAndType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[AllInternal](allinternal.md) <br/> |Renvoie **la valeur true** si tous les destinataires d’un message électronique sont internes à l’organisation de l’expéditeur.  <br/> |
|**And** <br/> |Spécifie que tous les éléments enfants doivent correspondre pour prendre la **valeur true**.  <br/> |
|[RecipientIs](recipientis.md) <br/> |Spécifie que n’importe quel destinataire du message électronique correspond à un des destinataires spécifiés dans les éléments de [valeur (ProtectionRuleValueType)](value-protectionrulevaluetype.md) enfants.  <br/> |
|[SenderDepartments](senderdepartments.md) <br/> |Spécifie que le service de l’expéditeur correspond à l’un des services spécifiés dans les éléments de [valeur (ProtectionRuleValueType)](value-protectionrulevaluetype.md) enfants.  <br/> |
|[True](true.md) <br/> |Spécifie une condition qui correspond toujours.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Condition](condition.md) <br/> |Identifie la condition qui doit être remplie pour la partie de l’action de la règle doit être exécutée.  <br/> |
|**And** <br/> |Spécifie que tous les éléments enfants doivent correspondre pour prendre la **valeur true**.  <br/> |
   
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

