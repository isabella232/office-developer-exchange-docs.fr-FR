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
description: L’opération GetMailTips obtient les informations de conseils de messagerie pour la boîte aux lettres spécifiée.
ms.openlocfilehash: 41a4bb99ee7ae4e416ec8a106968bb7869e60345
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458655"
---
# <a name="getmailtips-operation"></a><span data-ttu-id="fe74e-103">Opération GetMailTips</span><span class="sxs-lookup"><span data-stu-id="fe74e-103">GetMailTips operation</span></span>

<span data-ttu-id="fe74e-104">L’opération **GetMailTips** obtient les informations de conseils de messagerie pour la boîte aux lettres spécifiée.</span><span class="sxs-lookup"><span data-stu-id="fe74e-104">The **GetMailTips** operation gets the mail tips information for the specified mailbox.</span></span> 
  
## <a name="getmailtips-request-example"></a><span data-ttu-id="fe74e-105">Exemple de requête GetMailTips</span><span class="sxs-lookup"><span data-stu-id="fe74e-105">GetMailTips request example</span></span>

### <a name="description"></a><span data-ttu-id="fe74e-106">Description</span><span class="sxs-lookup"><span data-stu-id="fe74e-106">Description</span></span>

<span data-ttu-id="fe74e-107">Le client construit le code XML de la demande et l’envoie au serveur.</span><span class="sxs-lookup"><span data-stu-id="fe74e-107">The client constructs the request XML and sends it to the server.</span></span> <span data-ttu-id="fe74e-108">La demande identifie le client sous la forme, la boîte aux lettres pour laquelle vous souhaitez récupérer les conseils de courrier, ainsi que les conseils de messagerie demandés.</span><span class="sxs-lookup"><span data-stu-id="fe74e-108">The request identifies who the client is sending as, the mailbox to retrieve the mail tips for, and what mail tips are requested.</span></span> <span data-ttu-id="fe74e-109">Dans cet exemple, le client demande que tous les conseils de courrier soient renvoyés pour la boîte aux lettres sélectionnée.</span><span class="sxs-lookup"><span data-stu-id="fe74e-109">In this example, the client requests that all mail tips be returned for the selected mailbox.</span></span>
  
### <a name="code"></a><span data-ttu-id="fe74e-110">Code</span><span class="sxs-lookup"><span data-stu-id="fe74e-110">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
        xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"> 
  <soap:Header> 
    <t:RequestServerVersion Version="Exchange2010" /> 
  </soap:Header> 
  <soap:Body> 
    <GetMailTips xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"> 
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

### <a name="request-elements"></a><span data-ttu-id="fe74e-111">Demander des éléments</span><span class="sxs-lookup"><span data-stu-id="fe74e-111">Request elements</span></span>

<span data-ttu-id="fe74e-112">Les éléments suivants sont inclus dans la demande :</span><span class="sxs-lookup"><span data-stu-id="fe74e-112">The following elements are included in the request:</span></span>
  
- [<span data-ttu-id="fe74e-113">GetMailTips</span><span class="sxs-lookup"><span data-stu-id="fe74e-113">GetMailTips</span></span>](getmailtips.md)
    
- [<span data-ttu-id="fe74e-114">Envoyeras</span><span class="sxs-lookup"><span data-stu-id="fe74e-114">SendingAs</span></span>](sendingas.md)
    
- [<span data-ttu-id="fe74e-115">Destinataires (ArrayOfRecipientsType)</span><span class="sxs-lookup"><span data-stu-id="fe74e-115">Recipients (ArrayOfRecipientsType)</span></span>](recipients-arrayofrecipientstype.md)
    
- [<span data-ttu-id="fe74e-116">MailTipsRequested</span><span class="sxs-lookup"><span data-stu-id="fe74e-116">MailTipsRequested</span></span>](mailtipsrequested.md)
    
## <a name="successful-getmailtips-response-example"></a><span data-ttu-id="fe74e-117">Exemple de réponse GetMailTips réussi</span><span class="sxs-lookup"><span data-stu-id="fe74e-117">Successful GetMailTips response example</span></span>

### <a name="description"></a><span data-ttu-id="fe74e-118">Description</span><span class="sxs-lookup"><span data-stu-id="fe74e-118">Description</span></span>

<span data-ttu-id="fe74e-119">L’exemple de corps SOAP (Simple Object Access Protocol) suivant montre une réponse réussie à la demande **GetMailTips** .</span><span class="sxs-lookup"><span data-stu-id="fe74e-119">The following Simple Object Access Protocol (SOAP) body example shows a successful response to the **GetMailTips** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="fe74e-120">Code</span><span class="sxs-lookup"><span data-stu-id="fe74e-120">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?> 
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/"> 
  <s:Header> 
    <h:ServerVersionInfo MajorVersion="14" MinorVersion="0" MajorBuildNumber="536" MinorBuildNumber="0" Version="Exchange2010" 
xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
xmlns:xsd="http://www.w3.org/2001/XMLSchema"/> 
  </s:Header> 
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema"> 
    <GetMailTipsResponse ResponseClass="Success" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"> 
      <ResponseCode>NoError</ResponseCode> 
      <ResponseMessages> 
        <MailTipsResponseMessageType ResponseClass="Success"> 
        <ResponseCode>NoError</ResponseCode> 
        <m:MailTips xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"> 20 / 29 [MS-OXWMT] — v20100517 Mail Tips Web Service Extensions Copyright © 2010 Microsoft Corporation. Release: Monday, May 17, 2010 
          <t:RecipientAddress xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"> 
          <t:Name/> 
          <t:EmailAddress>user2@contoso.com</t:EmailAddress> 
          <t:RoutingType>SMTP</t:RoutingType> 
          </t:RecipientAddress> 
          <t:PendingMailTips xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"/> 
          <t:OutOfOffice xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"> 
            <t:ReplyBody> 
              <t:Message/> 
            </t:ReplyBody> 
          </t:OutOfOffice> 
          <t:MailboxFull xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">false</t:MailboxFull> 
          <t:CustomMailTip xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">Hello World Mailtips</t:CustomMailTip> 
          <t:TotalMemberCount xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">1</t:TotalMemberCount> 
          <t:ExternalMemberCount xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">0</t:ExternalMemberCount> 
          <t:MaxMessageSize xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">10485760</t:MaxMessageSize> 
          <t:DeliveryRestricted xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">false</t:DeliveryRestricted> 
          <t:IsModerated xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">false</t:IsModerated> 
          <t:InvalidRecipient xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">false</t:InvalidRecipient> 
        </m:MailTips> 
        </MailTipsResponseMessageType> 
      </ResponseMessages> 
    </GetMailTipsResponse> 
  </s:Body> 
</s:Envelope>
```

### <a name="response-elements"></a><span data-ttu-id="fe74e-121">Éléments Response</span><span class="sxs-lookup"><span data-stu-id="fe74e-121">Response elements</span></span>

<span data-ttu-id="fe74e-122">Les éléments suivants sont inclus dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="fe74e-122">The following elements are included in the response:</span></span>
  
- [<span data-ttu-id="fe74e-123">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="fe74e-123">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="fe74e-124">Infos-courrier</span><span class="sxs-lookup"><span data-stu-id="fe74e-124">MailTips</span></span>](mailtips.md)
    
## <a name="see-also"></a><span data-ttu-id="fe74e-125">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="fe74e-125">See also</span></span>



[<span data-ttu-id="fe74e-126">Opérations EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="fe74e-126">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
  
- [<span data-ttu-id="fe74e-127">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="fe74e-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

