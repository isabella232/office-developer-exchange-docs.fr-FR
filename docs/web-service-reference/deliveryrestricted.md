---
title: DeliveryRestricted
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeliveryRestricted
api_type:
- schema
ms.assetid: 05989915-121c-4f26-93cc-af8d454ab442
description: L’élément DeliveryRestricted indique si les restrictions de remise empêche le message de l’expéditeur d’atteindre le destinataire.
ms.openlocfilehash: ba1c6e00b93c9e442a427fe98a5e15bf5fe1effd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755892"
---
# <a name="deliveryrestricted"></a>DeliveryRestricted

L’élément **DeliveryRestricted** indique si les restrictions de remise empêche le message de l’expéditeur d’atteindre le destinataire. 
  
```XML
<DeliveryRestricted>true | false</DeliveryRestricted>
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
|[Les infos-courrier](mailtips.md) <br/> |Représente les valeurs pour les différents types d’astuces de la messagerie.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

La valeur de texte de cet élément est **la valeur true** si les restrictions de remise empêchera le message de l’expéditeur d’atteindre le destinataire. La valeur est **false** si les restrictions de remise n’empêcheront pas de message de l’expéditeur d’atteindre le destinataire. 
  
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

