---
title: GetMessageTrackingReport
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetMessageTrackingReport
api_type:
- schema
ms.assetid: b6ffa8ef-90f6-402d-afac-c3f5ee55cf49
description: L’élément GetMessageTrackingReport contient la demande pour l’opération GetMessageTrackingReport afin de récupérer le rapport de suivi complet des messages pour l’ID spécifié.
ms.openlocfilehash: 30596acd209580147e0f03e12a7868502159b29c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466576"
---
# <a name="getmessagetrackingreport"></a>GetMessageTrackingReport

L’élément **GetMessageTrackingReport** contient la demande pour l' [opération GetMessageTrackingReport](getmessagetrackingreport-operation.md) afin de récupérer le rapport de suivi complet des messages pour l’ID spécifié. 
  
```XML
<GetMessageTrackingReport>
   <Scope/>
   <ReportTemplate/>
   <RecipientFilter/>
   <MessageTrackingReportId/>
   <ReturnQueueEvents/>
   <DiagnosticsLevel/>
   <Properties/>
</GetMessageTrackingReport>
```

 **GetMessageTrackingReportRequestType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Étendue (NonEmptyStringType)](scope-nonemptystringtype.md) <br/> |Indique où effectuer la recherche. Cet élément est obligatoire.  <br/> |
|[ReportTemplate](reporttemplate.md) <br/> |Spécifie le type de rapport de suivi à récupérer. Cet élément est obligatoire.  <br/> |
|[RecipientFilter](recipientfilter.md) <br/> |Spécifie l’adresse d’un destinataire à utiliser avec le rapport de suivi spécifié. Cet élément est facultatif.  <br/> |
|[MessageTrackingReportId](messagetrackingreportid.md) <br/> |Spécifie une chaîne d’identité obtenue à partir de l’opération **FindMessageTrackingReport** . Cet élément est obligatoire.  <br/> |
|[ReturnQueueEvents](returnqueueevents.md) <br/> |Spécifie que la personne qui exécute la tâche dispose d’un rôle privilégié. Cet élément est facultatif.  <br/> |
|[DiagnosticsLevel](diagnosticslevel.md) <br/> |Spécifie les informations de temps et de performances qui seront utilisées pour dériver le rapport de suivi. Cet élément est facultatif.  <br/> |
|[Propriétés (ArrayOfTrackingPropertiesType)](properties-arrayoftrackingpropertiestype.md) <br/> |Spécifie une liste d’une ou plusieurs propriétés de suivi. Cet élément est facultatif.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération de GetMessageTrackingReport](getmessagetrackingreport-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

