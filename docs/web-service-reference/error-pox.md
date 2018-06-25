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
description: L’élément Error contient une réponse d’erreur de découverte automatique.
ms.openlocfilehash: 3135a352365fe3000ce2d202ad78452d5c8ccc7f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756202"
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

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|Heure  <br/> |Représente le temps lorsque la réponse d’erreur a été renvoyée.  <br/> |
|ID  <br/> |Représente un hachage du nom de l’ordinateur qui exécute Microsoft Exchange Server 2007 ayant le rôle de serveur d’accès au Client est installé.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[ErrorCode (POX)](errorcode-pox.md) <br/> |Contient le code d’erreur pour une erreur de réponse de découverte automatique.  <br/> |
|[Message (POX)](message-pox.md) <br/> |Contient le message d’erreur pour une erreur de réponse de découverte automatique.  <br/> |
|[DebugData (POX)](debugdata-pox.md) <br/> |Contient les données de débogage pour une erreur de réponse de découverte automatique.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Compte (POX)](account-pox.md) <br/> |Contient une réponse d’erreur de découverte automatique.  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Éléments du fichier XML Autodiscover variole pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

