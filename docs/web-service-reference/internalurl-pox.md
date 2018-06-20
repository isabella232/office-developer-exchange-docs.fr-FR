---
title: InternalUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 4649baa9-eec9-426d-952b-361818c25fe0
description: L’élément InternalUrl contient l’URL pour la connexion d’un client pour le serveur de carnet d’adresses ou de boîte aux lettres d’un utilisateur à l’intérieur de l’organisation de l’utilisateur à l’aide du protocole MAPI/HTTP.
ms.openlocfilehash: 3823236081961128b31bb2c0f563062897c55814
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19827950"
---
# <a name="internalurl-pox"></a>InternalUrl (POX)

L’élément **InternalUrl** contient l’URL pour la connexion d’un client pour le serveur de carnet d’adresses ou de boîte aux lettres d’un utilisateur à l’intérieur de l’organisation de l’utilisateur à l’aide du protocole MAPI/HTTP. 
  
```XML
<InternalUrl/>
```

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Carnet d’adresses (POX)](addressbook-pox.md) <br/> |Contient les spécifications pour la connexion d’un client pour le serveur de carnet d’adresses à l’aide du protocole MAPI/HTTP.  <br/> |
|[Magasin de courrier électronique (POX)](mailstore-pox.md) <br/> |Contient les spécifications pour connecter un client à la boîte aux lettres de l’utilisateur à l’aide du protocole MAPI/HTTP.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

La valeur de texte représente une URL qui peut être utilisée pour accéder à un serveur de carnet d’adresses ou de boîte aux lettres d’utilisateur à l’intérieur de l’organisation de l’utilisateur.
  
## <a name="remarks"></a>Remarques

L’élément **InternalUrl** peut être présent dans une réponse qui a un élément de [Protocole (POX)](protocol-pox.md) avec une valeur d’attribut de **Type** de « mapiHttp ». 
  
L’élément **InternalUrl** est disponible pour les clients qui implémentent le protocole MAPI/HTTP et cible Exchange Online, Exchange Online dans le cadre d’Office 365, et créer des versions locales d’Exchange commençant par 15.00.0847.032 (Exchange Server 2013 SP1) . 
  
## <a name="see-also"></a>Voir aussi



[Éléments du fichier XML Autodiscover variole pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

