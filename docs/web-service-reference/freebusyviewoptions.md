---
title: FreeBusyViewOptions
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FreeBusyViewOptions
api_type:
- schema
ms.assetid: c07f3ddb-874b-4d30-a60e-7e5c7793bb6f
description: L’élément FreeBusyViewOptions spécifie le type d’informations de disponibilité renvoyées dans la réponse.
ms.openlocfilehash: b67d3f461e0edaa82f074f75b0c1c54efc8af4d0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459573"
---
# <a name="freebusyviewoptions"></a><span data-ttu-id="2c478-103">FreeBusyViewOptions</span><span class="sxs-lookup"><span data-stu-id="2c478-103">FreeBusyViewOptions</span></span>

<span data-ttu-id="2c478-104">L’élément **FreeBusyViewOptions** spécifie le type d’informations de disponibilité renvoyées dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="2c478-104">The **FreeBusyViewOptions** element specifies the type of free/busy information returned in the response.</span></span> 
  
[<span data-ttu-id="2c478-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="2c478-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="2c478-106">FreeBusyViewOptions</span><span class="sxs-lookup"><span data-stu-id="2c478-106">FreeBusyViewOptions</span></span>](freebusyviewoptions.md)
  
```xml
<FreeBusyViewOptions>
   <TimeWindow>...</TimeWindow>
   <MergedFreeBusyIntervalInMinutes>...</MergedFreeBusyIntervalInMinutes>
<RequestedView>...</RequestedView>
</FreeBusyViewOptions>

```

 <span data-ttu-id="2c478-107">**FreeBusyViewOptionsType**</span><span class="sxs-lookup"><span data-stu-id="2c478-107">**FreeBusyViewOptionsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2c478-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="2c478-108">Attributes and elements</span></span>

<span data-ttu-id="2c478-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="2c478-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2c478-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="2c478-110">Attributes</span></span>

<span data-ttu-id="2c478-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="2c478-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2c478-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="2c478-112">Child elements</span></span>

|<span data-ttu-id="2c478-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2c478-113">**Element**</span></span>|<span data-ttu-id="2c478-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="2c478-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2c478-115">TimeWindow</span><span class="sxs-lookup"><span data-stu-id="2c478-115">TimeWindow</span></span>](timewindow.md) <br/> |<span data-ttu-id="2c478-116">Identifie la période interrogée pour les informations de disponibilité de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="2c478-116">Identifies the time span queried for the user availability information.</span></span>  <br/> |
|[<span data-ttu-id="2c478-117">MergedFreeBusyIntervalInMinutes</span><span class="sxs-lookup"><span data-stu-id="2c478-117">MergedFreeBusyIntervalInMinutes</span></span>](mergedfreebusyintervalinminutes.md) <br/> |<span data-ttu-id="2c478-118">Représente la différence de temps entre deux slots successifs dans la vue **FreeBusyMerged** .</span><span class="sxs-lookup"><span data-stu-id="2c478-118">Represents the time difference between two successive slots in the **FreeBusyMerged** view.</span></span>  <br/> |
|[<span data-ttu-id="2c478-119">RequestedView</span><span class="sxs-lookup"><span data-stu-id="2c478-119">RequestedView</span></span>](requestedview.md) <br/> |<span data-ttu-id="2c478-120">Définit le type d’informations de calendrier demandées par un client.</span><span class="sxs-lookup"><span data-stu-id="2c478-120">Defines the type of calendar information that a client requests.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2c478-121">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="2c478-121">Parent elements</span></span>

|<span data-ttu-id="2c478-122">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2c478-122">**Element**</span></span>|<span data-ttu-id="2c478-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="2c478-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2c478-124">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="2c478-124">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md) <br/> |<span data-ttu-id="2c478-125">Contient les arguments utilisés pour obtenir les informations de disponibilité de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="2c478-125">Contains the arguments used to obtain user availability information.</span></span> <span data-ttu-id="2c478-126">Il s’agit d’un élément racine.</span><span class="sxs-lookup"><span data-stu-id="2c478-126">This is a root element.</span></span>  <br/> <span data-ttu-id="2c478-127">Voici le XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="2c478-127">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2c478-128">Remarques</span><span class="sxs-lookup"><span data-stu-id="2c478-128">Remarks</span></span>

<span data-ttu-id="2c478-129">Cet élément n’est pas obligatoire et ne peut se produire qu’une seule fois s’il est utilisé.</span><span class="sxs-lookup"><span data-stu-id="2c478-129">This element is not required and can only occur once if used.</span></span> <span data-ttu-id="2c478-130">Cette valeur peut être null si la valeur de l’élément [SuggestionsViewOptions](suggestionsviewoptions.md) n’est pas null.</span><span class="sxs-lookup"><span data-stu-id="2c478-130">This value can be null if the value of the [SuggestionsViewOptions](suggestionsviewoptions.md) element is not null.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="2c478-131">Le schéma qui décrit cet élément se trouve dans le répertoire/EPI/de l’ordinateur exécutant Microsoft® Exchange Server 2007 sur lequel le rôle serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="2c478-131">The schema that describes this element is located in the /epi/ directory of the computer that is running Microsoft® Exchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="example"></a><span data-ttu-id="2c478-132">Exemple</span><span class="sxs-lookup"><span data-stu-id="2c478-132">Example</span></span>

<span data-ttu-id="2c478-133">L’exemple suivant obtient une liste de réunions et un flux de disponibilité dans les intervalles de 60 minutes.</span><span class="sxs-lookup"><span data-stu-id="2c478-133">The following example obtains a list of meetings and a free/busy stream in 60-minute intervals.</span></span>
  
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
            <Address>someone@ExServer.example.com</Address>
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
          <EndTime>2006-02-25T23:59:59</EndTime>
        </TimeWindow>
        <MergedFreeBusyIntervalInMinutes>60</MergedFreeBusyIntervalInMinutes>
        <RequestedView>FreeBusyMerged</RequestedView>
      </FreeBusyViewOptions>
    </GetUserAvailabilityRequest>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a><span data-ttu-id="2c478-134">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="2c478-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2c478-135">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="2c478-135">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2c478-136">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="2c478-136">Schema Name</span></span>  <br/> |<span data-ttu-id="2c478-137">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="2c478-137">Types schema</span></span>  <br/> |
|<span data-ttu-id="2c478-138">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="2c478-138">Validation File</span></span>  <br/> |<span data-ttu-id="2c478-139">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2c478-139">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2c478-140">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="2c478-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="2c478-141">False</span><span class="sxs-lookup"><span data-stu-id="2c478-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2c478-142">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="2c478-142">See also</span></span>



[<span data-ttu-id="2c478-143">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="2c478-143">GetUserAvailability operation</span></span>](getuseravailability-operation.md)


[<span data-ttu-id="2c478-144">Obtention de la disponibilité des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="2c478-144">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

