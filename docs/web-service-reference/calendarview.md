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
description: L’élément CalendarView définit une opération FindItem comme renvoyant des éléments de calendrier dans un jeu tel qu’ils apparaissent dans un calendrier.
ms.openlocfilehash: e547a4b2db5c09ebefd9a072da6cc4733818002e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462261"
---
# <a name="calendarview"></a><span data-ttu-id="c245e-103">CalendarView</span><span class="sxs-lookup"><span data-stu-id="c245e-103">CalendarView</span></span>

<span data-ttu-id="c245e-104">L’élément **CalendarView** définit une [opération FindItem](finditem-operation.md) comme renvoyant des éléments de calendrier dans un jeu tel qu’ils apparaissent dans un calendrier.</span><span class="sxs-lookup"><span data-stu-id="c245e-104">The **CalendarView** element defines a [FindItem operation](finditem-operation.md) as returning calendar items in a set as they appear in a calendar.</span></span> 
  
[<span data-ttu-id="c245e-105">FindItem</span><span class="sxs-lookup"><span data-stu-id="c245e-105">FindItem</span></span>](finditem.md)
  
[<span data-ttu-id="c245e-106">CalendarView</span><span class="sxs-lookup"><span data-stu-id="c245e-106">CalendarView</span></span>](calendarview.md)
  
```XML
<CalendarView MaxEntriesReturned="" StartDate="" EndDate="" />
```

<span data-ttu-id="c245e-107">**CalendarView**</span><span class="sxs-lookup"><span data-stu-id="c245e-107">**CalendarView**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="c245e-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="c245e-108">Attributes and elements</span></span>

<span data-ttu-id="c245e-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="c245e-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c245e-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="c245e-110">Attributes</span></span>

|<span data-ttu-id="c245e-111">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="c245e-111">**Attribute**</span></span>|<span data-ttu-id="c245e-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="c245e-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c245e-113">**MaxEntriesReturned**</span><span class="sxs-lookup"><span data-stu-id="c245e-113">**MaxEntriesReturned**</span></span> <br/> |<span data-ttu-id="c245e-114">Décrit le nombre maximal de résultats à renvoyer dans la réponse FindItem.</span><span class="sxs-lookup"><span data-stu-id="c245e-114">Describes the maximum number of results to return in the FindItem response.</span></span>  <br/> |
|<span data-ttu-id="c245e-115">**StartDate**</span><span class="sxs-lookup"><span data-stu-id="c245e-115">**StartDate**</span></span> <br/> |<span data-ttu-id="c245e-116">Identifie le début d’un intervalle de temps interrogé pour les éléments de calendrier.</span><span class="sxs-lookup"><span data-stu-id="c245e-116">Identifies the start of a time span queried for calendar items.</span></span> <span data-ttu-id="c245e-117">Tous les éléments de calendrier dont l’heure de fin est antérieure à **StartDate** ne seront pas renvoyés.</span><span class="sxs-lookup"><span data-stu-id="c245e-117">All calendar items that have an end time that is before **StartDate** will not be returned.</span></span> <span data-ttu-id="c245e-118">La valeur de **StartDate** peut être spécifiée au format UTC (Coordinated Universal Time), en 2006-01-02T12:00:00Z, ou dans un format où l’heure locale et le décalage du fuseau horaire sont spécifiés, comme indiqué en 2006-01-02T04:00:00-08:00.</span><span class="sxs-lookup"><span data-stu-id="c245e-118">The value of **StartDate** can be specified in coordinated universal time (UTC) format, as in 2006-01-02T12:00:00Z, or in a format where local time and time zone offset is specified, as in 2006-01-02T04:00:00-08:00.</span></span>  <br/><br/><span data-ttu-id="c245e-119">Cet attribut est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="c245e-119">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="c245e-120">**EndDate**</span><span class="sxs-lookup"><span data-stu-id="c245e-120">**EndDate**</span></span> <br/> |<span data-ttu-id="c245e-121">Identifie la fin d’un intervalle de temps interrogé pour les éléments de calendrier.</span><span class="sxs-lookup"><span data-stu-id="c245e-121">Identifies the end of a time span queried for calendar items.</span></span> <span data-ttu-id="c245e-122">Tous les éléments de calendrier dont l’heure de début est identique ou **postérieure** à la date d’expiration ne sont pas renvoyés.</span><span class="sxs-lookup"><span data-stu-id="c245e-122">All calendar items that have a start time that is on or after **EndDate** will not be returned.</span></span> <span data-ttu-id="c245e-123">La valeur de **EndDate** peut être spécifiée au format UTC, comme en 2006-02-02T12:00:00Z, ou dans un format où l’heure locale et le décalage du fuseau horaire sont spécifiés, comme indiqué en 2006-02-02T04:00:00-08:00.</span><span class="sxs-lookup"><span data-stu-id="c245e-123">The value of **EndDate** can be specified in UTC format, as in 2006-02-02T12:00:00Z, or in a format where local time and time zone offset is specified, as in 2006-02-02T04:00:00-08:00.</span></span>  <br/><br/><span data-ttu-id="c245e-124">La date de **fin doit être** supérieure ou **égale à la**date de début ; Sinon, une erreur est renvoyée.</span><span class="sxs-lookup"><span data-stu-id="c245e-124">**EndDate** must be greater than or equal to **StartDate**; otherwise an error is returned.</span></span> <span data-ttu-id="c245e-125">Cet attribut est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="c245e-125">This attribute is required.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="c245e-126">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="c245e-126">Child elements</span></span>

