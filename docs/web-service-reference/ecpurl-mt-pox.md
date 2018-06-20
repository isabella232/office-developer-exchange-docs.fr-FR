---
title: EcpUrl-mt (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 5221745b-572c-44a5-afdb-41b58af44971
description: L’élément EcpUrl-mt spécifie une URL partielle peut être combinée avec la valeur de l’élément EcpUrl (POX) pour générer une URL qui peut être utilisée pour accéder aux paramètres d’un utilisateur à extension messagerie de suivi des messages électroniques.
ms.openlocfilehash: 13954a4dab8e81f4ba75b3578e6ba7f67f4b8b96
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756060"
---
# <a name="ecpurl-mt-pox"></a>EcpUrl-mt (POX)

L’élément **EcpUrl-mt** spécifie une URL partielle peut être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour accéder aux paramètres d’un utilisateur à extension messagerie de suivi des messages électroniques. 
  
[Découverte automatique (POX)](autodiscover-pox.md)
  
[Réponse (POX)](response-pox.md)
  
[Compte (POX)](account-pox.md)
  
[Protocole (POX)](protocol-pox.md)
  
[EcpUrl-mt (POX)](ecpurl-mt-pox.md)
  
```XML
<EcpUrl-mt/>
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
|[Protocole (POX)](protocol-pox.md) <br/> |Contient les spécifications pour connecter un client à l’ordinateur qui exécute Microsoft Exchange Server qui a le rôle de serveur d’accès au Client est installé.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

La valeur de texte représente une URL partielle peut être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut servir à accéder à leur messagerie suivi des paramètres de l’utilisateur. La valeur de l’élément **EcpUrl-mt** contient des paramètres contenus dans « < » et « > » caractères sont remplacés par le client, comme indiqué dans le tableau suivant. 
  
|**Paramètre**|**Remplacer par**|
|:-----|:-----|
| _IsOwa_ <br/> |n  <br/> |
| _Identificateur de message_ <br/> |Identificateur de message Internet du message suivi comme spécifié par l’en-tête de Message-ID.  <br/> |
| _Mbx_ <br/> |L’adresse SMTP du propriétaire de boîte aux lettres.  <br/> |
| _Sender_ <br/> |L’adresse SMTP de l’expéditeur du message.  <br/> |
   
## <a name="remarks"></a>Remarques

L’élément **EcpUrl-mt** est un élément enfant facultatif de l’élément de **protocole** . 
  
## <a name="see-also"></a>Voir aussi



[Éléments du fichier XML Autodiscover variole pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

