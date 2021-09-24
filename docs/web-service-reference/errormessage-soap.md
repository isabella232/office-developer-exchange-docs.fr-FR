---
title: ErrorMessage (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: b84dd664-4c49-42c9-a49f-2ec4a9f7588b
description: L’élément ErrorMessage représente un message associé à un code d’erreur renvoyé par le service de découverte automatique.
ms.openlocfilehash: ebaa20f796787862ce3438bd496e29f88cb6ec6a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59517076"
---
# <a name="errormessage-soap"></a>ErrorMessage (SOAP)

**L’élément ErrorMessage** représente un message associé à un code d’erreur renvoyé par le service de découverte automatique. 
  
```XML
<ErrorMessage/>
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

La valeur de texte représente le message d’erreur.
  
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

