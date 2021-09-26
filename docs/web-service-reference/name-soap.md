---
title: Name (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: dce6d823-dc33-4a47-babe-6370a15ac7b4
description: L’élément Name représente le nom d’un paramètre.
ms.openlocfilehash: 39bb2b6bbf7e29dedb13a9bf828f130c076dfb6b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541993"
---
# <a name="name-soap"></a>Name (SOAP)

**L’élément Name** représente le nom d’un paramètre. 
  
```XML
<Name/>
```

**chaîne**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[DomainSetting (SOAP)](domainsetting-soap.md) <br/> |Contient les paramètres de domaine renvoyés par la [demande d’opération GetDomainSettings (SOAP).](getdomainsettings-operation-soap.md)  <br/> |
|[DomainStringSetting (SOAP)](domainstringsetting-soap.md) <br/> |Représente un paramètre de domaine dont la valeur est de type chaîne.  <br/> |
|[OrganizationRelationshipSettings (SOAP)](organizationrelationshipsettings-soap.md) <br/> |Représente une liste de relations organisationnelles pour une seule organisation.  <br/> |
|[UserSetting (SOAP)](usersetting-soap.md) <br/> |Représente un paramètre utilisateur unique.  <br/> |
|[ProtocolConnectionCollectionSetting (SOAP)](protocolconnectioncollectionsetting-soap.md) <br/> |Représente une collection de paramètres de connexion de protocole serveur.  <br/> |
|[StringSetting (SOAP)](stringsetting-soap.md) <br/> |Représente un utilisateur qui a pour valeur une chaîne de type.  <br/> |
|[WebClientUrlCollectionSetting (SOAP)](webclienturlcollectionsetting-soap.md) <br/> |Représente un paramètre utilisateur qui est une collection d’URL Exchange client Web.  <br/> |
|[AlternateMailboxCollectionSetting (SOAP)](alternatemailboxcollectionsetting-soap.md) <br/> |Contient une collection de paramètres de boîte aux lettres de remplacement.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur de texte de **l’élément Name** est le nom d’un paramètre. 
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nom du schéma  <br/> |Schéma de découverte automatique  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)
- [Opération GetUserSettings (SOAP)](getusersettings-operation-soap.md)
- [Opération GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md)
- [Opération GetOrganizationRelationshipSettings (SOAP)](getorganizationrelationshipsettings-operation-soap.md)

