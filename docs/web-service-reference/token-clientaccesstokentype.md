---
title: Jeton (ClientAccessTokenType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cddd6075-06b6-4858-9ffa-9db4d9d9b030
description: L’élément Token spécifie un jeton d’accès au client.
ms.openlocfilehash: d195e81d8d20eb2288e921c640c7b2898a5341ab
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467864"
---
# <a name="token-clientaccesstokentype"></a>Jeton (ClientAccessTokenType)

L’élément **Token** spécifie un jeton d’accès au client. 
  
```XML
<Token>
   <Id/>
   <TokenType/>
   <TokenValue/>
   <TTL/>
</Token>
```

 **ClientAccessTokenType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

[ID (chaîne)](id-string.md)  |  [TokenType](tokentype.md)  |  [TokenValue](tokenvalue.md)  |  [TTL](ttl.md)
  
### <a name="parent-elements"></a>Éléments parents

[GetClientAccessTokenResponseMessage](getclientaccesstokenresponsemessage.md)
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> ||
   

