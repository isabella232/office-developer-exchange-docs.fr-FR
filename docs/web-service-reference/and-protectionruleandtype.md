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
description: L’élément and spécifie que tous les éléments enfants doivent correspondre pour avoir la valeur true.
ms.openlocfilehash: ba898ccd77518971afaf713d1c7c7955f46465d5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464734"
---
# <a name="and-protectionruleandtype"></a>Et (ProtectionRuleAndType)

L’élément **and** spécifie que tous les éléments enfants doivent correspondre pour avoir la **valeur true**.
  
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

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[AllInternal](allinternal.md) <br/> |Renvoie la **valeur true** si tous les destinataires d’un message électronique sont internes à l’organisation de l’expéditeur.  <br/> |
|**And** <br/> |Spécifie que tous les éléments enfants doivent correspondre pour avoir la **valeur true**.  <br/> |
|[Destinataireest](recipientis.md) <br/> |Spécifie que tout destinataire du message électronique correspond à l’un des destinataires spécifiés dans les éléments de [valeur enfant (ProtectionRuleValueType)](value-protectionrulevaluetype.md) .  <br/> |
|[SenderDepartments](senderdepartments.md) <br/> |Indique que le service de l’expéditeur correspond à l’un des services spécifiés dans les éléments de [valeur enfant (ProtectionRuleValueType)](value-protectionrulevaluetype.md) .  <br/> |
|[True](true.md) <br/> |Spécifie une condition qui correspond toujours à.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Condition](condition.md) <br/> |Identifie la condition qui doit être remplie pour que la partie action de la règle soit exécutée.  <br/> |
|**And** <br/> |Spécifie que tous les éléments enfants doivent correspondre pour avoir la **valeur true**.  <br/> |
   
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

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