<span data-ttu-id="c245e-127">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c245e-127">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c245e-128">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="c245e-128">Parent elements</span></span>

|<span data-ttu-id="c245e-129">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c245e-129">**Element**</span></span>|<span data-ttu-id="c245e-130">**Description**</span><span class="sxs-lookup"><span data-stu-id="c245e-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c245e-131">FindItem</span><span class="sxs-lookup"><span data-stu-id="c245e-131">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="c245e-132">Définit une requête pour rechercher des éléments dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="c245e-132">Defines a request to find items in a mailbox.</span></span><br/><br/> <span data-ttu-id="c245e-133">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="c245e-133">The following is the XPath expression to this element:</span></span>  <br/>  `/FindItem` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c245e-134">Remarques</span><span class="sxs-lookup"><span data-stu-id="c245e-134">Remarks</span></span>

<span data-ttu-id="c245e-135">Si l’élément **CalendarView** est spécifié dans une demande FindItem, le service Web renvoie une liste d’éléments de calendrier uniques et d’occurrences d’éléments de calendrier périodiques dans la plage spécifiée par **StartDate** et **EndDate**.</span><span class="sxs-lookup"><span data-stu-id="c245e-135">If the **CalendarView** element is specified in a FindItem request, the Web service returns a list of single calendar items and occurrences of recurring calendar items within the range specified by **StartDate** and **EndDate**.</span></span>
  
<span data-ttu-id="c245e-136">Si l’élément **CalendarView** n’est pas spécifié dans une demande FindItem, le service Web renvoie une liste des éléments de calendrier uniques et des éléments de calendrier principal périodiques.</span><span class="sxs-lookup"><span data-stu-id="c245e-136">If the **CalendarView** element is not specified in a FindItem request, the Web service returns a list of single calendar items and recurring master calendar items.</span></span> <span data-ttu-id="c245e-137">Les occurrences de calendrier d’un élément de calendrier périodique ne sont pas développées.</span><span class="sxs-lookup"><span data-stu-id="c245e-137">Calendar occurrences of a recurring calendar item are not expanded.</span></span> 
  
<span data-ttu-id="c245e-138">Les requêtes CalendarView doivent uniquement utiliser les propriétés suivantes, car elles prennent en charge des requêtes de calendrier plus rapides.</span><span class="sxs-lookup"><span data-stu-id="c245e-138">CalendarView queries should only make use of the following properties since they support faster calendar queries.</span></span>
  
### <a name="recurrence-blob-properties"></a><span data-ttu-id="c245e-139">Propriétés de l’objet blob de récurrence</span><span class="sxs-lookup"><span data-stu-id="c245e-139">Recurrence blob properties</span></span>
  
- <span data-ttu-id="c245e-140">MapiStartTime</span><span class="sxs-lookup"><span data-stu-id="c245e-140">MapiStartTime</span></span>
    
- <span data-ttu-id="c245e-141">MapiEndTime</span><span class="sxs-lookup"><span data-stu-id="c245e-141">MapiEndTime</span></span>
    
- <span data-ttu-id="c245e-142">SubjectPrefixInternal</span><span class="sxs-lookup"><span data-stu-id="c245e-142">SubjectPrefixInternal</span></span>
    
- <span data-ttu-id="c245e-143">NormalizedSubjectInternal</span><span class="sxs-lookup"><span data-stu-id="c245e-143">NormalizedSubjectInternal</span></span>
    
- <span data-ttu-id="c245e-144">MapiSubject</span><span class="sxs-lookup"><span data-stu-id="c245e-144">MapiSubject</span></span>
    
- <span data-ttu-id="c245e-145">Emplacement</span><span class="sxs-lookup"><span data-stu-id="c245e-145">Location</span></span>
    
- <span data-ttu-id="c245e-146">AppointmentColor</span><span class="sxs-lookup"><span data-stu-id="c245e-146">AppointmentColor</span></span>
    
