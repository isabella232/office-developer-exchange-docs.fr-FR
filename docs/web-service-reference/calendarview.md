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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755485"
---
# <a name="calendarview"></a><span data-ttu-id="d5431-103">CalendarView</span><span class="sxs-lookup"><span data-stu-id="d5431-103">CalendarView</span></span>

<span data-ttu-id="d5431-104">L’élément **CalendarView** définit une [opération FindItem](finditem-operation.md) renvoi d’éléments de calendrier dans un ensemble lorsqu’ils s’affichent dans un calendrier.</span><span class="sxs-lookup"><span data-stu-id="d5431-104">The **CalendarView** element defines a [FindItem operation](finditem-operation.md) as returning calendar items in a set as they appear in a calendar.</span></span> 
  
[<span data-ttu-id="d5431-105">FindItem</span><span class="sxs-lookup"><span data-stu-id="d5431-105">FindItem</span></span>](finditem.md)
  
[<span data-ttu-id="d5431-106">CalendarView</span><span class="sxs-lookup"><span data-stu-id="d5431-106">CalendarView</span></span>](calendarview.md)
  
```XML
<CalendarView MaxEntriesReturned="" StartDate="" EndDate="" />
```

<span data-ttu-id="d5431-107">**CalendarView**</span><span class="sxs-lookup"><span data-stu-id="d5431-107">**CalendarView**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="d5431-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d5431-108">Attributes and elements</span></span>

<span data-ttu-id="d5431-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d5431-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d5431-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="d5431-110">Attributes</span></span>

|<span data-ttu-id="d5431-111">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="d5431-111">**Attribute**</span></span>|<span data-ttu-id="d5431-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="d5431-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d5431-113">**MaxEntriesReturned**</span><span class="sxs-lookup"><span data-stu-id="d5431-113">**MaxEntriesReturned**</span></span> <br/> |<span data-ttu-id="d5431-114">Indique le nombre maximal de résultats à retourner dans la réponse FindItem.</span><span class="sxs-lookup"><span data-stu-id="d5431-114">Describes the maximum number of results to return in the FindItem response.</span></span>  <br/> |
|<span data-ttu-id="d5431-115">**Date de début**</span><span class="sxs-lookup"><span data-stu-id="d5431-115">**StartDate**</span></span> <br/> |<span data-ttu-id="d5431-116">Identifie le début d’une période interrogé des éléments de calendrier.</span><span class="sxs-lookup"><span data-stu-id="d5431-116">Identifies the start of a time span queried for calendar items.</span></span> <span data-ttu-id="d5431-117">Tous les éléments de calendrier dont l’heure de fin avant la **date de début** ne sont pas renvoyés.</span><span class="sxs-lookup"><span data-stu-id="d5431-117">All calendar items that have an end time that is before **StartDate** will not be returned.</span></span> <span data-ttu-id="d5431-118">La valeur de **date de début** peut être spécifiée au format de temps universel coordonné (UTC), comme dans 2006-01-02T12:00:00Z, ou dans un format où décalage de l’heure locale et le fuseau horaire est spécifié, comme dans 2006-01-02T04:00:00-08:00.</span><span class="sxs-lookup"><span data-stu-id="d5431-118">The value of **StartDate** can be specified in coordinated universal time (UTC) format, as in 2006-01-02T12:00:00Z, or in a format where local time and time zone offset is specified, as in 2006-01-02T04:00:00-08:00.</span></span>  <br/><br/><span data-ttu-id="d5431-119">Cet attribut est requis.</span><span class="sxs-lookup"><span data-stu-id="d5431-119">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="d5431-120">**Date de fin**</span><span class="sxs-lookup"><span data-stu-id="d5431-120">**EndDate**</span></span> <br/> |<span data-ttu-id="d5431-121">Identifie la fin d’une période interrogée des éléments de calendrier.</span><span class="sxs-lookup"><span data-stu-id="d5431-121">Identifies the end of a time span queried for calendar items.</span></span> <span data-ttu-id="d5431-122">Tous les éléments de calendrier dont l’heure de début ou après la **date de fin** ne sont pas renvoyés.</span><span class="sxs-lookup"><span data-stu-id="d5431-122">All calendar items that have a start time that is on or after **EndDate** will not be returned.</span></span> <span data-ttu-id="d5431-123">La valeur de **date de fin** peut être spécifiée au format UTC, comme dans 2006-02-02T12:00:00Z, ou dans un format où décalage de l’heure locale et le fuseau horaire est spécifié, comme dans 2006-02-02T04:00:00-08:00.</span><span class="sxs-lookup"><span data-stu-id="d5431-123">The value of **EndDate** can be specified in UTC format, as in 2006-02-02T12:00:00Z, or in a format where local time and time zone offset is specified, as in 2006-02-02T04:00:00-08:00.</span></span>  <br/><br/><span data-ttu-id="d5431-124">**Date de fin** doit être supérieure ou égale à la **date de début**; dans le cas contraire, une erreur est renvoyée.</span><span class="sxs-lookup"><span data-stu-id="d5431-124">**EndDate** must be greater than or equal to **StartDate**; otherwise an error is returned.</span></span> <span data-ttu-id="d5431-125">Cet attribut est requis.</span><span class="sxs-lookup"><span data-stu-id="d5431-125">This attribute is required.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="d5431-126">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d5431-126">Child elements</span></span>

