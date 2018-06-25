---
title: GetUMPropertiesResponse (service web de messagerie unifiée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- GetUMPropertiesResponse
api_type:
- schema
ms.assetid: fcd93ce5-7403-46a9-b46e-56d2ebdd2f79
description: L’élément GetUMPropertiesResponse définit une réponse à une demande de (service web de messagerie unifiée) opération GetUMProperties.
ms.openlocfilehash: c0df872ad6b8e6541fa750ab87f4c1e5f0118b00
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827685"
---
# <a name="getumpropertiesresponse-um-web-service"></a>GetUMPropertiesResponse (service web de messagerie unifiée)

L’élément **GetUMPropertiesResponse** définit une réponse à une demande de [l’opération GetUMProperties (service web de messagerie unifiée)](getumproperties-operation-um-web-service.md) . 
  
[GetUMPropertiesResponse (service web de messagerie unifiée)](getumpropertiesresponse-um-web-service.md)
  
```xml
<GetUMPropertiesResponse>
  <OofStatus/>
  <MissedCallNotificationEnabled/>
  <PlayOnPhoneDialString/>
  <TelephoneAccessNumbers/>
  <TelephoneAccessFolderEmail/>
</GetUMPropertiesResponse>
```

 **UMProperties**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[MissedCallNotificationEnabled (service web de messagerie unifiée)](missedcallnotificationenabled-um-web-service.md) <br/> |Indique si les notifications d’appels manqués sont activées.  <br/> |
|[PlayOnPhoneDialString (service web de messagerie unifiée)](playonphonedialstring-um-web-service.md) <br/> |Contient la chaîne de numérotation par défaut à utiliser pour [l’opération PlayOnPhone (service web de messagerie unifiée)](playonphone-operation-um-web-service.md) et [l’opération PlayOnPhoneGreeting (service web de messagerie unifiée)](playonphonegreeting-operation-um-web-service.md).  <br/> |
|[TelephoneAccessNumbers (service web de messagerie unifiée)](telephoneaccessnumbers-um-web-service.md) <br/> |Contient la liste des numéros de téléphone que l’utilisateur peut utiliser pour accéder à la messagerie unifiée par le biais d’un téléphone.  <br/> |
|[TelephoneAccessFolderEmail (service web de messagerie unifiée)](telephoneaccessfolderemail-um-web-service.md) <br/> |Contient l’identificateur pour le dossier de courrier électronique à partir de laquelle la messagerie unifiée sera lire des messages par téléphone.  <br/> |
   
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



[Opération GetUMProperties (service web de messagerie unifiée)](getumproperties-operation-um-web-service.md)

