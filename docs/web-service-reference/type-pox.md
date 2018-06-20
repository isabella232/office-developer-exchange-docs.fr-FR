---
title: Type (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 9a627244-554f-4223-b9d8-a601b81a4a1a
description: L’élément Type identifie le type du compte de messagerie configuré.
ms.openlocfilehash: 6e1349769c6a5349304f576419e0c609d3edd9a0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838783"
---
# <a name="type-pox"></a>Type (POX)

L’élément **Type** identifie le type du compte de messagerie configuré. 
  
[Découverte automatique (POX)](autodiscover-pox.md)
  
[Réponse (POX)](response-pox.md)
  
[Compte (POX)](account-pox.md)
  
[Protocole (POX)](protocol-pox.md)
  
[Type (POX)](type-pox.md)
  
```XML
<Type>WEB or EXCH or EXPR or EXHTTP</Type>
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
|[Protocole (POX)](protocol-pox.md) <br/> |Contient les spécifications pour la connexion d’un client sur le serveur Exchange.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

La valeur de texte représente le type de compte de messagerie. Le tableau suivant répertorie les valeurs possibles.
  
|**Valeur**|**Description**|
|:-----|:-----|
|EXCH  <br/> |Le protocole utilisé pour se connecter au serveur est RPC Exchange.  <br/> |
|EXHTTP  <br/> |Le protocole utilisé pour se connecter aux connexions RPC/HTTP server.  <br/> |
|EXPR  <br/> |Le protocole utilisé pour se connecter au serveur est Exchange RPC sur HTTP, à l’aide d’un serveur proxy RPC.  <br/> Cela s’applique uniquement lorsque l’élément [AccountType (POX)](accounttype-pox.md) est définie pour les courriers électroniques.  <br/> |
|WEB  <br/> |Courrier électronique est accessible à partir d’un navigateur Web à l’aide de l’URL qui est spécifié dans l’élément [Serveur (POX)](server-pox.md) .  <br/> Cela s’applique uniquement lorsque l’élément [AccountType (POX)](accounttype-pox.md) est définie pour les courriers électroniques.  <br/> |
   
### <a name="version-differences"></a>Différences entre les versions

Office 365, Exchange Online et les versions locales d’Exchange commençant par créer 15.00.0995.014 retour une valeur de « EXHTTP » uniquement si le serveur est configuré pour accepter les connexions RPC/HTTP et le client inclut un en-tête [X-ClientCanHandle](pox-autodiscover-request-for-exchange.md) qui contient « ExHttpInfo ». 
  
## <a name="see-also"></a>Voir aussi



[Éléments du fichier XML Autodiscover variole pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

