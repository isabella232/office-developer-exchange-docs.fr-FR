---
title: TokenType (ClientAccessTokenType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 96103f15-a3e0-497c-af21-90adbf9a4b14
description: L’élément TokenType identifie le type de jeton d’accès au client qui sera renvoyé dans la réponse GetClientAccessToken.
ms.openlocfilehash: 49ba2973967b12396e0c7f56129c89c40ccbcf97
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466051"
---
# <a name="tokentype-clientaccesstokentype"></a>TokenType (ClientAccessTokenType)

L’élément **TokenType** identifie le type de jeton d’accès au client qui sera renvoyé dans la réponse **GetClientAccessToken** . 
  
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

[TokenRequest](tokenrequest.md)  |  [Jeton (ClientAccessTokenType)](token-clientaccesstokentype.md)
  
## <a name="text-value"></a>Valeur texte

Une valeur de texte de **CallerIdentity** signifie qu’un jeton d’accès client d’identité de l’appelant est renvoyé. Une valeur de texte de **ExtensionCallback** indique qu’un jeton d’accès au client de rappel d’extension est renvoyé. Une valeur de texte de **ScopedToken** indique que le jeton d’accès au client est un jeton d’étendue. 
  
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
   

