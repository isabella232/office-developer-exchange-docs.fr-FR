---
title: GetFederationInformationResponse (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 2033c14f-dcc8-43c2-9fd9-a51946ec7055
description: L’élément GetFederationInformationResponse contient la réponse SOAP (GetFederationInformation operation).
ms.openlocfilehash: 20d00f047acae6c9eba1347ae7e8110656fefb4b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59529878"
---
# <a name="getfederationinformationresponse-soap"></a>GetFederationInformationResponse (SOAP)

**L’élément GetFederationInformationResponse** contient la réponse [SOAP (GetFederationInformation](getfederationinformation-operation-soap.md) operation). 
  
```XML
<GetFederationInformationResponse>
   <ErrorCode/>
   <ErrorMessage/>
   <TokenIssuers/>
   <ApplicationUri/>
   <Domains/>
</GetFederationInformationResponse>
```

 **GetFederationInformationResponse**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[ErrorCode (SOAP)](errorcode-soap.md) <br/> |Représente un code d’erreur renvoyé par le service de découverte automatique.  <br/> |
|[ErrorMessage (SOAP)](errormessage-soap.md) <br/> |Représente un message associé à un code d’erreur renvoyé par le service de découverte automatique.  <br/> |
|[ApplicationUri (SOAP)](applicationuri-soap.md) <br/> |Définit l’emplacement d’une application.  <br/> |
|[TokenIssuers (SOAP)](tokenissuers-soap.md) <br/> |Représente une collection de jetons de sécurité, qui contiennent des identificateurs de service de jeton de sécurité et des points de terminaison.  <br/> |
|[Domaines (SOAP)](domains-soap.md) <br/> |Représente les domaines pour lesquels les configurations sont renvoyées dans une opération [GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md) **GetDomainSettings** ou les domaines que l’organisation a fédérés dans une opération [GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md) **GetFederationInformation.**  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
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



[Opération GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md)

