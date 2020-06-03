---
title: GetUMPropertiesResponse (service Web de messagerie unifiée)
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
description: L’élément GetUMPropertiesResponse définit une réponse à une opération GetUMProperties (service Web de messagerie unifiée).
ms.openlocfilehash: 3247489a305c694c10764d7a0c6f02b1fad51ebf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459124"
---
# <a name="getumpropertiesresponse-um-web-service"></a>GetUMPropertiesResponse (service Web de messagerie unifiée)

L’élément **GetUMPropertiesResponse** définit une réponse à une [opération GetUMProperties (service Web de messagerie unifiée)](getumproperties-operation-um-web-service.md) . 
  
[GetUMPropertiesResponse (service Web de messagerie unifiée)](getumpropertiesresponse-um-web-service.md)
  
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

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[MissedCallNotificationEnabled (service Web de messagerie unifiée)](missedcallnotificationenabled-um-web-service.md) <br/> |Indique si les notifications d’appels manqués sont activées.  <br/> |
|[PlayOnPhoneDialString (service Web de messagerie unifiée)](playonphonedialstring-um-web-service.md) <br/> |Contient la chaîne de numérotation par défaut à utiliser pour l' [opération PlayOnPhone (service Web de messagerie unifiée)](playonphone-operation-um-web-service.md) et l' [opération PlayOnPhoneGreeting (service Web de messagerie unifiée)](playonphonegreeting-operation-um-web-service.md).  <br/> |
|[TelephoneAccessNumbers (service Web de messagerie unifiée)](telephoneaccessnumbers-um-web-service.md) <br/> |Contient la liste des numéros de téléphone que l’utilisateur peut utiliser pour accéder à la messagerie unifiée via un téléphone.  <br/> |
|[TelephoneAccessFolderEmail (service Web de messagerie unifiée)](telephoneaccessfolderemail-um-web-service.md) <br/> |Contient l’identificateur du dossier de messagerie à partir duquel la messagerie unifiée lira les messages par téléphone.  <br/> |
   
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



[Opération GetUMProperties (service Web de messagerie unifiée)](getumproperties-operation-um-web-service.md)

