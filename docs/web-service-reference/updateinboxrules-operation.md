---
title: Opération de UpdateInboxRules
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateInboxRules
api_type:
- schema
ms.assetid: f982a237-471e-45c5-a2b5-468cfc53150b
description: L’opération UpdateInboxRules met à jour les règles de boîte de réception de l’utilisateur authentifié en appliquant les opérations spécifiées. UpdateInboxRules permet de créer une règle de boîte de réception, de définir une règle de boîte de réception ou de supprimer une règle de boîte de réception.
ms.openlocfilehash: a6ced4be25c6fe4649ad649ba01194791548bf67
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530999"
---
# <a name="updateinboxrules-operation"></a><span data-ttu-id="5179b-104">Opération de UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="5179b-104">UpdateInboxRules operation</span></span>

<span data-ttu-id="5179b-105">L’opération UpdateInboxRules met à jour les règles de boîte de réception de l’utilisateur authentifié en appliquant les opérations spécifiées.</span><span class="sxs-lookup"><span data-stu-id="5179b-105">The UpdateInboxRules operation updates the authenticated user's Inbox rules by applying the specified operations.</span></span> <span data-ttu-id="5179b-106">**UpdateInboxRules** permet de créer une règle de boîte de réception, de définir une règle de boîte de réception ou de supprimer une règle de boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="5179b-106">**UpdateInboxRules** is used to create an Inbox rule, to set an Inbox rule, or to delete an Inbox rule.</span></span> 
  
<span data-ttu-id="5179b-107">Lorsque vous utilisez l’opération **UpdateInboxRules** , les services Web Exchange suppriment les règles d’envoi côté client.</span><span class="sxs-lookup"><span data-stu-id="5179b-107">When you use the **UpdateInboxRules** operation, Exchange Web Services deletes client-side send rules.</span></span> <span data-ttu-id="5179b-108">Les règles d’envoi côté client sont stockées sur le client dans le message du dossier de la règle (FAI) et nulle part ailleurs.</span><span class="sxs-lookup"><span data-stu-id="5179b-108">Client-side send rules are stored on the client in the rule Folder Associated Information (FAI) Message and nowhere else.</span></span> <span data-ttu-id="5179b-109">EWS supprime cette règle par défaut, en fonction de la prévision qu’Outlook va recréer.</span><span class="sxs-lookup"><span data-stu-id="5179b-109">EWS deletes this rule FAI message by default, based on the expectation that Outlook will recreate it.</span></span> <span data-ttu-id="5179b-110">Toutefois, Outlook ne peut pas recréer des règles qui n’existent pas également en tant que règle étendue, et les règles d’envoi côté client n’existent pas en tant que règles étendues.</span><span class="sxs-lookup"><span data-stu-id="5179b-110">However, Outlook can't recreate rules that don't also exist as an extended rule, and client-side send rules don't exist as extended rules.</span></span> <span data-ttu-id="5179b-111">Par conséquent, ces règles sont perdues.</span><span class="sxs-lookup"><span data-stu-id="5179b-111">As a result, these rules are lost.</span></span> <span data-ttu-id="5179b-112">Nous vous suggérons de vous en prendre en compte lors de la conception de votre solution.</span><span class="sxs-lookup"><span data-stu-id="5179b-112">We suggest you consider this when designing your solution.</span></span> 
  
## <a name="updateinboxrules-create-rule-request-example"></a><span data-ttu-id="5179b-113">Exemple de requête UpdateInboxRules (Create Rule)</span><span class="sxs-lookup"><span data-stu-id="5179b-113">UpdateInboxRules (Create Rule) request example</span></span>

<span data-ttu-id="5179b-114">Vous pouvez utiliser les services Web Exchange pour créer une règle de boîte de réception dans la boîte aux lettres d’un utilisateur dans la Banque d’aide Exchange.</span><span class="sxs-lookup"><span data-stu-id="5179b-114">You can use Exchange Web Services to create an Inbox rule in a user's mailbox in the Exchange store.</span></span> <span data-ttu-id="5179b-115">Utilisez l’élément [UpdateInboxRules](updateinboxrules.md) en association avec l’élément [CreateRuleOperation](createruleoperation.md) pour créer une règle.</span><span class="sxs-lookup"><span data-stu-id="5179b-115">Use the [UpdateInboxRules](updateinboxrules.md) element in conjunction with the [CreateRuleOperation](createruleoperation.md) element to create a rule.</span></span> 
  
### <a name="description"></a><span data-ttu-id="5179b-116">Description</span><span class="sxs-lookup"><span data-stu-id="5179b-116">Description</span></span>

