---
title: External (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: 8eed1f79-6eb3-4a88-80fb-d4edf9f34fda
description: L’élément External contient une collection d’URL qu’un client peut utiliser pour se connecter à Exchange à partir de l’extérieur du réseau de l’organisation.
ms.openlocfilehash: 0e7e92029a01a25d5017d3b5199a7899403c975f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510098"
---
# <a name="external-pox"></a>External (POX)

**L’élément External** contient une collection d’URL qu’un client peut utiliser pour se connecter à Exchange en dehors du réseau de l’organisation. 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[External (POX)](external-pox.md)
  
```XML
<External>
   <OWAUrl/>
   <Protocol>
      <Type/>
      <ASUrl/>
   </Protocol>
</External>

```

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[OWAUrl (POX)](owaurl-pox.md) <br/> |Décrit l’URL et le schéma d’authentification utilisés pour accéder à un ordinateur particulier qui exécute Microsoft Exchange Server sur qui le rôle serveur d’accès au client est installé et qui héberge Outlook Web Access.  <br/> |
|[Protocol (POX)](protocol-pox.md) <br/> |Contient les spécifications de connexion d’un client à l’ordinateur qui exécute Microsoft Exchange Server sur qui le rôle serveur d’accès au client est installé. Cet élément **Protocol** ne possède que deux éléments enfants : un élément [Type (POX)](type-pox.md) spécifiant le protocole de connexion et un élément [ASUrl (POX),](asurl-pox.md) spécifiant le point de terminaison EWS pour le service web de disponibilité.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Protocol (POX)](protocol-pox.md) <br/> |Contient les spécifications de connexion d’un client à l’ordinateur qui exécute Microsoft Exchange Server sur qui le rôle serveur d’accès au client est installé.  <br/> |
   
## <a name="remarks"></a>Remarques

**L’élément External** est un élément enfant facultatif de **l’élément Protocol.** 
  
## <a name="see-also"></a>Voir aussi



[Éléments XML de découverte automatique POX pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

