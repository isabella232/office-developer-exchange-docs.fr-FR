---
title: Opération GetRoomLists
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetRoomLists
api_type:
- schema
ms.assetid: 55d451f9-547f-44ac-872e-9cb220ea7b7c
description: L’opération GetRoomLists Obtient les listes d’espace qui sont disponibles dans l’organisation Exchange.
ms.openlocfilehash: 139a669bfc6b7c4bc9bd9c07f9f9cf52954860c0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756730"
---
# <a name="getroomlists-operation"></a><span data-ttu-id="267ce-103">Opération GetRoomLists</span><span class="sxs-lookup"><span data-stu-id="267ce-103">GetRoomLists operation</span></span>

<span data-ttu-id="267ce-104">L’opération **GetRoomLists** Obtient les listes d’espace qui sont disponibles dans l’organisation Exchange.</span><span class="sxs-lookup"><span data-stu-id="267ce-104">The **GetRoomLists** operation gets the room lists that are available within the Exchange organization.</span></span> 
  
## <a name="soap-headers"></a><span data-ttu-id="267ce-105">En-têtes SOAP</span><span class="sxs-lookup"><span data-stu-id="267ce-105">SOAP Headers</span></span>

<span data-ttu-id="267ce-106">L’opération **GetRoomLists** permettre utiliser les en-têtes SOAP qui sont répertoriés et décrits dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="267ce-106">The **GetRoomLists** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="267ce-107">**Header**</span><span class="sxs-lookup"><span data-stu-id="267ce-107">**Header**</span></span>|<span data-ttu-id="267ce-108">**Élément**</span><span class="sxs-lookup"><span data-stu-id="267ce-108">**Element**</span></span>|<span data-ttu-id="267ce-109">**Description**</span><span class="sxs-lookup"><span data-stu-id="267ce-109">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="267ce-110">Emprunt d’identité</span><span class="sxs-lookup"><span data-stu-id="267ce-110">Impersonation</span></span>  <br/> |[<span data-ttu-id="267ce-111">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="267ce-111">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="267ce-112">Identifie l’utilisateur emprunte l’identité de l’application cliente.</span><span class="sxs-lookup"><span data-stu-id="267ce-112">Identifies the user whom the client application is impersonating.</span></span>  <br/> |
|<span data-ttu-id="267ce-113">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="267ce-113">MailboxCulture</span></span>  <br/> |[<span data-ttu-id="267ce-114">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="267ce-114">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="267ce-115">Identifie la culture RFC3066 à utiliser pour accéder à la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="267ce-115">Identifies the RFC3066 culture to be used to access the mailbox.</span></span>  <br/> |
|<span data-ttu-id="267ce-116">RequestVersion</span><span class="sxs-lookup"><span data-stu-id="267ce-116">RequestVersion</span></span>  <br/> |[<span data-ttu-id="267ce-117">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="267ce-117">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="267ce-118">Identifie la version du schéma pour la requête d’opération.</span><span class="sxs-lookup"><span data-stu-id="267ce-118">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="267ce-119">ServerVersion</span><span class="sxs-lookup"><span data-stu-id="267ce-119">ServerVersion</span></span>  <br/> |[<span data-ttu-id="267ce-120">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="267ce-120">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="267ce-121">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="267ce-121">Identifies the version of the server that responded to the request.</span></span>  <br/> |
   
## <a name="getroomlists-request-example"></a><span data-ttu-id="267ce-122">Exemple de requête GetRoomLists</span><span class="sxs-lookup"><span data-stu-id="267ce-122">GetRoomLists request example</span></span>

### <a name="description"></a><span data-ttu-id="267ce-123">Description</span><span class="sxs-lookup"><span data-stu-id="267ce-123">Description</span></span>

<span data-ttu-id="267ce-124">Voici un exemple d’une demande **GetRoomLists** qui renvoie les listes de salle sont disponibles sur le serveur.</span><span class="sxs-lookup"><span data-stu-id="267ce-124">The following is an example of a **GetRoomLists** request that returns the room lists that are available on the server.</span></span> 
  
### <a name="code"></a><span data-ttu-id="267ce-125">Code</span><span class="sxs-lookup"><span data-stu-id="267ce-125">Code</span></span>

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
    <m:GetRoomLists />
  </soap:Body>
</soap:Envelope>

```

### <a name="request-elements"></a><span data-ttu-id="267ce-126">Éléments de la demande</span><span class="sxs-lookup"><span data-stu-id="267ce-126">Request elements</span></span>

<span data-ttu-id="267ce-127">L’élément suivant est utilisé dans la demande :</span><span class="sxs-lookup"><span data-stu-id="267ce-127">The following element is used in the request:</span></span>
  
- [<span data-ttu-id="267ce-128">GetRoomLists</span><span class="sxs-lookup"><span data-stu-id="267ce-128">GetRoomLists</span></span>](getroomlists.md)
    
## <a name="successful-getroomlists-response-example"></a><span data-ttu-id="267ce-129">Exemple de réponse GetRoomLists réussie</span><span class="sxs-lookup"><span data-stu-id="267ce-129">Successful GetRoomLists response example</span></span>

### <a name="description"></a><span data-ttu-id="267ce-130">Description</span><span class="sxs-lookup"><span data-stu-id="267ce-130">Description</span></span>

<span data-ttu-id="267ce-131">Voici un exemple d’une réponse à une demande de **GetRoomLists** .</span><span class="sxs-lookup"><span data-stu-id="267ce-131">The following is an example of a response to a **GetRoomLists** request.</span></span> <span data-ttu-id="267ce-132">Cette réponse affiche une liste de salles sur le serveur.</span><span class="sxs-lookup"><span data-stu-id="267ce-132">This response shows one room list on the server.</span></span> 
  
### <a name="code"></a><span data-ttu-id="267ce-133">Code</span><span class="sxs-lookup"><span data-stu-id="267ce-133">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" MinorVersion="1" MajorBuildNumber="164" MinorBuildNumber="0" Version="Exchange2010_SP1" xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" xmlns="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetRoomListsResponse ResponseClass="Success" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <m:RoomLists xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
        <t:Address xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
          <t:Name>Room List</t:Name>
          <t:EmailAddress>RoomList@contoso.com</t:EmailAddress>
          <t:RoutingType>SMTP</t:RoutingType>
          <t:MailboxType>PublicDL</t:MailboxType>
        </t:Address>
      </m:RoomLists>
    </GetRoomListsResponse>
  </s:Body>
</s:Envelope>

```

### <a name="successful-getroomlists-response-elements"></a><span data-ttu-id="267ce-134">Éléments de réponse GetRoomLists réussies</span><span class="sxs-lookup"><span data-stu-id="267ce-134">Successful GetRoomLists response elements</span></span>

<span data-ttu-id="267ce-135">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="267ce-135">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="267ce-136">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="267ce-136">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="267ce-137">GetRoomListsResponse</span><span class="sxs-lookup"><span data-stu-id="267ce-137">GetRoomListsResponse</span></span>](getroomlistsresponse.md)
    
- [<span data-ttu-id="267ce-138">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="267ce-138">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="267ce-139">RoomLists</span><span class="sxs-lookup"><span data-stu-id="267ce-139">RoomLists</span></span>](roomlists.md)
    
- [<span data-ttu-id="267ce-140">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="267ce-140">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md)
    
- [<span data-ttu-id="267ce-141">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="267ce-141">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md)
    
- [<span data-ttu-id="267ce-142">MailboxType</span><span class="sxs-lookup"><span data-stu-id="267ce-142">MailboxType</span></span>](mailboxtype.md)
    
### <a name="getroomlists-error-response-example"></a><span data-ttu-id="267ce-143">Exemple de réponse d’erreur GetRoomLists</span><span class="sxs-lookup"><span data-stu-id="267ce-143">GetRoomLists Error response example</span></span>

#### <a name="description"></a><span data-ttu-id="267ce-144">Description</span><span class="sxs-lookup"><span data-stu-id="267ce-144">Description</span></span>

<span data-ttu-id="267ce-145">L’exemple suivant montre la réponse à la tentative d’obtention des listes d’espace d’un serveur qui ne dispose pas des listes de salle définis.</span><span class="sxs-lookup"><span data-stu-id="267ce-145">The following example shows the response to an attempt to get room lists from a server that does not have any room lists defined.</span></span>
  
#### <a name="code"></a><span data-ttu-id="267ce-146">Code</span><span class="sxs-lookup"><span data-stu-id="267ce-146">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" MinorVersion="1" MajorBuildNumber="164" MinorBuildNumber="0" Version="Exchange2010_SP1" xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" xmlns="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetRoomListsResponse ResponseClass="Success" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <m:RoomLists xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"/>
    </GetRoomListsResponse>
  </s:Body>
</s:Envelope>

```

#### <a name="getroomlists-error-response-elements"></a><span data-ttu-id="267ce-147">Éléments de réponse d’erreur GetRoomLists</span><span class="sxs-lookup"><span data-stu-id="267ce-147">GetRoomLists Error response elements</span></span>

<span data-ttu-id="267ce-148">Les éléments suivants sont utilisés dans la réponse d'erreur :</span><span class="sxs-lookup"><span data-stu-id="267ce-148">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="267ce-149">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="267ce-149">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="267ce-150">GetRoomListsResponse</span><span class="sxs-lookup"><span data-stu-id="267ce-150">GetRoomListsResponse</span></span>](getroomlistsresponse.md)
    
- [<span data-ttu-id="267ce-151">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="267ce-151">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="267ce-152">RoomLists</span><span class="sxs-lookup"><span data-stu-id="267ce-152">RoomLists</span></span>](roomlists.md)
    
## <a name="see-also"></a><span data-ttu-id="267ce-153">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="267ce-153">See also</span></span>



[<span data-ttu-id="267ce-154">Opérations EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="267ce-154">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
  
- [<span data-ttu-id="267ce-155">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="267ce-155">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

