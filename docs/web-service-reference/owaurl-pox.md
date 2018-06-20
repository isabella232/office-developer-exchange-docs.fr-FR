---
title: OWAUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 450b86a1-1722-49f5-b541-16c1edc3db7a
description: L’élément OWAUrl décrit l’URL et le schéma d’authentification qui est utilisé pour accéder à un ordinateur qui exécute Microsoft Exchange Server 2007 qui a le rôle de serveur Client Access installé qui héberge Outlook Web Access.
ms.openlocfilehash: 93d03506e2a74aa1b4ef6d2a49ccbda01cfc1f9a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828673"
---
# <a name="owaurl-pox"></a>OWAUrl (POX)

L’élément **OWAUrl** décrit l’URL et le schéma d’authentification qui est utilisé pour accéder à un ordinateur qui exécute Microsoft Exchange Server 2007 qui a le rôle de serveur Client Access installé qui héberge Outlook Web Access. 
  
[Découverte automatique (POX)](autodiscover-pox.md)
  
[Réponse (POX)](response-pox.md)
  
[Compte (POX)](account-pox.md)
  
[Protocole (POX)](protocol-pox.md)
  
[Interne (POX)](internal-pox.md)
  
[OWAUrl (POX)](owaurl-pox.md)
  
```xml
<OWAUrl AuthenticationMethod=""/>
```

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**AuthenticationMethod** <br/> |Décrit les méthodes d’authentification pour accéder à Outlook Web Access.  <br/> |
   
#### <a name="authenticationmethod-attribute"></a>Attribut AuthenticationMethod

|**Valeur**|**Description**|
|:-----|:-----|
|WindowsIntegrated  <br/> |Authentification Windows intégrée.  <br/> |
|AVEC AUTHENTIFICATION PAR FORMULAIRE  <br/> |Authentification basée sur les formulaires.  <br/> |
|NTLM  <br/> |Authentification NTLM.  <br/> |
|Digest  <br/> |Authentification Digest.  <br/> |
|Basic  <br/> |Authentification de base.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Interne (POX)](internal-pox.md) <br/> |Contient la collection d’URL Outlook Web Access un client peut se connecter à lorsqu’il est à l’intérieur du pare-feu.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

La valeur de text représente l’URL pour le service d’Outlook Web Access sur un serveur d’accès au Client.
  
## <a name="see-also"></a>Voir aussi



[Éléments du fichier XML Autodiscover variole pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

