---
title: PlayOnPhoneGreeting (service Web de messagerie unifiée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- PlayOnPhoneGreeting
api_type:
- schema
ms.assetid: 43eda596-3609-4e1b-8502-1db2636535cf
description: L’élément PlayOnPhoneGreeting définit une demande de lecture d’un message d’accueil de la messagerie unifiée sur un téléphone.
ms.openlocfilehash: 197e4ba671e1711b73b1e7c239339db589357581
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529923"
---
# <a name="playonphonegreeting-um-web-service"></a>PlayOnPhoneGreeting (service Web de messagerie unifiée)

L’élément **PlayOnPhoneGreeting** définit une demande de lecture d’un message d’accueil de la messagerie unifiée sur un téléphone. 
  
[PlayOnPhoneGreeting (service Web de messagerie unifiée)](playonphonegreeting-um-web-service.md)
  
```xml
<PlayOnPhoneGreeting>
  <GreetingType/>
  <DialString/>
</PlayOnPhoneGreeting>
```

 **complexType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[GreetingType (service Web de messagerie unifiée)](greetingtype-um-web-service.md) <br/> |Définit le type de message d’accueil à utiliser dans une demande d' [opération PlayOnPhoneGreeting (service Web de messagerie unifiée)](playonphonegreeting-operation-um-web-service.md) .  <br/> |
|[dialString (service Web de messagerie unifiée)](dialstring-um-web-service.md) <br/> |Contient la valeur du numéro de téléphone à composer.  <br/> |
   
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



[Opération PlayOnPhoneGreeting (service Web de messagerie unifiée)](playonphonegreeting-operation-um-web-service.md)

