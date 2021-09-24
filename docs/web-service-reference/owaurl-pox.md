---
title: OWAUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 450b86a1-1722-49f5-b541-16c1edc3db7a
description: L’élément OWAUrl décrit l’URL et le schéma d’authentification utilisés pour accéder à un ordinateur particulier exécutant Microsoft Exchange Server 2007 sur qui le rôle serveur d’accès au client est installé et qui héberge Outlook Web Access.
ms.openlocfilehash: fbd61eb75018c57dada40f5ed7472379d365e752
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59534890"
---
# <a name="owaurl-pox"></a>OWAUrl (POX)

L’élément **OWAUrl** décrit l’URL et le schéma d’authentification utilisés pour accéder à un ordinateur particulier exécutant Microsoft Exchange Server 2007 sur qui le rôle serveur d’accès au client est installé et qui héberge Outlook Web Access. 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[Internal (POX)](internal-pox.md)
  
[OWAUrl (POX)](owaurl-pox.md)
  
```xml
<OWAUrl AuthenticationMethod=""/>
```

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**AuthenticationMethod** <br/> |Décrit les méthodes d’authentification pour accéder à Outlook Web Access.  <br/> |
   
#### <a name="authenticationmethod-attribute"></a>Attribut AuthenticationMethod

|**Valeur**|**Description**|
|:-----|:-----|
|WindowsIntegrated  <br/> |Authentification Windows intégrée.  <br/> |
|FBA  <br/> |Authentification basée sur les formulaires.  <br/> |
|NTLM  <br/> |Authentification NTLM.  <br/> |
|Digérer  <br/> |Authentification Digest.  <br/> |
|De base  <br/> |Authentification de base.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Internal (POX)](internal-pox.md) <br/> |Contient la collection d’URL Outlook Web Access à qui un client peut se connecter lorsqu’il se trouve à l’intérieur du pare-feu.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur de texte représente l’URL du service Outlook Web Access sur un serveur d’accès au client.
  
## <a name="see-also"></a>Voir aussi



[Éléments XML de découverte automatique POX pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

