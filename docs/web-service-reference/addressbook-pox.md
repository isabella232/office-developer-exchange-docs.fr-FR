---
title: AddressBook (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: b2d62fd0-741c-4a41-9762-cc7d0ff01c9c
description: L’élément AddressBook contient les spécifications de connexion d’un client au serveur de carnet d’adresses à l’aide du protocole MAPI/HTTP.
ms.openlocfilehash: 28de1d41146b082c8b7f82c868fbbed1ce2c483e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546797"
---
# <a name="addressbook-pox"></a>AddressBook (POX)

**L’élément AddressBook** contient les spécifications de connexion d’un client au serveur de carnet d’adresses à l’aide du protocole MAPI/HTTP. 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[AddressBook (POX)](addressbook-pox.md)
  
```XML
<AddressBook>
   <ExternalUrl/>
   <InternalUrl/>
</AddressBook>
```

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[ExternalUrl (POX)](externalurl-pox.md) <br/> |Contient l’URL qui doit être utilisée pour accéder au carnet d’adresses depuis l’extérieur du réseau de l’organisation à l’aide du protocole MAPI/HTTP.  <br/> |
|[InternalUrl (POX)](internalurl-pox.md) <br/> |Contient l’URL qui doit être utilisée pour accéder au carnet d’adresses depuis l’intérieur du réseau de l’organisation à l’aide du protocole MAPI/HTTP.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Protocol (POX)](protocol-pox.md) <br/> |Contient les spécifications de connexion d’un client au serveur d’accès au client.  <br/> |
   
## <a name="remarks"></a>Remarques

**L’élément AddressBook** est présent dans une réponse qui a un élément de protocole [(POX)](protocol-pox.md) avec une valeur d’attribut **Type** de « mapiHttp ». 
  
L’élément **AddressBook** est disponible pour les clients qui implémentent le protocole MAPI/HTTP et les Exchange Online, Exchange Online cibles dans le cadre de Office 365 et les versions sur site de Exchange à partir de la build 15.00.0847.032 (Exchange Server 2013 SP1). 
  
## <a name="see-also"></a>Voir aussi

- [Éléments XML de découverte automatique POX pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

