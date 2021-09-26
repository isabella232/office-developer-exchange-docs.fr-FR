---
title: DeliveryRestricted
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DeliveryRestricted
api_type:
- schema
ms.assetid: 05989915-121c-4f26-93cc-af8d454ab442
description: L’élément DeliveryRestricted indique si les restrictions de remise empêcheront le message de l’expéditeur d’atteindre le destinataire.
ms.openlocfilehash: 1df5254a284989a8ffc02a8c650eaf69b2214583
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59545362"
---
# <a name="deliveryrestricted"></a>DeliveryRestricted

**L’élément DeliveryRestricted** indique si les restrictions de remise empêcheront le message de l’expéditeur d’atteindre le destinataire. 
  
```XML
<DeliveryRestricted>true | false</DeliveryRestricted>
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
|[Infos-courrier](mailtips.md) <br/> |Représente les valeurs de différents types de conseils de messagerie.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur de texte de cet élément est **true** si les restrictions de remise empêchent le message de l’expéditeur d’atteindre le destinataire. La valeur est **false si** les restrictions de remise n’empêchent pas le message de l’expéditeur d’atteindre le destinataire. 
  
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

