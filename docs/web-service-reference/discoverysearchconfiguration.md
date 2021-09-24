---
title: DiscoverySearchConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 085384f9-dca4-4534-82e2-dd782471d0da
description: L’élément DiscoverySearchConfiguration spécifie la configuration de la recherche eDiscovery.
ms.openlocfilehash: 4f5f0a5b8e78521302fd136f0a0280aa3ff4e4c3
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523096"
---
# <a name="discoverysearchconfiguration"></a>DiscoverySearchConfiguration

**L’élément DiscoverySearchConfiguration** spécifie la configuration de la recherche eDiscovery. 
  
```XML
<DiscoverySearchConfiguration>
    <SearchId></SearchId>
    <SearchQuery></SearchQuery>
    <SearchableMailboxes></SearchableMailboxes>
</DiscoverySearchConfiguration>
```

 **DiscoverySearchConfigurationType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[SearchId](searchid.md) <br/> |Spécifie l’identificateur de la recherche.  <br/> |
|[SearchQuery](searchquery.md) <br/> |Spécifie le nom d’une requête de recherche de découverte électronique.  <br/> |
|[SearchableMailboxes](searchablemailboxes.md) <br/> |Contient une liste des boîtes aux lettres renvoyées par une **demande GetSearchableMailboxes.**  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[DiscoverySearchConfigurations](discoverysearchconfigurations.md) <br/> |Spécifie un tableau **d’éléments DiscoverySearchConfiguration.**  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma des messages  <br/> |
|Fichier de validation  <br/> |messages.xsd  <br/> |
|Peut être vide  <br/> ||
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

