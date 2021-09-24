---
title: Type (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 9a627244-554f-4223-b9d8-a601b81a4a1a
description: L’élément Type identifie le type du compte de messagerie configuré.
ms.openlocfilehash: bb92913071509fec46736341bce56b1a00730f6b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59517524"
---
# <a name="type-pox"></a>Type (POX)

**L’élément Type** identifie le type du compte de messagerie configuré. 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[Type (POX)](type-pox.md)
  
```XML
<Type>WEB or EXCH or EXPR or EXHTTP</Type>
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
|[Protocol (POX)](protocol-pox.md) <br/> |Contient les spécifications de connexion d’un client au Exchange serveur.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur texte représente le type de compte de messagerie. Le tableau suivant répertorie les valeurs possibles.
  
|**Valeur**|**Description**|
|:-----|:-----|
|EXCH  <br/> |Le protocole utilisé pour se connecter au serveur est Exchange RPC.  <br/> |
|EXHTTP  <br/> |Protocole utilisé pour se connecter aux connexions RPC/HTTP du serveur.  <br/> |
|EXPR  <br/> |Le protocole utilisé pour se connecter au serveur est Exchange RPC sur HTTP, à l’aide d’un serveur proxy RPC.  <br/> Cela s’applique uniquement lorsque [l’élément AccountType (POX)](accounttype-pox.md) est définie sur e-mail.  <br/> |
|WEB  <br/> |Le courrier électronique est accessible à partir d’un navigateur Web à l’aide de l’URL spécifiée dans l’élément [Server (POX).](server-pox.md)  <br/> Cela s’applique uniquement lorsque [l’élément AccountType (POX)](accounttype-pox.md) est définie sur e-mail.  <br/> |
   
### <a name="version-differences"></a>Différences entre les versions

Office 365, Exchange Online et les versions sur site de Exchange à partir de la build 15.00.0995.014 retournent la valeur « EXHTTP » uniquement si le serveur est configuré pour accepter les connexions RPC/HTTP et que le client inclut un [en-tête X-ClientCanHandle](pox-autodiscover-request-for-exchange.md) qui contient « ExHttpInfo ». 
  
## <a name="see-also"></a>Voir aussi



[Éléments XML de découverte automatique POX pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

