---
title: Opération AddDelegate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AddDelegate
api_type:
- schema
ms.assetid: 012d8cc5-648c-4ba0-a155-15c422b1e994
description: L’opération AddDelegate ajoute un ou plusieurs délégués à la boîte aux lettres d’un principal et définit des autorisations d’accès spécifiques.
ms.openlocfilehash: 80adbe71d69be1025dc9593c6a9002bc68fdcb76
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466513"
---
# <a name="adddelegate-operation"></a><span data-ttu-id="beca9-103">Opération AddDelegate</span><span class="sxs-lookup"><span data-stu-id="beca9-103">AddDelegate operation</span></span>

<span data-ttu-id="beca9-104">L’opération **AddDelegate** ajoute un ou plusieurs délégués à la boîte aux lettres d’un principal et définit des autorisations d’accès spécifiques.</span><span class="sxs-lookup"><span data-stu-id="beca9-104">The **AddDelegate** operation adds one or more delegates to a principal's mailbox and sets specific access permissions.</span></span> 
  
## <a name="soap-headers"></a><span data-ttu-id="beca9-105">En-têtes SOAP</span><span class="sxs-lookup"><span data-stu-id="beca9-105">SOAP headers</span></span>

<span data-ttu-id="beca9-106">L’opération **AddDelegate** peut utiliser les en-têtes SOAP répertoriés et décrits dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="beca9-106">The **AddDelegate** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="beca9-107">**Header**</span><span class="sxs-lookup"><span data-stu-id="beca9-107">**Header**</span></span>|<span data-ttu-id="beca9-108">**Élément**</span><span class="sxs-lookup"><span data-stu-id="beca9-108">**Element**</span></span>|<span data-ttu-id="beca9-109">**Description**</span><span class="sxs-lookup"><span data-stu-id="beca9-109">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="beca9-110">Emprunt d’identité</span><span class="sxs-lookup"><span data-stu-id="beca9-110">Impersonation</span></span>  <br/> |[<span data-ttu-id="beca9-111">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="beca9-111">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="beca9-112">Identifie l’utilisateur qui emprunte l’identité de l’application cliente.</span><span class="sxs-lookup"><span data-stu-id="beca9-112">Identifies the user whom the client application is impersonating.</span></span>  <br/> |
|<span data-ttu-id="beca9-113">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="beca9-113">MailboxCulture</span></span>  <br/> |[<span data-ttu-id="beca9-114">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="beca9-114">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="beca9-115">Identifie la culture RFC3066 à utiliser pour accéder à la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="beca9-115">Identifies the RFC3066 culture to be used to access the mailbox.</span></span>  <br/> |
|<span data-ttu-id="beca9-116">RequestVersion</span><span class="sxs-lookup"><span data-stu-id="beca9-116">RequestVersion</span></span>  <br/> |[<span data-ttu-id="beca9-117">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="beca9-117">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="beca9-118">Identifie la version de schéma de la demande d’opération.</span><span class="sxs-lookup"><span data-stu-id="beca9-118">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="beca9-119">ServerVersion</span><span class="sxs-lookup"><span data-stu-id="beca9-119">ServerVersion</span></span>  <br/> |[<span data-ttu-id="beca9-120">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="beca9-120">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="beca9-121">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="beca9-121">Identifies the version of the server that responded to the request.</span></span>  <br/> |
   
## <a name="adddelegate-request-example"></a><span data-ttu-id="beca9-122">Exemple de requête AddDelegate</span><span class="sxs-lookup"><span data-stu-id="beca9-122">AddDelegate request example</span></span>

### <a name="description"></a><span data-ttu-id="beca9-123">Description</span><span class="sxs-lookup"><span data-stu-id="beca9-123">Description</span></span>

<span data-ttu-id="beca9-124">L’exemple de requête **AddDelegate** suivant montre une tentative d’octroi d’autorisations déléguées à user1 sur les dossiers appartenant à l’utilisateur 2.</span><span class="sxs-lookup"><span data-stu-id="beca9-124">The following example of an **AddDelegate** request shows an attempt to give user1 delegate permissions on folders that are owned by user2.</span></span> <span data-ttu-id="beca9-125">Utilisateur1 dispose d’autorisations au niveau de l’auteur pour user2's les autorisations de dossier de calendrier et de relecteur sur user2's dossier de contacts.</span><span class="sxs-lookup"><span data-stu-id="beca9-125">User1 is given Author-level permissions to user2's Calendar folder and Reviewer-level permissions to user2's Contacts folder.</span></span> <span data-ttu-id="beca9-126">Utilisateur1 ne reçoit pas de copies des messages de réunion et ne sera pas en mesure d’afficher les éléments privés dans la boîte aux lettres user2's.</span><span class="sxs-lookup"><span data-stu-id="beca9-126">User1 will not receive copies of meeting messages and will be unable to view private items in user2's mailbox.</span></span> <span data-ttu-id="beca9-127">Les demandes de réunion seront envoyées à User1 et à utilisateur2.</span><span class="sxs-lookup"><span data-stu-id="beca9-127">Meeting requests will be sent to both user1 and user2.</span></span> 
  
### <a name="code"></a><span data-ttu-id="beca9-128">Code</span><span class="sxs-lookup"><span data-stu-id="beca9-128">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1"/>
  </soap:Header>
  <soap:Body xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
    <AddDelegate>
      <Mailbox>
        <t:EmailAddress>user2@example.com</t:EmailAddress>
      </Mailbox>
      <DelegateUsers>
        <t:DelegateUser>
          <t:UserId>
            <t:PrimarySmtpAddress>user1@example.com</t:PrimarySmtpAddress>
          </t:UserId>
          <t:DelegatePermissions>
            <t:CalendarFolderPermissionLevel>Author</t:CalendarFolderPermissionLevel>
            <t:ContactsFolderPermissionLevel>Reviewer</t:ContactsFolderPermissionLevel>
          </t:DelegatePermissions>
          <t:ReceiveCopiesOfMeetingMessages>false</t:ReceiveCopiesOfMeetingMessages>
          <t:ViewPrivateItems>false</t:ViewPrivateItems>
        </t:DelegateUser>
      </DelegateUsers>
      <DeliverMeetingRequests>DelegatesAndMe</DeliverMeetingRequests>
    </AddDelegate>
  </soap:Body>
</soap:Envelope>
```

## <a name="adddelegate-response-example"></a><span data-ttu-id="beca9-129">Exemple de réponse AddDelegate</span><span class="sxs-lookup"><span data-stu-id="beca9-129">AddDelegate response example</span></span>

### <a name="description"></a><span data-ttu-id="beca9-130">Description</span><span class="sxs-lookup"><span data-stu-id="beca9-130">Description</span></span>

<span data-ttu-id="beca9-131">L’exemple suivant de réponse **AddDelegate** indique une réponse réussie à une demande **AddDelegate** .</span><span class="sxs-lookup"><span data-stu-id="beca9-131">The following example of an **AddDelegate** response shows a successful response to an **AddDelegate** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="beca9-132">Code</span><span class="sxs-lookup"><span data-stu-id="beca9-132">Code</span></span>

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
    <m:AddDelegateResponse xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                           ResponseClass="Success" 
                           xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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
              <t:ReceiveCopiesOfMeetingMessages>false</t:ReceiveCopiesOfMeetingMessages>
            <t:ViewPrivateItems>false</t:ViewPrivateItems>
            </m:DelegateUser>
        </m:DelegateUserResponseMessageType>
      </m:ResponseMessages>
    </m:AddDelegateResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="adddelegate-error-response-example"></a><span data-ttu-id="beca9-133">Exemple de réponse d’erreur AddDelegate</span><span class="sxs-lookup"><span data-stu-id="beca9-133">AddDelegate error response example</span></span>

### <a name="description"></a><span data-ttu-id="beca9-134">Description</span><span class="sxs-lookup"><span data-stu-id="beca9-134">Description</span></span>

<span data-ttu-id="beca9-135">L’exemple suivant illustre la réponse à une demande d’ajout d’un délégué qui a déjà été ajouté à la boîte aux lettres de l’entité.</span><span class="sxs-lookup"><span data-stu-id="beca9-135">The following example shows the response to a request to add a delegate who has already been added to the principal's mailbox.</span></span>
  
### <a name="code"></a><span data-ttu-id="beca9-136">Code</span><span class="sxs-lookup"><span data-stu-id="beca9-136">Code</span></span>

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
    <m:AddDelegateResponse xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
                           ResponseClass="Success"
                           xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseCode>NoError</m:ResponseCode>
      <m:ResponseMessages>
        <m:DelegateUserResponseMessageType ResponseClass="Error">
          <m:MessageText>The user is already a delegate for the mailbox.</m:MessageText>
          <m:ResponseCode>ErrorDelegateAlreadyExists</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:DelegateUserResponseMessageType>
      </m:ResponseMessages>
      </m:AddDelegateResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="beca9-137">Commentaires</span><span class="sxs-lookup"><span data-stu-id="beca9-137">Comments</span></span>

<span data-ttu-id="beca9-138">Si le code de réponse ErrorDelegateAlreadyExists est renvoyé lorsque vous essayez d’ajouter un délégué, utilisez l' [opération GetDelegate](getdelegate-operation.md) pour obtenir toutes les autorisations actuelles pour le délégué, puis utilisez l' [opération UpdateDelegate](updatedelegate-operation.md) pour définir les nouvelles autorisations.</span><span class="sxs-lookup"><span data-stu-id="beca9-138">If the ErrorDelegateAlreadyExists response code is returned when you try to add a delegate, use the [GetDelegate operation](getdelegate-operation.md) to get all the current permissions for the delegate, and then use the [UpdateDelegate operation](updatedelegate-operation.md) to set the new permissions.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="beca9-139">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="beca9-139">See also</span></span>

- [<span data-ttu-id="beca9-140">Ajout de délégués</span><span class="sxs-lookup"><span data-stu-id="beca9-140">Adding Delegates</span></span>](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

