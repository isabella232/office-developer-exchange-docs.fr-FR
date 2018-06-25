---
title: SetPlayOnPhoneDialString (service web de messagerie unifiée)
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
description: L’élément SetPlayOnPhoneDialString définit une demande pour définir la chaîne de numérotation par défaut pour l’opération PlayOnPhone (service web de messagerie unifiée) et les demandes d’opérations (service web de messagerie unifiée) PlayOnPhoneGreeting.
ms.openlocfilehash: fd82dc6ef0dd90a2318da93191f657005b7a5c87
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829450"
---
# <a name="setplayonphonedialstring-um-web-service"></a>SetPlayOnPhoneDialString (service web de messagerie unifiée)

L’élément **SetPlayOnPhoneDialString** définit une demande pour définir la chaîne de numérotation par défaut pour les demandes [PlayOnPhone (service web de messagerie unifiée)](playonphone-operation-um-web-service.md) et [les opérations PlayOnPhoneGreeting (service web de messagerie unifiée)](playonphonegreeting-operation-um-web-service.md) . 
  
[SetPlayOnPhoneDialString (service web de messagerie unifiée)](setplayonphonedialstring-um-web-service.md)
  
```xml
<SetPlayOnPhoneDialString>
  <dialString>   </dialString>
</SetPlayOnPhoneDialString>
```

 **complexType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[dialString (service web de messagerie unifiée)](dialstring-um-web-service.md) <br/> |Le numéro de téléphone à définir comme la chaîne de numérotation par défaut.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération SetPlayOnPhoneDialString (service web de messagerie unifiée)](setplayonphonedialstring-operation-um-web-service.md)

