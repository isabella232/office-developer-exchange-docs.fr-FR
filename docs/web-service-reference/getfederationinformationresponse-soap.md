---
title: GetFederationInformationResponse (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 2033c14f-dcc8-43c2-9fd9-a51946ec7055
description: L’élément GetFederationInformationResponse contient la réponse SOAP (GetFederationInformation Operation).
ms.openlocfilehash: c9e65a2b1759946b8493b3c730f08df6fe353fd8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460042"
---
# <a name="getfederationinformationresponse-soap"></a>GetFederationInformationResponse (SOAP)

L’élément **GetFederationInformationResponse** contient la réponse [SOAP (GetFederationInformation Operation)](getfederationinformation-operation-soap.md) . 
  
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
|[TokenIssuers (SOAP)](tokenissuers-soap.md) <br/> |Représente une collection de jetons de sécurité, qui contiennent des identificateurs de service d’émission de jeton de sécurité et des points de terminaison.  <br/> |
|[Domaines (SOAP)](domains-soap.md) <br/> |Représente les domaines dont les configurations sont renvoyées dans une opération [GetDomainSettings Operation (SOAP)](getdomainsettings-operation-soap.md) **GetDomainSettings** ou les domaines dans lesquels l’organisation a fédéré dans une opération [GetFederationInformation Operation (SOAP)](getfederationinformation-operation-soap.md) **GetFederationInformation** .  <br/> |
   
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



[Opération GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md)

