---
title: Opération GetRooms
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetRooms
api_type:
- schema
ms.assetid: 5501ddc0-3bfa-4da6-8e15-4223ca5499a3
description: L’opération GetRooms Obtient les salles dans la liste de salles spécifié.
ms.openlocfilehash: 3718c476881ae8aa538646464e7c61845d849562
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756734"
---
# <a name="getrooms-operation"></a><span data-ttu-id="2839a-103">Opération GetRooms</span><span class="sxs-lookup"><span data-stu-id="2839a-103">GetRooms operation</span></span>

<span data-ttu-id="2839a-104">L’opération **GetRooms** Obtient les salles dans la liste de salles spécifié.</span><span class="sxs-lookup"><span data-stu-id="2839a-104">The **GetRooms** operation gets the rooms within the specified room list.</span></span> 
  
## <a name="soap-headers"></a><span data-ttu-id="2839a-105">En-têtes SOAP</span><span class="sxs-lookup"><span data-stu-id="2839a-105">SOAP Headers</span></span>

<span data-ttu-id="2839a-106">L’opération **GetRooms** permettre utiliser les en-têtes SOAP qui sont répertoriés et décrits dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="2839a-106">The **GetRooms** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="2839a-107">**Header**</span><span class="sxs-lookup"><span data-stu-id="2839a-107">**Header**</span></span>|<span data-ttu-id="2839a-108">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2839a-108">**Element**</span></span>|<span data-ttu-id="2839a-109">**Description**</span><span class="sxs-lookup"><span data-stu-id="2839a-109">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="2839a-110">Emprunt d’identité</span><span class="sxs-lookup"><span data-stu-id="2839a-110">Impersonation</span></span>  <br/> |[<span data-ttu-id="2839a-111">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="2839a-111">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="2839a-112">Identifie l’utilisateur emprunte l’identité de l’application cliente.</span><span class="sxs-lookup"><span data-stu-id="2839a-112">Identifies the user whom the client application is impersonating.</span></span>  <br/> |
|<span data-ttu-id="2839a-113">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="2839a-113">MailboxCulture</span></span>  <br/> |[<span data-ttu-id="2839a-114">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="2839a-114">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="2839a-115">Identifie la culture RFC3066 à utiliser pour accéder à la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="2839a-115">Identifies the RFC3066 culture to be used to access the mailbox.</span></span>  <br/> |
|<span data-ttu-id="2839a-116">RequestVersion</span><span class="sxs-lookup"><span data-stu-id="2839a-116">RequestVersion</span></span>  <br/> |[<span data-ttu-id="2839a-117">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="2839a-117">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="2839a-118">Identifie la version du schéma pour la requête d’opération.</span><span class="sxs-lookup"><span data-stu-id="2839a-118">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="2839a-119">ServerVersion</span><span class="sxs-lookup"><span data-stu-id="2839a-119">ServerVersion</span></span>  <br/> |[<span data-ttu-id="2839a-120">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="2839a-120">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="2839a-121">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="2839a-121">Identifies the version of the server that responded to the request.</span></span>  <br/> |
   
## <a name="getrooms-request-example"></a><span data-ttu-id="2839a-122">Exemple de requête GetRooms</span><span class="sxs-lookup"><span data-stu-id="2839a-122">GetRooms request example</span></span>

### <a name="description"></a><span data-ttu-id="2839a-123">Description</span><span class="sxs-lookup"><span data-stu-id="2839a-123">Description</span></span>

<span data-ttu-id="2839a-124">Voici un exemple d’une demande **GetRooms** qui obtient les salles qui sont associés à une liste de salles.</span><span class="sxs-lookup"><span data-stu-id="2839a-124">The following is an example of a **GetRooms** request that gets the rooms that are associated with a room list.</span></span> 
  
### <a name="code"></a><span data-ttu-id="2839a-125">Code</span><span class="sxs-lookup"><span data-stu-id="2839a-125">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version ="Exchange2010_SP1"/>
  </soap:Header>
  <soap:Body>
    <m:GetRooms>
      <m:RoomList>
        <t:EmailAddress>RoomList@contoso.com</t:EmailAddress>
      </m:RoomList>
    </m:GetRooms>
  </soap:Body>

```

### <a name="request-elements"></a><span data-ttu-id="2839a-126">Éléments de la demande</span><span class="sxs-lookup"><span data-stu-id="2839a-126">Request elements</span></span>

<span data-ttu-id="2839a-127">Les éléments suivants sont utilisés dans la demande :</span><span class="sxs-lookup"><span data-stu-id="2839a-127">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="2839a-128">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="2839a-128">RequestServerVersion</span></span>](requestserverversion.md)
    
- [<span data-ttu-id="2839a-129">GetRooms</span><span class="sxs-lookup"><span data-stu-id="2839a-129">GetRooms</span></span>](getrooms.md)
    
- [<span data-ttu-id="2839a-130">RoomList</span><span class="sxs-lookup"><span data-stu-id="2839a-130">RoomList</span></span>](roomlist.md)
    
- [<span data-ttu-id="2839a-131">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="2839a-131">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md)
    
## <a name="successful-getrooms-response-example"></a><span data-ttu-id="2839a-132">Exemple de réponse GetRooms réussie</span><span class="sxs-lookup"><span data-stu-id="2839a-132">Successful GetRooms response example</span></span>

### <a name="description"></a><span data-ttu-id="2839a-133">Description</span><span class="sxs-lookup"><span data-stu-id="2839a-133">Description</span></span>

<span data-ttu-id="2839a-134">La réponse suivante montre les informations d’adresse de messagerie pour les salles qui sont associées à la liste de salles.</span><span class="sxs-lookup"><span data-stu-id="2839a-134">The following response shows the email address information for the rooms that are associated with the room list.</span></span>
  
### <a name="code"></a><span data-ttu-id="2839a-135">Code</span><span class="sxs-lookup"><span data-stu-id="2839a-135">Code</span></span>

```xml
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" MinorVersion="1" MajorBuildNumber="164" MinorBuildNumber="0" Version="Exchange2010_SP1" xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" xmlns="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetRoomsResponse ResponseClass="Success" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <m:Rooms xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
        <t:Room xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
          <t:Id>
            <t:Name>Room01</t:Name>
            <t:EmailAddress>Room01@contoso.com</t:EmailAddress>
            <t:RoutingType>SMTP</t:RoutingType>
            <t:MailboxType>Mailbox</t:MailboxType>
          </t:Id>
        </t:Room>
        <t:Room xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
          <t:Id>
            <t:Name>Room02</t:Name>
            <t:EmailAddress>Room02@contoso.com</t:EmailAddress>
            <t:RoutingType>SMTP</t:RoutingType>
            <t:MailboxType>Mailbox</t:MailboxType>
          </t:Id>
        </t:Room>
      </m:Rooms>
    </GetRoomsResponse>
  </s:Body>
</s:Envelope>
```

### <a name="successful-getrooms-response-elements"></a><span data-ttu-id="2839a-136">Éléments de réponse GetRooms réussies</span><span class="sxs-lookup"><span data-stu-id="2839a-136">Successful GetRooms response elements</span></span>

<span data-ttu-id="2839a-137">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="2839a-137">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="2839a-138">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="2839a-138">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="2839a-139">GetRoomsResponse</span><span class="sxs-lookup"><span data-stu-id="2839a-139">GetRoomsResponse</span></span>](getroomsresponse.md)
    
- [<span data-ttu-id="2839a-140">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="2839a-140">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="2839a-141">Salles</span><span class="sxs-lookup"><span data-stu-id="2839a-141">Rooms</span></span>](rooms.md)
    
- [<span data-ttu-id="2839a-142">Salle</span><span class="sxs-lookup"><span data-stu-id="2839a-142">Room</span></span>](room.md)
    
- [<span data-ttu-id="2839a-143">Nom (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="2839a-143">Name (EmailAddress)</span></span>](name-emailaddress.md)
    
- [<span data-ttu-id="2839a-144">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="2839a-144">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md)
    
- [<span data-ttu-id="2839a-145">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="2839a-145">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md)
    
- [<span data-ttu-id="2839a-146">MailboxType</span><span class="sxs-lookup"><span data-stu-id="2839a-146">MailboxType</span></span>](mailboxtype.md)
    
## <a name="getrooms-error-response-example"></a><span data-ttu-id="2839a-147">Exemple de réponse d’erreur GetRooms</span><span class="sxs-lookup"><span data-stu-id="2839a-147">GetRooms Error response example</span></span>

### <a name="description"></a><span data-ttu-id="2839a-148">Description</span><span class="sxs-lookup"><span data-stu-id="2839a-148">Description</span></span>

<span data-ttu-id="2839a-149">L’exemple suivant montre une réponse d’erreur due à une tentative pour obtenir des informations de salle pour une liste de salles qui n’existe pas.</span><span class="sxs-lookup"><span data-stu-id="2839a-149">The following example shows an error response caused by an attempt to get room information for a nonexistent room list.</span></span>
  
### <a name="code"></a><span data-ttu-id="2839a-150">Code</span><span class="sxs-lookup"><span data-stu-id="2839a-150">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" MinorVersion="1" MajorBuildNumber="164" MinorBuildNumber="0" Version="Exchange2010_SP1" xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" xmlns="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetRoomsResponse ResponseClass="Error" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <MessageText>No results were found.</MessageText>
      <ResponseCode>ErrorNameResolutionNoResults</ResponseCode>
      <DescriptiveLinkKey>0</DescriptiveLinkKey>
    </GetRoomsResponse>
  </s:Body>
</s:Envelope>
```

### <a name="getrooms-error-response-elements"></a><span data-ttu-id="2839a-151">Éléments de réponse d’erreur GetRooms</span><span class="sxs-lookup"><span data-stu-id="2839a-151">GetRooms Error response elements</span></span>

<span data-ttu-id="2839a-152">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="2839a-152">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="2839a-153">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="2839a-153">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="2839a-154">GetRoomsResponse</span><span class="sxs-lookup"><span data-stu-id="2839a-154">GetRoomsResponse</span></span>](getroomsresponse.md)
    
- [<span data-ttu-id="2839a-155">MessageText</span><span class="sxs-lookup"><span data-stu-id="2839a-155">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="2839a-156">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="2839a-156">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="2839a-157">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="2839a-157">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="2839a-158">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="2839a-158">See also</span></span>

- [<span data-ttu-id="2839a-159">Opérations EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="2839a-159">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
- [<span data-ttu-id="2839a-160">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="2839a-160">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

