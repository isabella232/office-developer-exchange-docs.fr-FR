---
title: CalendarView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CalendarView
api_type:
- schema
ms.assetid: a4a953b8-0710-416c-95ef-59e51eba9982
description: L’élément CalendarView définit une opération FindItem renvoi d’éléments de calendrier dans un ensemble lorsqu’ils s’affichent dans un calendrier.
ms.openlocfilehash: 79b5ad268a8013092c1122c99bdcd10d876abf2c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755485"
---
# <a name="calendarview"></a>CalendarView

L’élément **CalendarView** définit une [opération FindItem](finditem-operation.md) renvoi d’éléments de calendrier dans un ensemble lorsqu’ils s’affichent dans un calendrier. 
  
[FindItem](finditem.md)
  
[CalendarView](calendarview.md)
  
```XML
<CalendarView MaxEntriesReturned="" StartDate="" EndDate="" />
```

**CalendarView**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**MaxEntriesReturned** <br/> |Indique le nombre maximal de résultats à retourner dans la réponse FindItem.  <br/> |
|**Date de début** <br/> |Identifie le début d’une période interrogé des éléments de calendrier. Tous les éléments de calendrier dont l’heure de fin avant la **date de début** ne sont pas renvoyés. La valeur de **date de début** peut être spécifiée au format de temps universel coordonné (UTC), comme dans 2006-01-02T12:00:00Z, ou dans un format où décalage de l’heure locale et le fuseau horaire est spécifié, comme dans 2006-01-02T04:00:00-08:00.  <br/><br/>Cet attribut est requis.  <br/> |
|**Date de fin** <br/> |Identifie la fin d’une période interrogée des éléments de calendrier. Tous les éléments de calendrier dont l’heure de début ou après la **date de fin** ne sont pas renvoyés. La valeur de **date de fin** peut être spécifiée au format UTC, comme dans 2006-02-02T12:00:00Z, ou dans un format où décalage de l’heure locale et le fuseau horaire est spécifié, comme dans 2006-02-02T04:00:00-08:00.  <br/><br/>**Date de fin** doit être supérieure ou égale à la **date de début**; dans le cas contraire, une erreur est renvoyée. Cet attribut est requis.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[FindItem](finditem.md) <br/> |Définit une requête pour rechercher des éléments dans une boîte aux lettres.<br/><br/> Vous trouverez ci-dessous l’expression XPath pour cet élément :  <br/>  `/FindItem` <br/> |
   
## <a name="remarks"></a>Remarques

Si l’élément **CalendarView** est spécifié dans une requête FindItem, le service Web retourne une liste d’éléments de calendrier et les occurrences du rendez-vous périodiques dans la plage spécifiée par les **arguments StartDate** et **EndDate**.
  
Si l’élément **CalendarView** n’est pas spécifié dans une requête FindItem, le service Web retourne une liste des éléments de calendrier unique et des éléments de calendrier principal périodique. Occurrences de calendrier d’un élément de calendrier périodique ne sont pas développés. 
  
Requêtes CalendarView doivent effectuer uniquement utiliser les propriétés suivantes dans la mesure où elles prennent en charge les requêtes de calendrier plus rapides.
  
### <a name="recurrence-blob-properties"></a>Propriétés des objets blob de périodicité
  
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
    
### <a name="calculated-from-the-primary-recurrence-blob-or-master"></a>Calculé à partir de l’objet blob de périodicité principal ou master
  
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
    
### <a name="master-calendar-item-properties"></a>Propriétés de l’élément calendrier principal
  
- Propriété EntryId
    
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
    
- Catégories
    
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="example"></a>Exemple

L’exemple suivant montre une demande FindItem. Une demande réussie retourne une réponse qui inclut les éléments de calendrier qui ont démarré à 2006-05-18T00:00:00-08:00 ou une fois et terminé avant 2006-05-19T00:00:00-08:00.
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindItem Traversal="Shallow" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération FindItem](finditem-operation.md)
- [Recherche d’éléments](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

