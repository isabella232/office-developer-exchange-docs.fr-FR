---
title: GetUserAvailabilityResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetUserAvailabilityResponse
api_type:
- schema
ms.assetid: 6999510a-d60e-43da-8964-57b5fb3e9d11
description: L’élément GetUserAvailabilityResponse est l’élément racine qui contient les propriétés qui définissent les informations de disponibilité de l’utilisateur ou les informations sur les heures de réunion suggérées.
ms.openlocfilehash: ceb24bc8b31a7d7313add213c26bef5efd3c89ae
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458214"
---
# <a name="getuseravailabilityresponse"></a><span data-ttu-id="ae213-103">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="ae213-103">GetUserAvailabilityResponse</span></span>

<span data-ttu-id="ae213-104">L’élément **GetUserAvailabilityResponse** est l’élément racine qui contient les propriétés qui définissent les informations de disponibilité de l’utilisateur ou les informations sur les heures de réunion suggérées.</span><span class="sxs-lookup"><span data-stu-id="ae213-104">The **GetUserAvailabilityResponse** element is the root element that contains the properties that define user availability information or suggested meeting time information.</span></span> 
  
```xml
<GetUserAvailabilityResponse>
   <FreeBusyResponseArray>...</FreeBusyResponseArray>
   <SuggestionsResponse>...</SuggestionsResponse>
</GetUserAvailabilityResponse>
```

 <span data-ttu-id="ae213-105">**GetUserAvailabilityResponseType**</span><span class="sxs-lookup"><span data-stu-id="ae213-105">**GetUserAvailabilityResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ae213-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ae213-106">Attributes and elements</span></span>

<span data-ttu-id="ae213-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ae213-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ae213-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="ae213-108">Attributes</span></span>

<span data-ttu-id="ae213-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="ae213-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ae213-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ae213-110">Child elements</span></span>

|<span data-ttu-id="ae213-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ae213-111">**Element**</span></span>|<span data-ttu-id="ae213-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="ae213-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ae213-113">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="ae213-113">FreeBusyResponseArray</span></span>](freebusyresponsearray.md) <br/> |<span data-ttu-id="ae213-114">Contient les informations de disponibilité des utilisateurs demandés et l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="ae213-114">Contains the requested users' availability information and the response status.</span></span>  <br/> |
|[<span data-ttu-id="ae213-115">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="ae213-115">SuggestionsResponse</span></span>](suggestionsresponse.md) <br/> |<span data-ttu-id="ae213-116">Contient des informations sur l’état de la réponse et des suggestions pour les suggestions de réunion demandées.</span><span class="sxs-lookup"><span data-stu-id="ae213-116">Contains response status information and suggestion data for requested meeting suggestions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ae213-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ae213-117">Parent elements</span></span>

<span data-ttu-id="ae213-118">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ae213-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ae213-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="ae213-119">Remarks</span></span>

<span data-ttu-id="ae213-120">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="ae213-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="ae213-121">Exemple</span><span class="sxs-lookup"><span data-stu-id="ae213-121">Example</span></span>

<span data-ttu-id="ae213-122">L’exemple suivant de réponse GetUserAvailability indique une réponse à une demande GetUserAvailability.</span><span class="sxs-lookup"><span data-stu-id="ae213-122">The following example of a GetUserAvailability response shows a response to a GetUserAvailability request.</span></span>
  
```
<?xml version="1.0" encoding="utf-8" ?>
<GetUserAvailabilityResponse xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
                             xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <FreeBusyResponseArray xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
    <FreeBusyResponse>
      <ResponseMessage ResponseClass="Success">
        <Path select="/m:GetUserAvailabilityRequest/MailboxDataArray[0]" />
      </ResponseMessage>
      <FreeBusyView>
        <FreeBusyViewType xmlns="https://schemas.microsoft.com/exchange/services/2006/types">Detailed</FreeBusyViewType>
        <CalendarEventArray xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <CalendarEvent>
            <StartTime>2006-02-28T19:00:00-08:00</StartTime>
            <EndTime>2006-02-28T23:30:00-08:00</EndTime>
            <BusyType>OOF</BusyType>
            <IsPrivate>false</IsPrivate>
            <CalendarEventDetails>
              <ID>00000</ID>
              <Subject>Exercise</Subject>
              <Location>the gym</Location>
              <IsMeeting>false</IsMeeting>
              <IsRecurring>false</IsRecurring>
              <IsException>false</IsException>
              <IsReminderSet>true</IsReminderSet>
            </CalendarEventDetails>
          </CalendarEvent>
        </CalendarEventArray>
        <WorkingHours xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <TimeZone>
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
          <WorkingPeriodArray>
            <WorkingPeriod>
              <DayOfWeek>Monday Tuesday Wednesday Thursday Friday</DayOfWeek>
              <StartTimeInMinutes>480</StartTimeInMinutes>
              <EndTimeInMinutes>1020</EndTimeInMinutes>
            </WorkingPeriod>
          </WorkingPeriodArray>
        </WorkingHours>
      </FreeBusyView>
    </FreeBusyResponse>
  </FreeBusyResponseArray>
</GetUserAvailabilityResponse>
```

<span data-ttu-id="ae213-123">Le contenu de l’élément [ID](id.md) a été raccourci afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="ae213-123">The [ID](id.md) element contents were shortened to preserve readability.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="ae213-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ae213-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ae213-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ae213-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ae213-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ae213-126">Schema Name</span></span>  <br/> |<span data-ttu-id="ae213-127">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="ae213-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ae213-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ae213-128">Validation File</span></span>  <br/> |<span data-ttu-id="ae213-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="ae213-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ae213-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ae213-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="ae213-131">False</span><span class="sxs-lookup"><span data-stu-id="ae213-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ae213-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ae213-132">See also</span></span>



[<span data-ttu-id="ae213-133">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="ae213-133">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)


[<span data-ttu-id="ae213-134">Obtention de la disponibilité des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="ae213-134">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

