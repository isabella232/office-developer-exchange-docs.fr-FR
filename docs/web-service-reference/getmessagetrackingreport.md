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
description: L’élément GetMessageTrackingReport contient la demande pour l’opération GetMessageTrackingReport récupérer le message complet suivi du rapport pour l’ID spécifié.
ms.openlocfilehash: cb16f6e9d322cefb0d59c962af8e2f60ebae0e90
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756680"
---
# <a name="getmessagetrackingreport"></a>GetMessageTrackingReport

L’élément **GetMessageTrackingReport** contient la demande pour l' [opération GetMessageTrackingReport](getmessagetrackingreport-operation.md) récupérer le message complet suivi du rapport pour l’ID spécifié. 
  
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

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Étendue (NonEmptyStringType)](scope-nonemptystringtype.md) <br/> |Spécifie l’emplacement où effectuer la recherche. Cet élément est obligatoire.  <br/> |
|[Modèle d’état](reporttemplate.md) <br/> |Spécifie le type de suivi du rapport à récupérer. Cet élément est obligatoire.  <br/> |
|[RecipientFilter](recipientfilter.md) <br/> |Spécifie une adresse de destinataire à utiliser avec le rapport de suivi spécifié. Cet élément est facultatif.  <br/> |
|[MessageTrackingReportId](messagetrackingreportid.md) <br/> |Spécifie une chaîne d’identité qui proviennent de l’opération **FindMessageTrackingReport** . Cet élément est obligatoire.  <br/> |
|[ReturnQueueEvents](returnqueueevents.md) <br/> |Spécifie que la personne qui exécute la tâche a un rôle de privilège. Cet élément est facultatif.  <br/> |
|[DiagnosticsLevel](diagnosticslevel.md) <br/> |Spécifie les informations de synchronisation et les performances qui seront utilisées pour déterminer le rapport de suivi. Cet élément est facultatif.  <br/> |
|[Propriétés (ArrayOfTrackingPropertiesType)](properties-arrayoftrackingpropertiestype.md) <br/> |Spécifie une liste d’un ou plusieurs des propriétés de suivi. Cet élément est facultatif.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

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



[Opération de GetMessageTrackingReport](getmessagetrackingreport-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

