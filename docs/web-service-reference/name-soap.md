---
title: Nom (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: dce6d823-dc33-4a47-babe-6370a15ac7b4
description: L’élément Name représente le nom d’un paramètre.
ms.openlocfilehash: 4689c306bb805a40fea0d58c9e04a5a47d3bb14d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828506"
---
# <a name="name-soap"></a>Nom (SOAP)

L’élément **Name** représente le nom d’un paramètre. 
  
```XML
<Name/>
```

**string**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[DomainSetting (SOAP)](domainsetting-soap.md) <br/> |Contient les paramètres de domaine qui sont renvoyées par la requête [d’opération GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md) .  <br/> |
|[DomainStringSetting (SOAP)](domainstringsetting-soap.md) <br/> |Représente un paramètre du domaine dont la valeur est de type chaîne.  <br/> |
|[OrganizationRelationshipSettings (SOAP)](organizationrelationshipsettings-soap.md) <br/> |Représente une liste des relations d’organisation pour une organisation unique.  <br/> |
|[UserSetting (SOAP)](usersetting-soap.md) <br/> |Représente un paramètre d’utilisateur unique.  <br/> |
|[ProtocolConnectionCollectionSetting (SOAP)](protocolconnectioncollectionsetting-soap.md) <br/> |Représente une collection de paramètres de connexion de protocole de serveur.  <br/> |
|[StringSetting (SOAP)](stringsetting-soap.md) <br/> |Représente un paramètre de l’utilisateur dont la valeur est de type chaîne.  <br/> |
|[WebClientUrlCollectionSetting (SOAP)](webclienturlcollectionsetting-soap.md) <br/> |Représente un utilisateur de paramètre qui est une collection d’URL de client Web Exchange.  <br/> |
|[AlternateMailboxCollectionSetting (SOAP)](alternatemailboxcollectionsetting-soap.md) <br/> |Contient une collection de paramètres de boîte aux lettres de substitution.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

La valeur de texte de l’élément **Name** est le nom d’un paramètre. 
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nom du schéma  <br/> |Schéma de découverte automatique  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)
- [Opération GetUserSettings (SOAP)](getusersettings-operation-soap.md)
- [Opération GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md)
- [Opération GetOrganizationRelationshipSettings (SOAP)](getorganizationrelationshipsettings-operation-soap.md)