<span data-ttu-id="5179b-117">Le client construit le code XML de la demande et l’envoie au serveur.</span><span class="sxs-lookup"><span data-stu-id="5179b-117">The client constructs the request XML and sends it to the server.</span></span>
  
### <a name="code"></a><span data-ttu-id="5179b-118">Code</span><span class="sxs-lookup"><span data-stu-id="5179b-118">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version ="Exchange2010_SP1"/>
  </soap:Header>
  <soap:Body>
      <m:UpdateInboxRules>
        <m:RemoveOutlookRuleBlob>true</m:RemoveOutlookRuleBlob>
        <m:Operations>
          <t:CreateRuleOperation>
            <t:Rule>
              <t:DisplayName>MoveInterestingToJunk</t:DisplayName>
              <t:Priority>1</t:Priority>
              <t:IsEnabled>true</t:IsEnabled>
              <t:Conditions>
                <t:ContainsSubjectStrings>
                  <t:String>Interesting</t:String>
                </t:ContainsSubjectStrings>
              </t:Conditions>
              <t:Exceptions />
              <t:Actions>
                <t:MoveToFolder>
                  <t:DistinguishedFolderId Id="junkemail" />
                </t:MoveToFolder>
              </t:Actions>
            </t:Rule>
          </t:CreateRuleOperation>
        </m:Operations>
      </m:UpdateInboxRules>
  </soap:Body>
</soap:Envelope>

```

### <a name="comments"></a><span data-ttu-id="5179b-119">Commentaires</span><span class="sxs-lookup"><span data-stu-id="5179b-119">Comments</span></span>

<span data-ttu-id="5179b-120">Cet exemple illustre la création d’une règle qui déplace un message électronique vers le dossier courrier indésirable si l’objet de l’e-mail contient une chaîne égale à « intéressante ».</span><span class="sxs-lookup"><span data-stu-id="5179b-120">This example builds a rule that will move an e-mail message to the Junk E-mail folder if the e-mail subject contains a string that equals "Interesting".</span></span>
  
### <a name="request-elements"></a><span data-ttu-id="5179b-121">Demander des éléments</span><span class="sxs-lookup"><span data-stu-id="5179b-121">Request elements</span></span>

<span data-ttu-id="5179b-122">La requête **UpdateInboxRules** inclut les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="5179b-122">The **UpdateInboxRules** request includes the following elements:</span></span> 
  
- [<span data-ttu-id="5179b-123">MailboxSmtpAddress</span><span class="sxs-lookup"><span data-stu-id="5179b-123">MailboxSmtpAddress</span></span>](mailboxsmtpaddress.md)
    
- [<span data-ttu-id="5179b-124">RemoveOutlookRuleBlob</span><span class="sxs-lookup"><span data-stu-id="5179b-124">RemoveOutlookRuleBlob</span></span>](removeoutlookruleblob.md)
    
- [<span data-ttu-id="5179b-125">Operations</span><span class="sxs-lookup"><span data-stu-id="5179b-125">Operations</span></span>](operations.md)
    
<span data-ttu-id="5179b-126">L’élément [Operations](operations.md) contient l’élément [CreateRuleOperation](createruleoperation.md) pour créer une règle.</span><span class="sxs-lookup"><span data-stu-id="5179b-126">The [Operations](operations.md) element contains the [CreateRuleOperation](createruleoperation.md) element to create a rule.</span></span> 
  
## <a name="updateinboxrules-create-rule-response-example"></a><span data-ttu-id="5179b-127">Exemple de réponse UpdateInboxRules (Create Rule)</span><span class="sxs-lookup"><span data-stu-id="5179b-127">UpdateInboxRules (Create Rule) response example</span></span>

### <a name="description"></a><span data-ttu-id="5179b-128">Description</span><span class="sxs-lookup"><span data-stu-id="5179b-128">Description</span></span>

<span data-ttu-id="5179b-129">L’exemple de corps SOAP (Simple Object Access Protocol) suivant montre une réponse réussie à la demande **UpdateInboxRules** qui crée une règle.</span><span class="sxs-lookup"><span data-stu-id="5179b-129">The following Simple Object Access Protocol (SOAP) body example shows a successful response to the **UpdateInboxRules** request that creates a rule.</span></span> 
  
### <a name="code"></a><span data-ttu-id="5179b-130">Code</span><span class="sxs-lookup"><span data-stu-id="5179b-130">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
        MinorVersion="1" 
        MajorBuildNumber="139" 
        MinorBuildNumber="0" Version="Exchange2010_SP1" 
        xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <UpdateInboxRulesResponse 
         ResponseClass="Success" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
    </UpdateInboxRulesResponse>
  </s:Body>
</s:Envelope>

```

