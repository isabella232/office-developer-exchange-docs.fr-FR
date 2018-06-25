---
title: Opération GetDelegate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetDelegate
api_type:
- schema
ms.assetid: 849b2c9e-4685-4bd1-9adb-aba0fcc52650
description: L’opération GetDelegate récupère les paramètres de délégué pour une boîte aux lettres spécifiée.
ms.openlocfilehash: bd1a0add54ee5fd1c23b4ba09a921a9061afa394
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756568"
---
# <a name="getdelegate-operation"></a><span data-ttu-id="542f4-103">Opération GetDelegate</span><span class="sxs-lookup"><span data-stu-id="542f4-103">GetDelegate operation</span></span>

<span data-ttu-id="542f4-104">L’opération **GetDelegate** récupère les paramètres de délégué pour une boîte aux lettres spécifiée.</span><span class="sxs-lookup"><span data-stu-id="542f4-104">The **GetDelegate** operation retrieves the delegate settings for a specified mailbox.</span></span> 
  
## <a name="soap-headers"></a><span data-ttu-id="542f4-105">En-têtes SOAP</span><span class="sxs-lookup"><span data-stu-id="542f4-105">SOAP Headers</span></span>

<span data-ttu-id="542f4-106">L’opération **GetDelegate** permettre utiliser les en-têtes SOAP qui sont répertoriés et décrits dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="542f4-106">The **GetDelegate** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="542f4-107">**Header**</span><span class="sxs-lookup"><span data-stu-id="542f4-107">**Header**</span></span>|<span data-ttu-id="542f4-108">**Élément**</span><span class="sxs-lookup"><span data-stu-id="542f4-108">**Element**</span></span>|<span data-ttu-id="542f4-109">**Description**</span><span class="sxs-lookup"><span data-stu-id="542f4-109">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="542f4-110">Emprunt d’identité</span><span class="sxs-lookup"><span data-stu-id="542f4-110">Impersonation</span></span>  <br/> |[<span data-ttu-id="542f4-111">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="542f4-111">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="542f4-112">Identifie l’utilisateur emprunte l’identité de l’application cliente.</span><span class="sxs-lookup"><span data-stu-id="542f4-112">Identifies the user whom the client application is impersonating.</span></span>  <br/> |
|<span data-ttu-id="542f4-113">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="542f4-113">MailboxCulture</span></span>  <br/> |[<span data-ttu-id="542f4-114">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="542f4-114">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="542f4-115">Identifie la culture RFC3066 à utiliser pour accéder à la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="542f4-115">Identifies the RFC3066 culture to be used to access the mailbox.</span></span>  <br/> |
|<span data-ttu-id="542f4-116">RequestVersion</span><span class="sxs-lookup"><span data-stu-id="542f4-116">RequestVersion</span></span>  <br/> |[<span data-ttu-id="542f4-117">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="542f4-117">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="542f4-118">Identifie la version du schéma pour la requête d’opération.</span><span class="sxs-lookup"><span data-stu-id="542f4-118">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="542f4-119">ServerVersion</span><span class="sxs-lookup"><span data-stu-id="542f4-119">ServerVersion</span></span>  <br/> |[<span data-ttu-id="542f4-120">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="542f4-120">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="542f4-121">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="542f4-121">Identifies the version of the server that responded to the request.</span></span>  <br/> |
   
## <a name="getdelegate-request-example"></a><span data-ttu-id="542f4-122">Exemple de requête GetDelegate</span><span class="sxs-lookup"><span data-stu-id="542f4-122">GetDelegate request example</span></span>

### <a name="description"></a><span data-ttu-id="542f4-123">Description</span><span class="sxs-lookup"><span data-stu-id="542f4-123">Description</span></span>

<span data-ttu-id="542f4-124">L’exemple de code suivant montre comment récupérer les paramètres de délégué pour tous les délégués sont définies sur les boîtes aux lettres de l’utilisateur 3.</span><span class="sxs-lookup"><span data-stu-id="542f4-124">The following code example shows how to retrieve the delegate settings for all the delegates that are set on user3's mailbox.</span></span> <span data-ttu-id="542f4-125">Toutes les autorisations pour chaque utilisateur sont retournées dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="542f4-125">All the permissions for each user are returned in the response.</span></span>
  
### <a name="code"></a><span data-ttu-id="542f4-126">Code</span><span class="sxs-lookup"><span data-stu-id="542f4-126">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1"/>
  </soap:Header>
  <soap:Body>
    <GetDelegate xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                 xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                 IncludePermissions="true">
      <Mailbox>
        <t:EmailAddress>user3@example.com</t:EmailAddress>
      </Mailbox>
    </GetDelegate>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="542f4-127">Commentaires</span><span class="sxs-lookup"><span data-stu-id="542f4-127">Comments</span></span>

<span data-ttu-id="542f4-128">Vous pouvez utiliser l’élément [UserId](userid.md) pour spécifier des utilisateurs individuels au lieu de retourner tous les utilisateurs qui disposent d’autorisations d’accès délégué sur la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="542f4-128">You can use the [UserId](userid.md) element to specify individual users instead of returning all users who have delegate access permissions on the mailbox.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="542f4-129">Exchange Web Services (EWS) ne gère pas la gestion des délégués de groupe.</span><span class="sxs-lookup"><span data-stu-id="542f4-129">Exchange Web Services (EWS) does not support managing group delegates.</span></span> <span data-ttu-id="542f4-130">EWS renvoie une erreur si l’opération **GetDelegate** est appelée pour une entité de sécurité qui possède un délégué de groupe de sécurité.</span><span class="sxs-lookup"><span data-stu-id="542f4-130">EWS will return an error if the **GetDelegate** operation is called for a principal that has a security group delegate.</span></span> 
  
## <a name="getdelegate-response-example"></a><span data-ttu-id="542f4-131">Exemple de réponse GetDelegate</span><span class="sxs-lookup"><span data-stu-id="542f4-131">GetDelegate response example</span></span>

### <a name="description"></a><span data-ttu-id="542f4-132">Description</span><span class="sxs-lookup"><span data-stu-id="542f4-132">Description</span></span>

<span data-ttu-id="542f4-133">Une réponse **GetDelegate** l’exemple suivant montre une réponse positive à une demande de **GetDelegate** .</span><span class="sxs-lookup"><span data-stu-id="542f4-133">The following example of a **GetDelegate** response shows a successful response to a **GetDelegate** request.</span></span> <span data-ttu-id="542f4-134">La réponse contienne des informations sur les autorisations d’accès délégué, si le délégué peut afficher les éléments privés, si le délégué reçoive des copies de messages de réunion et à qui la réunion demandes ont été remis.</span><span class="sxs-lookup"><span data-stu-id="542f4-134">The response contains information about the delegate access permissions, whether the delegate can view private items, whether the delegate receives copies of meeting messages, and to whom meeting requests were delivered.</span></span> 
  
### <a name="code"></a><span data-ttu-id="542f4-135">Code</span><span class="sxs-lookup"><span data-stu-id="542f4-135">Code</span></span>

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
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <m:GetDelegateResponse xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                           ResponseClass="Success" 
                           xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseCode>NoError</m:ResponseCode>
      <m:ResponseMessages>
        <m:DelegateUserResponseMessageType ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:DelegateUser>
              <t:UserId>
                <t:SID>S-1-5-21-1333220396-2200287332-232816053-1116</t:SID>
                <t:PrimarySmtpAddress>User1@example.com</t:PrimarySmtpAddress>
                <t:DisplayName>User1</t:DisplayName>
              </t:UserId>
              <t:DelegatePermissions>
                <t:CalendarFolderPermissionLevel>Author</t:CalendarFolderPermissionLevel>
                <t:ContactsFolderPermissionLevel>Reviewer</t:ContactsFolderPermissionLevel>
              </t:DelegatePermissions>
              <t:ReceiveCopiesOfMeetingMessages>false</t:ReceiveCopiesOfMeetingMessages>
            <t:ViewPrivateItems>false</t:ViewPrivateItems>
            </m:DelegateUser>
          </m:DelegateUserResponseMessageType>
      </m:ResponseMessages>
      <m:DeliverMeetingRequests>DelegatesAndMe</m:DeliverMeetingRequests>
      </m:GetDelegateResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="542f4-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="542f4-136">See also</span></span>



- [<span data-ttu-id="542f4-137">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="542f4-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

