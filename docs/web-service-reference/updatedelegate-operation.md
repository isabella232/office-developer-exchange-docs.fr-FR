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
description: L’opération UpdateDelegate met à jour les autorisations déléguées sur la boîte aux lettres d’un principal.
ms.openlocfilehash: b7cf5325d925f8d6588115a8657a2077e940f9d2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/01/2020
ms.locfileid: "44468557"
---
# <a name="updatedelegate-operation"></a><span data-ttu-id="8f0a0-103">Opération UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="8f0a0-103">UpdateDelegate operation</span></span>

<span data-ttu-id="8f0a0-104">L’opération **UpdateDelegate** met à jour les autorisations déléguées sur la boîte aux lettres d’un principal.</span><span class="sxs-lookup"><span data-stu-id="8f0a0-104">The **UpdateDelegate** operation updates delegate permissions on a principal's mailbox.</span></span> 
  
## <a name="soap-headers"></a><span data-ttu-id="8f0a0-105">En-têtes SOAP</span><span class="sxs-lookup"><span data-stu-id="8f0a0-105">SOAP Headers</span></span>

<span data-ttu-id="8f0a0-106">L’opération **UpdateDelegate** peut utiliser les en-têtes SOAP répertoriés et décrits dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="8f0a0-106">The **UpdateDelegate** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="8f0a0-107">**Header**</span><span class="sxs-lookup"><span data-stu-id="8f0a0-107">**Header**</span></span>|<span data-ttu-id="8f0a0-108">**Élément**</span><span class="sxs-lookup"><span data-stu-id="8f0a0-108">**Element**</span></span>|<span data-ttu-id="8f0a0-109">**Description**</span><span class="sxs-lookup"><span data-stu-id="8f0a0-109">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="8f0a0-110">Emprunt d’identité</span><span class="sxs-lookup"><span data-stu-id="8f0a0-110">Impersonation</span></span>  <br/> |[<span data-ttu-id="8f0a0-111">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="8f0a0-111">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="8f0a0-112">Identifie l’utilisateur qui emprunte l’identité de l’application cliente.</span><span class="sxs-lookup"><span data-stu-id="8f0a0-112">Identifies the user whom the client application is impersonating.</span></span>  <br/> |
|<span data-ttu-id="8f0a0-113">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="8f0a0-113">MailboxCulture</span></span>  <br/> |[<span data-ttu-id="8f0a0-114">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="8f0a0-114">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="8f0a0-115">Identifie la culture RFC3066 à utiliser pour accéder à la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="8f0a0-115">Identifies the RFC3066 culture to be used to access the mailbox.</span></span>  <br/> |
|<span data-ttu-id="8f0a0-116">RequestVersion</span><span class="sxs-lookup"><span data-stu-id="8f0a0-116">RequestVersion</span></span>  <br/> |[<span data-ttu-id="8f0a0-117">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="8f0a0-117">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="8f0a0-118">Identifie la version de schéma de la demande d’opération.</span><span class="sxs-lookup"><span data-stu-id="8f0a0-118">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="8f0a0-119">ServerVersion</span><span class="sxs-lookup"><span data-stu-id="8f0a0-119">ServerVersion</span></span>  <br/> |[<span data-ttu-id="8f0a0-120">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="8f0a0-120">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="8f0a0-121">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="8f0a0-121">Identifies the version of the server that responded to the request.</span></span>  <br/> |
   
## <a name="updatedelegate-request-example"></a><span data-ttu-id="8f0a0-122">Exemple de requête UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="8f0a0-122">UpdateDelegate request example</span></span>

### <a name="description"></a><span data-ttu-id="8f0a0-123">Description</span><span class="sxs-lookup"><span data-stu-id="8f0a0-123">Description</span></span>

<span data-ttu-id="8f0a0-124">L’exemple de requête **UpdateDelegate** suivant montre comment mettre à jour les autorisations déléguées sur un compte utilisateur1.</span><span class="sxs-lookup"><span data-stu-id="8f0a0-124">The following example of an **UpdateDelegate** request shows you how to update delegate permissions on user1's account.</span></span> <span data-ttu-id="8f0a0-125">Utilisateur2 reçoit le niveau d’autorisation None pour le dossier tâches et dispose de l’autorisation d’afficher des éléments privés.</span><span class="sxs-lookup"><span data-stu-id="8f0a0-125">User2 is granted the None permission level for the Tasks folder and is granted permission to view private items.</span></span> <span data-ttu-id="8f0a0-126">L’util_3 dispose des autorisations de relecteur pour le dossier journal.</span><span class="sxs-lookup"><span data-stu-id="8f0a0-126">User3 is granted Reviewer permissions for the Journal folder.</span></span> <span data-ttu-id="8f0a0-127">Les demandes de réunion sont envoyées aux délégués, et les informations sur la demande sont envoyées à utilisateur1.</span><span class="sxs-lookup"><span data-stu-id="8f0a0-127">Meeting requests are sent to the delegates, and information about the request is sent to User1.</span></span> 
  
### <a name="code"></a><span data-ttu-id="8f0a0-128">Code</span><span class="sxs-lookup"><span data-stu-id="8f0a0-128">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1"/>
  </soap:Header>
  <soap:Body>
    <UpdateDelegate xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

### <a name="comments"></a><span data-ttu-id="8f0a0-129">Commentaires</span><span class="sxs-lookup"><span data-stu-id="8f0a0-129">Comments</span></span>

<span data-ttu-id="8f0a0-130">La requête [UpdateDelegate](updatedelegate.md) n’exige pas que les mises à jour soient appliquées aux délégués.</span><span class="sxs-lookup"><span data-stu-id="8f0a0-130">The [UpdateDelegate](updatedelegate.md) request does not require that updates be applied to delegates.</span></span> <span data-ttu-id="8f0a0-131">Les clients peuvent modifier uniquement le paramètre **DeliverMeetingMessage** .</span><span class="sxs-lookup"><span data-stu-id="8f0a0-131">Clients can change only the **DeliverMeetingMessage** setting.</span></span> 
  
## <a name="updatedelegate-response-example"></a><span data-ttu-id="8f0a0-132">Exemple de réponse UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="8f0a0-132">UpdateDelegate response example</span></span>

### <a name="description"></a><span data-ttu-id="8f0a0-133">Description</span><span class="sxs-lookup"><span data-stu-id="8f0a0-133">Description</span></span>

<span data-ttu-id="8f0a0-134">L’exemple suivant montre une réponse réussie à une opération **UpdateDelegate** .</span><span class="sxs-lookup"><span data-stu-id="8f0a0-134">The following example shows a successful response to an **UpdateDelegate** operation.</span></span> 
  
### <a name="code"></a><span data-ttu-id="8f0a0-135">Code</span><span class="sxs-lookup"><span data-stu-id="8f0a0-135">Code</span></span>

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
    <m:UpdateDelegateResponse xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
                              ResponseClass="Success"
                              xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

## <a name="updatedelegate-error-response-example"></a><span data-ttu-id="8f0a0-136">Exemple de réponse d’erreur UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="8f0a0-136">UpdateDelegate Error response example</span></span>

### <a name="description"></a><span data-ttu-id="8f0a0-137">Description</span><span class="sxs-lookup"><span data-stu-id="8f0a0-137">Description</span></span>

<span data-ttu-id="8f0a0-138">L’exemple suivant montre une réponse d’erreur à une demande **UpdateDelegate** .</span><span class="sxs-lookup"><span data-stu-id="8f0a0-138">The following example shows an error response to an **UpdateDelegate** request.</span></span> <span data-ttu-id="8f0a0-139">L’erreur a été générée car le délégué n’existe pas dans la liste des délégués de l’entité de sécurité.</span><span class="sxs-lookup"><span data-stu-id="8f0a0-139">The error was generated because the delegate does not exist in the principal's delegate list.</span></span> 
  
### <a name="code"></a><span data-ttu-id="8f0a0-140">Code</span><span class="sxs-lookup"><span data-stu-id="8f0a0-140">Code</span></span>

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
    <m:UpdateDelegateResponse xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
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
      </m:UpdateDelegateResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="8f0a0-141">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="8f0a0-141">See also</span></span>



- [<span data-ttu-id="8f0a0-142">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="8f0a0-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

