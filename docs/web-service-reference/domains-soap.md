---
title: Domaines (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 5f81d1b7-c6a4-456f-9935-13d04a3d92d7
description: L’élément de domaines représente la collection de domaine qui est retournée dans une opération de GetDomainSettings (SOAP), les domaines que l’organisation a fédérés dans une opération de GetFederationInformation (SOAP) ou les domaines avec une relation d’organisation renvoyée par l’opération GetOrganizationRelationshipSettings (SOAP).
ms.openlocfilehash: 7a21a3a09516de2d1c38021ca3ccd2161d9cdd1e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756040"
---
# <a name="domains-soap"></a>Domaines (SOAP)

L’élément de **domaines** représente la collection de domaine qui est retournée dans une [opération GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md), les domaines que l’organisation a fédérés dans une [opération GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md)ou les domaines avec une relation d’organisation renvoyé par [l’opération GetOrganizationRelationshipSettings (SOAP)](getorganizationrelationshipsettings-operation-soap.md).
  
```XML
<Domains>
   <Domain/>
</Domains>
```

 **Domaines**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Domaine (SOAP)](domain-soap.md) <br/> |Représente un seul domaine.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetDomainSettingsRequest (SOAP)](getdomainsettingsrequest-soap.md) <br/> |Représente une demande [d’opération GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md) .  <br/> |
|[Réponse (GetFederationInformation) (SOAP)](response-getfederationinformationsoap.md) <br/> |Contient les informations de réponse de [l’opération GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md) .  <br/> |
|[GetOrganizationRelationshipSettingsRequest (SOAP)](getorganizationrelationshipsettingsrequest-soap.md) <br/> |Représente une demande [d’opération GetOrganizationRelationshipSettings (SOAP)](getorganizationrelationshipsettings-operation-soap.md) .  <br/> |
   
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

- [GetDomainSettingsRequest (SOAP)](getdomainsettingsrequest-soap.md)  
- [GetFederationInformationResponse (SOAP)](getfederationinformationresponse-soap.md)

