---
title: Opération GetUserOofSettings
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetUserOofSettings
api_type:
- schema
ms.assetid: 153e4440-495b-4972-9811-2fbea740142a
description: L’opération GetUserOofSettings Obtient les paramètres d’absence du bureau (OOF) et les messages d’un utilisateur de boîte aux lettres.
ms.openlocfilehash: 75a734999842cc33c213e02dc114f23372ae51fd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19827691"
---
# <a name="getuseroofsettings-operation"></a><span data-ttu-id="4f3e2-103">Opération GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="4f3e2-103">GetUserOofSettings operation</span></span>

<span data-ttu-id="4f3e2-104">L’opération **GetUserOofSettings** Obtient les paramètres d’absence du bureau (OOF) et les messages d’un utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="4f3e2-104">The **GetUserOofSettings** operation gets a mailbox user's Out of Office (OOF) settings and messages.</span></span> 
  
## <a name="soap-headers"></a><span data-ttu-id="4f3e2-105">En-têtes SOAP</span><span class="sxs-lookup"><span data-stu-id="4f3e2-105">SOAP Headers</span></span>

<span data-ttu-id="4f3e2-106">L’opération **GetUserOofSettings** permettre utiliser les en-têtes SOAP qui sont répertoriés et décrits dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="4f3e2-106">The **GetUserOofSettings** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="4f3e2-107">**Header**</span><span class="sxs-lookup"><span data-stu-id="4f3e2-107">**Header**</span></span>|<span data-ttu-id="4f3e2-108">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4f3e2-108">**Element**</span></span>|<span data-ttu-id="4f3e2-109">**Description**</span><span class="sxs-lookup"><span data-stu-id="4f3e2-109">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="4f3e2-110">Emprunt d’identité</span><span class="sxs-lookup"><span data-stu-id="4f3e2-110">Impersonation</span></span>  <br/> |[<span data-ttu-id="4f3e2-111">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="4f3e2-111">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="4f3e2-112">Identifie l’utilisateur emprunte l’identité de l’application cliente.</span><span class="sxs-lookup"><span data-stu-id="4f3e2-112">Identifies the user whom the client application is impersonating.</span></span>  <br/> |
|<span data-ttu-id="4f3e2-113">ServerVersion</span><span class="sxs-lookup"><span data-stu-id="4f3e2-113">ServerVersion</span></span>  <br/> |[<span data-ttu-id="4f3e2-114">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="4f3e2-114">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="4f3e2-115">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="4f3e2-115">Identifies the version of the server that responded to the request.</span></span>  <br/> |
   
## <a name="using-the-getuseroofsettings-operation"></a><span data-ttu-id="4f3e2-116">Utilisation de l’opération GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="4f3e2-116">Using the GetUserOofSettings Operation</span></span>

<span data-ttu-id="4f3e2-117">L’opération **GetUserOofSettings** permet d’accéder aux paramètres d’absence du bureau d’un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="4f3e2-117">The **GetUserOofSettings** operation provides access to a user's OOF settings.</span></span> <span data-ttu-id="4f3e2-118">Un utilisateur est identifié par l’adresse de messagerie de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="4f3e2-118">A user is identified by the user's email address.</span></span> <span data-ttu-id="4f3e2-119">Si le message d’absence du bureau est null et absence du bureau est n’activé, aucun message d’absence du bureau est envoyé.</span><span class="sxs-lookup"><span data-stu-id="4f3e2-119">If the OOF message is null and OOF is enabled, no OOF message is sent.</span></span> 
  
> [!IMPORTANT]
> <span data-ttu-id="4f3e2-120">Si les messages d’absence du bureau sont définis par MicrosoftOfficeOutlook, cette opération renverra les messages d’absence du bureau au format HTML.</span><span class="sxs-lookup"><span data-stu-id="4f3e2-120">If the OOF messages are set by MicrosoftOfficeOutlook, this operation will return the OOF messages in HTML format.</span></span> 
  
## <a name="getuseroofsettings-request-example"></a><span data-ttu-id="4f3e2-121">Exemple de requête GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="4f3e2-121">GetUserOofSettings request example</span></span>

### <a name="description"></a><span data-ttu-id="4f3e2-122">Description</span><span class="sxs-lookup"><span data-stu-id="4f3e2-122">Description</span></span>

<span data-ttu-id="4f3e2-123">L’exemple suivant montre une demande **GetUserOofSettings** qui obtient des informations d’absence du bureau d’un utilisateur unique.</span><span class="sxs-lookup"><span data-stu-id="4f3e2-123">The following example shows a **GetUserOofSettings** request that gets a single user's OOF information.</span></span> 
  
### <a name="code"></a><span data-ttu-id="4f3e2-124">Code</span><span class="sxs-lookup"><span data-stu-id="4f3e2-124">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <GetUserOofSettingsRequest xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <Mailbox xmlns ="http://schemas.microsoft.com/exchange/services/2006/types">
        <Address>User1@example.com</Address>
      </Mailbox>
    </GetUserOofSettingsRequest>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="4f3e2-125">Éléments de la demande</span><span class="sxs-lookup"><span data-stu-id="4f3e2-125">Request elements</span></span>

<span data-ttu-id="4f3e2-126">Les éléments suivants sont utilisés dans la demande :</span><span class="sxs-lookup"><span data-stu-id="4f3e2-126">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="4f3e2-127">GetUserOofSettingsRequest</span><span class="sxs-lookup"><span data-stu-id="4f3e2-127">GetUserOofSettingsRequest</span></span>](getuseroofsettingsrequest.md)
    
