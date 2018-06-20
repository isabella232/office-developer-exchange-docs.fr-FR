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
description: L’élément GetFederationInformationResponse contient la réponse de l’opération (SOAP) GetFederationInformation.
ms.openlocfilehash: 28b002b45968278ad4c7160b4eed29721422646d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756614"
---
# <a name="getfederationinformationresponse-soap"></a>GetFederationInformationResponse (SOAP)

L’élément **GetFederationInformationResponse** contient la réponse de [l’opération GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md) . 
  
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

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[ErrorCode (SOAP)](errorcode-soap.md) <br/> |Représente un code d’erreur retourné par le service de découverte automatique.  <br/> |
|[ErrorMessage (SOAP)](errormessage-soap.md) <br/> |Représente un message qui est associé à un code d’erreur retourné par le service de découverte automatique.  <br/> |
|[ApplicationUri (SOAP)](applicationuri-soap.md) <br/> |Définit l’emplacement d’une application.  <br/> |
|[TokenIssuers (SOAP)](tokenissuers-soap.md) <br/> |Représente une collection de jetons de sécurité qui contiennent des points de terminaison et les identificateurs de service de jeton de sécurité.  <br/> |
|[Domaines (SOAP)](domains-soap.md) <br/> |Représente les domaines les configurations pour lesquelles sont retournées dans une opération de [l’opération GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md) **GetDomainSettings** ou les domaines de que l’organisation a fédérés dans une [opération GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md) Opération **GetFederationInformation** .  <br/> |
   
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



[Opération GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md)

