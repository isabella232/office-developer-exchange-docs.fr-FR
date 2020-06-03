---
title: AutodiscoverResponse (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 203a5ac3-ebd0-4514-acbe-bc1c74638127
description: L’élément AutodiscoverResponse (SOAP) représente l’élément de base pour toutes les réponses renvoyées par le service de découverte automatique.
ms.openlocfilehash: 81fd557578bde9552d07e24386c93903e44a9afa
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463964"
---
# <a name="autodiscoverresponse-soap"></a>AutodiscoverResponse (SOAP)

L’élément **AutodiscoverResponse (SOAP)** représente l’élément de base pour toutes les réponses renvoyées par le service de découverte automatique. 
  
- [AutodiscoverResponse (SOAP)](autodiscoverresponse-soap.md)
  
```XML
<AutodiscoverResponse>
    <UserResponses/>
    <UserSettingErrors/>
    <UserSettings/>
</AutodiscoverResponse>

```

 **AutodiscoverResponse**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[UserResponses (SOAP)](userresponses-soap.md) <br/> |Représente une collection d’éléments [UserResponse (SOAP)](userresponse-soap.md) .  <br/> |
|[UserSettingErrors (SOAP)](usersettingerrors-soap.md) <br/> |Représente une collection d’éléments [UserSettingError (SOAP)](usersettingerror-soap.md) .  <br/> |
|[UserSettings (SOAP)](usersettings-soap.md) <br/> |Représente une collection d’éléments [UserSetting (SOAP)](usersetting-soap.md) .  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="text-value"></a>Valeur de texte

Aucune.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nom du schéma  <br/> |Schéma de découverte automatique  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération GetUserSettings (SOAP)](getusersettings-operation-soap.md)
- [Opération GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md)
- [Opération GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)

