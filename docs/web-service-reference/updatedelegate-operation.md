---
title: Opération UpdateDelegate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateDelegate
api_type:
- schema
ms.assetid: 03f618ac-ad1a-4772-9b81-c5bb0f12d6ab
description: L’opération UpdateDelegate met à jour déléguer des autorisations de boîte aux lettres d’un utilisateur principal.
ms.openlocfilehash: 9f69d784617d10d8902a260bbf6639703dd33b6d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838853"
---
# <a name="updatedelegate-operation"></a><span data-ttu-id="06106-103">Opération UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="06106-103">UpdateDelegate operation</span></span>

<span data-ttu-id="06106-104">L’opération **UpdateDelegate** met à jour déléguer des autorisations de boîte aux lettres d’un utilisateur principal.</span><span class="sxs-lookup"><span data-stu-id="06106-104">The **UpdateDelegate** operation updates delegate permissions on a principal's mailbox.</span></span> 
  
## <a name="soap-headers"></a><span data-ttu-id="06106-105">En-têtes SOAP</span><span class="sxs-lookup"><span data-stu-id="06106-105">SOAP Headers</span></span>

<span data-ttu-id="06106-106">L’opération **UpdateDelegate** permettre utiliser les en-têtes SOAP qui sont répertoriés et décrits dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="06106-106">The **UpdateDelegate** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="06106-107">**Header**</span><span class="sxs-lookup"><span data-stu-id="06106-107">**Header**</span></span>|<span data-ttu-id="06106-108">**Élément**</span><span class="sxs-lookup"><span data-stu-id="06106-108">**Element**</span></span>|<span data-ttu-id="06106-109">**Description**</span><span class="sxs-lookup"><span data-stu-id="06106-109">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="06106-110">Emprunt d’identité</span><span class="sxs-lookup"><span data-stu-id="06106-110">Impersonation</span></span>  <br/> |[<span data-ttu-id="06106-111">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="06106-111">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="06106-112">Identifie l’utilisateur emprunte l’identité de l’application cliente.</span><span class="sxs-lookup"><span data-stu-id="06106-112">Identifies the user whom the client application is impersonating.</span></span>  <br/> |
|<span data-ttu-id="06106-113">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="06106-113">MailboxCulture</span></span>  <br/> |[<span data-ttu-id="06106-114">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="06106-114">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="06106-115">Identifie la culture RFC3066 à utiliser pour accéder à la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="06106-115">Identifies the RFC3066 culture to be used to access the mailbox.</span></span>  <br/> |
|<span data-ttu-id="06106-116">RequestVersion</span><span class="sxs-lookup"><span data-stu-id="06106-116">RequestVersion</span></span>  <br/> |[<span data-ttu-id="06106-117">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="06106-117">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="06106-118">Identifie la version du schéma pour la requête d’opération.</span><span class="sxs-lookup"><span data-stu-id="06106-118">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="06106-119">ServerVersion</span><span class="sxs-lookup"><span data-stu-id="06106-119">ServerVersion</span></span>  <br/> |[<span data-ttu-id="06106-120">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="06106-120">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="06106-121">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="06106-121">Identifies the version of the server that responded to the request.</span></span>  <br/> |
   
## <a name="updatedelegate-request-example"></a><span data-ttu-id="06106-122">Exemple de requête UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="06106-122">UpdateDelegate request example</span></span>

### <a name="description"></a><span data-ttu-id="06106-123">Description</span><span class="sxs-lookup"><span data-stu-id="06106-123">Description</span></span>

<span data-ttu-id="06106-124">Une demande de **UpdateDelegate** l’exemple suivant montre comment mettre à jour de déléguer des autorisations sur le compte de l’utilisateur1.</span><span class="sxs-lookup"><span data-stu-id="06106-124">The following example of an **UpdateDelegate** request shows you how to update delegate permissions on user1's account.</span></span> <span data-ttu-id="06106-125">User2 est accordé aucune autorisation pour le dossier de tâches de niveau et reçoit l’autorisation Afficher les éléments privés.</span><span class="sxs-lookup"><span data-stu-id="06106-125">User2 is granted the None permission level for the Tasks folder and is granted permission to view private items.</span></span> <span data-ttu-id="06106-126">User3 reçoit les autorisations de relecteur pour le dossier Journal.</span><span class="sxs-lookup"><span data-stu-id="06106-126">User3 is granted Reviewer permissions for the Journal folder.</span></span> <span data-ttu-id="06106-127">Demandes de réunion sont envoyées aux délégués, et des informations sur la demande sont envoyées à User1.</span><span class="sxs-lookup"><span data-stu-id="06106-127">Meeting requests are sent to the delegates, and information about the request is sent to User1.</span></span> 
  
### <a name="code"></a><span data-ttu-id="06106-128">Code</span><span class="sxs-lookup"><span data-stu-id="06106-128">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1"/>
  </soap:Header>
  <soap:Body>
    <UpdateDelegate xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <Mailbox>
        <t:EmailAddress>user1@example.com</t:EmailAddress>
      </Mailbox>
      <DelegateUsers>
        <t:DelegateUser>
          <t:UserId>
            <t:PrimarySmtpAddress>user2@example.com</t:PrimarySmtpAddress>
          </t:UserId>
          <t:DelegatePermissions>
            <t:TasksFolderPermissionLevel>None</t:TasksFolderPermissionLevel>
          </t:DelegatePermissions>
          <t:ViewPrivateItems>true</t:ViewPrivateItems>
        </t:DelegateUser>
        <t:DelegateUser>
          <t:UserId>
            <t:PrimarySmtpAddress>user3@example.com</t:PrimarySmtpAddress>
          </t:UserId>
          <t:DelegatePermissions>
            <t:JournalFolderPermissionLevel>Reviewer</t:JournalFolderPermissionLevel>
          </t:DelegatePermissions>
        </t:DelegateUser>
      </DelegateUsers>
      <DeliverMeetingRequests>DelegatesAndSendInformationToMe</DeliverMeetingRequests>
    </UpdateDelegate>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="06106-129">Commentaires</span><span class="sxs-lookup"><span data-stu-id="06106-129">Comments</span></span>

<span data-ttu-id="06106-130">La demande [UpdateDelegate](updatedelegate.md) ne nécessite pas que les mises à jour être appliquées aux délégués.</span><span class="sxs-lookup"><span data-stu-id="06106-130">The [UpdateDelegate](updatedelegate.md) request does not require that updates be applied to delegates.</span></span> <span data-ttu-id="06106-131">Les clients peuvent modifier uniquement le paramètre **DeliverMeetingMessage** .</span><span class="sxs-lookup"><span data-stu-id="06106-131">Clients can change only the **DeliverMeetingMessage** setting.</span></span> 
  
## <a name="updatedelegate-response-example"></a><span data-ttu-id="06106-132">Exemple de réponse UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="06106-132">UpdateDelegate response example</span></span>

### <a name="description"></a><span data-ttu-id="06106-133">Description</span><span class="sxs-lookup"><span data-stu-id="06106-133">Description</span></span>

<span data-ttu-id="06106-134">L’exemple suivant montre une réponse positive à une opération **UpdateDelegate** .</span><span class="sxs-lookup"><span data-stu-id="06106-134">The following example shows a successful response to an **UpdateDelegate** operation.</span></span> 
  
### <a name="code"></a><span data-ttu-id="06106-135">Code</span><span class="sxs-lookup"><span data-stu-id="06106-135">Code</span></span>

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
    <m:UpdateDelegateResponse xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                              ResponseClass="Success"
                              xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseCode>NoError</m:ResponseCode>
      <m:ResponseMessages>
        <m:DelegateUserResponseMessageType ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:DelegateUser>
            <t:UserId>
              <t:SID>S-1-5-21-1333220396-2200287332-232816053-1117</t:SID>
              <t:PrimarySmtpAddress>User2@example.com</t:PrimarySmtpAddress>
              <t:DisplayName>User2</t:DisplayName>
            </t:UserId>
            <t:ReceiveCopiesOfMeetingMessages>true</t:ReceiveCopiesOfMeetingMessages>
            <t:ViewPrivateItems>true</t:ViewPrivateItems>
          </m:DelegateUser>
        </m:DelegateUserResponseMessageType>
        <m:DelegateUserResponseMessageType ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:DelegateUser>
            <t:UserId>
              <t:SID>S-1-5-21-1333220396-2200287332-232816053-1118</t:SID>
              <t:PrimarySmtpAddress>User3@example.com</t:PrimarySmtpAddress>
              <t:DisplayName>User3</t:DisplayName>
            </t:UserId>
            <t:ReceiveCopiesOfMeetingMessages>true</t:ReceiveCopiesOfMeetingMessages>
            <t:ViewPrivateItems>false</t:ViewPrivateItems>
          </m:DelegateUser>
        </m:DelegateUserResponseMessageType>
      </m:ResponseMessages>
    </m:UpdateDelegateResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="updatedelegate-error-response-example"></a><span data-ttu-id="06106-136">Exemple de réponse d’erreur UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="06106-136">UpdateDelegate Error response example</span></span>

### <a name="description"></a><span data-ttu-id="06106-137">Description</span><span class="sxs-lookup"><span data-stu-id="06106-137">Description</span></span>

<span data-ttu-id="06106-138">L’exemple suivant montre une réponse d’erreur à une demande de **UpdateDelegate** .</span><span class="sxs-lookup"><span data-stu-id="06106-138">The following example shows an error response to an **UpdateDelegate** request.</span></span> <span data-ttu-id="06106-139">L’erreur a été généré, car le délégué n’existe pas dans la liste des délégués du principal.</span><span class="sxs-lookup"><span data-stu-id="06106-139">The error was generated because the delegate does not exist in the principal's delegate list.</span></span> 
  
### <a name="code"></a><span data-ttu-id="06106-140">Code</span><span class="sxs-lookup"><span data-stu-id="06106-140">Code</span></span>

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
    <m:UpdateDelegateResponse xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                              ResponseClass="Success" 
                              xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseCode>NoError</m:ResponseCode>
      <m:ResponseMessages>
        <m:DelegateUserResponseMessageType ResponseClass="Error">
          <m:MessageText>The user is not a delegate for the mailbox.</m:MessageText>
          <m:ResponseCode>ErrorNotDelegate</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:DelegateUserResponseMessageType>
      </m:ResponseMessages>
      </m:UpdateDelegateResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="06106-141">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="06106-141">See also</span></span>



- [<span data-ttu-id="06106-142">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="06106-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

