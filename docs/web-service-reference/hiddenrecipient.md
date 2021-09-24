---
title: HiddenRecipient
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- HiddenRecipient
api_type:
- schema
ms.assetid: a8209f75-0070-4424-8dcd-273cfd192728
description: L’élément HiddenRecipient indique que le destinataire a été ajouté par une stratégie d’organisation qui doit être masquée pour les utilisateurs non privilégiés.
ms.openlocfilehash: 24d7dcad5b8b744351804160ef8d9988b9e393a3
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539688"
---
# <a name="hiddenrecipient"></a>HiddenRecipient

**L’élément HiddenRecipient** indique que le destinataire a été ajouté par une stratégie d’organisation qui doit être masquée pour les utilisateurs non privilégiés. 
  
```XML
<HiddenRecipient>true | false</HiddenRecipient>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[RecipientTrackingEvent](recipienttrackingevent.md) <br/> |Contient des informations pour un événement unique pour un destinataire.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Cet élément peut être **vrai** ou **faux**. La valeur **true indique** que l’utilisateur a été ajouté par une stratégie d’organisation ; Une valeur false **indique** que l’utilisateur n’a pas été ajouté par une stratégie d’organisation. 
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