### <a name="successful-response-elements"></a><span data-ttu-id="5179b-131">Éléments de réponse réussis</span><span class="sxs-lookup"><span data-stu-id="5179b-131">Successful response elements</span></span>

<span data-ttu-id="5179b-132">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="5179b-132">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="5179b-133">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="5179b-133">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="5179b-134">UpdateInboxRulesResponse</span><span class="sxs-lookup"><span data-stu-id="5179b-134">UpdateInboxRulesResponse</span></span>](updateinboxrulesresponse.md)
    
- [<span data-ttu-id="5179b-135">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="5179b-135">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="5179b-136">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="5179b-136">ResponseCode</span></span>](responsecode.md)
    
## <a name="updateinboxrules-set-rule-request-example"></a><span data-ttu-id="5179b-137">Exemple de requête UpdateInboxRules (Set Rule)</span><span class="sxs-lookup"><span data-stu-id="5179b-137">UpdateInboxRules (Set Rule) request example</span></span>

<span data-ttu-id="5179b-138">Vous pouvez utiliser les services Web Exchange pour modifier une règle de boîte de réception dans la boîte aux lettres d’un utilisateur dans la Banque d’aide Exchange.</span><span class="sxs-lookup"><span data-stu-id="5179b-138">You can use Exchange Web Services to modify an Inbox rule in a user's mailbox in the Exchange store.</span></span> <span data-ttu-id="5179b-139">Utilisez l’élément [UpdateInboxRules](updateinboxrules.md) en association avec l’élément [SetRuleOperation](setruleoperation.md) pour modifier une règle.</span><span class="sxs-lookup"><span data-stu-id="5179b-139">Use the [UpdateInboxRules](updateinboxrules.md) element in conjunction with the [SetRuleOperation](setruleoperation.md) element to modify a rule.</span></span> 
  
### <a name="description"></a><span data-ttu-id="5179b-140">Description</span><span class="sxs-lookup"><span data-stu-id="5179b-140">Description</span></span>

<span data-ttu-id="5179b-141">Le client construit le code XML de la demande et l’envoie au serveur.</span><span class="sxs-lookup"><span data-stu-id="5179b-141">The client constructs the request XML and sends it to the server.</span></span>
  
### <a name="code"></a><span data-ttu-id="5179b-142">Code</span><span class="sxs-lookup"><span data-stu-id="5179b-142">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version ="Exchange2010_SP1"/>
  </soap:Header>
  <soap:Body>
      <m:UpdateInboxRules>
        <m:RemoveOutlookRuleBlob>true</m:RemoveOutlookRuleBlob>
        <Operations xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
          <SetRuleOperation xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
            <Rule>
              <RuleId>Nh8AAAAwW/w=</RuleId>
              <DisplayName>(Modified) This is Junk</DisplayName>
              <Priority>1</Priority>
              <IsEnabled>true</IsEnabled>
              <Conditions>
                <ContainsSubjectStrings>
                  <String>Interesting</String>
                </ContainsSubjectStrings>
              </Conditions>
              <Actions>
                <MoveToFolder>
                  <FolderId Id="AAMkADQ1YTE1" ChangeKey="AQAAAA==" />
                </MoveToFolder>
              </Actions>
            </Rule>
          </SetRuleOperation>
        </Operations>
      </m:UpdateInboxRules>
  </soap:Body>
</soap:Envelope>