- [<span data-ttu-id="4f3e2-128">Boîte aux lettres (disponibilité)</span><span class="sxs-lookup"><span data-stu-id="4f3e2-128">Mailbox (Availability)</span></span>](mailbox-availability.md)
    
- [<span data-ttu-id="4f3e2-129">Adresse (chaîne)</span><span class="sxs-lookup"><span data-stu-id="4f3e2-129">Address (string)</span></span>](address-string.md)
    
## <a name="successful-getuseroofsettings-response-example"></a><span data-ttu-id="4f3e2-130">Exemple de réponse GetUserOofSettings réussie</span><span class="sxs-lookup"><span data-stu-id="4f3e2-130">Successful GetUserOofSettings response example</span></span>

### <a name="description"></a><span data-ttu-id="4f3e2-131">Description</span><span class="sxs-lookup"><span data-stu-id="4f3e2-131">Description</span></span>

<span data-ttu-id="4f3e2-132">L’exemple suivant montre un état d’absence du bureau désactivé avec les messages d’absence du bureau.</span><span class="sxs-lookup"><span data-stu-id="4f3e2-132">The following example shows a disabled OOF state with the OOF messages.</span></span>
  
### <a name="code"></a><span data-ttu-id="4f3e2-133">Code</span><span class="sxs-lookup"><span data-stu-id="4f3e2-133">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetUserOofSettingsResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseMessage ResponseClass="Success">
        <ResponseCode>NoError</ResponseCode>
      </ResponseMessage>
      <OofSettings xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
        <OofState>Disabled</OofState>
        <ExternalAudience>All</ExternalAudience>
        <Duration>
          <StartTime>2006-11-03T23:00:00</StartTime>
          <EndTime>2006-11-04T23:00:00</EndTime>
        </Duration>
        <InternalReply>
          <Message>I am out of office. This is my internal reply.</Message>
        </InternalReply>
        <ExternalReply>
          <Message>I am out of office. This is my external reply.</Message>
        </ExternalReply>
      </OofSettings>
      <AllowExternalOof>All</AllowExternalOof>
    </GetUserOofSettingsResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-getuseroofsettings-response-elements"></a><span data-ttu-id="4f3e2-134">Éléments de réponse GetUserOofSettings réussies</span><span class="sxs-lookup"><span data-stu-id="4f3e2-134">Successful GetUserOofSettings response elements</span></span>

