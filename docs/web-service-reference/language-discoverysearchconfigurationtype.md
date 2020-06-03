---
title: Langue (DiscoverySearchConfigurationType)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 34eab81c-d832-4925-9f76-d69f24b36931
description: L’élément Language (DiscoverySearchConfigurationType) identifie la culture à utiliser pour le format spécifique à la culture des plages de dates. Il spécifie également la langue utilisée dans une requête de recherche.
ms.openlocfilehash: 3cf85525147bec5d6dfc6fe2b2af5916d42c44be
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463285"
---
# <a name="language-discoverysearchconfigurationtype"></a>Langue (DiscoverySearchConfigurationType)

L’élément **Language (DiscoverySearchConfigurationType)** identifie la culture à utiliser pour le format spécifique à la culture des plages de dates. Il spécifie également la langue utilisée dans une requête de recherche. 
  
```XML
<Language />
```

 **chaîne**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[DiscoverySearchConfiguration](discoverysearchconfiguration.md)
  
## <a name="text-value"></a>Valeur texte

La valeur de texte de l’élément **Language (DiscoverySearchConfigurationType)** est une culture ou une langue. 
  
## <a name="remarks"></a>Remarques

Cet élément spécifie le format des plages de dates spécifiées dans l' [opération SearchMailboxes](searchmailboxes-operation.md) ou l' [opération SetHoldOnMailboxes](setholdonmailboxes-operation.md).
  
Cet élément est une nouveauté d'Exchange Server 2013 Service Pack 1 (SP1).
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi



[DiscoverySearchConfiguration](discoverysearchconfiguration.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

