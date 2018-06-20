---
title: Opération GetMailTips
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetMailTips
api_type:
- schema
ms.assetid: 025483ec-a9f3-4735-8a95-d26e30ea7974
description: L’opération GetMailTips Obtient les informations de conseils de messagerie pour la boîte aux lettres spécifiée.
ms.openlocfilehash: 15c21bef90fdc4cbc6cd65512cdc078fcdf31e60
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756670"
---
# <a name="getmailtips-operation"></a><span data-ttu-id="2853d-103">Opération GetMailTips</span><span class="sxs-lookup"><span data-stu-id="2853d-103">GetMailTips operation</span></span>

<span data-ttu-id="2853d-104">L’opération **GetMailTips** Obtient les informations de conseils de messagerie pour la boîte aux lettres spécifiée.</span><span class="sxs-lookup"><span data-stu-id="2853d-104">The **GetMailTips** operation gets the mail tips information for the specified mailbox.</span></span> 
  
## <a name="getmailtips-request-example"></a><span data-ttu-id="2853d-105">Exemple de requête GetMailTips</span><span class="sxs-lookup"><span data-stu-id="2853d-105">GetMailTips request example</span></span>

### <a name="description"></a><span data-ttu-id="2853d-106">Description</span><span class="sxs-lookup"><span data-stu-id="2853d-106">Description</span></span>

<span data-ttu-id="2853d-107">Le client construit la requête XML et l’envoie au serveur.</span><span class="sxs-lookup"><span data-stu-id="2853d-107">The client constructs the request XML and sends it to the server.</span></span> <span data-ttu-id="2853d-108">La demande identifie qui envoie le client en tant que la boîte aux lettres pour récupérer les conseils de messagerie et les conseils de la messagerie sont demandées.</span><span class="sxs-lookup"><span data-stu-id="2853d-108">The request identifies who the client is sending as, the mailbox to retrieve the mail tips for, and what mail tips are requested.</span></span> <span data-ttu-id="2853d-109">Dans cet exemple, le client demande que tous les conseils de messagerie être renvoyés pour la boîte aux lettres sélectionnée.</span><span class="sxs-lookup"><span data-stu-id="2853d-109">In this example, the client requests that all mail tips be returned for the selected mailbox.</span></span>
  
### <a name="code"></a><span data-ttu-id="2853d-110">Code</span><span class="sxs-lookup"><span data-stu-id="2853d-110">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
        xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"> 
  <soap:Header> 
    <t:RequestServerVersion Version="Exchange2010" /> 
  </soap:Header> 
  <soap:Body> 
    <GetMailTips xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"> 
      <SendingAs> 
        <t:EmailAddress> user1@contoso.com </t:EmailAddress> 
        <t:RoutingType>SMTP</t:RoutingType> 
      </SendingAs> 
      <Recipients> 
        <t:Mailbox> 
          <t:EmailAddress> user2@contoso.com </t:EmailAddress> 
          <t:RoutingType>SMTP</t:RoutingType> 
        </t:Mailbox> 
      </Recipients> 
      <MailTipsRequested>All</MailTipsRequested> 
    </GetMailTips> 
  </soap:Body> 
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="2853d-111">Éléments de la demande</span><span class="sxs-lookup"><span data-stu-id="2853d-111">Request elements</span></span>

<span data-ttu-id="2853d-112">Les éléments suivants sont inclus dans la demande :</span><span class="sxs-lookup"><span data-stu-id="2853d-112">The following elements are included in the request:</span></span>
  
- [<span data-ttu-id="2853d-113">GetMailTips</span><span class="sxs-lookup"><span data-stu-id="2853d-113">GetMailTips</span></span>](getmailtips.md)
    
- [<span data-ttu-id="2853d-114">SendingAs</span><span class="sxs-lookup"><span data-stu-id="2853d-114">SendingAs</span></span>](sendingas.md)
    
- [<span data-ttu-id="2853d-115">Destinataires (ArrayOfRecipientsType)</span><span class="sxs-lookup"><span data-stu-id="2853d-115">Recipients (ArrayOfRecipientsType)</span></span>](recipients-arrayofrecipientstype.md)
    