<span data-ttu-id="d5431-127">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d5431-127">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d5431-128">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d5431-128">Parent elements</span></span>

|<span data-ttu-id="d5431-129">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d5431-129">**Element**</span></span>|<span data-ttu-id="d5431-130">**Description**</span><span class="sxs-lookup"><span data-stu-id="d5431-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d5431-131">FindItem</span><span class="sxs-lookup"><span data-stu-id="d5431-131">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="d5431-132">Définit une requête pour rechercher des éléments dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="d5431-132">Defines a request to find items in a mailbox.</span></span><br/><br/> <span data-ttu-id="d5431-133">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="d5431-133">The following is the XPath expression to this element:</span></span>  <br/>  `/FindItem` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d5431-134">Remarques</span><span class="sxs-lookup"><span data-stu-id="d5431-134">Remarks</span></span>

<span data-ttu-id="d5431-135">Si l’élément **CalendarView** est spécifié dans une requête FindItem, le service Web retourne une liste d’éléments de calendrier et les occurrences du rendez-vous périodiques dans la plage spécifiée par les **arguments StartDate** et **EndDate**.</span><span class="sxs-lookup"><span data-stu-id="d5431-135">If the **CalendarView** element is specified in a FindItem request, the Web service returns a list of single calendar items and occurrences of recurring calendar items within the range specified by **StartDate** and **EndDate**.</span></span>
  
<span data-ttu-id="d5431-136">Si l’élément **CalendarView** n’est pas spécifié dans une requête FindItem, le service Web retourne une liste des éléments de calendrier unique et des éléments de calendrier principal périodique.</span><span class="sxs-lookup"><span data-stu-id="d5431-136">If the **CalendarView** element is not specified in a FindItem request, the Web service returns a list of single calendar items and recurring master calendar items.</span></span> <span data-ttu-id="d5431-137">Occurrences de calendrier d’un élément de calendrier périodique ne sont pas développés.</span><span class="sxs-lookup"><span data-stu-id="d5431-137">Calendar occurrences of a recurring calendar item are not expanded.</span></span> 
  
<span data-ttu-id="d5431-138">Requêtes CalendarView doivent effectuer uniquement utiliser les propriétés suivantes dans la mesure où elles prennent en charge les requêtes de calendrier plus rapides.</span><span class="sxs-lookup"><span data-stu-id="d5431-138">CalendarView queries should only make use of the following properties since they support faster calendar queries.</span></span>
  
### <a name="recurrence-blob-properties"></a><span data-ttu-id="d5431-139">Propriétés des objets blob de périodicité</span><span class="sxs-lookup"><span data-stu-id="d5431-139">Recurrence blob properties</span></span>
  
- <span data-ttu-id="d5431-140">MapiStartTime</span><span class="sxs-lookup"><span data-stu-id="d5431-140">MapiStartTime</span></span>
    
- <span data-ttu-id="d5431-141">MapiEndTime</span><span class="sxs-lookup"><span data-stu-id="d5431-141">MapiEndTime</span></span>
    
- <span data-ttu-id="d5431-142">SubjectPrefixInternal</span><span class="sxs-lookup"><span data-stu-id="d5431-142">SubjectPrefixInternal</span></span>
    
- <span data-ttu-id="d5431-143">NormalizedSubjectInternal</span><span class="sxs-lookup"><span data-stu-id="d5431-143">NormalizedSubjectInternal</span></span>
    
- <span data-ttu-id="d5431-144">MapiSubject</span><span class="sxs-lookup"><span data-stu-id="d5431-144">MapiSubject</span></span>
    
- <span data-ttu-id="d5431-145">Emplacement</span><span class="sxs-lookup"><span data-stu-id="d5431-145">Location</span></span>
    
- <span data-ttu-id="d5431-146">AppointmentColor</span><span class="sxs-lookup"><span data-stu-id="d5431-146">AppointmentColor</span></span>
    
