---
title: Demande (GetDomainSettings) (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 3ea026fc-74f1-4118-86ae-908ed4f82a4b
description: L’élément de demande contient une demande pour renvoyer les paramètres de domaine.
ms.openlocfilehash: 71a6072d476fd665dad8b0c0fe388a40db56e059
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829135"
---
# <a name="request-getdomainsettings-soap"></a>Demande (GetDomainSettings) (SOAP)

L’élément de **demande** contient une demande pour renvoyer les paramètres de domaine. 
  
```xml
<Request>
   <Domains/>
   <RequestedSettings/>
</Request>
```

 **GetDomainSettingsRequest**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Domaines (SOAP)](domains-soap.md) <br/> |Représente les domaines les configurations pour lesquelles sont retournées dans une [opération GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md) ou les domaines de que l’organisation a fédérés dans une [opération GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md).  <br/> |
|[RequestedSettings (SOAP)](requestedsettings-soap.md) <br/> |Contient les noms des paramètres de configuration demandé.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetDomainSettingsRequestMessage (SOAP)](getdomainsettingsrequestmessage-soap.md) <br/> |Représente une demande [d’opération GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md).  <br/> |
   
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



[Opération GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)

