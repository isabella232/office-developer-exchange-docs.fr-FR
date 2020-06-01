---
title: AccessLevel
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 09475586-00fa-4e82-a915-5ca263ab4d1c
description: L’élément AccessLevel spécifie le niveau d’accès d’une réunion en ligne.
ms.openlocfilehash: 3c1375ef37ea666c6c4fafce7daa46ae0d0a2696
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462338"
---
# <a name="accesslevel"></a>AccessLevel

L’élément **AccessLevel** spécifie le niveau d’accès d’une réunion en ligne. 
  
```XML
<AccessLevel/>
```

 **OnlineMeetingSettingsType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[OnlineMeetingSettings](onlinemeetingsettings.md) <br/> |Spécifie les paramètres pour les réunions en ligne.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Le tableau suivant répertorie les valeurs de texte de l’élément **AccessLevel** . 
  
**Valeurs de texte de l’élément AccessLevel**

|**Valeur**|**Description**|
|:-----|:-----|
|Tout le monde  <br/> |Le niveau d’accès est ouvert à tous.  <br/> |
|Interne  <br/> |Le niveau d’accès est uniquement interne.  <br/> |
|Vite  <br/> |Le niveau d’accès est invités uniquement.  <br/> |
|Verrouillé  <br/> |Le niveau d’accès est verrouillé.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
Cet élément est une nouveauté d’Exchange Server 2013.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma type  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> ||
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

