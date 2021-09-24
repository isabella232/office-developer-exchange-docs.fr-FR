---
title: Response (GetOrganizationRelationship) (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: e6bbe800-3cbc-48b2-87b3-2043f575e88b
description: L’élément Response contient les informations de réponse de l’opération GetOrganizationRelationshipSettings (SOAP). L’élément Response est uniquement à usage interne. Cet élément n’est pas utilisé par les clients.
ms.openlocfilehash: 4aed4721fd443c5068055f4d802793e7cd1be14d
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59514150"
---
# <a name="response-getorganizationrelationship-soap"></a>Response (GetOrganizationRelationship) (SOAP)

**L’élément Response** contient les informations de réponse [de l’opération GetOrganizationRelationshipSettings (SOAP).](getorganizationrelationshipsettings-operation-soap.md) **L’élément Response** est uniquement à usage interne. Cet élément n’est pas utilisé par les clients. 
  
```XML
<GetOrganizationRelationshipSettingsResponse>
   <ErrorCode/>
   <ErrorMessage/>
   <OrganizationRelationshipSettingsCollection/>
</GetOrganizationRelationshipSettingResponse>
```

 **GetOrganizationRelationshipSettingsResponse**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[ErrorCode (SOAP)](errorcode-soap.md) <br/> |Représente un code d’erreur renvoyé par le service de découverte automatique.  <br/> |
|[ErrorMessage (SOAP)](errormessage-soap.md) <br/> |Représente un message associé à un code d’erreur renvoyé par le service de découverte automatique.  <br/> |
|[OrganizationRelationshipSettingsCollection (SOAP)](organizationrelationshipsettingscollection-soap.md) <br/> |Représente une liste des relations d’organisation qui correspondent à la requête.  <br/> |
   
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



[Opération GetOrganizationRelationshipSettings (SOAP)](getorganizationrelationshipsettings-operation-soap.md)

