---
title: SetPlayOnPhoneDialString (service web de messagerie unifiée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- SetPlayOnPhoneDialString
api_type:
- schema
ms.assetid: 513a5072-c3ac-405f-98c2-0ab982d0a360
description: L’élément SetPlayOnPhoneDialString définit une demande de définition de la chaîne de numérotation par défaut pour les demandes d’opération PlayOnPhone (service web de um) et d’opération PlayOnPhoneGreeting (service web de um).
ms.openlocfilehash: e485fd092da29a3f54b1acc2b7e50167084e13fa
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540502"
---
# <a name="setplayonphonedialstring-um-web-service"></a>SetPlayOnPhoneDialString (service web de messagerie unifiée)

**L’élément SetPlayOnPhoneDialString** définit une demande de définition de la chaîne de numérotation par défaut pour les demandes d’opération [PlayOnPhone (service web](playonphone-operation-um-web-service.md) de um) et [d’opération PlayOnPhoneGreeting (service web](playonphonegreeting-operation-um-web-service.md) de um). 
  
[SetPlayOnPhoneDialString (service web de messagerie unifiée)](setplayonphonedialstring-um-web-service.md)
  
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
|[dialString (service web de messagerie unifiée)](dialstring-um-web-service.md) <br/> |Numéro de téléphone à définir comme chaîne de numérotation par défaut.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="text-value"></a>Valeur de texte

Aucune.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération SetPlayOnPhoneDialString (service web de messagerie unifiée)](setplayonphonedialstring-operation-um-web-service.md)

