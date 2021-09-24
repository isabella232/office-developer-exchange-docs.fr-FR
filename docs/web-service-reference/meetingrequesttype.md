---
title: MeetingRequestType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- MeetingRequestType
api_type:
- schema
ms.assetid: bcd5c97c-19aa-4b1d-a8e8-e8c4bd473dd9
description: L’élément MeetingRequestType décrit le type de la demande de réunion.
ms.openlocfilehash: 1a8371331691bb9dee5595b0130ec0c3c75c47c5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539373"
---
# <a name="meetingrequesttype"></a>MeetingRequestType

**L’élément MeetingRequestType** décrit le type de la demande de réunion. 
  
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
|[MeetingRequest](meetingrequest.md) <br/> |Représente une demande de réunion dans la banque d'informations Exchange.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte est requise. Le tableau suivant répertorie les valeurs de texte possibles pour cet élément.
  
|**Valeur**|**Description**|
|:-----|:-----|
|FullUpdate  <br/> |Identifie la demande de réunion comme une mise à jour complète d’une demande existante. Une mise à jour complète a mis à jour le temps et le contenu d’information.  <br/> |
|InformationalUpdate  <br/> |Identifie la demande de réunion comme contenant uniquement du contenu d’information mis à jour.  <br/> |
|NewMeetingRequest  <br/> |Identifie la demande de réunion en tant que nouvelle demande de réunion.  <br/> |
|Aucun  <br/> |Indique que le type de demande de réunion n’est pas défini.  <br/> |
|Obsolète  <br/> |Identifie la demande de réunion comme obsolète.  <br/> |
|PrincipalWantsCopy  <br/> |Indique que la demande de réunion appartient à un principal qui a transmis des messages de réunion à un délégué et dont les copies sont marquées comme étant des informations.  <br/> |
|SilentUpdate  <br/> |Identifie la demande de réunion comme une mise à jour silencieuse d’une réunion existante.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur exécutant Microsoft Exchange Server 2010 sur qui le rôle serveur d’accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

