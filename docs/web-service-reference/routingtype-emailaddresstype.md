---
title: RoutingType (EmailAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RoutingType
api_type:
- schema
ms.assetid: 683216be-9972-4f48-a148-c34bfe7f53e5
description: L’élément RoutingType définit le type d’adresse pour la boîte aux lettres.
ms.openlocfilehash: d4229f2857a5c99cc9bb7ff9b9b103de099a0055
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465085"
---
# <a name="routingtype-emailaddresstype"></a>RoutingType (EmailAddressType)

L’élément **RoutingType** définit le type d’adresse pour la boîte aux lettres. 
  
```XML
<RoutingType/>
```

 **NonEmptyStringType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Actionas](actingas.md) <br/> |Identifie les personnes qui envoient l’appelant.  <br/> |
|[Boîte aux lettres](mailbox.md) <br/> |Identifie une adresse de messagerie entièrement résolue.  <br/> |
|[RoomList](roomlist.md) <br/> |Identifie une liste de salles de réunion.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur texte représente un type de routage. SMTP est la valeur de texte standard de cet élément.
  
## <a name="remarks"></a>Remarques

Cet élément est facultatif dans l’élément [Mailbox](mailbox.md) . Un autre élément [RoutingType (EmailAddress)](routingtype-emailaddress.md) est utilisé pour les opérations de disponibilité. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

