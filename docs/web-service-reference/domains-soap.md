---
title: Domaines (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 5f81d1b7-c6a4-456f-9935-13d04a3d92d7
description: L’élément Domains représente la collection de domaines renvoyée dans une opération GetDomainSettings (SOAP), les domaines que l’organisation a fédérés dans une opération GetFederationInformation (SOAP) ou les domaines avec une relation d’organisation, comme renvoyé par l’opération GetOrganizationRelationshipSettings (SOAP).
ms.openlocfilehash: 667b2611ce8b393252f9bdda6dd7ec201b605047
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59538322"
---
# <a name="domains-soap"></a>Domaines (SOAP)

L’élément **Domains** représente la collection de domaines renvoyée dans une opération [GetDomainSettings (SOAP),](getdomainsettings-operation-soap.md)les domaines que l’organisation a fédérés dans une opération [GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md)ou les domaines avec une relation d’organisation, comme renvoyé par [l’opération GetOrganizationRelationshipSettings (SOAP).](getorganizationrelationshipsettings-operation-soap.md)
  
```XML
<Domains>
   <Domain/>
</Domains>
```

 **Domaines**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Domaine (SOAP)](domain-soap.md) <br/> |Représente un domaine unique.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetDomainSettingsRequest (SOAP)](getdomainsettingsrequest-soap.md) <br/> |Représente une [demande d’opération GetDomainSettings (SOAP).](getdomainsettings-operation-soap.md)  <br/> |
|[Response (GetFederationInformation) (SOAP)](response-getfederationinformationsoap.md) <br/> |Contient les informations de réponse de l’opération [GetFederationInformation (SOAP).](getfederationinformation-operation-soap.md)  <br/> |
|[GetOrganizationRelationshipSettingsRequest (SOAP)](getorganizationrelationshipsettingsrequest-soap.md) <br/> |Représente une [demande d’opération GetOrganizationRelationshipSettings (SOAP).](getorganizationrelationshipsettings-operation-soap.md)  <br/> |
   
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

- [GetDomainSettingsRequest (SOAP)](getdomainsettingsrequest-soap.md)  
- [GetFederationInformationResponse (SOAP)](getfederationinformationresponse-soap.md)

