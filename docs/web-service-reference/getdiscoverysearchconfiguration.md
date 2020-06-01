---
title: GetDiscoverySearchConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e15dbfca-3b9d-463e-94ec-4f1b6115bee3
description: L’élément GetDiscoverySearchConfiguration spécifie une demande de récupération de la configuration de recherche de découverte électronique.
ms.openlocfilehash: 821c5e1429c160e326f6d99df3ff4fcc831b83d1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461001"
---
# <a name="getdiscoverysearchconfiguration"></a>GetDiscoverySearchConfiguration

L’élément **GetDiscoverySearchConfiguration** spécifie une demande de récupération de la configuration de recherche de découverte électronique. 
  
```XML
<GetDiscoverySearchConfiguration>
    <SearchId/>
    <ExpandGroupMembership/>
</GetDiscoverySearchConfiguration>
```

 **GetDiscoverySearchConfigurationType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[SearchId](searchid.md) <br/> |Spécifie l’identificateur de la recherche.  <br/> |
|[ExpandGroupMembership](expandgroupmembership.md) <br/> |Contient une valeur de type Boolean qui indique s’il faut développer l’appartenance au groupe renvoyé à partir d’une demande **GetSearchableMailboxes** .  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma de message  <br/> |
|Fichier de validation  <br/> |messages. xsd  <br/> |
|Peut être vide  <br/> ||
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

