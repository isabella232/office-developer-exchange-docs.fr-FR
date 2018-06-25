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
description: L’élément AutodiscoverResponse (SOAP) représente l’élément de base pour toutes les réponses sont renvoyées par le service de découverte automatique.
ms.openlocfilehash: b92a71deb77e2b1dee42d970e2dc43a56044487a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755360"
---
# <a name="autodiscoverresponse-soap"></a>AutodiscoverResponse (SOAP)

L’élément **AutodiscoverResponse (SOAP)** représente l’élément de base pour toutes les réponses sont renvoyées par le service de découverte automatique. 
  
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

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[UserResponses (SOAP)](userresponses-soap.md) <br/> |Représente une collection d’éléments de [Réponse utilisateur (SOAP)](userresponse-soap.md) .  <br/> |
|[UserSettingErrors (SOAP)](usersettingerrors-soap.md) <br/> |Représente une collection d’éléments [UserSettingError (SOAP)](usersettingerror-soap.md) .  <br/> |
|[UserSettings (SOAP)](usersettings-soap.md) <br/> |Représente une collection d’éléments [UserSetting (SOAP)](usersetting-soap.md) .  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nom du schéma  <br/> |Schéma de découverte automatique  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération GetUserSettings (SOAP)](getusersettings-operation-soap.md)
- [Opération GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md)
- [Opération GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)

