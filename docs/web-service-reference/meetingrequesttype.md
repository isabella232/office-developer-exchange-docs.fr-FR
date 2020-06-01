---
title: MeetingRequestType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MeetingRequestType
api_type:
- schema
ms.assetid: bcd5c97c-19aa-4b1d-a8e8-e8c4bd473dd9
description: L’élément MeetingRequestType décrit le type de la demande de réunion.
ms.openlocfilehash: e90c44dd4124d698ca5ef7655f6429a7167673e6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/01/2020
ms.locfileid: "44465785"
---
# <a name="meetingrequesttype"></a>MeetingRequestType

L’élément **MeetingRequestType** décrit le type de la demande de réunion. 
  
```xml
<MeetingRequestType/>
```

 **MeetingRequestTypeType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Propriété meetingrequest](meetingrequest.md) <br/> |Représente une demande de réunion dans la banque d'informations Exchange.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte est requise. Le tableau suivant répertorie les valeurs de texte possibles pour cet élément.
  
|**Valeur**|**Description**|
|:-----|:-----|
|FullUpdate  <br/> |Identifie la demande de réunion en tant que mise à jour complète d’une demande existante. Une mise à jour complète a mis à jour le contenu horaire et informatif.  <br/> |
|InformationalUpdate  <br/> |Identifie la demande de réunion uniquement avec le contenu informatif mis à jour.  <br/> |
|NewMeetingRequest  <br/> |Identifie la demande de réunion en tant que nouvelle demande de réunion.  <br/> |
|Aucun  <br/> |Indique que le type de demande de réunion n’est pas défini.  <br/> |
|Obsolètes  <br/> |Identifie la demande de réunion comme étant obsolète.  <br/> |
|PrincipalWantsCopy  <br/> |Indique que la demande de réunion appartient à un principal qui a transféré des messages de réunion à un délégué et que ses copies sont marquées comme informations.  <br/> |
|SilentUpdate  <br/> |Identifie la demande de réunion en tant que mise à jour silencieuse d’une réunion existante.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 sur lequel le rôle de serveur d’accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

