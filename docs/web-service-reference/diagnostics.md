---
title: Diagnostics
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Diagnostics
api_type:
- schema
ms.assetid: fecea440-970a-49da-9796-534ca470cbd6
description: L’élément de diagnostic fournit des informations de synchronisation et les performances qui sont utilisées pour la création de rapports dans un centre de données.
ms.openlocfilehash: 2b9cac54a683967ec274b8681fb9a0c8a844205e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755912"
---
# <a name="diagnostics"></a>Diagnostics

L’élément de **diagnostic** fournit des informations de synchronisation et les performances qui sont utilisées pour la création de rapports dans un centre de données. 
  
```XML
<Diagnostics>
   <String/>
</Diagnostics>

```

 **ArrayOfStringsType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[String](string.md) <br/> |Contient une chaîne qui est utilisée par les éléments, des contacts, des tâches et des conversations.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) <br/> |Contient l’état et les résultats d’une seule demande [d’opération FindMessageTrackingReport](findmessagetrackingreport-operation.md) .  <br/> |
|[GetMessageTrackingReportResponse](getmessagetrackingreportresponse.md) <br/> |Contient la réponse de l' [opération GetMessageTrackingReport](getmessagetrackingreport-operation.md).  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération FindMessageTrackingReport](findmessagetrackingreport-operation.md)
- [Opération de GetMessageTrackingReport](getmessagetrackingreport-operation.md)
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

