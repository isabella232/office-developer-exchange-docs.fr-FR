---
title: FirstHopServer
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FirstHopServer
api_type:
- schema
ms.assetid: 79c89d74-b0ad-4643-9177-b75d3baa3b67
description: L’élément FirstHopServer contient le nom du serveur dans la forêt qui a accepté tout d’abord le message.
ms.openlocfilehash: 1852b95f94b174b57c8175a45035a97686384c20
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756422"
---
# <a name="firsthopserver"></a>FirstHopServer

L’élément **FirstHopServer** contient le nom du serveur dans la forêt qui a accepté tout d’abord le message. 
  
```xml
<FirstHopServer/>
```

 **NonEmptyStringType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[MessageTrackingSearchResult](messagetrackingsearchresult.md) <br/> |Contient un résultat de message unique d’un élément [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) .  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
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

