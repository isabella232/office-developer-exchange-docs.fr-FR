---
title: PlayOnPhoneGreeting (service web de messagerie unifiée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- PlayOnPhoneGreeting
api_type:
- schema
ms.assetid: 43eda596-3609-4e1b-8502-1db2636535cf
description: L’élément PlayOnPhoneGreeting définit une demande de lecture d’un message d’accueil de messagerie unifiée sur un téléphone.
ms.openlocfilehash: e3b6a7720be6d046a379af460adbcc88725c0ea3
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543120"
---
# <a name="playonphonegreeting-um-web-service"></a>PlayOnPhoneGreeting (service web de messagerie unifiée)

**L’élément PlayOnPhoneGreeting** définit une demande de lecture d’un message d’accueil de messagerie unifiée sur un téléphone. 
  
[PlayOnPhoneGreeting (service web de messagerie unifiée)](playonphonegreeting-um-web-service.md)
  
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
|[GreetingType (service web de messagerie unifiée)](greetingtype-um-web-service.md) <br/> |Définit le type de message d’accueil à utiliser dans une [demande d’opération PlayOnPhoneGreeting (service web de um).](playonphonegreeting-operation-um-web-service.md)  <br/> |
|[dialString (service web de messagerie unifiée)](dialstring-um-web-service.md) <br/> |Contient la valeur du numéro de téléphone à composer.  <br/> |
   
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



[Opération PlayOnPhoneGreeting (service web de messagerie unifiée)](playonphonegreeting-operation-um-web-service.md)

