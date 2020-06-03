---
title: Propriétés (ArrayOfTrackingPropertiesType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Properties
api_type:
- schema
ms.assetid: 175566d2-fd62-45a2-8518-2827912cec88
description: L’élément properties contient une liste d’une ou plusieurs propriétés de suivi.
ms.openlocfilehash: 007a4dc14c84c47ea7af8ccacc554c134d563e44
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465631"
---
# <a name="properties-arrayoftrackingpropertiestype"></a>Propriétés (ArrayOfTrackingPropertiesType)

L’élément **Properties** contient une liste d’une ou plusieurs propriétés de suivi. 
  
- [FindMessageTrackingReport](findmessagetrackingreport.md)
  
- [Propriétés (ArrayOfTrackingPropertiesType)](properties-arrayoftrackingpropertiestype.md)
  
```xml
<Properties>
   <TrackingPropertyType/>
</Properties>
```

**ArrayOfTrackingPropertiesType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[TrackingPropertyType](trackingpropertytype.md) <br/> |Représente une paire nom/valeur de chaînes qui est utilisée pour créer des propriétés pour les rapports de suivi des messages.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[FindMessageTrackingReport](findmessagetrackingreport.md) <br/> |Spécifie les critères pour les types de messages à rechercher.  <br/> |
|[FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) <br/> |Contient l’État et le résultat d’une seule demande d' [opération FindMessageTrackingReport](findmessagetrackingreport-operation.md) .  <br/> |
|[GetMessageTrackingReport](getmessagetrackingreport.md) <br/> |Contient la demande pour l' [opération GetMessageTrackingReport](getmessagetrackingreport-operation.md) afin de récupérer le rapport de suivi complet des messages pour l’ID spécifié.  <br/> |
|[GetMessageTrackingReportResponse](getmessagetrackingreportresponse.md) <br/> |Contient le résultat d’une demande d' [opération GetMessageTrackingReport](getmessagetrackingreport-operation.md) unique.  <br/> |
|[RecipientTrackingEvent](recipienttrackingevent.md) <br/> |Contient des informations pour un seul événement pour un destinataire.  <br/> |
|[MessageTrackingReport](messagetrackingreport.md) <br/> |Contient un seul message renvoyé dans un [Opération de GetMessageTrackingReport](getmessagetrackingreport-operation.md).  <br/> |
|[MessageTrackingSearchResult](messagetrackingsearchresult.md) <br/> |Contient un seul résultat de message pour un élément [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) .  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération FindMessageTrackingReport](findmessagetrackingreport-operation.md)
- [Opération de GetMessageTrackingReport](getmessagetrackingreport-operation.md)
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

