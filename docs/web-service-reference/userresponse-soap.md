---
title: UserResponse (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 5007b1ba-bfcc-40d7-b1cb-e32fbaf54ffd
description: L’élément UserResponse représente une réponse à une demande GetUserSettings pour un utilisateur individuel.
ms.openlocfilehash: 8def0183a5c2e212e80699a3c2f58c64f67ce690
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59538540"
---
# <a name="userresponse-soap"></a>UserResponse (SOAP)

**L’élément UserResponse** représente une réponse à une demande GetUserSettings pour un utilisateur individuel. 
  
```XML
<UserResponse>
   <ErrorCode/>
   <ErrorMessage/>
   <RedirectTarget/>
   <UserSettingErrors/>
   <UserSettings/>
</UserResponse>
```

 **UserResponse**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[ErrorCode (SOAP)](errorcode-soap.md) <br/> |Représente un code d’erreur renvoyé par le service de découverte automatique.  <br/> |
|[ErrorMessage (SOAP)](errormessage-soap.md) <br/> |Représente un message associé à un code d’erreur renvoyé par le service de découverte automatique.  <br/> |
|[RedirectTarget (SOAP)](redirecttarget-soap.md) <br/> |Contient la cible de l’URL ou de l’adresse e-mail de redirection.  <br/> |
|[UserSettingErrors (SOAP)](usersettingerrors-soap.md) <br/> |Représente une collection d’informations sur les paramètres qui n’ont pas pu être renvoyés.  <br/> |
|[UserSettings (SOAP)](usersettings-soap.md) <br/> |Paramètres demandés pour l’utilisateur.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ArrayOfUserResponse (SOAP)](arrayofuserresponse-soap.md) <br/> |Contient un tableau de réponses utilisateur.  <br/> |
|[UserResponses (SOAP)](userresponses-soap.md) <br/> |Contient les paramètres de configuration pour chaque utilisateur demandé.  <br/> |
   
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nom du schéma  <br/> |Schéma de découverte automatique  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Éléments XML de découverte automatique SOAP pour Exchange 2013](soap-autodiscover-xml-elements-for-exchange-2013.md)

