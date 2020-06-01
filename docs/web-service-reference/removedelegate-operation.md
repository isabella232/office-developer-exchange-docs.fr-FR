---
title: Opération RemoveDelegate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RemoveDelegate
api_type:
- schema
ms.assetid: 1d42d5ff-8fde-4f8a-b18d-57b1ef7a946a
description: L’opération RemoveDelegate supprime un ou plusieurs délégués de la boîte aux lettres d’un utilisateur.
ms.openlocfilehash: b2e342225e7e79c44dcd86b76b4b7d47b16b860b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466597"
---
# <a name="removedelegate-operation"></a><span data-ttu-id="6264a-103">Opération RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="6264a-103">RemoveDelegate operation</span></span>

<span data-ttu-id="6264a-104">L’opération **RemoveDelegate** supprime un ou plusieurs délégués de la boîte aux lettres d’un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="6264a-104">The **RemoveDelegate** operation removes one or more delegates from a user's mailbox.</span></span> 
  
## <a name="soap-headers"></a><span data-ttu-id="6264a-105">En-têtes SOAP</span><span class="sxs-lookup"><span data-stu-id="6264a-105">SOAP Headers</span></span>

<span data-ttu-id="6264a-106">L’opération **RemoveDelegate** peut utiliser les en-têtes SOAP répertoriés et décrits dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="6264a-106">The **RemoveDelegate** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="6264a-107">**Header**</span><span class="sxs-lookup"><span data-stu-id="6264a-107">**Header**</span></span>|<span data-ttu-id="6264a-108">**Élément**</span><span class="sxs-lookup"><span data-stu-id="6264a-108">**Element**</span></span>|<span data-ttu-id="6264a-109">**Description**</span><span class="sxs-lookup"><span data-stu-id="6264a-109">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="6264a-110">Emprunt d’identité</span><span class="sxs-lookup"><span data-stu-id="6264a-110">Impersonation</span></span>  <br/> |[<span data-ttu-id="6264a-111">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="6264a-111">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="6264a-112">Identifie l’utilisateur qui emprunte l’identité de l’application cliente.</span><span class="sxs-lookup"><span data-stu-id="6264a-112">Identifies the user whom the client application is impersonating.</span></span>  <br/> |
|<span data-ttu-id="6264a-113">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="6264a-113">MailboxCulture</span></span>  <br/> |[<span data-ttu-id="6264a-114">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="6264a-114">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="6264a-115">Identifie la culture RFC3066 à utiliser pour accéder à la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="6264a-115">Identifies the RFC3066 culture to be used to access the mailbox.</span></span>  <br/> |
|<span data-ttu-id="6264a-116">RequestVersion</span><span class="sxs-lookup"><span data-stu-id="6264a-116">RequestVersion</span></span>  <br/> |[<span data-ttu-id="6264a-117">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="6264a-117">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="6264a-118">Identifie la version de schéma de la demande d’opération.</span><span class="sxs-lookup"><span data-stu-id="6264a-118">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="6264a-119">ServerVersion</span><span class="sxs-lookup"><span data-stu-id="6264a-119">ServerVersion</span></span>  <br/> |[<span data-ttu-id="6264a-120">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="6264a-120">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="6264a-121">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="6264a-121">Identifies the version of the server that responded to the request.</span></span>  <br/> |
   
## <a name="removedelegate-request-example"></a><span data-ttu-id="6264a-122">Exemple de requête RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="6264a-122">RemoveDelegate request example</span></span>

### <a name="description"></a><span data-ttu-id="6264a-123">Description</span><span class="sxs-lookup"><span data-stu-id="6264a-123">Description</span></span>

<span data-ttu-id="6264a-124">L’exemple de code suivant montre comment supprimer deux délégués de la boîte aux lettres utilisateur1.</span><span class="sxs-lookup"><span data-stu-id="6264a-124">The following code example shows how to remove two delegates from user1's mailbox.</span></span> <span data-ttu-id="6264a-125">Dans cet exemple, un délégué est supprimé à l’aide de l’adresse SMTP principale du délégué, et l’autre est supprimé à l’aide de l’identificateur de sécurité (SID) du délégué.</span><span class="sxs-lookup"><span data-stu-id="6264a-125">In this example, one delegate is removed by using the delegate's primary SMTP address, and the other one is removed by using the delegate's security identifier (SID).</span></span>
  
### <a name="code"></a><span data-ttu-id="6264a-126">Code</span><span class="sxs-lookup"><span data-stu-id="6264a-126">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1"/>
  </soap:Header>
  <soap:Body>
    <RemoveDelegate xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <Mailbox>
        <t:EmailAddress>user1@example.com</t:EmailAddress>
      </Mailbox>
      <UserIds>
        <t:UserId>
          <t:PrimarySmtpAddress>user2@example.com</t:PrimarySmtpAddress>
        </t:UserId>
        <t:UserId>
          <t:SID>S-1-5-21-1333220396-2200287332-232816053-1118</t:SID>
        </t:UserId>
      </UserIds>
    </RemoveDelegate>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="6264a-127">Commentaires</span><span class="sxs-lookup"><span data-stu-id="6264a-127">Comments</span></span>

<span data-ttu-id="6264a-128">L’opération **RemoveDelegate** ne nécessite pas que l’utilisateur délégué spécifié dispose d’une boîte aux lettres ou qu’elle existe dans le service d’annuaire Active Directory.</span><span class="sxs-lookup"><span data-stu-id="6264a-128">The **RemoveDelegate** operation does not require the specified delegate user to have a mailbox or to exist in the Active Directory directory service.</span></span> <span data-ttu-id="6264a-129">L’opération **RemoveDelegate** réussit si l’entrée de délégué est orpheline.</span><span class="sxs-lookup"><span data-stu-id="6264a-129">The **RemoveDelegate** operation will succeed if the delegate entry is orphaned.</span></span> 
  
## <a name="removedelegate-response-example"></a><span data-ttu-id="6264a-130">Exemple de réponse RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="6264a-130">RemoveDelegate response example</span></span>

### <a name="description"></a><span data-ttu-id="6264a-131">Description</span><span class="sxs-lookup"><span data-stu-id="6264a-131">Description</span></span>

<span data-ttu-id="6264a-132">L’exemple suivant de réponse **RemoveDelegate** indique une réponse réussie à une demande **RemoveDelegate** .</span><span class="sxs-lookup"><span data-stu-id="6264a-132">The following example of a **RemoveDelegate** response shows a successful response to a **RemoveDelegate** request.</span></span> <span data-ttu-id="6264a-133">La réponse contient un élément **DelegateUserResponseMessageType** pour chaque délégué qui est supprimé de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="6264a-133">The response contains a **DelegateUserResponseMessageType** element for each delegate that is removed from the mailbox.</span></span> 
  
### <a name="code"></a><span data-ttu-id="6264a-134">Code</span><span class="sxs-lookup"><span data-stu-id="6264a-134">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" 
                         MinorVersion="1" 
                         MajorBuildNumber="206" 
                         MinorBuildNumber="0" 
                         Version="Exchange2007_SP1" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <m:RemoveDelegateResponse xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                              ResponseClass="Success" 
                              xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseCode>NoError</m:ResponseCode>
      <m:ResponseMessages>
        <m:DelegateUserResponseMessageType ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:DelegateUserResponseMessageType>
        <m:DelegateUserResponseMessageType ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:DelegateUserResponseMessageType>
      </m:ResponseMessages>
      </m:RemoveDelegateResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="removedelegate-error-response-example"></a><span data-ttu-id="6264a-135">Exemple de réponse d’erreur RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="6264a-135">RemoveDelegate Error response example</span></span>

### <a name="description"></a><span data-ttu-id="6264a-136">Description</span><span class="sxs-lookup"><span data-stu-id="6264a-136">Description</span></span>

<span data-ttu-id="6264a-137">L’exemple suivant de réponse d’erreur **RemoveDelegate** indique les résultats d’une demande de suppression d’un délégué qui n’existe pas.</span><span class="sxs-lookup"><span data-stu-id="6264a-137">The following example of a **RemoveDelegate** error response shows the results of a request to remove a delegate that does not exist.</span></span> 
  
### <a name="code"></a><span data-ttu-id="6264a-138">Code</span><span class="sxs-lookup"><span data-stu-id="6264a-138">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8"
                         MinorVersion="1"
                         MajorBuildNumber="206"
                         MinorBuildNumber="0"
                         Version="Exchange2007_SP1"
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <m:RemoveDelegateResponse xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
                              ResponseClass="Success"
                              xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseCode>NoError</m:ResponseCode>
      <m:ResponseMessages>
        <m:DelegateUserResponseMessageType ResponseClass="Error">
          <m:MessageText>The user is not a delegate for the mailbox.</m:MessageText>
          <m:ResponseCode>ErrorNotDelegate</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:DelegateUserResponseMessageType>
      </m:ResponseMessages>
    </m:RemoveDelegateResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="6264a-139">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="6264a-139">See also</span></span>



- [<span data-ttu-id="6264a-140">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="6264a-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

