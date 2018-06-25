---
title: GetOrganizationRelationshipSettingsResponse (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 2f43b817-92c2-4e04-8095-479d790f768c
description: L’élément GetOrganizationRelationshipSettingsResponse contient la réponse de l’opération (SOAP) GetOrganizationRelationshipSettings. L’élément GetOrganizationRelationshipSettingsResponse est à usage interne uniquement. Cet élément n’est pas utilisé par les clients.
ms.openlocfilehash: 907113df2186a93345c6e0bc7dd470909508bd38
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756692"
---
# <a name="getorganizationrelationshipsettingsresponse-soap"></a>GetOrganizationRelationshipSettingsResponse (SOAP)

L’élément **GetOrganizationRelationshipSettingsResponse** contient la réponse de [l’opération GetOrganizationRelationshipSettings (SOAP)](getorganizationrelationshipsettings-operation-soap.md) . L’élément **GetOrganizationRelationshipSettingsResponse** est à usage interne uniquement. Cet élément n’est pas utilisé par les clients. 
  
```XML
<GetOrganizationRelationshipSettingResponse>
   <ErrorCode/>
   <ErrorMessage/>
   <OrganizationRelationshipSettingsCollection/>
</GetOrganizationRelationshipSettingResponse>
```

 **GetOrganizationRelationshipSettingsResponse**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[ErrorCode (SOAP)](errorcode-soap.md) <br/> |Représente un code d’erreur retourné par le service de découverte automatique.  <br/> |
|[ErrorMessage (SOAP)](errormessage-soap.md) <br/> |Représente un message qui est associé à un code d’erreur retourné par le service de découverte automatique.  <br/> |
|[OrganizationRelationshipSettingsCollection (SOAP)](organizationrelationshipsettingscollection-soap.md) <br/> |Représente une collection de relations qui correspondent à la requête.  <br/> |
   
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



[Opération GetOrganizationRelationshipSettings (SOAP)](getorganizationrelationshipsettings-operation-soap.md)

