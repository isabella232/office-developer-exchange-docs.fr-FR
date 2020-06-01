---
title: ExternalUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 3b647d88-6feb-40d7-9299-b2ca47b707db
description: L’élément ExternalUrl contient l’URL permettant de connecter un client au serveur de carnet d’adresses ou à la boîte aux lettres d’un utilisateur à l’extérieur de l’organisation de l’utilisateur à l’aide du protocole MAPI/HTTP.
ms.openlocfilehash: 94265051be68ed06d1dab8d46dd4ce29d8694c93
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457955"
---
# <a name="externalurl-pox"></a>ExternalUrl (POX)

L’élément **ExternalURL** contient l’URL permettant de connecter un client au serveur de carnet d’adresses ou à la boîte aux lettres d’un utilisateur à l’extérieur de l’organisation de l’utilisateur à l’aide du protocole MAPI/http. 
  
```XML
<ExternalUrl/>
```

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[AddressBook (POX)](addressbook-pox.md) <br/> |Contient les spécifications relatives à la connexion d’un client au serveur de carnet d’adresses à l’aide du protocole MAPI/HTTP.  <br/> |
|[MailStore (POX)](mailstore-pox.md) <br/> |Contient les spécifications relatives à la connexion d’un client à la boîte aux lettres de l’utilisateur à l’aide du protocole MAPI/HTTP.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur texte représente une URL qui peut être utilisée pour accéder à un serveur de carnet d’adresses ou à une boîte aux lettres d’utilisateur à l’extérieur de l’organisation de l’utilisateur.
  
## <a name="remarks"></a>Remarques

L’élément **ExternalURL** peut être présent dans une réponse qui a un élément [Protocol (POX)](protocol-pox.md) avec une valeur d’attribut **type** « MAPI ». 
  
L’élément **ExternalURL** est disponible pour les clients qui implémentent le protocole MAPI/http et ciblent Exchange Online, Exchange Online dans le cadre d’Office 365 et les versions locales d’Exchange à partir de Build 15.00.0847.032 (Exchange Server 2013 SP1). 
  
## <a name="see-also"></a>Voir aussi



[Éléments XML de découverte automatique de la VARIOle pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

