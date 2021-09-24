---
title: TokenType (ClientAccessTokenType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 96103f15-a3e0-497c-af21-90adbf9a4b14
description: L’élément TokenType identifie le type de jeton d’accès client qui sera renvoyé dans la réponse GetClientAccessToken.
ms.openlocfilehash: 967d64796799147876ef6443b40b16154b55c01a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523355"
---
# <a name="tokentype-clientaccesstokentype"></a>TokenType (ClientAccessTokenType)

**L’élément TokenType** identifie le type de jeton d’accès client qui sera renvoyé dans la réponse **GetClientAccessToken.** 
  
```XML
<TokenType>CallerIdentity | ExtensionCallback | ScopedToken</TokenType>
```

 **ClientAccessTokenTypeType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[TokenRequest](tokenrequest.md)  |  [Token (ClientAccessTokenType)](token-clientaccesstokentype.md)
  
## <a name="text-value"></a>Valeur texte

Une valeur textuelle **CallerIdentity** signifie qu’un jeton d’accès client d’identité d’appelant est renvoyé. Une valeur de texte **ExtensionCallback** indique qu’un jeton d’accès client de rappel d’extension est renvoyé. Une valeur de texte **ScopedToken** indique que le jeton d’accès client est un jeton d’étendue. 
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |false  <br/> |
   

