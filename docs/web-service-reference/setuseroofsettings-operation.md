---
title: Opération SetUserOofSettings
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SetUserOofSettings
api_type:
- schema
ms.assetid: 36277ef0-18ee-4b35-9e6e-8c321d8f5433
description: La méthode Web SetUserOofSettings définit les paramètres et les messages d’absence du Bureau d’un utilisateur de boîte aux lettres.
ms.openlocfilehash: 88b5475dd2f0fe6d334bad51a0fe8d0beb767634
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463152"
---
# <a name="setuseroofsettings-operation"></a><span data-ttu-id="ce33d-103">Opération SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="ce33d-103">SetUserOofSettings operation</span></span>

<span data-ttu-id="ce33d-104">La méthode Web **SetUserOofSettings** définit les paramètres et les messages d’absence du Bureau d’un utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="ce33d-104">The **SetUserOofSettings** Web method sets a mailbox user's Out of Office (OOF) settings and message.</span></span> 
  
## <a name="soap-headers"></a><span data-ttu-id="ce33d-105">En-têtes SOAP</span><span class="sxs-lookup"><span data-stu-id="ce33d-105">SOAP Headers</span></span>

<span data-ttu-id="ce33d-106">L’opération **SetUserOofSettings** peut utiliser les en-têtes SOAP répertoriés et décrits dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="ce33d-106">The **SetUserOofSettings** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="ce33d-107">**Header**</span><span class="sxs-lookup"><span data-stu-id="ce33d-107">**Header**</span></span>|<span data-ttu-id="ce33d-108">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ce33d-108">**Element**</span></span>|<span data-ttu-id="ce33d-109">**Description**</span><span class="sxs-lookup"><span data-stu-id="ce33d-109">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="ce33d-110">Emprunt d’identité</span><span class="sxs-lookup"><span data-stu-id="ce33d-110">Impersonation</span></span>  <br/> |[<span data-ttu-id="ce33d-111">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="ce33d-111">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="ce33d-112">Identifie l’utilisateur qui emprunte l’identité de l’application cliente.</span><span class="sxs-lookup"><span data-stu-id="ce33d-112">Identifies the user whom the client application is impersonating.</span></span>  <br/> |
|<span data-ttu-id="ce33d-113">ServerVersion</span><span class="sxs-lookup"><span data-stu-id="ce33d-113">ServerVersion</span></span>  <br/> |[<span data-ttu-id="ce33d-114">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="ce33d-114">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="ce33d-115">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="ce33d-115">Identifies the version of the server that responded to the request.</span></span>  <br/> |
   
## <a name="setuseroofsettings-request-example"></a><span data-ttu-id="ce33d-116">Exemple de requête SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="ce33d-116">SetUserOofSettings request example</span></span>

### <a name="description"></a><span data-ttu-id="ce33d-117">Description</span><span class="sxs-lookup"><span data-stu-id="ce33d-117">Description</span></span>

<span data-ttu-id="ce33d-118">L’exemple de requête **SetUserOofSettings** suivant définit un paramètre OOF sur 10 jours.</span><span class="sxs-lookup"><span data-stu-id="ce33d-118">The following example of a **SetUserOofSettings** request sets an OOF setting for 10 days.</span></span> 
  
### <a name="code"></a><span data-ttu-id="ce33d-119">Code</span><span class="sxs-lookup"><span data-stu-id="ce33d-119">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetUserOofSettingsRequest xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <Mailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
        <Name>User1</Name>
        <Address>user1@example.com</Address>
        <RoutingType>SMTP</RoutingType>
      </Mailbox>
      <UserOofSettings xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
        <OofState>Enabled</OofState>
        <ExternalAudience>All</ExternalAudience>
        <Duration>
          <StartTime>2006-10-05T00:00:00</StartTime>
          <EndTime>2006-10-25T00:00:00</EndTime>
        </Duration>
        <InternalReply>
          <Message>I am out of office.  This is my internal reply.</Message>
        </InternalReply>
        <ExternalReply>
          <Message>I am out of office. This is my external reply.</Message>
        </ExternalReply>
      </UserOofSettings>
    </SetUserOofSettingsRequest>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="ce33d-120">Demander des éléments</span><span class="sxs-lookup"><span data-stu-id="ce33d-120">Request elements</span></span>

<span data-ttu-id="ce33d-121">Les éléments suivants sont utilisés dans la demande :</span><span class="sxs-lookup"><span data-stu-id="ce33d-121">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="ce33d-122">SetUserOofSettingsRequest</span><span class="sxs-lookup"><span data-stu-id="ce33d-122">SetUserOofSettingsRequest</span></span>](setuseroofsettingsrequest.md)
    
