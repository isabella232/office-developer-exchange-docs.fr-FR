---
title: Opération GetServerTimeZones
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetServerTimeZones
api_type:
- schema
ms.assetid: 680173e1-e916-466b-b573-5a3182316345
description: L’opération GetServerTimeZones retourne des informations à partir des définitions de fuseau horaire sont disponibles sur un serveur Exchange.
ms.openlocfilehash: 9b202d510a599c9082d075228be4c479a2086753
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756744"
---
# <a name="getservertimezones-operation"></a><span data-ttu-id="97dd1-103">Opération GetServerTimeZones</span><span class="sxs-lookup"><span data-stu-id="97dd1-103">GetServerTimeZones operation</span></span>

<span data-ttu-id="97dd1-104">L’opération **GetServerTimeZones** retourne des informations à partir des définitions de fuseau horaire sont disponibles sur un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="97dd1-104">The **GetServerTimeZones** operation returns information from time zone definitions that are available on an Exchange server.</span></span> 
  
## <a name="soap-headers"></a><span data-ttu-id="97dd1-105">En-têtes SOAP</span><span class="sxs-lookup"><span data-stu-id="97dd1-105">SOAP Headers</span></span>

<span data-ttu-id="97dd1-106">L’opération **GetServerTimeZones** permettre utiliser les en-têtes SOAP qui sont répertoriés et décrits dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="97dd1-106">The **GetServerTimeZones** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="97dd1-107">**Header**</span><span class="sxs-lookup"><span data-stu-id="97dd1-107">**Header**</span></span>|<span data-ttu-id="97dd1-108">**Élément**</span><span class="sxs-lookup"><span data-stu-id="97dd1-108">**Element**</span></span>|<span data-ttu-id="97dd1-109">**Description**</span><span class="sxs-lookup"><span data-stu-id="97dd1-109">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="97dd1-110">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="97dd1-110">MailboxCulture</span></span>  <br/> |[<span data-ttu-id="97dd1-111">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="97dd1-111">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="97dd1-112">Identifie la culture RFC3066 à utiliser pour accéder à la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="97dd1-112">Identifies the RFC3066 culture to be used to access the mailbox.</span></span>  <br/> |
|<span data-ttu-id="97dd1-113">RequestVersion</span><span class="sxs-lookup"><span data-stu-id="97dd1-113">RequestVersion</span></span>  <br/> |[<span data-ttu-id="97dd1-114">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="97dd1-114">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="97dd1-115">Identifie la version du schéma pour la requête d’opération.</span><span class="sxs-lookup"><span data-stu-id="97dd1-115">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="97dd1-116">ServerVersion</span><span class="sxs-lookup"><span data-stu-id="97dd1-116">ServerVersion</span></span>  <br/> |[<span data-ttu-id="97dd1-117">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="97dd1-117">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="97dd1-118">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="97dd1-118">Identifies the version of the server that responded to the request.</span></span>  <br/> |
   
## <a name="getservertimezones-request-examples"></a><span data-ttu-id="97dd1-119">Exemples de requêtes GetServerTimeZones</span><span class="sxs-lookup"><span data-stu-id="97dd1-119">GetServerTimeZones request examples</span></span>

### <a name="getting-the-name-and-identifier-of-each-time-zone"></a><span data-ttu-id="97dd1-120">Obtenir le nom et l’identificateur de chaque fuseau horaire</span><span class="sxs-lookup"><span data-stu-id="97dd1-120">Getting the Name and Identifier of Each Time Zone</span></span>

<span data-ttu-id="97dd1-121">L’exemple de code suivant montre comment récupérer le nom et l’identificateur pour le fuseau horaire Pacifique l’heure.</span><span class="sxs-lookup"><span data-stu-id="97dd1-121">The following code example shows how to retrieve the name and identifier for the Eastern Standard Time and Pacific Standard Time time zones.</span></span>
  
### <a name="code"></a><span data-ttu-id="97dd1-122">Code</span><span class="sxs-lookup"><span data-stu-id="97dd1-122">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010"/>
  </soap:Header>
  <soap:Body>
    <m:GetServerTimeZones ReturnFullTimeZoneData="false">
      <m:Ids>
        <t:Id>Eastern Standard Time</Id>
        <t:Id>Pacific Standard Time</Id>
      </m:Ids>
    </m:GetServerTimeZones>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="97dd1-123">Commentaires</span><span class="sxs-lookup"><span data-stu-id="97dd1-123">Comments</span></span>

<span data-ttu-id="97dd1-124">Chaque élément [Id (fuseau horaire)](id-timezone.md) contient l’identificateur d’une définition de fuseau horaire est demandée.</span><span class="sxs-lookup"><span data-stu-id="97dd1-124">Each [Id (TimeZone)](id-timezone.md) element contains the identifier of a time zone definition that is being requested.</span></span> <span data-ttu-id="97dd1-125">Pour obtenir des informations pour tous les fuseaux horaires, omettez l’élément [ID](ids.md) à partir de la demande.</span><span class="sxs-lookup"><span data-stu-id="97dd1-125">To request information for all time zones, omit the [Ids](ids.md) element from the request.</span></span> 
  
### <a name="getting-the-full-definition-of-each-time-zone"></a><span data-ttu-id="97dd1-126">Obtention de la définition complète de chaque fuseau horaire</span><span class="sxs-lookup"><span data-stu-id="97dd1-126">Getting the Full Definition of Each Time Zone</span></span>

<span data-ttu-id="97dd1-127">L’exemple de code suivant montre comment récupérer la définition de la zone à plein temps pour le fuseau horaire de l’heure.</span><span class="sxs-lookup"><span data-stu-id="97dd1-127">The following code example shows how to retrieve the full time zone definition for the Eastern Standard Time time zone.</span></span>
  
### <a name="code"></a><span data-ttu-id="97dd1-128">Code</span><span class="sxs-lookup"><span data-stu-id="97dd1-128">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010"/>
  </soap:Header>
  <soap:Body>
    <m:GetServerTimeZones ReturnFullTimeZoneData="true">
      <m:Ids>
        <t:Id>Eastern Standard Time</Id>
      </m:Ids>
    </m:GetServerTimeZones>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="97dd1-129">Commentaires</span><span class="sxs-lookup"><span data-stu-id="97dd1-129">Comments</span></span>

<span data-ttu-id="97dd1-130">Chaque élément [Id (fuseau horaire)](id-timezone.md) contient l’identificateur d’une définition de fuseau horaire est demandée.</span><span class="sxs-lookup"><span data-stu-id="97dd1-130">Each [Id (TimeZone)](id-timezone.md) element contains the identifier of a time zone definition that is being requested.</span></span> <span data-ttu-id="97dd1-131">Pour obtenir des informations pour tous les fuseaux horaires, omettez l’élément [ID](ids.md) à partir de la demande.</span><span class="sxs-lookup"><span data-stu-id="97dd1-131">To request information for all time zones, omit the [Ids](ids.md) element from the request.</span></span> 
  
## <a name="getservertimezones-response-examples"></a><span data-ttu-id="97dd1-132">Exemples de réponse GetServerTimeZones</span><span class="sxs-lookup"><span data-stu-id="97dd1-132">GetServerTimeZones response examples</span></span>

### <a name="receiving-the-time-zone-name-and-identifier-only"></a><span data-ttu-id="97dd1-133">Reçoit le nom du fuseau horaire et l’identificateur uniquement</span><span class="sxs-lookup"><span data-stu-id="97dd1-133">Receiving the Time Zone Name and Identifier Only</span></span>

<span data-ttu-id="97dd1-134">Une réponse **GetServerTimeZones** l’exemple suivant montre une réponse positive à une demande de **GetServerTimeZones** dans laquelle l’attribut **ReturnFullTimeZoneData** a été défini sur **false**.</span><span class="sxs-lookup"><span data-stu-id="97dd1-134">The following example of a **GetServerTimeZones** response shows a successful response to a **GetServerTimeZones** request in which the **ReturnFullTimeZoneData** attribute was set to **false**.</span></span> <span data-ttu-id="97dd1-135">La réponse contient le nom et l’identificateur pour le fuseau horaire Pacifique l’heure.</span><span class="sxs-lookup"><span data-stu-id="97dd1-135">The response contains the name and identifier for the Eastern Standard Time and Pacific Standard Time time zones.</span></span>
  
### <a name="code"></a><span data-ttu-id="97dd1-136">Code</span><span class="sxs-lookup"><span data-stu-id="97dd1-136">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="0" 
                         MajorBuildNumber="639" 
                         MinorBuildNumber="11" 
                         Version="Exchange2010" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetServerTimeZonesResponse xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                                xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetServerTimeZonesResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</ResponseCode>
          <m:TimeZoneDefinitions>
            <t:TimeZoneDefinition Id="Eastern Standard Time" Name="(GMT-05:00) Eastern Time (US &amp;amp; Canada)" />
            <t:TimeZoneDefinition Id="Pacific Standard Time" Name="(GMT-08:00) Pacific Time (US &amp;amp; Canada)" />
          </m:TimeZoneDefinitions>
        </m:GetServerTimeZonesResponseMessage>
      </m:ResponseMessages>
    </m:GetServerTimeZonesResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="receiving-a-full-time-zone-definition"></a><span data-ttu-id="97dd1-137">Réception d’une définition de fuseau horaire à temps plein</span><span class="sxs-lookup"><span data-stu-id="97dd1-137">Receiving a Full Time Zone Definition</span></span>

<span data-ttu-id="97dd1-138">Une réponse **GetServerTimeZones** l’exemple suivant montre une réponse positive à une demande de **GetServerTimeZones** dans laquelle l’attribut **ReturnFullTimeZoneData** a été défini sur **true**.</span><span class="sxs-lookup"><span data-stu-id="97dd1-138">The following example of a **GetServerTimeZones** response shows a successful response to a **GetServerTimeZones** request in which the **ReturnFullTimeZoneData** attribute was set to **true**.</span></span> <span data-ttu-id="97dd1-139">La réponse contient la définition de la zone à plein temps pour le fuseau horaire de l’heure.</span><span class="sxs-lookup"><span data-stu-id="97dd1-139">The response contains the full time zone definition for the Eastern Standard Time time zone.</span></span>
  
### <a name="code"></a><span data-ttu-id="97dd1-140">Code</span><span class="sxs-lookup"><span data-stu-id="97dd1-140">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="0" 
                         MajorBuildNumber="639" 
                         MinorBuildNumber="11" 
                         Version="Exchange2010" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetServerTimeZonesResponse xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                                xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetServerTimeZonesResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</ResponseCode>
          <m:TimeZoneDefinitions>
            <t:TimeZoneDefinition Id="Eastern Standard Time" Name="(GMT-05:00) Eastern Time (US &amp;amp; Canada)">
              <t:Periods>
                <t:Period Bias="PT5H" Name="Standard" Id="trule:Microsoft/Registry/EasternStandardTime/2006-Standard" />
                <t:Period Bias="PT4H" Name="Daylight" Id="trule:Microsoft/Registry/EasternStandardTime/2006-Daylight" />
                <t:Period Bias="PT5H" Name="Standard" Id="trule:Microsoft/Registry/EasternStandardTime/2007-Standard" />
                <t:Period Bias="PT4H" Name="Daylight" Id="trule:Microsoft/Registry/EasternStandardTime/2007-Daylight" />
              </t:Periods>
              <t:TransitionsGroups>
                <t:TransitionsGroup Id="0">
                  <t:RecurringDayTransition>
                    <t:To Kind="Period">trule:Microsoft/Registry/EasternStandardTime/2006-Daylight</t:To>
                    <t:TimeOffset>PT2H</t:TimeOffset>
                    <t:Month>4</t:Month>
                    <t:DayOfWeek>Sunday</t:DayOfWeek>
                    <t:Occurrence>1</t:Occurrence>
                  </t:RecurringDayTransition>
                  <t:RecurringDayTransition>
                    <t:To Kind="Period">trule:Microsoft/Registry/EasternStandardTime/2006-Standard</t:To>
                    <t:TimeOffset>PT2H</t:TimeOffset>
                    <t:Month>10</t:Month>
                    <t:DayOfWeek>Sunday</t:DayOfWeek>
                    <t:Occurrence>-1</t:Occurrence>
                  </t:RecurringDayTransition>
                </t:TransitionsGroup>
                <t:TransitionsGroup Id="1">
                  <t:RecurringDayTransition>
                    <t:To Kind="Period">trule:Microsoft/Registry/EasternStandardTime/2007-Daylight</t:To>
                    <t:TimeOffset>PT2H</t:TimeOffset>
                    <t:Month>3</t:Month>
                    <t:DayOfWeek>Sunday</t:DayOfWeek>
                    <t:Occurrence>2</t:Occurrence>
                  </t:RecurringDayTransition>
                  <t:RecurringDayTransition>
                    <t:To Kind="Period">trule:Microsoft/Registry/EasternStandardTime/2007-Standard</t:To>
                    <t:TimeOffset>PT2H</t:TimeOffset>
                    <t:Month>11</t:Month>
                    <t:DayOfWeek>Sunday</t:DayOfWeek>
                    <t:Occurrence>1</t:Occurrence>
                  </t:RecurringDayTransition>
                </t:TransitionsGroup>
              </t:TransitionsGroups>
              <t:Transitions>
                <t:Transition>
                  <t:To Kind="Group">0</t:To>
                </t:Transition>
                <t:AbsoluteDateTransition>
                  <t:To Kind="Group">1</t:To>
                  <t:DateTime>2007-01-01T00:00:00</t:DateTime>
                </t:AbsoluteDateTransition>
              </t:Transitions>
            </t:TimeZoneDefinition>
          </m:TimeZoneDefinitions>
        </m:GetServerTimeZonesResponseMessage>
      </m:ResponseMessages>
    </m:GetServerTimeZonesResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="97dd1-141">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="97dd1-141">See also</span></span>



[<span data-ttu-id="97dd1-142">GetServerTimeZones</span><span class="sxs-lookup"><span data-stu-id="97dd1-142">GetServerTimeZones</span></span>](getservertimezones.md)
  
[<span data-ttu-id="97dd1-143">GetServerTimeZonesResponse</span><span class="sxs-lookup"><span data-stu-id="97dd1-143">GetServerTimeZonesResponse</span></span>](getservertimezonesresponse.md)
  
 <span data-ttu-id="97dd1-144">**GetServerTimeZonesType**</span><span class="sxs-lookup"><span data-stu-id="97dd1-144">**GetServerTimeZonesType**</span></span>


[<span data-ttu-id="97dd1-145">Opérations EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="97dd1-145">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
  
- [<span data-ttu-id="97dd1-146">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="97dd1-146">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

