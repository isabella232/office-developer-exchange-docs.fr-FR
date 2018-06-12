---
title: TokenRequests
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fbab89e9-b41a-44c4-8ad3-d46aa8e56652
description: L’élément TokenRequests contient un tableau de demandes de jeton.
ms.openlocfilehash: 01d847d7d496a5bd1d5621a3787d0e3cc6ddd7ff
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838772"
---
# <a name="tokenrequests"></a>TokenRequests

L’élément **TokenRequests** contient un tableau de demandes de jeton. 
  
```XML
<TokenRequests>
   <TokenRequest/>
</TokenRequests>
```

 **NonEmptyArrayOfClientAccessTokenRequestsType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

[TokenRequest](tokenrequest.md)
  
### <a name="parent-elements"></a>Éléments parents

[GetClientAccessToken](getclientaccesstoken.md)
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |messages.xsd  <br/> |
|Peut être vide  <br/> ||
   