- [<span data-ttu-id="ce33d-123">Boîte aux lettres (disponibilité)</span><span class="sxs-lookup"><span data-stu-id="ce33d-123">Mailbox (Availability)</span></span>](mailbox-availability.md)
    
- [<span data-ttu-id="ce33d-124">Nom (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="ce33d-124">Name (EmailAddress)</span></span>](name-emailaddress.md)
    
- [<span data-ttu-id="ce33d-125">Address (chaîne)</span><span class="sxs-lookup"><span data-stu-id="ce33d-125">Address (string)</span></span>](address-string.md)
    
- [<span data-ttu-id="ce33d-126">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="ce33d-126">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md)
    
- [<span data-ttu-id="ce33d-127">UserOofSettings</span><span class="sxs-lookup"><span data-stu-id="ce33d-127">UserOofSettings</span></span>](useroofsettings.md)
    
- [<span data-ttu-id="ce33d-128">OofState</span><span class="sxs-lookup"><span data-stu-id="ce33d-128">OofState</span></span>](oofstate.md)
    
- [<span data-ttu-id="ce33d-129">ExternalAudience</span><span class="sxs-lookup"><span data-stu-id="ce33d-129">ExternalAudience</span></span>](externalaudience.md)
    
- [<span data-ttu-id="ce33d-130">Durée (UserOofSettings)</span><span class="sxs-lookup"><span data-stu-id="ce33d-130">Duration (UserOofSettings)</span></span>](duration-useroofsettings.md)
    
- [<span data-ttu-id="ce33d-131">StartTime</span><span class="sxs-lookup"><span data-stu-id="ce33d-131">StartTime</span></span>](starttime.md)
    
- [<span data-ttu-id="ce33d-132">EndTime</span><span class="sxs-lookup"><span data-stu-id="ce33d-132">EndTime</span></span>](endtime.md)
    
- [<span data-ttu-id="ce33d-133">InternalReply</span><span class="sxs-lookup"><span data-stu-id="ce33d-133">InternalReply</span></span>](internalreply.md)
    
- [<span data-ttu-id="ce33d-134">Message (disponibilité)</span><span class="sxs-lookup"><span data-stu-id="ce33d-134">Message (Availability)</span></span>](message-availability.md)
    
- [<span data-ttu-id="ce33d-135">ExternalReply</span><span class="sxs-lookup"><span data-stu-id="ce33d-135">ExternalReply</span></span>](externalreply.md)
    
## <a name="successful-setuseroofsettings-response-example"></a><span data-ttu-id="ce33d-136">Exemple de réponse SetUserOofSettings réussi</span><span class="sxs-lookup"><span data-stu-id="ce33d-136">Successful SetUserOofSettings response example</span></span>

### <a name="description"></a><span data-ttu-id="ce33d-137">Description</span><span class="sxs-lookup"><span data-stu-id="ce33d-137">Description</span></span>

<span data-ttu-id="ce33d-138">L’exemple suivant montre une réponse réussie à la demande **SetUserOofSettings** .</span><span class="sxs-lookup"><span data-stu-id="ce33d-138">The following example shows a successful response to the **SetUserOofSettings** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="ce33d-139">Code</span><span class="sxs-lookup"><span data-stu-id="ce33d-139">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" /> 
  </soap:Header>
  <soap:Body>
    <SetUserOofSettingsResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseMessage ResponseClass="Success">
        <ResponseCode>NoError</ResponseCode> 
      </ResponseMessage>
    </SetUserOofSettingsResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a><span data-ttu-id="ce33d-140">Éléments de réponse réussis</span><span class="sxs-lookup"><span data-stu-id="ce33d-140">Successful response elements</span></span>

<span data-ttu-id="ce33d-141">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="ce33d-141">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="ce33d-142">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="ce33d-142">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="ce33d-143">SetUserOofSettingsResponse</span><span class="sxs-lookup"><span data-stu-id="ce33d-143">SetUserOofSettingsResponse</span></span>](setuseroofsettingsresponse.md)
    
- [<span data-ttu-id="ce33d-144">ResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ce33d-144">ResponseMessage</span></span>](responsemessage.md)
    
- [<span data-ttu-id="ce33d-145">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="ce33d-145">ResponseCode</span></span>](responsecode.md)
    
## <a name="see-also"></a><span data-ttu-id="ce33d-146">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ce33d-146">See also</span></span>



- [<span data-ttu-id="ce33d-147">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ce33d-147">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