- <span data-ttu-id="d5431-147">MapiIsAllDayEvent</span><span class="sxs-lookup"><span data-stu-id="d5431-147">MapiIsAllDayEvent</span></span>
    
- <span data-ttu-id="d5431-148">MapiHasAttachment</span><span class="sxs-lookup"><span data-stu-id="d5431-148">MapiHasAttachment</span></span>
    
- <span data-ttu-id="d5431-149">FreeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="d5431-149">FreeBusyStatus</span></span>
    
- <span data-ttu-id="d5431-150">ReminderIsSetInternal</span><span class="sxs-lookup"><span data-stu-id="d5431-150">ReminderIsSetInternal</span></span>
    
- <span data-ttu-id="d5431-151">ReminderMinutesBeforeStartInternal</span><span class="sxs-lookup"><span data-stu-id="d5431-151">ReminderMinutesBeforeStartInternal</span></span>
    
- <span data-ttu-id="d5431-152">AppointmentState</span><span class="sxs-lookup"><span data-stu-id="d5431-152">AppointmentState</span></span>
    
- <span data-ttu-id="d5431-153">AllAttachmentsHidden</span><span class="sxs-lookup"><span data-stu-id="d5431-153">AllAttachmentsHidden</span></span>
    
- <span data-ttu-id="d5431-154">ChangeHighlight</span><span class="sxs-lookup"><span data-stu-id="d5431-154">ChangeHighlight</span></span>
    
### <a name="calculated-from-the-primary-recurrence-blob-or-master"></a><span data-ttu-id="d5431-155">Calculé à partir de l’objet blob de périodicité principal ou master</span><span class="sxs-lookup"><span data-stu-id="d5431-155">Calculated from the primary recurrence blob or master</span></span>
  
- <span data-ttu-id="d5431-156">ItemId</span><span class="sxs-lookup"><span data-stu-id="d5431-156">ItemId</span></span>
    
- <span data-ttu-id="d5431-157">IsRecurring</span><span class="sxs-lookup"><span data-stu-id="d5431-157">IsRecurring</span></span>
    
- <span data-ttu-id="d5431-158">IsException</span><span class="sxs-lookup"><span data-stu-id="d5431-158">IsException</span></span>
    
- <span data-ttu-id="d5431-159">AppointmentRecurring</span><span class="sxs-lookup"><span data-stu-id="d5431-159">AppointmentRecurring</span></span>
    
- <span data-ttu-id="d5431-160">MapiStartTime</span><span class="sxs-lookup"><span data-stu-id="d5431-160">MapiStartTime</span></span>
    
- <span data-ttu-id="d5431-161">MapiPRStartDate</span><span class="sxs-lookup"><span data-stu-id="d5431-161">MapiPRStartDate</span></span>
    
- <span data-ttu-id="d5431-162">MapiEndTime</span><span class="sxs-lookup"><span data-stu-id="d5431-162">MapiEndTime</span></span>
    
- <span data-ttu-id="d5431-163">MapiPREndDate</span><span class="sxs-lookup"><span data-stu-id="d5431-163">MapiPREndDate</span></span>
    
- <span data-ttu-id="d5431-164">CalendarItemType</span><span class="sxs-lookup"><span data-stu-id="d5431-164">CalendarItemType</span></span>
    
- <span data-ttu-id="d5431-165">GlobalObjectId</span><span class="sxs-lookup"><span data-stu-id="d5431-165">GlobalObjectId</span></span>
    
- <span data-ttu-id="d5431-166">TimeZoneDefinitionStart</span><span class="sxs-lookup"><span data-stu-id="d5431-166">TimeZoneDefinitionStart</span></span>
    
- <span data-ttu-id="d5431-167">TimeZoneDefinitionEnd</span><span class="sxs-lookup"><span data-stu-id="d5431-167">TimeZoneDefinitionEnd</span></span>
    
### <a name="master-calendar-item-properties"></a><span data-ttu-id="d5431-168">Propriétés de l’élément calendrier principal</span><span class="sxs-lookup"><span data-stu-id="d5431-168">Master calendar item properties</span></span>
  
- <span data-ttu-id="d5431-169">Propriété EntryId</span><span class="sxs-lookup"><span data-stu-id="d5431-169">EntryId</span></span>
    
- <span data-ttu-id="d5431-170">ChangeKey</span><span class="sxs-lookup"><span data-stu-id="d5431-170">ChangeKey</span></span>
    
- <span data-ttu-id="d5431-171">ItemClass</span><span class="sxs-lookup"><span data-stu-id="d5431-171">ItemClass</span></span>
    
- <span data-ttu-id="d5431-172">SentRepresentingEmailAddress</span><span class="sxs-lookup"><span data-stu-id="d5431-172">SentRepresentingEmailAddress</span></span>
    