```

### <a name="comments"></a><span data-ttu-id="5179b-143">Commentaires</span><span class="sxs-lookup"><span data-stu-id="5179b-143">Comments</span></span>

<span data-ttu-id="5179b-144">Cet exemple montre comment modifier le nom complet en « (modifié) This is junk ».</span><span class="sxs-lookup"><span data-stu-id="5179b-144">This example changes the display name to "(Modified) This is Junk".</span></span>
  
> [!NOTE]
> <span data-ttu-id="5179b-145">Les valeurs des attributs **ID** et **ChangeKey** de l’élément [FolderId](folderid.md) ont été raccourcies pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="5179b-145">The values of the **Id** and **ChangeKey** attributes of the [FolderId](folderid.md) element have been shortened for readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="5179b-146">Demander des éléments</span><span class="sxs-lookup"><span data-stu-id="5179b-146">Request elements</span></span>

<span data-ttu-id="5179b-147">La requête **UpdateInboxRules** inclut les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="5179b-147">The **UpdateInboxRules** request includes the following elements:</span></span> 
  
- [<span data-ttu-id="5179b-148">MailboxSmtpAddress</span><span class="sxs-lookup"><span data-stu-id="5179b-148">MailboxSmtpAddress</span></span>](mailboxsmtpaddress.md)
    
- [<span data-ttu-id="5179b-149">RemoveOutlookRuleBlob</span><span class="sxs-lookup"><span data-stu-id="5179b-149">RemoveOutlookRuleBlob</span></span>](removeoutlookruleblob.md)
    
- [<span data-ttu-id="5179b-150">Operations</span><span class="sxs-lookup"><span data-stu-id="5179b-150">Operations</span></span>](operations.md)
    
<span data-ttu-id="5179b-151">L’élément [Operations](operations.md) contient l’élément [SetRuleOperation](setruleoperation.md) pour modifier une règle.</span><span class="sxs-lookup"><span data-stu-id="5179b-151">The [Operations](operations.md) element contains the [SetRuleOperation](setruleoperation.md) element to modify a rule.</span></span> 
  
## <a name="updateinboxrules-set-rule-response-example"></a><span data-ttu-id="5179b-152">Exemple de réponse UpdateInboxRules (Set Rule)</span><span class="sxs-lookup"><span data-stu-id="5179b-152">UpdateInboxRules (Set Rule) response example</span></span>

### <a name="description"></a><span data-ttu-id="5179b-153">Description</span><span class="sxs-lookup"><span data-stu-id="5179b-153">Description</span></span>

<span data-ttu-id="5179b-154">L’exemple de corps SOAP (Simple Object Access Protocol) suivant montre une réponse réussie à la demande **UpdateInboxRules** qui modifie une règle.</span><span class="sxs-lookup"><span data-stu-id="5179b-154">The following Simple Object Access Protocol (SOAP) body example shows a successful response to the **UpdateInboxRules** request that modifies a rule.</span></span> 
  
### <a name="code"></a><span data-ttu-id="5179b-155">Code</span><span class="sxs-lookup"><span data-stu-id="5179b-155">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
        MinorVersion="1" 
        MajorBuildNumber="139" 
        MinorBuildNumber="0" 
        Version="Exchange2010_SP1" 
        xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <UpdateInboxRulesResponse 
          ResponseClass="Success" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
    </UpdateInboxRulesResponse>
  </s:Body>
</s:Envelope>

```

### <a name="successful-response-elements"></a><span data-ttu-id="5179b-156">Éléments de réponse réussis</span><span class="sxs-lookup"><span data-stu-id="5179b-156">Successful response elements</span></span>

<span data-ttu-id="5179b-157">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="5179b-157">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="5179b-158">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="5179b-158">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="5179b-159">UpdateInboxRulesResponse</span><span class="sxs-lookup"><span data-stu-id="5179b-159">UpdateInboxRulesResponse</span></span>](updateinboxrulesresponse.md)
    
- [<span data-ttu-id="5179b-160">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="5179b-160">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="5179b-161">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="5179b-161">ResponseCode</span></span>](responsecode.md)
    
## <a name="updateinboxrules-delete-rule-request-example"></a><span data-ttu-id="5179b-162">Exemple de requête UpdateInboxRules (Delete Rule)</span><span class="sxs-lookup"><span data-stu-id="5179b-162">UpdateInboxRules (Delete Rule) request example</span></span>

<span data-ttu-id="5179b-163">Vous pouvez utiliser les services Web Exchange pour supprimer une règle de boîte de réception dans la boîte aux lettres d’un utilisateur dans la Banque d’aide Exchange.</span><span class="sxs-lookup"><span data-stu-id="5179b-163">You can use Exchange Web Services to delete an Inbox rule in a user's mailbox in the Exchange store.</span></span> <span data-ttu-id="5179b-164">Utilisez l' [UpdateInboxRules](updateinboxrules.md) en association avec l’élément [DeleteRuleOperation](deleteruleoperation.md) pour supprimer une règle.</span><span class="sxs-lookup"><span data-stu-id="5179b-164">Use the [UpdateInboxRules](updateinboxrules.md) in conjunction with the [DeleteRuleOperation](deleteruleoperation.md) element to delete a rule.</span></span> 
  
### <a name="description"></a><span data-ttu-id="5179b-165">Description</span><span class="sxs-lookup"><span data-stu-id="5179b-165">Description</span></span>

<span data-ttu-id="5179b-166">Le client construit le code XML de la demande et l’envoie au serveur.</span><span class="sxs-lookup"><span data-stu-id="5179b-166">The client constructs the request XML and sends it to the server.</span></span>
  
