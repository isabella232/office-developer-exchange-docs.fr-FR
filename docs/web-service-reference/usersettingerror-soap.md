---
title: UserSettingError (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: abb175c5-4f38-4dcc-81e3-b511686862eb
description: L’élément UserSettingError représente une erreur qui est renvoyée suite à une tentative d’obtention d’un paramètre utilisateur.
ms.openlocfilehash: 61603038ce93780f690d72226b1356b239d2002d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468606"
---
# <a name="usersettingerror-soap"></a>UserSettingError (SOAP)

L’élément **UserSettingError** représente une erreur qui est renvoyée suite à une tentative d’obtention d’un paramètre utilisateur. 
  
```XML
<UserSettingError>
    <ErrorCode/>
    <ErrorMessage/>
    <SettingName/>
</UserSettingError>
```

 **UserSettingError**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[ErrorCode (SOAP)](errorcode-soap.md) <br/> |Représente un code d’erreur renvoyé par le service de découverte automatique.  <br/> |
|[ErrorMessage (SOAP)](errormessage-soap.md) <br/> |Représenté par un message associé à un code d’erreur renvoyé par le service de découverte automatique.  <br/> |
|[Propriétés SettingName (SOAP)](settingname-soap.md) <br/> |Représente le nom d’un paramètre utilisateur.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[UserSettingErrors (SOAP)](usersettingerrors-soap.md) <br/> |Représente une collection d’informations sur les paramètres qui n’ont pas pu être renvoyés.  <br/> |
   
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



[Éléments XML de découverte automatique SOAP pour Exchange 2013](soap-autodiscover-xml-elements-for-exchange-2013.md)

