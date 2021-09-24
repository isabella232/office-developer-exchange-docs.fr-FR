---
title: Internal (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 69c22546-ebd6-4a03-b0b4-bbac72ec5551
description: L’élément Internal contient la collection d’URL qu’un client peut utiliser pour se connecter à Exchange à partir de l’intérieur du réseau de l’organisation.
ms.openlocfilehash: f87c5e21eff87965c9b6ff6f3d59e2b3a37b87f1
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541118"
---
# <a name="internal-pox"></a>Internal (POX)

**L’élément Internal** contient la collection d’URL qu’un client peut utiliser pour se connecter à Exchange à partir de l’intérieur du réseau de l’organisation. 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[Internal (POX)](internal-pox.md)
  
```xml
<Internal>
   <OWAUrl/>
   <Protocol>
      <Type/>
      <ASUrl/>
   </Protocol>
</Internal>
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

**L’élément Internal** est un élément enfant facultatif de **l’élément Protocol.** 
  
## <a name="see-also"></a>Voir aussi



[Éléments XML de découverte automatique POX pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

