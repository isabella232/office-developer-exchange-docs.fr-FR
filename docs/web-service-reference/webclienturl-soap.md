---
title: WebClientUrl (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 7f8cb6d6-4aac-4a1f-8bec-2dcb90fc1df6
description: L’élément WebClientUrl représente l’URL d’un client Web Exchange.
ms.openlocfilehash: bcf9c8d4fe80de8af4c9500e5e850558a8451d4e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464972"
---
# <a name="webclienturl-soap"></a>WebClientUrl (SOAP)

L’élément **WebClientUrl** représente l’URL d’un client Web Exchange. 
  
[UserSetting (SOAP)](usersetting-soap.md)
  
[WebClientUrls (SOAP)](webclienturls-soap.md)
  
[WebClientUrl (SOAP)](webclienturl-soap.md)
  
```XML
<WebClientUrl>
    <AuthenticationMethods/>
    <Url/>
</WebClientUrl>
```

 **WebClientUrl**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[AuthenticationMethods (SOAP)](authenticationmethods-soap.md) <br/> |Représente la méthode d’authentification à utiliser lors de l’accès à l’URL spécifiée.  <br/> |
|[URL (SOAP)](url-soap.md) <br/> |Représente l’adresse Web de l’URL.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[WebClientUrls (SOAP)](webclienturls-soap.md) <br/> |Représente un paramètre utilisateur qui contient une collection d’éléments **WebClientUrl** .  <br/> |
   
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nom du schéma  <br/> |Schéma de découverte automatique  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi



[URL (SOAP)](url-soap.md)
  
[WebClientUrls (SOAP)](webclienturls-soap.md)

