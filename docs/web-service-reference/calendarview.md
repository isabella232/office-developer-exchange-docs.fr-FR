---
title: CalendarView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CalendarView
api_type:
- schema
ms.assetid: a4a953b8-0710-416c-95ef-59e51eba9982
description: L’élément CalendarView définit une opération FindItem comme renvoyant des éléments de calendrier dans un ensemble tel qu’ils apparaissent dans un calendrier.
ms.openlocfilehash: 5e0180bb5e8a6d9fcbe42380abbe32820117ae29
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518826"
---
# <a name="calendarview"></a>CalendarView

**L’élément CalendarView** définit une [opération FindItem](finditem-operation.md) comme renvoyant des éléments de calendrier dans un ensemble tel qu’ils apparaissent dans un calendrier. 
  
[FindItem](finditem.md)
  
[CalendarView](calendarview.md)
  
```XML
<CalendarView MaxEntriesReturned="" StartDate="" EndDate="" />
```

**CalendarView**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**MaxEntriesReturned** <br/> |Décrit le nombre maximal de résultats à renvoyer dans la réponse FindItem.  <br/> |
|**StartDate** <br/> |Identifie le début d’une période de temps pour les éléments de calendrier. Tous les éléments de calendrier dont l’heure de fin est avant **StartDate** ne sont pas renvoyés. La valeur de **StartDate** peut être spécifiée au format UTC (temps universel coordonné), comme dans 2006-01-02T12:00:00Z, ou dans un format où le décalage de l’heure locale et du fuseau horaire est spécifié, comme dans 2006-01-02T04:00:00-08:00.  <br/><br/>Cet attribut est obligatoire.  <br/> |
|**EndDate** <br/> |Identifie la fin d’une période de temps pour les éléments de calendrier. Tous les éléments de calendrier dont l’heure de début est sur ou après **EndDate** ne sont pas renvoyés. La valeur de **EndDate** peut être spécifiée au format UTC, comme dans 2006-02-02T12:00:00Z, ou dans un format où l’heure locale et le décalage de fuseau horaire sont spécifiés, comme dans 2006-02-02T04:00:00-08:00.  <br/><br/>**EndDate doit** être supérieur ou égal à **StartDate**; Sinon, une erreur est renvoyée. Cet attribut est obligatoire.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[FindItem](finditem.md) <br/> |Définit une demande de recherche d’éléments dans une boîte aux lettres.<br/><br/> Voici l’expression XPath de cet élément :  <br/>  `/FindItem` <br/> |
   
## <a name="remarks"></a>Remarques

Si **l’élément CalendarView** est spécifié dans une demande FindItem, le service Web renvoie une liste d’éléments de calendrier et d’occurrences d’éléments de calendrier périodiques dans la plage spécifiée par **StartDate** et **EndDate**.
  
Si **l’élément CalendarView** n’est pas spécifié dans une demande FindItem, le service Web renvoie une liste d’éléments de calendrier unique et d’éléments de calendrier principal périodiques. Les occurrences de calendrier d’un élément de calendrier périodique ne sont pas étendues. 
  
Les requêtes CalendarView doivent uniquement utiliser les propriétés suivantes, car elles peuvent prendre en charge des requêtes de calendrier plus rapides.
  
### <a name="recurrence-blob-properties"></a>Propriétés blob de récurrence
  
- MapiStartTime
    
- MapiEndTime
    
- SubjectPrefixInternal
    
- NormalizedSubjectInternal
    
- MapiSubject
    
- Emplacement
    
- AppointmentColor
    
- MapiIsAllDayEvent
    
- MapiHasAttachment
    
- FreeBusyStatus
    
- ReminderIsSetInternal
    
- ReminderMinutesBeforeStartInternal
    
- AppointmentState
    
- AllAttachmentsHidden
    
- ChangeHighlight
    
### <a name="calculated-from-the-primary-recurrence-blob-or-master"></a>Calculé à partir du blob ou de la récurrence principale
  
- ItemId
    
- IsRecurring
    
- IsException
    
- AppointmentRecurring
    
- MapiStartTime
    
- MapiPRStartDate
    
- MapiEndTime
    
- MapiPREndDate
    
- CalendarItemType
    
- GlobalObjectId
    
- TimeZoneDefinitionStart
    
- TimeZoneDefinitionEnd
    
### <a name="master-calendar-item-properties"></a>Propriétés d’élément de calendrier master
  
- EntryId
    
- ChangeKey
    
- ItemClass
    
- SentRepresentingEmailAddress
    
- SentRepresentingDisplayName
    
- SentRepresentingEntryId
    
- AppointmentRecurrenceBlob
    
- TimeZone
    
- TimeZoneBlob
    
- TimeZoneDefinitionRecurring
    
- CleanGlobalObjectId
    
- AppointmentRecurring
    
- IsException
    
- IsRecurring
    
- MapiSensitivity
    
- ContainerClass
    
- MapiPRStartDate
    
- MapiPREndDate
    
- Categories
    
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="example"></a>Exemple

L’exemple suivant illustre une demande FindItem. Une requête réussie renvoie une réponse qui inclut les éléments de calendrier qui ont commencé à 2006-05-18T00:00:00-08:00 ou après et se sont terminés avant 2006-05-19T00:00:00-08:00.
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindItem Traversal="Shallow" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="calendar:Start"/>
          <t:FieldURI FieldURI="calendar:End"/>
          <t:FieldURI FieldURI="item:Subject"/>
        </t:AdditionalProperties>
      </ItemShape>
      <CalendarView MaxEntriesReturned="2" StartDate="2006-05-18T00:00:00-08:00" EndDate="2006-05-19T00:00:00-08:00"/>
      <ParentFolderIds>
        <t:DistinguishedFolderId Id="calendar"/>
      </ParentFolderIds>
    </FindItem>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération FindItem](finditem-operation.md)
- [Recherche d’éléments](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

