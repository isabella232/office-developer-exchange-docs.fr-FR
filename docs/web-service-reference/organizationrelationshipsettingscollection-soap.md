---
title: OrganizationRelationshipSettingsCollection (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: 33456abf-a1b6-46da-a864-3ec8af2780de
description: L’élément OrganizationRelationshipSettingsCollection représente une liste de relations d’organisation qui correspondent à la requête. L’élément OrganizationRelationshipSettingsCollection est uniquement à usage interne. Cet élément n’est pas utilisé par les clients.
ms.openlocfilehash: e3bb4c21e77bc22af051c63b714aaaef4d883609
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59514234"
---
# <a name="organizationrelationshipsettingscollection-soap"></a>OrganizationRelationshipSettingsCollection (SOAP)

**L’élément OrganizationRelationshipSettingsCollection** représente une liste de relations d’organisation qui correspondent à la requête. **L’élément OrganizationRelationshipSettingsCollection** est uniquement à usage interne. Cet élément n’est pas utilisé par les clients. 
  
```XML
<OrganizationRelationshipSettingsCollection>
   <OrganizationRelationshipSettings/>
</OrganizationRelationshipSettingsCollection>
```

 **OrganizationRelationshipSettingsCollection**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[OrganizationRelationshipSettings (SOAP)](organizationrelationshipsettings-soap.md) <br/> |Représente la liste des relations d’organisation pour l’organisation sélectionnée et les adresses SMTP.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Response (GetOrganizationRelationship) (SOAP)](response-getorganizationrelationshipsoap.md) <br/> |Contient les informations de réponse de l’opération [SOAP (GetOrganizationRelationshipSettings).](getorganizationrelationshipsettings-operation-soap.md)  <br/> |
   
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

