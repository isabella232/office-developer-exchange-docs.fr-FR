---
title: Magasin de courrier électronique (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: af338f99-9e62-4124-9bff-8d7cc2008161
description: L’élément de magasin de courrier électronique contient les spécifications pour connecter un client à la boîte aux lettres de l’utilisateur à l’aide du protocole MAPI/HTTP.
ms.openlocfilehash: 4c82c7b61752cf7d91287a3968f6c642f4943855
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828301"
---
# <a name="mailstore-pox"></a>Magasin de courrier électronique (POX)

L’élément de **magasin de courrier électronique** contient les spécifications pour connecter un client à la boîte aux lettres de l’utilisateur à l’aide du protocole MAPI/HTTP. 
  
[Découverte automatique (POX)](autodiscover-pox.md)
  
[Réponse (POX)](response-pox.md)
  
[Compte (POX)](account-pox.md)
  
[Protocole (POX)](protocol-pox.md)
  
[Magasin de courrier électronique (POX)](mailstore-pox.md)
  
```XML
<MailStore>
   <ExternalUrl/>
   <InternalUrl/>
</MailStore>
```

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[ExternalUrl (POX)](externalurl-pox.md) <br/> |Contient l’URL qui doit être utilisé pour accéder à la boîte aux lettres à partir de l’extérieur du réseau de l’organisation au moyen du protocole MAPI/HTTP.  <br/> |
|[InternalUrl (POX)](internalurl-pox.md) <br/> |Contient l’URL qui doit être utilisé pour accéder à la boîte aux lettres à partir de l’intérieur du réseau de l’organisation au moyen du protocole MAPI/HTTP.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Protocole (POX)](protocol-pox.md) <br/> |Contient les spécifications pour la connexion d’un client vers le serveur d’accès au Client.  <br/> |
   
## <a name="remarks"></a>Remarques

L’élément de **magasin de courrier électronique** est présente dans une réponse qui a un élément de [Protocole (POX)](protocol-pox.md) avec une valeur d’attribut de **Type** de « mapiHttp ». 
  
L’élément de **magasin de courrier électronique** est disponible pour les clients qui implémentent le protocole MAPI/HTTP et cible Exchange Online, Exchange Online dans le cadre d’Office 365, et créer des versions locales d’Exchange commençant par 15.00.0847.032 (Exchange Server 2013 SP1). 
  
## <a name="see-also"></a>Voir aussi



[Éléments du fichier XML Autodiscover variole pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

