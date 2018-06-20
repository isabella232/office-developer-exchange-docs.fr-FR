---
title: ErrorCode (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 5e5ec861-0191-4ecb-a906-47ce8ed96381
description: L’élément ErrorCode représente un code d’erreur retourné par le service de découverte automatique.
ms.openlocfilehash: 2dd91cec4645325c02bc8588af0ee0547909b945
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756204"
---
# <a name="errorcode-soap"></a>ErrorCode (SOAP)

L’élément **ErrorCode** représente un code d’erreur retourné par le service de découverte automatique. 
  
```XML
<ErrorCode/>
```

 **string**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[AutodiscoverResponse (SOAP)](autodiscoverresponse-soap.md) <br/> |Représente le type de base pour toutes les réponses sont renvoyées par le service de découverte automatique.  <br/> |
|[DomainResponse (SOAP)](domainresponse-soap.md) <br/> |Contient les paramètres requis pour le domaine spécifié.  <br/> |
|[GetDomainSettingsResponse (SOAP)](getdomainsettingsresponse-soap.md) <br/> |Contient la réponse à un appel de [l’opération GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md) pour un domaine spécifique.  <br/> |
|[GetFederationInformationResponse (SOAP)](getfederationinformationresponse-soap.md) <br/> |Contient la réponse à une demande [d’opération GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md) .  <br/> |
|[Réponse (SOAP)](response-soap.md) <br/> |Contient la réponse à une demande [d’opération GetUserSettings (SOAP)](getusersettings-operation-soap.md).  <br/> |
|[UserSettingError (SOAP)](usersettingerror-soap.md) <br/> |Représente une erreur est renvoyée lors de la récupération d’un paramètre de l’utilisateur.  <br/> |
|[Réponse de l’utilisateur (SOAP)](userresponse-soap.md) <br/> |Représente une réponse à une demande de [l’opération GetUserSettings (SOAP)](getusersettings-operation-soap.md) pour un utilisateur individuel.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

La valeur de texte représente le code d’erreur pour une réponse d’erreur de découverte automatique. Le tableau suivant répertorie les valeurs de texte possibles pour l’élément de **code d’erreur** . 
  
|**Valeur texte code d’erreur**|**Description**|
|:-----|:-----|
|NoError  <br/> |Aucune erreur s’est produite.  <br/> |
|RedirectAddress  <br/> |L’appelant doit suivre la redirection d’adresse de messagerie qui a été renvoyée par le service de découverte automatique.  <br/> |
|RedirectUrl  <br/> |L’appelant doit suivre la redirection d’URL qui a été renvoyée par le service de découverte automatique.  <br/> |
|InvalidUser  <br/> |L’utilisateur qui a été passée dans la demande n’est pas valide.  <br/> |
|InvalidRequest  <br/> |La demande n’est pas valide.  <br/> |
|InvalidSetting  <br/> |Un paramètre spécifié n’est pas valide.  <br/> |
|SettingIsNotAvailable  <br/> |Un paramètre spécifié n’est pas disponible.  <br/> |
|ServerBusy  <br/> |Le serveur est trop occupé pour traiter la demande.  <br/> |
|InvalidDomain  <br/> |Le domaine demandé n’est pas valid.  <br/> |
|NotFederated  <br/> |L’organisation n’est pas fédérée.  <br/> |
|InternalServerError  <br/> |Il existe une erreur serveur interne.  <br/> |
   
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nom du schéma  <br/> |Schéma de découverte automatique  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetUserSettings (SOAP)](getusersettings-operation-soap.md)
  
[Opération GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)
  
[Opération GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md)

