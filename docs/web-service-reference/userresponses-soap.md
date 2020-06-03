---
title: UserResponses (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: a48766df-4cc8-47c2-a8c1-826daec94e5a
description: L’élément UserResponses contient les paramètres de configuration pour chaque utilisateur demandé.
ms.openlocfilehash: db2bab16334b90395d29dc03353dce05b0e45357
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526745"
---
# <a name="userresponses-soap"></a>UserResponses (SOAP)

L’élément **UserResponses** contient les paramètres de configuration pour chaque utilisateur demandé. 
  
```XML
<UserResponses>
   <UserResponse/>
</UserResponses>
```

 **ArrayOfUserResponse**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[UserResponse (SOAP)](userresponse-soap.md) <br/> |Représente une réponse à une demande d' [opération GetUserSettings (SOAP)](getusersettings-operation-soap.md) pour un utilisateur individuel.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Réponse (SOAP)](response-soap.md) <br/> |Contient la réponse à une demande d' [opération GetUserSettings (SOAP)](getusersettings-operation-soap.md) .  <br/> |
   
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nom du schéma  <br/> |Schéma de découverte automatique  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetUserSettings (SOAP)](getusersettings-operation-soap.md)

