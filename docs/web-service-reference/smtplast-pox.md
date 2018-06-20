---
title: SMTPLast (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: f1aa8bd9-c6ac-41ac-8d2d-56fb20006005
description: L’élément SMTPLast indique si le serveur SMTP Simple Mail Transfer Protocol () nécessite que courrier électronique doit être téléchargée avant qu’il envoie un message électronique à l’aide du serveur SMTP.
ms.openlocfilehash: 5359f20b33855f4ef48566058bc46bd618e3b2ff
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829505"
---
# <a name="smtplast-pox"></a>SMTPLast (POX)

L’élément **SMTPLast** indique si le serveur SMTP Simple Mail Transfer Protocol () nécessite que courrier électronique doit être téléchargée avant qu’il envoie un message électronique à l’aide du serveur SMTP. 
  
- [Découverte automatique (POX)](autodiscover-pox.md)
  
- [Réponse (POX)](response-pox.md)
  
- [Compte (POX)](account-pox.md)
  
- [Protocole (POX)](protocol-pox.md)
  
- [SMTPLast (POX)](smtplast-pox.md)
  
```xml
<SMTPLast>on or off</SMTPLast>
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
|[Protocole (POX)](protocol-pox.md) <br/> |Contient les spécifications pour connecter un client à l’ordinateur qui exécute Microsoft Exchange Server 2007 ayant le rôle de serveur d’accès au Client est installé.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

La valeur texte spécifie si le serveur SMTP requiert que courrier électronique doit être téléchargée avant qu’il envoie un message électronique à l’aide du serveur SMTP. Les valeurs possibles sont **on** et **off**. La valeur par défaut est **désactivé**.
  
## <a name="see-also"></a>Voir aussi

- [Éléments du fichier XML Autodiscover variole pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

