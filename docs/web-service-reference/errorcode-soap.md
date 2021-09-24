---
title: ErrorCode (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 5e5ec861-0191-4ecb-a906-47ce8ed96381
description: L’élément ErrorCode représente un code d’erreur renvoyé par le service de découverte automatique.
ms.openlocfilehash: fa40cb8b7a2ec80ecf752058f540969013748d39
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59530772"
---
# <a name="errorcode-soap"></a>ErrorCode (SOAP)

**L’élément ErrorCode** représente un code d’erreur renvoyé par le service de découverte automatique. 
  
```XML
<ErrorCode/>
```

 **chaîne**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[AutodiscoverResponse (SOAP)](autodiscoverresponse-soap.md) <br/> |Représente le type de base pour toutes les réponses renvoyées par le service de découverte automatique.  <br/> |
|[DomainResponse (SOAP)](domainresponse-soap.md) <br/> |Contient les paramètres demandés pour le domaine spécifié.  <br/> |
|[GetDomainSettingsResponse (SOAP)](getdomainsettingsresponse-soap.md) <br/> |Contient la réponse à un [appel d’opération GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md) pour un domaine individuel.  <br/> |
|[GetFederationInformationResponse (SOAP)](getfederationinformationresponse-soap.md) <br/> |Contient la réponse à une [demande d’opération GetFederationInformation (SOAP).](getfederationinformation-operation-soap.md)  <br/> |
|[Response (SOAP)](response-soap.md) <br/> |Contient la réponse à [une demande d’opération GetUserSettings (SOAP).](getusersettings-operation-soap.md)  <br/> |
|[UserSettingError (SOAP)](usersettingerror-soap.md) <br/> |Représente une erreur renvoyée lors de la récupération d’un paramètre utilisateur.  <br/> |
|[UserResponse (SOAP)](userresponse-soap.md) <br/> |Représente une réponse à une [demande d’opération GetUserSettings (SOAP)](getusersettings-operation-soap.md) pour un utilisateur individuel.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur de texte représente le code d’erreur pour une réponse d’erreur de découverte automatique. Le tableau suivant répertorie les valeurs de texte possibles pour **l’élément ErrorCode.** 
  
|**Valeur de texte du code d’erreur**|**Description**|
|:-----|:-----|
|NoError  <br/> |Aucune erreur n’a été produite.  <br/> |
|RedirectAddress  <br/> |L’appelant doit suivre la redirection d’adresse de messagerie qui a été renvoyée par la découverte automatique.  <br/> |
|RedirectUrl  <br/> |L’appelant doit suivre la redirection d’URL qui a été renvoyée par la découverte automatique.  <br/> |
|InvalidUser  <br/> |L’utilisateur qui a été transmis dans la demande n’est pas valide.  <br/> |
|InvalidRequest  <br/> |La demande n’est pas valide.  <br/> |
|InvalidSetting  <br/> |Un paramètre spécifié n’est pas valide.  <br/> |
|SettingIsNotAvailable  <br/> |Un paramètre spécifié n’est pas disponible.  <br/> |
|ServerBusy  <br/> |Le serveur est trop occupé pour traiter la demande.  <br/> |
|InvalidDomain  <br/> |Domaine demandé non valide.  <br/> |
|NotFederated  <br/> |L’organisation n’est pas fédérée.  <br/> |
|InternalServerError  <br/> |Erreur de serveur interne.  <br/> |
   
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nom du schéma  <br/> |Schéma de découverte automatique  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetUserSettings (SOAP)](getusersettings-operation-soap.md)
  
[Opération GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)
  
[Opération GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md)

