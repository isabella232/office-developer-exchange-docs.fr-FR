---
title: Opération de GetInboxRules
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetInboxRules
api_type:
- schema
ms.assetid: b4b2701a-4a23-4acc-8c75-19f7955ad7ae
description: L’opération GetInboxRules utilise les services Web Exchange pour récupérer les règles de boîte de réception dans la boîte aux lettres de l’utilisateur identifié.
ms.openlocfilehash: f4c4c03f55c9f32be4a067024f4387888edd5fe9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457934"
---
# <a name="getinboxrules-operation"></a><span data-ttu-id="6b994-103">Opération de GetInboxRules</span><span class="sxs-lookup"><span data-stu-id="6b994-103">GetInboxRules operation</span></span>

<span data-ttu-id="6b994-104">L’opération **GetInboxRules** utilise les services Web Exchange pour récupérer les règles de boîte de réception dans la boîte aux lettres de l’utilisateur identifié.</span><span class="sxs-lookup"><span data-stu-id="6b994-104">The **GetInboxRules** operation uses Exchange Web Services to retrieve Inbox rules in the identified user's mailbox.</span></span> 
  
## <a name="getinboxrules-request-example"></a><span data-ttu-id="6b994-105">Exemple de requête GetInboxRules</span><span class="sxs-lookup"><span data-stu-id="6b994-105">GetInboxRules request example</span></span>

### <a name="description"></a><span data-ttu-id="6b994-106">Description</span><span class="sxs-lookup"><span data-stu-id="6b994-106">Description</span></span>

<span data-ttu-id="6b994-107">L’exemple suivant montre le code XML de la demande que le client envoie au serveur.</span><span class="sxs-lookup"><span data-stu-id="6b994-107">The following example shows the request XML that the client sends to the server.</span></span> <span data-ttu-id="6b994-108">La requête identifie l’utilisateur dans l’élément [MailboxSmtpAddress](mailboxsmtpaddress.md) .</span><span class="sxs-lookup"><span data-stu-id="6b994-108">The request identifies the user in the [MailboxSmtpAddress](mailboxsmtpaddress.md) element.</span></span> <span data-ttu-id="6b994-109">Toutes les règles de boîte de réception de l’utilisateur identifié doivent être renvoyées dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="6b994-109">All Inbox rules for the identified user are to be returned in the response.</span></span> 
  
### <a name="code"></a><span data-ttu-id="6b994-110">Code</span><span class="sxs-lookup"><span data-stu-id="6b994-110">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
        xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
        xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010_SP1" />
  </soap:Header>
  <soap:Body>
    <m:GetInboxRules>
      <m:MailboxSmtpAddress>User1@Contoso.com</m:MailboxSmtpAddress>
    </m:GetInboxRules>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="6b994-111">Demander des éléments</span><span class="sxs-lookup"><span data-stu-id="6b994-111">Request elements</span></span>

<span data-ttu-id="6b994-112">La demande inclut l’élément facultatif suivant :</span><span class="sxs-lookup"><span data-stu-id="6b994-112">The request includes the following optional element:</span></span>
  
- [<span data-ttu-id="6b994-113">MailboxSmtpAddress</span><span class="sxs-lookup"><span data-stu-id="6b994-113">MailboxSmtpAddress</span></span>](mailboxsmtpaddress.md)
    
## <a name="successful-getinboxrules-response-example"></a><span data-ttu-id="6b994-114">Exemple de réponse GetInboxRules réussi</span><span class="sxs-lookup"><span data-stu-id="6b994-114">Successful GetInboxRules response example</span></span>

### <a name="description"></a><span data-ttu-id="6b994-115">Description</span><span class="sxs-lookup"><span data-stu-id="6b994-115">Description</span></span>

<span data-ttu-id="6b994-116">L’exemple de corps SOAP (Simple Object Access Protocol) suivant montre une réponse réussie à la demande **GetInboxRules** .</span><span class="sxs-lookup"><span data-stu-id="6b994-116">The following Simple Object Access Protocol (SOAP) body example shows a successful response to the **GetInboxRules** request.</span></span> <span data-ttu-id="6b994-117">Dans cet exemple, la réponse inclut une règle.</span><span class="sxs-lookup"><span data-stu-id="6b994-117">In this example, the response includes one rule.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="6b994-118">Les valeurs des attributs **ID** et **ChangeKey** de l’élément [FolderId](folderid.md) ont été raccourcies afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="6b994-118">The values of the **Id** and the **ChangeKey** attributes of the [FolderId](folderid.md) element have been shortened to preserve readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="6b994-119">Code</span><span class="sxs-lookup"><span data-stu-id="6b994-119">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14"
        MinorVersion="1" MajorBuildNumber="139"
        MinorBuildNumber="0"
        Version="Exchange2010_SP1"
        xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
        xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
        xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetInboxRulesResponse ResponseClass="Success"
        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <OutlookRuleBlobExists>true</OutlookRuleBlobExists>
      <InboxRules>
        <Rule xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <RuleId>dCsAAABjzvA=</RuleId>
          <DisplayName>MoveInterestingToJunk</DisplayName>
          <Priority>1</Priority>
          <IsEnabled>true</IsEnabled>
          <Conditions>
            <ContainsSubjectStrings>
              <String>Interesting</String>
            </ContainsSubjectStrings>
          </Conditions>
          <Actions>
            <MoveToFolder>
              <FolderId ChangeKey="AQAAAA==" Id="AAMkAGYzZjZm" />
            </MoveToFolder>
          </Actions>
        </Rule>
      </InboxRules>
    </GetInboxRulesResponse>
  </s:Body>
</s:Envelope>
```

### <a name="response-elements"></a><span data-ttu-id="6b994-120">Éléments Response</span><span class="sxs-lookup"><span data-stu-id="6b994-120">Response elements</span></span>

<span data-ttu-id="6b994-121">Les éléments suivants sont inclus dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="6b994-121">The following elements are included in the response:</span></span>
  
- [<span data-ttu-id="6b994-122">GetInboxRulesResponse</span><span class="sxs-lookup"><span data-stu-id="6b994-122">GetInboxRulesResponse</span></span>](getinboxrulesresponse.md)
    
- [<span data-ttu-id="6b994-123">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="6b994-123">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="6b994-124">OutlookRuleBlobExists</span><span class="sxs-lookup"><span data-stu-id="6b994-124">OutlookRuleBlobExists</span></span>](outlookruleblobexists.md)
    
- [<span data-ttu-id="6b994-125">InboxRules</span><span class="sxs-lookup"><span data-stu-id="6b994-125">InboxRules</span></span>](inboxrules.md)
    
## <a name="see-also"></a><span data-ttu-id="6b994-126">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="6b994-126">See also</span></span>



[<span data-ttu-id="6b994-127">Opération de UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="6b994-127">UpdateInboxRules operation</span></span>](updateinboxrules-operation.md)

