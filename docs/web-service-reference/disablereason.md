---
title: DisableReason
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f41b5be6-9b79-4e83-8cdb-aa779e13cb3f
description: L’élément DisableReason spécifie la raison de la désactivation d’une application.
ms.openlocfilehash: f900bd1b98b294900f767c778b9c5f87f74042ca
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755953"
---
# <a name="disablereason"></a>DisableReason

L’élément **DisableReason** spécifie la raison de la désactivation d’une application. 
  
```XML
<DisableReason> NoReason | OutlookClientPerformance | OWAClientPerformance | MobileClientPerformance </DisableReason>
```

 **DisableReasonType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[DisableApp](disableapp.md) <br/> |Spécifie une demande pour désactiver une application.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

**Valeur texte de l’élément DisableReason**

|**Valeur**|**Description**|
|:-----|:-----|
|NoReason  <br/> |Aucune raison donnée  <br/> |
|OutlookClientPerformance  <br/> |Pour améliorer les performances de client de messagerie.  <br/> |
|OWAClientPerformance  <br/> |Pour améliorer les performances du client Web app.  <br/> |
|MobileClientPerformance  <br/> |Pour améliorer les performances de client mobile.  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma type  <br/> |
|Validation File  <br/> |types.xsd  <br/> |
|Peut être vide  <br/> ||
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

