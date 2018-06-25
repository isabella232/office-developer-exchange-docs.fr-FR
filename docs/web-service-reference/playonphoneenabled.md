---
title: PlayOnPhoneEnabled
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PlayOnPhoneEnabled
api_type:
- schema
ms.assetid: 6f800912-be4c-46f9-aa1e-dff0bbf877c5
description: L’élément PlayOnPhoneEnabled indique si la fonctionnalité de lecture sur le téléphone est activée.
ms.openlocfilehash: 1a6c5c41a4fe723f37d07ad0151dfbd6512cf4f7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828829"
---
# <a name="playonphoneenabled"></a>PlayOnPhoneEnabled

L’élément **PlayOnPhoneEnabled** indique si la fonctionnalité de lecture sur le téléphone est activée. 
  
```XML
<PlayOnPhoneEnabled>true | false</PlayOnPhoneEnabled>
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
|[UnifiedMessagingConfiguration](unifiedmessagingconfiguration.md) <br/> |Contient des informations de configuration pour le service de messagerie unifiée.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

L’élément **PlayOnPhoneEnabled** a la valeur **true** si les lire sur le téléphone est activé pour le compte. dans le cas contraire, la valeur est **false**.
  
## <a name="remarks"></a>Remarques

Cet élément est obligatoire.
  
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

