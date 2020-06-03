---
title: AddressBook (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: b2d62fd0-741c-4a41-9762-cc7d0ff01c9c
description: L’élément AddressBook contient les spécifications permettant de connecter un client au serveur de carnet d’adresses à l’aide du protocole MAPI/HTTP.
ms.openlocfilehash: 0967ac123cd3bb0086fd004ea0d0d37c08d2e037
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463635"
---
# <a name="addressbook-pox"></a>AddressBook (POX)

L’élément **AddressBook** contient les spécifications permettant de connecter un client au serveur de carnet d’adresses à l’aide du protocole MAPI/http. 
  
[Découverte automatique (POX)](autodiscover-pox.md)
  
[Réponse (POX)](response-pox.md)
  
[Compte (POX)](account-pox.md)
  
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
|[ExternalUrl (POX)](externalurl-pox.md) <br/> |Contient l’URL à utiliser pour accéder au carnet d’adresses en dehors du réseau de l’organisation à l’aide du protocole MAPI/HTTP.  <br/> |
|[InternalUrl (POX)](internalurl-pox.md) <br/> |Contient l’URL à utiliser pour accéder au carnet d’adresses depuis l’intérieur du réseau de l’organisation à l’aide du protocole MAPI/HTTP.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Protocol (POX)](protocol-pox.md) <br/> |Contient les spécifications relatives à la connexion d’un client au serveur d’accès au client.  <br/> |
   
## <a name="remarks"></a>Remarques

L’élément **AddressBook** est présent dans une réponse qui a un élément [Protocol (POX)](protocol-pox.md) avec une valeur d’attribut de **type** « MAPI ». 
  
L’élément **AddressBook** est disponible pour les clients qui implémentent le protocole MAPI/http et ciblent Exchange Online, Exchange Online dans le cadre d’Office 365 et les versions locales d’Exchange à partir de Build 15.00.0847.032 (Exchange Server 2013 SP1). 
  
## <a name="see-also"></a>Voir aussi

- [Éléments XML de découverte automatique de la VARIOle pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

