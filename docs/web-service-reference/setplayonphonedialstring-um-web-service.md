---
title: SetPlayOnPhoneDialString (service Web de messagerie unifiée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- SetPlayOnPhoneDialString
api_type:
- schema
ms.assetid: 513a5072-c3ac-405f-98c2-0ab982d0a360
description: L’élément SetPlayOnPhoneDialString définit une demande de définition de la chaîne de numérotation par défaut pour les opérations PlayOnPhone (service Web de messagerie unifiée) et PlayOnPhoneGreeting (service Web de messagerie unifiée).
ms.openlocfilehash: 40021e9dedafb5fafda91bf3612d8a6485dae8e7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458627"
---
# <a name="setplayonphonedialstring-um-web-service"></a>SetPlayOnPhoneDialString (service Web de messagerie unifiée)

L’élément **SetPlayOnPhoneDialString** définit une demande de définition de la chaîne de numérotation par défaut pour les [opérations PlayOnPhone (service Web de messagerie unifiée)](playonphone-operation-um-web-service.md) et [PlayOnPhoneGreeting (service Web de messagerie unifiée)](playonphonegreeting-operation-um-web-service.md) . 
  
[SetPlayOnPhoneDialString (service Web de messagerie unifiée)](setplayonphonedialstring-um-web-service.md)
  
```xml
<SetPlayOnPhoneDialString>
  <dialString>   </dialString>
</SetPlayOnPhoneDialString>
```

 **complexType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[dialString (service Web de messagerie unifiée)](dialstring-um-web-service.md) <br/> |Numéro de téléphone à définir comme chaîne de numérotation par défaut.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="text-value"></a>Valeur de texte

Aucune.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Messages  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération SetPlayOnPhoneDialString (service Web de messagerie unifiée)](setplayonphonedialstring-operation-um-web-service.md)

