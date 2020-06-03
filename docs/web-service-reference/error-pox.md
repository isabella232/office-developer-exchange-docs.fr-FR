---
title: Erreur (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 91c63b62-ab68-4c32-a2f7-5a87c188335b
description: L’élément error contient une réponse d’erreur de découverte automatique.
ms.openlocfilehash: 1a1a3e83898674e605921cb75371036a8a561a95
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530648"
---
# <a name="error-pox"></a>Erreur (POX)

L’élément **Error** contient une réponse d’erreur de découverte automatique. 
  
[Découverte automatique (POX)](autodiscover-pox.md)
  
[Réponse (POX)](response-pox.md)
  
[Compte (POX)](account-pox.md)
  
[Erreur (POX)](error-pox.md)
  
```xml
<Error Time="" Id="">
   <ErrorCode/>
   <Message/>
   <DebugData/>
</Error>
```

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|Time  <br/> |Représente l’heure à laquelle la réponse d’erreur a été renvoyée.  <br/> |
|ID  <br/> |Représente un hachage du nom de l’ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d’accès au client est installé.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[ErrorCode (POX)](errorcode-pox.md) <br/> |Contient le code d’erreur d’une réponse de découverte automatique d’erreur.  <br/> |
|[Message (POX)](message-pox.md) <br/> |Contient le message d’erreur pour une réponse de découverte automatique d’erreur.  <br/> |
|[DebugData (POX)](debugdata-pox.md) <br/> |Contient les données de débogage pour une réponse de découverte automatique d’erreur.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Compte (POX)](account-pox.md) <br/> |Contient une réponse d’erreur de découverte automatique.  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Éléments XML de découverte automatique de la VARIOle pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

