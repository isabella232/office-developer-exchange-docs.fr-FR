---
title: AccessLevel
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 09475586-00fa-4e82-a915-5ca263ab4d1c
description: L’élément AccessLevel Spécifie le niveau d’accès pour une réunion en ligne.
ms.openlocfilehash: 1bf0a191fad529b555117e4ff992c352615bc79b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756304"
---
# <a name="accesslevel"></a>AccessLevel

L’élément **AccessLevel** Spécifie le niveau d’accès pour une réunion en ligne. 
  
```XML
<AccessLevel/>
```

 **OnlineMeetingSettingsType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[OnlineMeetingSettings](onlinemeetingsettings.md) <br/> |Spécifie les paramètres pour les réunions en ligne.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Le tableau suivant répertorie les valeurs de texte de l’élément **AccessLevel** . 
  
**Valeurs de texte des éléments AccessLevel**

|**Valeur**|**Description**|
|:-----|:-----|
|Tout le monde  <br/> |Le niveau d’accès est ouvert à l’ensemble.  <br/> |
|Interne  <br/> |Le niveau d’accès est interne uniquement.  <br/> |
|Invités  <br/> |Le niveau d’accès est uniquement les participants invités.  <br/> |
|Verrouillé  <br/> |Le niveau d’accès est verrouillé.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
Cet élément est une nouveauté d'Exchange Server 2013.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma type  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> ||
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