- [<span data-ttu-id="2853d-116">MailTipsRequested</span><span class="sxs-lookup"><span data-stu-id="2853d-116">MailTipsRequested</span></span>](mailtipsrequested.md)
    
## <a name="successful-getmailtips-response-example"></a><span data-ttu-id="2853d-117">Exemple de réponse GetMailTips réussie</span><span class="sxs-lookup"><span data-stu-id="2853d-117">Successful GetMailTips response example</span></span>

### <a name="description"></a><span data-ttu-id="2853d-118">Description</span><span class="sxs-lookup"><span data-stu-id="2853d-118">Description</span></span>

<span data-ttu-id="2853d-119">L’exemple de corps Simple Object Access Protocol (SOAP) suivant montre une réponse positive à la demande **GetMailTips** .</span><span class="sxs-lookup"><span data-stu-id="2853d-119">The following Simple Object Access Protocol (SOAP) body example shows a successful response to the **GetMailTips** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="2853d-120">Code</span><span class="sxs-lookup"><span data-stu-id="2853d-120">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?> 
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/"> 
  <s:Header> 
    <h:ServerVersionInfo MajorVersion="14" MinorVersion="0" MajorBuildNumber="536" MinorBuildNumber="0" Version="Exchange2010" 
xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
xmlns:xsd="http://www.w3.org/2001/XMLSchema"/> 
  </s:Header> 
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema"> 
    <GetMailTipsResponse ResponseClass="Success" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"> 
      <ResponseCode>NoError</ResponseCode> 
      <ResponseMessages> 
        <MailTipsResponseMessageType ResponseClass="Success"> 
        <ResponseCode>NoError</ResponseCode> 
        <m:MailTips xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"> 20 / 29 [MS-OXWMT] — v20100517 Mail Tips Web Service Extensions Copyright © 2010 Microsoft Corporation. Release: Monday, May 17, 2010 
          <t:RecipientAddress xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"> 
          <t:Name/> 
          <t:EmailAddress>user2@contoso.com</t:EmailAddress> 
          <t:RoutingType>SMTP</t:RoutingType> 
          </t:RecipientAddress> 
          <t:PendingMailTips xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/> 
          <t:OutOfOffice xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"> 
            <t:ReplyBody> 
              <t:Message/> 
            </t:ReplyBody> 
          </t:OutOfOffice> 
          <t:MailboxFull xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">false</t:MailboxFull> 
          <t:CustomMailTip xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">Hello World Mailtips</t:CustomMailTip> 
          <t:TotalMemberCount xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">1</t:TotalMemberCount> 
          <t:ExternalMemberCount xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">0</t:ExternalMemberCount> 
          <t:MaxMessageSize xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">10485760</t:MaxMessageSize> 
          <t:DeliveryRestricted xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">false</t:DeliveryRestricted> 
          <t:IsModerated xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">false</t:IsModerated> 
          <t:InvalidRecipient xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">false</t:InvalidRecipient> 
        </m:MailTips> 
        </MailTipsResponseMessageType> 
      </ResponseMessages> 
    </GetMailTipsResponse> 
  </s:Body> 
</s:Envelope>
```

### <a name="response-elements"></a><span data-ttu-id="2853d-121">Éléments de réponse</span><span class="sxs-lookup"><span data-stu-id="2853d-121">Response elements</span></span>

<span data-ttu-id="2853d-122">Les éléments suivants sont inclus dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="2853d-122">The following elements are included in the response:</span></span>
  
- [<span data-ttu-id="2853d-123">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="2853d-123">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="2853d-124">Les infos-courrier</span><span class="sxs-lookup"><span data-stu-id="2853d-124">MailTips</span></span>](mailtips.md)
    
## <a name="see-also"></a><span data-ttu-id="2853d-125">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="2853d-125">See also</span></span>



[<span data-ttu-id="2853d-126">Opérations EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="2853d-126">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
  
- [<span data-ttu-id="2853d-127">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="2853d-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