### <a name="code"></a><span data-ttu-id="5179b-167">Code</span><span class="sxs-lookup"><span data-stu-id="5179b-167">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version ="Exchange2010_SP1"/>
  </soap:Header>
  <soap:Body>
      <m:UpdateInboxRules>
        <m:RemoveOutlookRuleBlob>true</m:RemoveOutlookRuleBlob>
        <m:Operations>
          <t:DeleteRuleOperation>
            <t:RuleId>Nh8AAAAwW/U=</t:RuleId>
          </t:DeleteRuleOperation>
        </m:Operations>
      </m:UpdateInboxRules>
  </soap:Body>
</soap:Envelope>

```

### <a name="comments"></a><span data-ttu-id="5179b-168">Commentaires</span><span class="sxs-lookup"><span data-stu-id="5179b-168">Comments</span></span>

<span data-ttu-id="5179b-169">Cet exemple supprime la règle identifiée existante.</span><span class="sxs-lookup"><span data-stu-id="5179b-169">This example deletes the existing identified rule.</span></span>
  
### <a name="request-elements"></a><span data-ttu-id="5179b-170">Demander des éléments</span><span class="sxs-lookup"><span data-stu-id="5179b-170">Request elements</span></span>

<span data-ttu-id="5179b-171">La requête **UpdateInboxRules** inclut les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="5179b-171">The **UpdateInboxRules** request includes the following elements:</span></span> 
  
- [<span data-ttu-id="5179b-172">MailboxSmtpAddress</span><span class="sxs-lookup"><span data-stu-id="5179b-172">MailboxSmtpAddress</span></span>](mailboxsmtpaddress.md)
    
- [<span data-ttu-id="5179b-173">RemoveOutlookRuleBlob</span><span class="sxs-lookup"><span data-stu-id="5179b-173">RemoveOutlookRuleBlob</span></span>](removeoutlookruleblob.md)
    
- [<span data-ttu-id="5179b-174">Operations</span><span class="sxs-lookup"><span data-stu-id="5179b-174">Operations</span></span>](operations.md)
    
<span data-ttu-id="5179b-175">L’élément [Operations](operations.md) contient l’élément [DeleteRuleOperation](deleteruleoperation.md) pour supprimer une règle.</span><span class="sxs-lookup"><span data-stu-id="5179b-175">The [Operations](operations.md) element contains the [DeleteRuleOperation](deleteruleoperation.md) element to delete a rule.</span></span> 
  
## <a name="updateinboxrules-delete-rule-response-example"></a><span data-ttu-id="5179b-176">Exemple de réponse UpdateInboxRules (Delete Rule)</span><span class="sxs-lookup"><span data-stu-id="5179b-176">UpdateInboxRules (Delete Rule) response example</span></span>

### <a name="description"></a><span data-ttu-id="5179b-177">Description</span><span class="sxs-lookup"><span data-stu-id="5179b-177">Description</span></span>

<span data-ttu-id="5179b-178">L’exemple de corps SOAP (Simple Object Access Protocol) suivant montre une réponse réussie à la demande **UpdateInboxRules** qui supprime une règle.</span><span class="sxs-lookup"><span data-stu-id="5179b-178">The following Simple Object Access Protocol (SOAP) body example shows a successful response to the **UpdateInboxRules** request that deletes a rule.</span></span> 
  
### <a name="code"></a><span data-ttu-id="5179b-179">Code</span><span class="sxs-lookup"><span data-stu-id="5179b-179">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
        MinorVersion="1" 
        MajorBuildNumber="139" 
        MinorBuildNumber="0" 
        Version="Exchange2010_SP1" 
        xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <UpdateInboxRulesResponse ResponseClass="Success" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
    </UpdateInboxRulesResponse>
  </s:Body>
</s:Envelope>

```

### <a name="successful-response-elements"></a><span data-ttu-id="5179b-180">Éléments de réponse réussis</span><span class="sxs-lookup"><span data-stu-id="5179b-180">Successful response elements</span></span>

<span data-ttu-id="5179b-181">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="5179b-181">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="5179b-182">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="5179b-182">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="5179b-183">UpdateInboxRulesResponse</span><span class="sxs-lookup"><span data-stu-id="5179b-183">UpdateInboxRulesResponse</span></span>](updateinboxrulesresponse.md)
    
- [<span data-ttu-id="5179b-184">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="5179b-184">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="5179b-185">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="5179b-185">ResponseCode</span></span>](responsecode.md)
    
## <a name="see-also"></a><span data-ttu-id="5179b-186">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="5179b-186">See also</span></span>



[<span data-ttu-id="5179b-187">Opération de GetInboxRules</span><span class="sxs-lookup"><span data-stu-id="5179b-187">GetInboxRules operation</span></span>](getinboxrules-operation.md)

