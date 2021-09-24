---
title: Response (GetFederationInformation) (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: ca48a4b3-5006-4bb7-973e-d9137ce67e16
description: L’élément Response contient les informations de réponse de l’opération GetFederationInformation (SOAP).
ms.openlocfilehash: b5618dc1d2c862e504ea3134b28edca39c71f62c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523523"
---
# <a name="response-getfederationinformation-soap"></a>Response (GetFederationInformation) (SOAP)

**L’élément Response** contient les informations de réponse [de l’opération GetFederationInformation (SOAP).](getfederationinformation-operation-soap.md) 
  
```XML
<Response>
   <ErrorCode/>
   <ErrorMessage/>
   <ApplicationUri/>
   <Domains/>
</Response>
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
|[Domaines (SOAP)](domains-soap.md) <br/> |Représente la collection de domaines dont les configurations sont renvoyées dans une opération [GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)ou les domaines que l’organisation a fédérés dans une opération [GetFederationInformation (SOAP).](getfederationinformation-operation-soap.md)  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetFederationInformationResponseMessage (SOAP)](getfederationinformationresponsemessage-soap.md) <br/> |Définit une réponse à une [demande d’opération GetFederationInformation (SOAP).](getfederationinformation-operation-soap.md)  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucune.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nom du schéma  <br/> |Schéma de découverte automatique  <br/> |
|Fichier de validation  <br/> |messages.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md)

