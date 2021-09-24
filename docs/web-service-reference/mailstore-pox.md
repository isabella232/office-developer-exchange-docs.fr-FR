---
title: MailStore (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: af338f99-9e62-4124-9bff-8d7cc2008161
description: L’élément MailStore contient les spécifications de connexion d’un client à la boîte aux lettres de l’utilisateur à l’aide du protocole MAPI/HTTP.
ms.openlocfilehash: 543bcb8df84904f2b70d6feeabf16d1cc021f3e5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59511121"
---
# <a name="mailstore-pox"></a>MailStore (POX)

**L’élément MailStore** contient les spécifications de connexion d’un client à la boîte aux lettres de l’utilisateur à l’aide du protocole MAPI/HTTP. 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[MailStore (POX)](mailstore-pox.md)
  
```XML
<MailStore>
   <ExternalUrl/>
   <InternalUrl/>
</MailStore>
```

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[ExternalUrl (POX)](externalurl-pox.md) <br/> |Contient l’URL qui doit être utilisée pour accéder à la boîte aux lettres de l’utilisateur depuis l’extérieur du réseau de l’organisation au moyen du protocole MAPI/HTTP.  <br/> |
|[InternalUrl (POX)](internalurl-pox.md) <br/> |Contient l’URL qui doit être utilisée pour accéder à la boîte aux lettres de l’utilisateur à partir de l’intérieur du réseau de l’organisation au moyen du protocole MAPI/HTTP.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Protocol (POX)](protocol-pox.md) <br/> |Contient les spécifications de connexion d’un client au serveur d’accès au client.  <br/> |
   
## <a name="remarks"></a>Remarques

**L’élément MailStore** est présent dans une réponse qui a un élément de protocole [(POX)](protocol-pox.md) avec une valeur d’attribut **Type** de « mapiHttp ». 
  
L’élément **MailStore** est disponible pour les clients qui implémentent le protocole MAPI/HTTP et les Exchange Online cibles, les Exchange Online dans le cadre de Office 365 et les versions sur site de Exchange à partir de la build 15.00.0847.032 (Exchange Server 2013 SP1). 
  
## <a name="see-also"></a>Voir aussi



[Éléments XML de découverte automatique POX pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

