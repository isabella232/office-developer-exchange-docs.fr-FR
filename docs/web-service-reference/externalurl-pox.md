---
title: ExternalUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: 3b647d88-6feb-40d7-9299-b2ca47b707db
description: L’élément ExternalUrl contient l’URL de connexion d’un client au serveur de carnet d’adresses ou à la boîte aux lettres d’un utilisateur en dehors de l’organisation de l’utilisateur à l’aide du protocole MAPI/HTTP.
ms.openlocfilehash: 90aaf9cabedba4ea89e0ed47da010245006407ba
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510071"
---
# <a name="externalurl-pox"></a>ExternalUrl (POX)

**L’élément ExternalUrl** contient l’URL de connexion d’un client au serveur de carnet d’adresses ou à la boîte aux lettres d’un utilisateur en dehors de l’organisation de l’utilisateur à l’aide du protocole MAPI/HTTP. 
  
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
|[AddressBook (POX)](addressbook-pox.md) <br/> |Contient les spécifications de connexion d’un client au serveur de carnet d’adresses à l’aide du protocole MAPI/HTTP.  <br/> |
|[MailStore (POX)](mailstore-pox.md) <br/> |Contient les spécifications de connexion d’un client à la boîte aux lettres de l’utilisateur à l’aide du protocole MAPI/HTTP.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur de texte représente une URL qui peut être utilisée pour accéder à un serveur de carnet d’adresses ou à la boîte aux lettres d’un utilisateur depuis l’extérieur de l’organisation de l’utilisateur.
  
## <a name="remarks"></a>Remarques

**L’élément ExternalUrl** peut être présent dans une réponse qui a un élément de protocole [(POX)](protocol-pox.md) avec une valeur d’attribut **Type** de « mapiHttp ». 
  
L’élément **ExternalUrl** est disponible pour les clients qui implémentent le protocole MAPI/HTTP et les Exchange Online cibles, Exchange Online dans le cadre de Office 365 et les versions sur site de Exchange à partir de la build 15.00.0847.032 (Exchange Server 2013 SP1). 
  
## <a name="see-also"></a>Voir aussi



[Éléments XML de découverte automatique POX pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

