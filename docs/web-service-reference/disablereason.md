---
title: DisableReason
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: f41b5be6-9b79-4e83-8cdb-aa779e13cb3f
description: L’élément DisableReason spécifie la raison de la désactivation d’une application.
ms.openlocfilehash: 8156dac17e81dd1c3f49575491924185b04d53e9
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59528835"
---
# <a name="disablereason"></a>DisableReason

**L’élément DisableReason** spécifie la raison de la désactivation d’une application. 
  
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
|NoReason  <br/> |Aucune raison n’est donnée  <br/> |
|OutlookClientPerformance  <br/> |Pour améliorer les performances du client de messagerie.  <br/> |
|OWAClientPerformance  <br/> |Pour améliorer les performances du client d’application Web.  <br/> |
|MobileClientPerformance  <br/> |Pour améliorer les performances du client mobile.  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma type  <br/> |
|Validation File  <br/> |types.xsd  <br/> |
|Peut être vide  <br/> ||
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

