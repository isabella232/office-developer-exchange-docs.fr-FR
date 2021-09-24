---
title: Erreur (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 91c63b62-ab68-4c32-a2f7-5a87c188335b
description: L’élément Error contient une réponse d’erreur de découverte automatique.
ms.openlocfilehash: 2f96f8b9d6d154aac6f10924095b5a5864e76750
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59530888"
---
# <a name="error-pox"></a>Erreur (POX)

**L’élément Error** contient une réponse d’erreur de découverte automatique. 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
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
|Temps  <br/> |Représente l’heure à quel moment la réponse d’erreur a été renvoyée.  <br/> |
|ID  <br/> |Représente un hachage du nom de l’ordinateur qui exécute Microsoft Exchange Server 2007 sur qui le rôle serveur d’accès au client est installé.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[ErrorCode (POX)](errorcode-pox.md) <br/> |Contient le code d’erreur d’une réponse de découverte automatique d’erreur.  <br/> |
|[Message (POX)](message-pox.md) <br/> |Contient le message d’erreur d’une réponse de découverte automatique d’erreur.  <br/> |
|[DebugData (POX)](debugdata-pox.md) <br/> |Contient les données de débogage d’une réponse de découverte automatique d’erreur.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Account (POX)](account-pox.md) <br/> |Contient une réponse d’erreur de découverte automatique.  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Éléments XML de découverte automatique POX pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

