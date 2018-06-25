---
title: Carnet d’adresses (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: b2d62fd0-741c-4a41-9762-cc7d0ff01c9c
description: L’élément de carnet d’adresses contient les spécifications pour la connexion d’un client pour le serveur de carnet d’adresses à l’aide du protocole MAPI/HTTP.
ms.openlocfilehash: c30f0ee7c36de7e63157d07d003a11187d661fd7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755179"
---
# <a name="addressbook-pox"></a>Carnet d’adresses (POX)

L’élément de **Carnet d’adresses** contient les spécifications pour la connexion d’un client pour le serveur de carnet d’adresses à l’aide du protocole MAPI/HTTP. 
  
[Découverte automatique (POX)](autodiscover-pox.md)
  
[Réponse (POX)](response-pox.md)
  
[Compte (POX)](account-pox.md)
  
[Protocole (POX)](protocol-pox.md)
  
[Carnet d’adresses (POX)](addressbook-pox.md)
  
```XML
<AddressBook>
   <ExternalUrl/>
   <InternalUrl/>
</AddressBook>
```

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[ExternalUrl (POX)](externalurl-pox.md) <br/> |Contient l’URL qui doit être utilisé pour accéder au carnet d’adresses à partir de l’extérieur du réseau de l’organisation à l’aide du protocole MAPI/HTTP.  <br/> |
|[InternalUrl (POX)](internalurl-pox.md) <br/> |Contient l’URL qui doit être utilisé pour accéder à du carnet d’adresses à partir de l’intérieur du réseau de l’organisation à l’aide du protocole MAPI/HTTP.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Protocole (POX)](protocol-pox.md) <br/> |Contient les spécifications pour la connexion d’un client vers le serveur d’accès au Client.  <br/> |
   
## <a name="remarks"></a>Remarques

L’élément de **Carnet d’adresses** est présente dans une réponse qui a un élément de [Protocole (POX)](protocol-pox.md) avec une valeur d’attribut de **Type** de « mapiHttp ». 
  
L’élément de **Carnet d’adresses** est disponible pour les clients qui implémentent le protocole MAPI/HTTP et cible Exchange Online, Exchange Online dans le cadre d’Office 365, et créer des versions locales d’Exchange commençant par 15.00.0847.032 (Exchange Server 2013 SP1) . 
  
## <a name="see-also"></a>Voir aussi

- [Éléments du fichier XML Autodiscover variole pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

