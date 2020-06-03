---
title: DisableReason
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f41b5be6-9b79-4e83-8cdb-aa779e13cb3f
description: L’élément DisableReason spécifie la raison pour laquelle vous désactivez une application.
ms.openlocfilehash: 1406d69647bde5389dc9bb61adf7537a57d5adfc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463670"
---
# <a name="disablereason"></a>DisableReason

L’élément **DisableReason** spécifie la raison pour laquelle vous désactivez une application. 
  
```XML
<DisableReason> NoReason | OutlookClientPerformance | OWAClientPerformance | MobileClientPerformance </DisableReason>
```

 **DisableReasonType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[DisableApp](disableapp.md) <br/> |Spécifie une demande de désactivation d’une application.  <br/> |
   
## <a name="text-value"></a>Valeur texte

**Valeur de texte de l’élément DisableReason**

|**Valeur**|**Description**|
|:-----|:-----|
|Noreason  <br/> |Aucune raison donnée  <br/> |
|OutlookClientPerformance  <br/> |Pour améliorer les performances des clients de messagerie.  <br/> |
|OWAClientPerformance  <br/> |Pour améliorer les performances du client Web App.  <br/> |
|MobileClientPerformance  <br/> |Pour améliorer les performances des clients mobiles.  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma type  <br/> |
|Validation File  <br/> |types. xsd  <br/> |
|Peut être vide  <br/> ||
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

