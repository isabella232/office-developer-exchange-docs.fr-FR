---
title: HiddenRecipient
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- HiddenRecipient
api_type:
- schema
ms.assetid: a8209f75-0070-4424-8dcd-273cfd192728
description: L’élément HiddenRecipient indique que le destinataire a été ajouté à une stratégie d’entreprise qui doit être masquée auprès des utilisateurs sans privilèges.
ms.openlocfilehash: 73b2e3e39c675cf3e2bc56105b1e76009d4a2451
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827810"
---
# <a name="hiddenrecipient"></a>HiddenRecipient

L’élément **HiddenRecipient** indique que le destinataire a été ajouté à une stratégie d’entreprise qui doit être masquée auprès des utilisateurs sans privilèges. 
  
```XML
<HiddenRecipient>true | false</HiddenRecipient>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[RecipientTrackingEvent](recipienttrackingevent.md) <br/> |Contient des informations pour un seul événement pour un destinataire.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Cet élément peut être **true** ou **false**. La valeur **true** indique que l’utilisateur a été ajouté à une stratégie d’entreprise ; la valeur **false** indique que l’utilisateur n’a pas été ajouté à une stratégie d’entreprise. 
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

