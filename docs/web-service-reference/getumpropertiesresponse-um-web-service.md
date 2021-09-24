---
title: GetUMPropertiesResponse (service web de messagerie unifiée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- GetUMPropertiesResponse
api_type:
- schema
ms.assetid: fcd93ce5-7403-46a9-b46e-56d2ebdd2f79
description: L’élément GetUMPropertiesResponse définit une réponse à une demande d’opération GetUMProperties (service web de um).
ms.openlocfilehash: 97c3850d46369d4ab533629a8b24e199db3dd44a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522963"
---
# <a name="getumpropertiesresponse-um-web-service"></a>GetUMPropertiesResponse (service web de messagerie unifiée)

**L’élément GetUMPropertiesResponse** définit une réponse à une demande d’opération [GetUMProperties (service web de](getumproperties-operation-um-web-service.md) um). 
  
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

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[MissedCallNotificationEnabled (service web de messagerie unifiée)](missedcallnotificationenabled-um-web-service.md) <br/> |Indique si les notifications d’appels manqués sont activées.  <br/> |
|[PlayOnPhoneDialString (service web de messagerie unifiée)](playonphonedialstring-um-web-service.md) <br/> |Contient la chaîne de numérotation par défaut à utiliser pour l’opération [PlayOnPhone (service web](playonphone-operation-um-web-service.md) de um) et [l’opération PlayOnPhoneGreeting (service web](playonphonegreeting-operation-um-web-service.md)de la um).  <br/> |
|[TelephoneAccessNumbers (service web de messagerie unifiée)](telephoneaccessnumbers-um-web-service.md) <br/> |Contient la liste des numéros de téléphone que l’utilisateur peut utiliser pour accéder à la messagerie unifiée via un téléphone.  <br/> |
|[TelephoneAccessFolderEmail (service web de messagerie unifiée)](telephoneaccessfolderemail-um-web-service.md) <br/> |Contient l’identificateur du dossier de messagerie à partir duquel la messagerie unifiée lit les messages par téléphone.  <br/> |
   
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



[Opération GetUMProperties (service web de messagerie unifiée)](getumproperties-operation-um-web-service.md)