- <span data-ttu-id="c245e-147">MapiIsAllDayEvent</span><span class="sxs-lookup"><span data-stu-id="c245e-147">MapiIsAllDayEvent</span></span>
    
- <span data-ttu-id="c245e-148">MapiHasAttachment</span><span class="sxs-lookup"><span data-stu-id="c245e-148">MapiHasAttachment</span></span>
    
- <span data-ttu-id="c245e-149">FreeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="c245e-149">FreeBusyStatus</span></span>
    
- <span data-ttu-id="c245e-150">ReminderIsSetInternal</span><span class="sxs-lookup"><span data-stu-id="c245e-150">ReminderIsSetInternal</span></span>
    
- <span data-ttu-id="c245e-151">ReminderMinutesBeforeStartInternal</span><span class="sxs-lookup"><span data-stu-id="c245e-151">ReminderMinutesBeforeStartInternal</span></span>
    
- <span data-ttu-id="c245e-152">AppointmentState</span><span class="sxs-lookup"><span data-stu-id="c245e-152">AppointmentState</span></span>
    
- <span data-ttu-id="c245e-153">AllAttachmentsHidden</span><span class="sxs-lookup"><span data-stu-id="c245e-153">AllAttachmentsHidden</span></span>
    
- <span data-ttu-id="c245e-154">ChangeHighlight</span><span class="sxs-lookup"><span data-stu-id="c245e-154">ChangeHighlight</span></span>
    
### <a name="calculated-from-the-primary-recurrence-blob-or-master"></a><span data-ttu-id="c245e-155">Calculé à partir de l’objet blob de récurrence principale ou de la forme de base</span><span class="sxs-lookup"><span data-stu-id="c245e-155">Calculated from the primary recurrence blob or master</span></span>
  
- <span data-ttu-id="c245e-156">ItemId</span><span class="sxs-lookup"><span data-stu-id="c245e-156">ItemId</span></span>
    
- <span data-ttu-id="c245e-157">IsRecurring</span><span class="sxs-lookup"><span data-stu-id="c245e-157">IsRecurring</span></span>
    
- <span data-ttu-id="c245e-158">IsException</span><span class="sxs-lookup"><span data-stu-id="c245e-158">IsException</span></span>
    
- <span data-ttu-id="c245e-159">AppointmentRecurring</span><span class="sxs-lookup"><span data-stu-id="c245e-159">AppointmentRecurring</span></span>
    
- <span data-ttu-id="c245e-160">MapiStartTime</span><span class="sxs-lookup"><span data-stu-id="c245e-160">MapiStartTime</span></span>
    
- <span data-ttu-id="c245e-161">MapiPRStartDate</span><span class="sxs-lookup"><span data-stu-id="c245e-161">MapiPRStartDate</span></span>
    
- <span data-ttu-id="c245e-162">MapiEndTime</span><span class="sxs-lookup"><span data-stu-id="c245e-162">MapiEndTime</span></span>
    
- <span data-ttu-id="c245e-163">MapiPREndDate</span><span class="sxs-lookup"><span data-stu-id="c245e-163">MapiPREndDate</span></span>
    
- <span data-ttu-id="c245e-164">CalendarItemType</span><span class="sxs-lookup"><span data-stu-id="c245e-164">CalendarItemType</span></span>
    
- <span data-ttu-id="c245e-165">GlobalObjectId</span><span class="sxs-lookup"><span data-stu-id="c245e-165">GlobalObjectId</span></span>
    
- <span data-ttu-id="c245e-166">TimeZoneDefinitionStart</span><span class="sxs-lookup"><span data-stu-id="c245e-166">TimeZoneDefinitionStart</span></span>
    
- <span data-ttu-id="c245e-167">TimeZoneDefinitionEnd</span><span class="sxs-lookup"><span data-stu-id="c245e-167">TimeZoneDefinitionEnd</span></span>
    
### <a name="master-calendar-item-properties"></a><span data-ttu-id="c245e-168">Propriétés de l’élément de calendrier principal</span><span class="sxs-lookup"><span data-stu-id="c245e-168">Master calendar item properties</span></span>
  
- <span data-ttu-id="c245e-169">Entrée</span><span class="sxs-lookup"><span data-stu-id="c245e-169">EntryId</span></span>
    
- <span data-ttu-id="c245e-170">ChangeKey</span><span class="sxs-lookup"><span data-stu-id="c245e-170">ChangeKey</span></span>
    
- <span data-ttu-id="c245e-171">ItemClass</span><span class="sxs-lookup"><span data-stu-id="c245e-171">ItemClass</span></span>
    
- <span data-ttu-id="c245e-172">SentRepresentingEmailAddress</span><span class="sxs-lookup"><span data-stu-id="c245e-172">SentRepresentingEmailAddress</span></span>
    
