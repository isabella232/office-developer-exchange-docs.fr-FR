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
description: L’élément OWAUrl décrit l’URL et le schéma d’authentification utilisés pour accéder à un ordinateur spécifique exécutant Microsoft Exchange Server 2007 sur lequel le rôle serveur d’accès au client est installé et qui héberge Outlook Web Access.
ms.openlocfilehash: c0728af063cfbf1353eb7d3b81f5fcfe8b398f7d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457262"
---
# <a name="owaurl-pox"></a>OWAUrl (POX)

L’élément **OWAUrl** décrit l’URL et le schéma d’authentification utilisés pour accéder à un ordinateur spécifique exécutant Microsoft Exchange Server 2007 sur lequel le rôle serveur d’accès au client est installé et qui héberge Outlook Web Access. 
  
[Découverte automatique (POX)](autodiscover-pox.md)
  
[Réponse (POX)](response-pox.md)
  
[Compte (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[Interne (POX)](internal-pox.md)
  
[OWAUrl (POX)](owaurl-pox.md)
  
```xml
<OWAUrl AuthenticationMethod=""/>
```

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**AuthenticationMethod** <br/> |Décrit les méthodes d’authentification permettant d’accéder à Outlook Web Access.  <br/> |
   
#### <a name="authenticationmethod-attribute"></a>Attribut AuthenticationMethod

|**Valeur**|**Description**|
|:-----|:-----|
|WindowsIntegrated  <br/> |Authentification Windows intégrée.  <br/> |
|FBA  <br/> |Authentification basée sur les formulaires.  <br/> |
|NTLM  <br/> |Authentification NTLM.  <br/> |
|Digest  <br/> |Authentification Digest.  <br/> |
|De base  <br/> |Authentification de base.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Interne (POX)](internal-pox.md) <br/> |Contient la collection d’URL Outlook Web Access à laquelle un client peut se connecter lorsqu’il se trouve à l’intérieur du pare-feu.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur texte représente l’URL du service Outlook Web Access sur un serveur d’accès au client.
  
## <a name="see-also"></a>Voir aussi



[Éléments XML de découverte automatique de la VARIOle pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

