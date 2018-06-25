---
title: GetUserAvailabilityRequest
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetUserAvailabilityRequest
api_type:
- schema
ms.assetid: 7906711b-80a1-42ae-8b33-26eeac036a5a
description: L’élément GetUserAvailabilityRequest contient les arguments utilisés pour obtenir des informations de disponibilité d’utilisateur. Il s’agit d’un élément racine.
ms.openlocfilehash: 5440f739b09bfbe27ad97cba99c08756686594f7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827683"
---
# <a name="getuseravailabilityrequest"></a><span data-ttu-id="c6764-104">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="c6764-104">GetUserAvailabilityRequest</span></span>

<span data-ttu-id="c6764-105">L’élément **GetUserAvailabilityRequest** contient les arguments utilisés pour obtenir des informations de disponibilité d’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="c6764-105">The **GetUserAvailabilityRequest** element contains the arguments used to obtain user availability information.</span></span> <span data-ttu-id="c6764-106">Il s’agit d’un élément racine.</span><span class="sxs-lookup"><span data-stu-id="c6764-106">This is a root element.</span></span> 
  
```xml
<GetUserAvailabilityRequest>
   <TimeZone>...</TimeZone>
   <MailboxDataArray>...</MailboxDataArray>
   <FreeBusyViewOptions>...</FreeBusyViewOptions>
   <SuggestionsViewOptions>...</SuggestionsViewOptions>
</GetUserAvailabilityRequest>
```

 <span data-ttu-id="c6764-107">**GetUserAvailabilityRequestType**</span><span class="sxs-lookup"><span data-stu-id="c6764-107">**GetUserAvailabilityRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c6764-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="c6764-108">Attributes and elements</span></span>

<span data-ttu-id="c6764-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="c6764-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c6764-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="c6764-110">Attributes</span></span>

<span data-ttu-id="c6764-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c6764-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c6764-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="c6764-112">Child elements</span></span>

|<span data-ttu-id="c6764-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c6764-113">**Element**</span></span>|<span data-ttu-id="c6764-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="c6764-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c6764-115">Fuseau horaire (disponibilité)</span><span class="sxs-lookup"><span data-stu-id="c6764-115">TimeZone (Availability)</span></span>](timezone-availability.md) <br/> |<span data-ttu-id="c6764-116">Contient des éléments qui identifient les informations de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="c6764-116">Contains elements that identify time zone information.</span></span> <span data-ttu-id="c6764-117">Cet élément contient également des informations sur la transition entre heure standard et l’heure d’été.</span><span class="sxs-lookup"><span data-stu-id="c6764-117">This element also contains information about the transition between standard time and daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="c6764-118">MailboxDataArray</span><span class="sxs-lookup"><span data-stu-id="c6764-118">MailboxDataArray</span></span>](mailboxdataarray.md) <br/> |<span data-ttu-id="c6764-119">Contient une liste des boîtes aux lettres pour interroger des informations de disponibilité.</span><span class="sxs-lookup"><span data-stu-id="c6764-119">Contains a list of mailboxes to query for availability information.</span></span>  <br/> |
|[<span data-ttu-id="c6764-120">FreeBusyViewOptions</span><span class="sxs-lookup"><span data-stu-id="c6764-120">FreeBusyViewOptions</span></span>](freebusyviewoptions.md) <br/> |<span data-ttu-id="c6764-121">Spécifie le type d’informations disponible/occupé retournés dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="c6764-121">Specifies the type of free/busy information returned in the response.</span></span>  <br/> |
|[<span data-ttu-id="c6764-122">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="c6764-122">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md) <br/> |<span data-ttu-id="c6764-123">Contient les options permettant d’obtenir des informations de suggestion de réunion.</span><span class="sxs-lookup"><span data-stu-id="c6764-123">Contains the options for obtaining meeting suggestion information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c6764-124">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="c6764-124">Parent elements</span></span>

<span data-ttu-id="c6764-125">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c6764-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c6764-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="c6764-126">Remarks</span></span>

<span data-ttu-id="c6764-127">Le schéma qui décrit cet élément se trouve dans le répertoire /EWS/ de l’ordinateur qui exécute Microsoft Exchange Server 2007 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="c6764-127">The schema that describes this element is located in the /EWS/ directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="c6764-128">Exemple</span><span class="sxs-lookup"><span data-stu-id="c6764-128">Example</span></span>

<span data-ttu-id="c6764-129">L’exemple suivant montre une demande d’informations de disponibilité.</span><span class="sxs-lookup"><span data-stu-id="c6764-129">The following example shows a request for free/busy information.</span></span>
  
```
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <GetUserAvailabilityRequest xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <TimeZone xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
        <Bias>480</Bias>
        <StandardTime>
          <Bias>0</Bias>
          <Time>02:00:00</Time>
          <DayOrder>5</DayOrder>
          <Month>10</Month>
          <DayOfWeek>Sunday</DayOfWeek>
        </StandardTime>
        <DaylightTime>
          <Bias>-60</Bias>
          <Time>02:00:00</Time>
          <DayOrder>1</DayOrder>
          <Month>4</Month>
          <DayOfWeek>Sunday</DayOfWeek>
        </DaylightTime>
      </TimeZone>
      <MailboxDataArray>
        <MailboxData xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <Email>
            <Name></Name>
            <Address>someone@exchangeserver.example.com</Address>
            <RoutingType>SMTP</RoutingType>
          </Email>
          <AttendeeType>Organizer</AttendeeType>
          <ExcludeConflicts>false</ExcludeConflicts>
          <ExcludeNonWorkingHours>false</ExcludeNonWorkingHours>
        </MailboxData>
      </MailboxDataArray>
      <FreeBusyViewOptions xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
        <TimeWindow>
          <StartTime>2006-02-06T00:00:00</StartTime>
          <EndTime>2006-02-30T23:59:59</EndTime>
        </TimeWindow>
        <MergedFreeBusyIntervalInMinutes>60</MergedFreeBusyIntervalInMinutes>
        <RequestedView>FreeBusyMerged</RequestedView>
      </FreeBusyViewOptions>
    </GetUserAvailabilityRequest>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a><span data-ttu-id="c6764-130">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="c6764-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c6764-131">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="c6764-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c6764-132">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="c6764-132">Schema Name</span></span>  <br/> |<span data-ttu-id="c6764-133">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="c6764-133">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c6764-134">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="c6764-134">Validation File</span></span>  <br/> |<span data-ttu-id="c6764-135">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c6764-135">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c6764-136">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="c6764-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="c6764-137">False</span><span class="sxs-lookup"><span data-stu-id="c6764-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c6764-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c6764-138">See also</span></span>



[<span data-ttu-id="c6764-139">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="c6764-139">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="c6764-140">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="c6764-140">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="c6764-141">Obtention de disponibilité de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="c6764-141">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