- <span data-ttu-id="d5431-173">SentRepresentingDisplayName</span><span class="sxs-lookup"><span data-stu-id="d5431-173">SentRepresentingDisplayName</span></span>
    
- <span data-ttu-id="d5431-174">SentRepresentingEntryId</span><span class="sxs-lookup"><span data-stu-id="d5431-174">SentRepresentingEntryId</span></span>
    
- <span data-ttu-id="d5431-175">AppointmentRecurrenceBlob</span><span class="sxs-lookup"><span data-stu-id="d5431-175">AppointmentRecurrenceBlob</span></span>
    
- <span data-ttu-id="d5431-176">TimeZone</span><span class="sxs-lookup"><span data-stu-id="d5431-176">TimeZone</span></span>
    
- <span data-ttu-id="d5431-177">TimeZoneBlob</span><span class="sxs-lookup"><span data-stu-id="d5431-177">TimeZoneBlob</span></span>
    
- <span data-ttu-id="d5431-178">TimeZoneDefinitionRecurring</span><span class="sxs-lookup"><span data-stu-id="d5431-178">TimeZoneDefinitionRecurring</span></span>
    
- <span data-ttu-id="d5431-179">CleanGlobalObjectId</span><span class="sxs-lookup"><span data-stu-id="d5431-179">CleanGlobalObjectId</span></span>
    
- <span data-ttu-id="d5431-180">AppointmentRecurring</span><span class="sxs-lookup"><span data-stu-id="d5431-180">AppointmentRecurring</span></span>
    
- <span data-ttu-id="d5431-181">IsException</span><span class="sxs-lookup"><span data-stu-id="d5431-181">IsException</span></span>
    
- <span data-ttu-id="d5431-182">IsRecurring</span><span class="sxs-lookup"><span data-stu-id="d5431-182">IsRecurring</span></span>
    
- <span data-ttu-id="d5431-183">MapiSensitivity</span><span class="sxs-lookup"><span data-stu-id="d5431-183">MapiSensitivity</span></span>
    
- <span data-ttu-id="d5431-184">ContainerClass</span><span class="sxs-lookup"><span data-stu-id="d5431-184">ContainerClass</span></span>
    
- <span data-ttu-id="d5431-185">MapiPRStartDate</span><span class="sxs-lookup"><span data-stu-id="d5431-185">MapiPRStartDate</span></span>
    
- <span data-ttu-id="d5431-186">MapiPREndDate</span><span class="sxs-lookup"><span data-stu-id="d5431-186">MapiPREndDate</span></span>
    
- <span data-ttu-id="d5431-187">Catégories</span><span class="sxs-lookup"><span data-stu-id="d5431-187">Categories</span></span>
    
<span data-ttu-id="d5431-188">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="d5431-188">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="example"></a><span data-ttu-id="d5431-189">Exemple</span><span class="sxs-lookup"><span data-stu-id="d5431-189">Example</span></span>

<span data-ttu-id="d5431-190">L’exemple suivant montre une demande FindItem.</span><span class="sxs-lookup"><span data-stu-id="d5431-190">The following example shows a FindItem request.</span></span> <span data-ttu-id="d5431-191">Une demande réussie retourne une réponse qui inclut les éléments de calendrier qui ont démarré à 2006-05-18T00:00:00-08:00 ou une fois et terminé avant 2006-05-19T00:00:00-08:00.</span><span class="sxs-lookup"><span data-stu-id="d5431-191">A successful request returns a response that includes calendar items that started at 2006-05-18T00:00:00-08:00 or after and ended before 2006-05-19T00:00:00-08:00.</span></span>
  
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

## <a name="element-information"></a><span data-ttu-id="d5431-192">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d5431-192">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d5431-193">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d5431-193">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d5431-194">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d5431-194">Schema Name</span></span>  <br/> |<span data-ttu-id="d5431-195">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="d5431-195">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d5431-196">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d5431-196">Validation File</span></span>  <br/> |<span data-ttu-id="d5431-197">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d5431-197">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d5431-198">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d5431-198">Can be Empty</span></span>  <br/> |<span data-ttu-id="d5431-199">False</span><span class="sxs-lookup"><span data-stu-id="d5431-199">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d5431-200">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d5431-200">See also</span></span>

- [<span data-ttu-id="d5431-201">Opération FindItem</span><span class="sxs-lookup"><span data-stu-id="d5431-201">FindItem operation</span></span>](finditem-operation.md)
- [<span data-ttu-id="d5431-202">Recherche d’éléments</span><span class="sxs-lookup"><span data-stu-id="d5431-202">Finding Items</span></span>](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

