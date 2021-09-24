---
title: EcpUrl-mt (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: 5221745b-572c-44a5-afdb-41b58af44971
description: L’élément EcpUrl-mt spécifie une URL partielle qui peut être combinée avec la valeur de l’élément EcpUrl (POX) pour générer une URL qui peut être utilisée pour accéder aux paramètres de suivi des messages électroniques pour un utilisateur à extension messagerie.
ms.openlocfilehash: bb0a60f3b3a2d65421164e40537e7514df20e357
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59520814"
---
# <a name="ecpurl-mt-pox"></a>EcpUrl-mt (POX)

L’élément **EcpUrl-mt** spécifie une URL partielle qui peut être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour accéder aux paramètres de suivi des messages électroniques pour un utilisateur à extension messagerie. 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[EcpUrl-mt (POX)](ecpurl-mt-pox.md)
  
```XML
<EcpUrl-mt/>
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
|[Protocol (POX)](protocol-pox.md) <br/> |Contient les spécifications de connexion d’un client à l’ordinateur qui exécute Microsoft Exchange Server sur qui le rôle serveur d’accès au client est installé.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur de texte représente une URL partielle qui peut être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour accéder aux paramètres de suivi des e-mails de l’utilisateur. La valeur de l’élément **EcpUrl-mt** contient les paramètres contenus dans les caractères « < » et « > » qui sont remplacés par le client, comme indiqué dans le tableau suivant. 
  
|**Paramètre**|**Remplacer par**|
|:-----|:-----|
| _IsOwa_ <br/> |n  <br/> |
| _MsgID_ <br/> |Identificateur de message Internet du message à suivre comme spécifié par l’en-tête Message-ID.  <br/> |
| _Mbx_ <br/> |Adresse SMTP du propriétaire de la boîte aux lettres.  <br/> |
| _Sender_ <br/> |Adresse SMTP de l’expéditeur du message.  <br/> |
   
## <a name="remarks"></a>Remarques

**L’élément EcpUrl-mt** est un élément enfant facultatif de **l’élément Protocol.** 
  
## <a name="see-also"></a>Voir aussi



[Éléments XML de découverte automatique POX pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

