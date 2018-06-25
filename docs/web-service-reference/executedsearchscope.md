---
title: ExecutedSearchScope
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExecutedSearchScope
api_type:
- schema
ms.assetid: 2de5f0ad-43f2-4d38-b520-06540066564e
description: L’élément ExecutedSearchScope contient l’étendue de la recherche a été effectuée pour obtenir les résultats de recherche.
ms.openlocfilehash: ece9fdfc156cedad2a9fa181897145ae4eea20a0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756251"
---
# <a name="executedsearchscope"></a>ExecutedSearchScope

L’élément **ExecutedSearchScope** contient l’étendue de la recherche a été effectuée pour obtenir les résultats de recherche. 
  
```xml
<ExecutedSearchScope/>
```

 **Chaîne**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) <br/> |Contient l’état et les résultats d’une seule demande [d’opération FindMessageTrackingReport](findmessagetrackingreport-operation.md) .  <br/> |
   
## <a name="text-value"></a>Valeur de texte

La valeur de texte est facultative. Cette information est utilisée par l’application cliente à mettre en cache les résultats de manière plus efficace.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération FindMessageTrackingReport](findmessagetrackingreport-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