- <span data-ttu-id="c245e-173">SentRepresentingDisplayName</span><span class="sxs-lookup"><span data-stu-id="c245e-173">SentRepresentingDisplayName</span></span>
    
- <span data-ttu-id="c245e-174">SentRepresentingEntryId</span><span class="sxs-lookup"><span data-stu-id="c245e-174">SentRepresentingEntryId</span></span>
    
- <span data-ttu-id="c245e-175">AppointmentRecurrenceBlob</span><span class="sxs-lookup"><span data-stu-id="c245e-175">AppointmentRecurrenceBlob</span></span>
    
- <span data-ttu-id="c245e-176">TimeZone</span><span class="sxs-lookup"><span data-stu-id="c245e-176">TimeZone</span></span>
    
- <span data-ttu-id="c245e-177">TimeZoneBlob</span><span class="sxs-lookup"><span data-stu-id="c245e-177">TimeZoneBlob</span></span>
    
- <span data-ttu-id="c245e-178">TimeZoneDefinitionRecurring</span><span class="sxs-lookup"><span data-stu-id="c245e-178">TimeZoneDefinitionRecurring</span></span>
    
- <span data-ttu-id="c245e-179">CleanGlobalObjectId</span><span class="sxs-lookup"><span data-stu-id="c245e-179">CleanGlobalObjectId</span></span>
    
- <span data-ttu-id="c245e-180">AppointmentRecurring</span><span class="sxs-lookup"><span data-stu-id="c245e-180">AppointmentRecurring</span></span>
    
- <span data-ttu-id="c245e-181">IsException</span><span class="sxs-lookup"><span data-stu-id="c245e-181">IsException</span></span>
    
- <span data-ttu-id="c245e-182">IsRecurring</span><span class="sxs-lookup"><span data-stu-id="c245e-182">IsRecurring</span></span>
    
- <span data-ttu-id="c245e-183">MapiSensitivity</span><span class="sxs-lookup"><span data-stu-id="c245e-183">MapiSensitivity</span></span>
    
- <span data-ttu-id="c245e-184">ContainerClass</span><span class="sxs-lookup"><span data-stu-id="c245e-184">ContainerClass</span></span>
    
- <span data-ttu-id="c245e-185">MapiPRStartDate</span><span class="sxs-lookup"><span data-stu-id="c245e-185">MapiPRStartDate</span></span>
    
- <span data-ttu-id="c245e-186">MapiPREndDate</span><span class="sxs-lookup"><span data-stu-id="c245e-186">MapiPREndDate</span></span>
    
- <span data-ttu-id="c245e-187">Catégories</span><span class="sxs-lookup"><span data-stu-id="c245e-187">Categories</span></span>
    
<span data-ttu-id="c245e-188">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="c245e-188">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="example"></a><span data-ttu-id="c245e-189">Exemple</span><span class="sxs-lookup"><span data-stu-id="c245e-189">Example</span></span>

<span data-ttu-id="c245e-190">L’exemple suivant montre une requête FindItem.</span><span class="sxs-lookup"><span data-stu-id="c245e-190">The following example shows a FindItem request.</span></span> <span data-ttu-id="c245e-191">Une demande réussie renvoie une réponse qui inclut des éléments de calendrier démarrés à 2006-05-18T00:00:00-08:00 ou après et s’est terminé avant 2006-05-19T00:00:00-08:00.</span><span class="sxs-lookup"><span data-stu-id="c245e-191">A successful request returns a response that includes calendar items that started at 2006-05-18T00:00:00-08:00 or after and ended before 2006-05-19T00:00:00-08:00.</span></span>
  
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

## <a name="element-information"></a><span data-ttu-id="c245e-192">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="c245e-192">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c245e-193">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="c245e-193">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c245e-194">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="c245e-194">Schema Name</span></span>  <br/> |<span data-ttu-id="c245e-195">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="c245e-195">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c245e-196">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="c245e-196">Validation File</span></span>  <br/> |<span data-ttu-id="c245e-197">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="c245e-197">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c245e-198">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="c245e-198">Can be Empty</span></span>  <br/> |<span data-ttu-id="c245e-199">False</span><span class="sxs-lookup"><span data-stu-id="c245e-199">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c245e-200">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c245e-200">See also</span></span>

- [<span data-ttu-id="c245e-201">Opération FindItem</span><span class="sxs-lookup"><span data-stu-id="c245e-201">FindItem operation</span></span>](finditem-operation.md)
- [<span data-ttu-id="c245e-202">Recherche d’éléments</span><span class="sxs-lookup"><span data-stu-id="c245e-202">Finding Items</span></span>](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