<span data-ttu-id="4f3e2-135">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="4f3e2-135">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="4f3e2-136">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="4f3e2-136">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="4f3e2-137">GetUserOofSettingsResponse</span><span class="sxs-lookup"><span data-stu-id="4f3e2-137">GetUserOofSettingsResponse</span></span>](getuseroofsettingsresponse.md)
    
- [<span data-ttu-id="4f3e2-138">ResponseMessage</span><span class="sxs-lookup"><span data-stu-id="4f3e2-138">ResponseMessage</span></span>](responsemessage.md)
    
- [<span data-ttu-id="4f3e2-139">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="4f3e2-139">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="4f3e2-140">OofSettings</span><span class="sxs-lookup"><span data-stu-id="4f3e2-140">OofSettings</span></span>](oofsettings.md)
    
- [<span data-ttu-id="4f3e2-141">OofState</span><span class="sxs-lookup"><span data-stu-id="4f3e2-141">OofState</span></span>](oofstate.md)
    
- [<span data-ttu-id="4f3e2-142">ExternalAudience</span><span class="sxs-lookup"><span data-stu-id="4f3e2-142">ExternalAudience</span></span>](externalaudience.md)
    
- [<span data-ttu-id="4f3e2-143">Durée (UserOofSettings)</span><span class="sxs-lookup"><span data-stu-id="4f3e2-143">Duration (UserOofSettings)</span></span>](duration-useroofsettings.md)
    
- [<span data-ttu-id="4f3e2-144">Heure de début</span><span class="sxs-lookup"><span data-stu-id="4f3e2-144">StartTime</span></span>](starttime.md)
    
- [<span data-ttu-id="4f3e2-145">Heure de fin</span><span class="sxs-lookup"><span data-stu-id="4f3e2-145">EndTime</span></span>](endtime.md)
    
- [<span data-ttu-id="4f3e2-146">InternalReply</span><span class="sxs-lookup"><span data-stu-id="4f3e2-146">InternalReply</span></span>](internalreply.md)
    
- [<span data-ttu-id="4f3e2-147">ExternalReply</span><span class="sxs-lookup"><span data-stu-id="4f3e2-147">ExternalReply</span></span>](externalreply.md)
    
- [<span data-ttu-id="4f3e2-148">Message</span><span class="sxs-lookup"><span data-stu-id="4f3e2-148">Message</span></span>](message-ex15websvcsotherref.md)
    
- [<span data-ttu-id="4f3e2-149">AllowExternalOof</span><span class="sxs-lookup"><span data-stu-id="4f3e2-149">AllowExternalOof</span></span>](allowexternaloof.md)
    
## <a name="getuseroofsettings-error-response-example"></a><span data-ttu-id="4f3e2-150">Exemple de réponse d’erreur GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="4f3e2-150">GetUserOofSettings Error response example</span></span>

### <a name="description"></a><span data-ttu-id="4f3e2-151">Description</span><span class="sxs-lookup"><span data-stu-id="4f3e2-151">Description</span></span>

<span data-ttu-id="4f3e2-152">L’exemple suivant montre une réponse d’erreur due à une tentative pour accéder aux informations d’absence du bureau d’un autre utilisateur.</span><span class="sxs-lookup"><span data-stu-id="4f3e2-152">The following example shows an error response caused by an attempt to access another user's OOF information.</span></span>
  
### <a name="code"></a><span data-ttu-id="4f3e2-153">Code</span><span class="sxs-lookup"><span data-stu-id="4f3e2-153">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <soap:Fault>
      <faultcode>soap:Client</faultcode>
      <faultstring>Microsoft.Exchange.Data.Storage.AccessDeniedException: User is not mailbox owner. User = S-1-5-21-3642464542-282065186-3871681729-1155, MailboxGuid = S-1-5-21-3642464542-282065186-3871681729-1156 ---> User is not mailbox owner. </faultstring>
      <faultactor>https://CAS01.example.com/EWS/Exchange.asmx</faultactor>
      <detail>
        <ErrorCode xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">-2146233088</ErrorCode>
      </detail>
    </soap:Fault>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="4f3e2-154">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4f3e2-154">See also</span></span>



- [<span data-ttu-id="4f3e2-155">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="4f3e2-155">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
