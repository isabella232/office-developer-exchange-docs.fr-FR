---
title: Langue (DiscoverySearchConfigurationType)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 34eab81c-d832-4925-9f76-d69f24b36931
description: L’élément de langage (DiscoverySearchConfigurationType) identifie la culture à utiliser pour le format spécifiques à la culture des plages de dates. Il indique également la langue utilisée dans une requête de recherche.
ms.openlocfilehash: 1e904ac4d7f525b2d12cfe83f0da33b9ed474066
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828197"
---
# <a name="language-discoverysearchconfigurationtype"></a>Langue (DiscoverySearchConfigurationType)

L’élément de **langage (DiscoverySearchConfigurationType)** identifie la culture à utiliser pour le format spécifiques à la culture des plages de dates. Il indique également la langue utilisée dans une requête de recherche. 
  
```XML
<Language />
```

 **string**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[DiscoverySearchConfiguration](discoverysearchconfiguration.md)
  
## <a name="text-value"></a>Valeur de texte

La valeur de texte de l’élément de **langage (DiscoverySearchConfigurationType)** est une culture ou une langue. 
  
## <a name="remarks"></a>Remarques

Cet élément spécifie le format des plages de dates spécifiée dans l' [opération SearchMailboxes](searchmailboxes-operation.md) ou l' [opération SetHoldOnMailboxes](setholdonmailboxes-operation.md).
  
Cet élément est une nouveauté d'Exchange Server 2013 Service Pack 1 (SP1).
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi



[DiscoverySearchConfiguration](discoverysearchconfiguration.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

