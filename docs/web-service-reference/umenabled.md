---
title: UMEnabled
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- UmEnabled
api_type:
- schema
ms.assetid: 87382d9b-0c02-49ec-85dc-3f5918df3195
description: L’élément UmEnabled indique si la messagerie unifiée est activée pour un compte.
ms.openlocfilehash: 9ff6432324e3a15b9ae805a7d6d836c9c895059c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59527152"
---
# <a name="umenabled"></a>UMEnabled

**L’élément UmEnabled** indique si la messagerie unifiée est activée pour un compte. 
  
```XML
<UmEnabled>true | false</UmEnabled>
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
|[UnifiedMessagingConfiguration](unifiedmessagingconfiguration.md) <br/> |Contient des informations de configuration de service pour le service de messagerie unifiée.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur texte de **l’élément UmEnabled** est **true** si la messagerie unifiée est activée pour le compte . Sinon, la valeur est **false**.
  
## <a name="remarks"></a>Remarques

Cet élément est obligatoire.
  
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

