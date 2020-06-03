---
title: Externe (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 8eed1f79-6eb3-4a88-80fb-d4edf9f34fda
description: L’élément External contient une collection d’URL qu’un client peut utiliser pour se connecter à Exchange depuis l’extérieur du réseau de l’organisation.
ms.openlocfilehash: 45d7e72c5a43c5c468c1edd303a5e5ea8c2cb62e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457969"
---
# <a name="external-pox"></a>Externe (POX)

L’élément **External** contient une collection d’URL qu’un client peut utiliser pour se connecter à Exchange depuis l’extérieur du réseau de l’organisation. 
  
[Découverte automatique (POX)](autodiscover-pox.md)
  
[Réponse (POX)](response-pox.md)
  
[Compte (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[Externe (POX)](external-pox.md)
  
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
|[OWAUrl (POX)](owaurl-pox.md) <br/> |Décrit l’URL et le schéma d’authentification utilisés pour accéder à un ordinateur spécifique qui exécute Microsoft Exchange Server sur lequel le rôle serveur d’accès au client est installé et qui héberge Outlook Web Access.  <br/> |
|[Protocol (POX)](protocol-pox.md) <br/> |Contient les spécifications relatives à la connexion d’un client à l’ordinateur qui exécute Microsoft Exchange Server sur lequel le rôle de serveur d’accès au client est installé. Cet élément de **protocole** n’a que deux éléments enfants : un élément de [type (POX)](type-pox.md) spécifiant le protocole de connexion et un élément [ASUrl (POX)](asurl-pox.md) , spécifiant le point de terminaison EWS pour le service Web de disponibilité.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Protocol (POX)](protocol-pox.md) <br/> |Contient les spécifications relatives à la connexion d’un client à l’ordinateur qui exécute Microsoft Exchange Server sur lequel le rôle de serveur d’accès au client est installé.  <br/> |
   
## <a name="remarks"></a>Remarques

L’élément **External** est un élément enfant facultatif de l’élément **Protocol** . 
  
## <a name="see-also"></a>Voir aussi



[Éléments XML de découverte automatique de la VARIOle pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

