---
title: Déconnecter (service web de messagerie unifiée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- Disconnect
api_type:
- schema
ms.assetid: 2f8c1e8c-3bd4-4988-96b9-735c347b29f7
description: L’élément de déconnexion définit une demande de déconnexion d’un appel.
ms.openlocfilehash: 764532bdadd69caaa68406c84277197def3160af
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755977"
---
# <a name="disconnect-um-web-service"></a>Déconnecter (service web de messagerie unifiée)

L’élément de **déconnexion** définit une demande de déconnexion d’un appel. 
  
- [Déconnecter (service web de messagerie unifiée)](disconnect-um-web-service.md)
  
```xml
<Disconnect>
  <CallId>   </CallId>
</Disconnect>
```

 **complexType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[ID d’appel (service web de messagerie unifiée)](callid-um-web-service.md) <br/> |L’identificateur de l’appel pour déconnecter la session.  <br/> |
   
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

- [(Service web de messagerie unifiée) de l’opération de déconnexion](disconnect-operation-um-web-service.md)  
- [Opération PlayOnPhone (service web de messagerie unifiée)](playonphone-operation-um-web-service.md) 
- [Opération PlayOnPhoneGreeting (service web de messagerie unifiée)](playonphonegreeting-operation-um-web-service.md)  
- [ID d’appel (service web de messagerie unifiée)](callid-um-web-service.md)

