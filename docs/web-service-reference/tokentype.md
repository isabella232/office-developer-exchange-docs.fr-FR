---
title: TokenType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 83c650eb-7ab8-480c-a7c9-df60072ee042
description: L’élément TokenType spécifie le type de jeton.
ms.openlocfilehash: a51ddfdd097a94370168077b9eca8be2e0581603
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523319"
---
# <a name="tokentype"></a>TokenType

**L’élément TokenType** spécifie le type de jeton. 
  
```XML
<TokenType> CallerIdentity | ExtensionCallback | ScopedToken </TokenType>
```

 **ClientAccessTokenTypeType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[TokenRequest](tokenrequest.md)  |  [Jeton](token.md)
  
## <a name="text-value"></a>Valeur texte

La valeur de texte de **l’élément TokenType** est le type de jeton. La valeur texte de **CallerIdentity indique** que le jeton est un jeton d’identité d’appelant. La valeur de texte **extensionCallback indique** que le jeton est pour un rappel d’extension. La valeur de texte **ScopedToken** indique que le jeton d’accès client est un jeton d’étendue. 
  
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
   

