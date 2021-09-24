---
title: Response (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 4c2bcdeb-95ce-4ffa-bd83-118af53b534f
description: L’élément Response contient la réponse à une opération GetUserSettings (SOAP), à une opération GetDomainSettings (SOAP) ou à une demande d’opération GetFederationInformation (SOAP).
ms.openlocfilehash: d42014991db8e93f88b80bed97970f043290cfb1
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59512358"
---
# <a name="response-soap"></a>Response (SOAP)

**L’élément Response** contient la réponse à une opération [GetUserSettings (SOAP),](getusersettings-operation-soap.md)à une opération [GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)ou à une demande d’opération [GetFederationInformation (SOAP).](getfederationinformation-operation-soap.md) 
  
```XML
<Response>
   <ErrorCode/>
   <ErrorMessage/>
   <UserResponses/>
</Response>
```

 **GetUserSettingsResponse**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[ErrorCode (SOAP)](errorcode-soap.md) <br/> |Représente un code d’erreur renvoyé par le service de découverte automatique.  <br/> |
|[ErrorMessage (SOAP)](errormessage-soap.md) <br/> |Représente un message associé à un code d’erreur renvoyé par le service de découverte automatique.  <br/> |
|[UserResponses (SOAP)](userresponses-soap.md) <br/> |Contient les paramètres de configuration pour chaque utilisateur demandé.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetUserSettingsResponseMessage (SOAP)](getusersettingsresponsemessage-soap.md) <br/> |Définit une réponse à [une demande GetUserSettingsRequest (SOAP)](getusersettingsrequest-soap.md) <br/> |
|[GetDomainSettingsResponseMessage (SOAP)](getdomainsettingsresponsemessage-soap.md) <br/> |Définit une réponse à [une demande GetDomainSettingsRequest (SOAP).](getdomainsettingsrequest-soap.md)  <br/> |
|[GetFederationInformationResponseMessage (SOAP)](getfederationinformationresponsemessage-soap.md) <br/> |Définit une réponse à [une getFederationInformationRequest (SOAP)](getfederationinformationrequest-soap.md).  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucune.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nom du schéma  <br/> |Schéma de découverte automatique  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetUserSettings (SOAP)](getusersettings-operation-soap.md)


[Référence de service web de découverte automatique pour Exchange](autodiscover-web-service-reference-for-exchange.md)
  
[Éléments XML de découverte automatique SOAP pour Exchange 2013](soap-autodiscover-xml-elements-for-exchange-2013.md)

