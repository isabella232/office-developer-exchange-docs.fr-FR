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
description: L’élément GetUserAvailabilityRequest contient les arguments utilisés pour obtenir les informations de disponibilité de l’utilisateur. Il s’agit d’un élément racine.
ms.openlocfilehash: 6c2e2c5452b6379171e49cf6aea2d437152ecb9b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459117"
---
# <a name="getuseravailabilityrequest"></a><span data-ttu-id="3e48f-104">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="3e48f-104">GetUserAvailabilityRequest</span></span>

<span data-ttu-id="3e48f-105">L’élément **GetUserAvailabilityRequest** contient les arguments utilisés pour obtenir les informations de disponibilité de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="3e48f-105">The **GetUserAvailabilityRequest** element contains the arguments used to obtain user availability information.</span></span> <span data-ttu-id="3e48f-106">Il s’agit d’un élément racine.</span><span class="sxs-lookup"><span data-stu-id="3e48f-106">This is a root element.</span></span> 
  
```xml
<GetUserAvailabilityRequest>
   <TimeZone>...</TimeZone>
   <MailboxDataArray>...</MailboxDataArray>
   <FreeBusyViewOptions>...</FreeBusyViewOptions>
   <SuggestionsViewOptions>...</SuggestionsViewOptions>
</GetUserAvailabilityRequest>
```

 <span data-ttu-id="3e48f-107">**GetUserAvailabilityRequestType**</span><span class="sxs-lookup"><span data-stu-id="3e48f-107">**GetUserAvailabilityRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3e48f-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="3e48f-108">Attributes and elements</span></span>

<span data-ttu-id="3e48f-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="3e48f-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3e48f-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="3e48f-110">Attributes</span></span>

<span data-ttu-id="3e48f-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="3e48f-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3e48f-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="3e48f-112">Child elements</span></span>

|<span data-ttu-id="3e48f-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3e48f-113">**Element**</span></span>|<span data-ttu-id="3e48f-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="3e48f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3e48f-115">TimeZone (disponibilité)</span><span class="sxs-lookup"><span data-stu-id="3e48f-115">TimeZone (Availability)</span></span>](timezone-availability.md) <br/> |<span data-ttu-id="3e48f-116">Contient des éléments qui identifient les informations de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="3e48f-116">Contains elements that identify time zone information.</span></span> <span data-ttu-id="3e48f-117">Cet élément contient également des informations sur la transition entre l’heure standard et l’heure d’été.</span><span class="sxs-lookup"><span data-stu-id="3e48f-117">This element also contains information about the transition between standard time and daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="3e48f-118">MailboxDataArray</span><span class="sxs-lookup"><span data-stu-id="3e48f-118">MailboxDataArray</span></span>](mailboxdataarray.md) <br/> |<span data-ttu-id="3e48f-119">Contient la liste des boîtes aux lettres à interroger pour obtenir des informations de disponibilité.</span><span class="sxs-lookup"><span data-stu-id="3e48f-119">Contains a list of mailboxes to query for availability information.</span></span>  <br/> |
|[<span data-ttu-id="3e48f-120">FreeBusyViewOptions</span><span class="sxs-lookup"><span data-stu-id="3e48f-120">FreeBusyViewOptions</span></span>](freebusyviewoptions.md) <br/> |<span data-ttu-id="3e48f-121">Spécifie le type d’informations de disponibilité renvoyées dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="3e48f-121">Specifies the type of free/busy information returned in the response.</span></span>  <br/> |
|[<span data-ttu-id="3e48f-122">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="3e48f-122">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md) <br/> |<span data-ttu-id="3e48f-123">Contient les options permettant d’obtenir des informations sur les suggestions de réunion.</span><span class="sxs-lookup"><span data-stu-id="3e48f-123">Contains the options for obtaining meeting suggestion information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3e48f-124">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="3e48f-124">Parent elements</span></span>

<span data-ttu-id="3e48f-125">Aucun.</span><span class="sxs-lookup"><span data-stu-id="3e48f-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3e48f-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="3e48f-126">Remarks</span></span>

<span data-ttu-id="3e48f-127">Le schéma qui décrit cet élément se trouve dans le répertoire/EWS/de l’ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="3e48f-127">The schema that describes this element is located in the /EWS/ directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="3e48f-128">Exemple</span><span class="sxs-lookup"><span data-stu-id="3e48f-128">Example</span></span>

<span data-ttu-id="3e48f-129">L’exemple suivant montre une demande d’informations de disponibilité.</span><span class="sxs-lookup"><span data-stu-id="3e48f-129">The following example shows a request for free/busy information.</span></span>
  
```
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <GetUserAvailabilityRequest xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <TimeZone xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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
        <MailboxData xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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
      <FreeBusyViewOptions xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="element-information"></a><span data-ttu-id="3e48f-130">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="3e48f-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3e48f-131">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="3e48f-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3e48f-132">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="3e48f-132">Schema Name</span></span>  <br/> |<span data-ttu-id="3e48f-133">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="3e48f-133">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3e48f-134">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="3e48f-134">Validation File</span></span>  <br/> |<span data-ttu-id="3e48f-135">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="3e48f-135">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3e48f-136">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="3e48f-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="3e48f-137">False</span><span class="sxs-lookup"><span data-stu-id="3e48f-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3e48f-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="3e48f-138">See also</span></span>



[<span data-ttu-id="3e48f-139">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="3e48f-139">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="3e48f-140">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="3e48f-140">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="3e48f-141">Obtention de la disponibilité des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="3e48f-141">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

