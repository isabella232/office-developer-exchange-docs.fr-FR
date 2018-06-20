---
title: Opération UpdateInboxRules
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
description: L’opération UpdateInboxRules met à jour les règles de boîte de réception de l’utilisateur authentifié en appliquant les opérations spécifiées. UpdateInboxRules est utilisé pour créer une règle de boîte de réception, pour définir une règle de boîte de réception, ou pour supprimer une règle de boîte de réception.
ms.openlocfilehash: 6e979421d619fed6625fe05db86c1f8c6a7418c9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838879"
---
# <a name="updateinboxrules-operation"></a><span data-ttu-id="5a1e8-104">Opération UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="5a1e8-104">UpdateInboxRules operation</span></span>

<span data-ttu-id="5a1e8-105">L’opération UpdateInboxRules met à jour les règles de boîte de réception de l’utilisateur authentifié en appliquant les opérations spécifiées.</span><span class="sxs-lookup"><span data-stu-id="5a1e8-105">The UpdateInboxRules operation updates the authenticated user's Inbox rules by applying the specified operations.</span></span> <span data-ttu-id="5a1e8-106">**UpdateInboxRules** est utilisé pour créer une règle de boîte de réception, pour définir une règle de boîte de réception, ou pour supprimer une règle de boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="5a1e8-106">**UpdateInboxRules** is used to create an Inbox rule, to set an Inbox rule, or to delete an Inbox rule.</span></span> 
  
<span data-ttu-id="5a1e8-107">Lorsque vous utilisez l’opération **UpdateInboxRules** , Services Web Exchange supprime les règles d’envoi côté client.</span><span class="sxs-lookup"><span data-stu-id="5a1e8-107">When you use the **UpdateInboxRules** operation, Exchange Web Services deletes client-side send rules.</span></span> <span data-ttu-id="5a1e8-108">Règles d’envoi côté client sont stockées sur le client dans la règle de Message dossier associé informations (FAI) et nulle part ailleurs.</span><span class="sxs-lookup"><span data-stu-id="5a1e8-108">Client-side send rules are stored on the client in the rule Folder Associated Information (FAI) Message and nowhere else.</span></span> <span data-ttu-id="5a1e8-109">EWS supprime cette règle message FAI par défaut, en fonction de l’attente qu’Outlook va le recréer.</span><span class="sxs-lookup"><span data-stu-id="5a1e8-109">EWS deletes this rule FAI message by default, based on the expectation that Outlook will recreate it.</span></span> <span data-ttu-id="5a1e8-110">Toutefois, Outlook ne peut pas recréer les règles qui n’existent pas également en tant qu’une règle d’étendue, et les règles côté client send n’existent pas sous forme de règles d’étendue.</span><span class="sxs-lookup"><span data-stu-id="5a1e8-110">However, Outlook can't recreate rules that don't also exist as an extended rule, and client-side send rules don't exist as extended rules.</span></span> <span data-ttu-id="5a1e8-111">Par conséquent, ces règles sont perdues.</span><span class="sxs-lookup"><span data-stu-id="5a1e8-111">As a result, these rules are lost.</span></span> <span data-ttu-id="5a1e8-112">Nous vous suggérons Voici lors de la conception de votre solution.</span><span class="sxs-lookup"><span data-stu-id="5a1e8-112">We suggest you consider this when designing your solution.</span></span> 
  
## <a name="updateinboxrules-create-rule-request-example"></a><span data-ttu-id="5a1e8-113">Exemple de requête UpdateInboxRules (créer une règle)</span><span class="sxs-lookup"><span data-stu-id="5a1e8-113">UpdateInboxRules (Create Rule) request example</span></span>

<span data-ttu-id="5a1e8-114">Vous pouvez utiliser les Services Web Exchange pour créer une règle de boîte de réception dans la boîte aux lettres d’un utilisateur dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="5a1e8-114">You can use Exchange Web Services to create an Inbox rule in a user's mailbox in the Exchange store.</span></span> <span data-ttu-id="5a1e8-115">Utilisez l’élément [UpdateInboxRules](updateinboxrules.md) en association avec l’élément [CreateRuleOperation](createruleoperation.md) pour créer une règle.</span><span class="sxs-lookup"><span data-stu-id="5a1e8-115">Use the [UpdateInboxRules](updateinboxrules.md) element in conjunction with the [CreateRuleOperation](createruleoperation.md) element to create a rule.</span></span> 
  
### <a name="description"></a><span data-ttu-id="5a1e8-116">Description</span><span class="sxs-lookup"><span data-stu-id="5a1e8-116">Description</span></span>

<span data-ttu-id="5a1e8-117">Le client construit la requête XML et l’envoie au serveur.</span><span class="sxs-lookup"><span data-stu-id="5a1e8-117">The client constructs the request XML and sends it to the server.</span></span>
  
### <a name="code"></a><span data-ttu-id="5a1e8-118">Code</span><span class="sxs-lookup"><span data-stu-id="5a1e8-118">Code</span></span>

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

### <a name="comments"></a><span data-ttu-id="5a1e8-119">Commentaires</span><span class="sxs-lookup"><span data-stu-id="5a1e8-119">Comments</span></span>

<span data-ttu-id="5a1e8-120">Cet exemple crée une règle qui va déplacer un message électronique dans le dossier courrier indésirable si l’objet du message électronique contient une chaîne qui est égale à « Intéressant ».</span><span class="sxs-lookup"><span data-stu-id="5a1e8-120">This example builds a rule that will move an e-mail message to the Junk E-mail folder if the e-mail subject contains a string that equals "Interesting".</span></span>
  
### <a name="request-elements"></a><span data-ttu-id="5a1e8-121">Éléments de la demande</span><span class="sxs-lookup"><span data-stu-id="5a1e8-121">Request elements</span></span>

<span data-ttu-id="5a1e8-122">La demande **UpdateInboxRules** comprend les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="5a1e8-122">The **UpdateInboxRules** request includes the following elements:</span></span> 
  
- [<span data-ttu-id="5a1e8-123">MailboxSmtpAddress</span><span class="sxs-lookup"><span data-stu-id="5a1e8-123">MailboxSmtpAddress</span></span>](mailboxsmtpaddress.md)
    
- [<span data-ttu-id="5a1e8-124">RemoveOutlookRuleBlob</span><span class="sxs-lookup"><span data-stu-id="5a1e8-124">RemoveOutlookRuleBlob</span></span>](removeoutlookruleblob.md)
    
- [<span data-ttu-id="5a1e8-125">Opérations</span><span class="sxs-lookup"><span data-stu-id="5a1e8-125">Operations</span></span>](operations.md)
    
<span data-ttu-id="5a1e8-126">L’élément [opérations](operations.md) contient l’élément [CreateRuleOperation](createruleoperation.md) pour créer une règle.</span><span class="sxs-lookup"><span data-stu-id="5a1e8-126">The [Operations](operations.md) element contains the [CreateRuleOperation](createruleoperation.md) element to create a rule.</span></span> 
  
## <a name="updateinboxrules-create-rule-response-example"></a><span data-ttu-id="5a1e8-127">Exemple de réponse UpdateInboxRules (créer une règle)</span><span class="sxs-lookup"><span data-stu-id="5a1e8-127">UpdateInboxRules (Create Rule) response example</span></span>

### <a name="description"></a><span data-ttu-id="5a1e8-128">Description</span><span class="sxs-lookup"><span data-stu-id="5a1e8-128">Description</span></span>

<span data-ttu-id="5a1e8-129">L’exemple de corps Simple Object Access Protocol (SOAP) suivant montre une réponse positive à la demande **UpdateInboxRules** qui crée une règle.</span><span class="sxs-lookup"><span data-stu-id="5a1e8-129">The following Simple Object Access Protocol (SOAP) body example shows a successful response to the **UpdateInboxRules** request that creates a rule.</span></span> 
  
### <a name="code"></a><span data-ttu-id="5a1e8-130">Code</span><span class="sxs-lookup"><span data-stu-id="5a1e8-130">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
        MinorVersion="1" 
        MajorBuildNumber="139" 
        MinorBuildNumber="0" Version="Exchange2010_SP1" 
        xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <UpdateInboxRulesResponse 
         ResponseClass="Success" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
    </UpdateInboxRulesResponse>
  </s:Body>
</s:Envelope>

```

### <a name="successful-response-elements"></a><span data-ttu-id="5a1e8-131">Éléments de réponse réussie</span><span class="sxs-lookup"><span data-stu-id="5a1e8-131">Successful response elements</span></span>

<span data-ttu-id="5a1e8-132">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="5a1e8-132">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="5a1e8-133">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="5a1e8-133">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="5a1e8-134">UpdateInboxRulesResponse</span><span class="sxs-lookup"><span data-stu-id="5a1e8-134">UpdateInboxRulesResponse</span></span>](updateinboxrulesresponse.md)
    
- [<span data-ttu-id="5a1e8-135">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="5a1e8-135">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="5a1e8-136">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="5a1e8-136">ResponseCode</span></span>](responsecode.md)
    
## <a name="updateinboxrules-set-rule-request-example"></a><span data-ttu-id="5a1e8-137">Exemple de requête UpdateInboxRules (définir les règles)</span><span class="sxs-lookup"><span data-stu-id="5a1e8-137">UpdateInboxRules (Set Rule) request example</span></span>

<span data-ttu-id="5a1e8-138">Vous pouvez utiliser les Services Web Exchange pour modifier une règle de boîte de réception dans la boîte aux lettres d’un utilisateur dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="5a1e8-138">You can use Exchange Web Services to modify an Inbox rule in a user's mailbox in the Exchange store.</span></span> <span data-ttu-id="5a1e8-139">Utilisez l’élément [UpdateInboxRules](updateinboxrules.md) en association avec l’élément [SetRuleOperation](setruleoperation.md) pour modifier une règle.</span><span class="sxs-lookup"><span data-stu-id="5a1e8-139">Use the [UpdateInboxRules](updateinboxrules.md) element in conjunction with the [SetRuleOperation](setruleoperation.md) element to modify a rule.</span></span> 
  
### <a name="description"></a><span data-ttu-id="5a1e8-140">Description</span><span class="sxs-lookup"><span data-stu-id="5a1e8-140">Description</span></span>

<span data-ttu-id="5a1e8-141">Le client construit la requête XML et l’envoie au serveur.</span><span class="sxs-lookup"><span data-stu-id="5a1e8-141">The client constructs the request XML and sends it to the server.</span></span>
  
### <a name="code"></a><span data-ttu-id="5a1e8-142">Code</span><span class="sxs-lookup"><span data-stu-id="5a1e8-142">Code</span></span>

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
      <m:UpdateInboxRules>
        <m:RemoveOutlookRuleBlob>true</m:RemoveOutlookRuleBlob>
        <Operations xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
          <SetRuleOperation xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
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

### <a name="comments"></a><span data-ttu-id="5a1e8-143">Commentaires</span><span class="sxs-lookup"><span data-stu-id="5a1e8-143">Comments</span></span>

<span data-ttu-id="5a1e8-144">Cet exemple modifie le nom complet « (modifié) il s’agit indésirable ».</span><span class="sxs-lookup"><span data-stu-id="5a1e8-144">This example changes the display name to "(Modified) This is Junk".</span></span>
  
> [!NOTE]
> <span data-ttu-id="5a1e8-145">Les valeurs de l' **Id** et les attributs de l’élément [FolderId](folderid.md) **ChangeKey** ont été raccourcies pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="5a1e8-145">The values of the **Id** and **ChangeKey** attributes of the [FolderId](folderid.md) element have been shortened for readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="5a1e8-146">Éléments de la demande</span><span class="sxs-lookup"><span data-stu-id="5a1e8-146">Request elements</span></span>

<span data-ttu-id="5a1e8-147">La demande **UpdateInboxRules** comprend les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="5a1e8-147">The **UpdateInboxRules** request includes the following elements:</span></span> 
  
- [<span data-ttu-id="5a1e8-148">MailboxSmtpAddress</span><span class="sxs-lookup"><span data-stu-id="5a1e8-148">MailboxSmtpAddress</span></span>](mailboxsmtpaddress.md)
    
- [<span data-ttu-id="5a1e8-149">RemoveOutlookRuleBlob</span><span class="sxs-lookup"><span data-stu-id="5a1e8-149">RemoveOutlookRuleBlob</span></span>](removeoutlookruleblob.md)
    
- [<span data-ttu-id="5a1e8-150">Opérations</span><span class="sxs-lookup"><span data-stu-id="5a1e8-150">Operations</span></span>](operations.md)
    
<span data-ttu-id="5a1e8-151">L’élément [opérations](operations.md) contient l’élément [SetRuleOperation](setruleoperation.md) pour modifier une règle.</span><span class="sxs-lookup"><span data-stu-id="5a1e8-151">The [Operations](operations.md) element contains the [SetRuleOperation](setruleoperation.md) element to modify a rule.</span></span> 
  
## <a name="updateinboxrules-set-rule-response-example"></a><span data-ttu-id="5a1e8-152">Exemple de réponse UpdateInboxRules (définir les règles)</span><span class="sxs-lookup"><span data-stu-id="5a1e8-152">UpdateInboxRules (Set Rule) response example</span></span>

### <a name="description"></a><span data-ttu-id="5a1e8-153">Description</span><span class="sxs-lookup"><span data-stu-id="5a1e8-153">Description</span></span>

<span data-ttu-id="5a1e8-154">L’exemple de corps Simple Object Access Protocol (SOAP) suivant montre une réponse positive à la demande **UpdateInboxRules** qui modifie une règle.</span><span class="sxs-lookup"><span data-stu-id="5a1e8-154">The following Simple Object Access Protocol (SOAP) body example shows a successful response to the **UpdateInboxRules** request that modifies a rule.</span></span> 
  
### <a name="code"></a><span data-ttu-id="5a1e8-155">Code</span><span class="sxs-lookup"><span data-stu-id="5a1e8-155">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
        MinorVersion="1" 
        MajorBuildNumber="139" 
        MinorBuildNumber="0" 
        Version="Exchange2010_SP1" 
        xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <UpdateInboxRulesResponse 
          ResponseClass="Success" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
    </UpdateInboxRulesResponse>
  </s:Body>
</s:Envelope>

```

### <a name="successful-response-elements"></a><span data-ttu-id="5a1e8-156">Éléments de réponse réussie</span><span class="sxs-lookup"><span data-stu-id="5a1e8-156">Successful response elements</span></span>

<span data-ttu-id="5a1e8-157">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="5a1e8-157">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="5a1e8-158">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="5a1e8-158">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="5a1e8-159">UpdateInboxRulesResponse</span><span class="sxs-lookup"><span data-stu-id="5a1e8-159">UpdateInboxRulesResponse</span></span>](updateinboxrulesresponse.md)
    
- [<span data-ttu-id="5a1e8-160">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="5a1e8-160">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="5a1e8-161">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="5a1e8-161">ResponseCode</span></span>](responsecode.md)
    
## <a name="updateinboxrules-delete-rule-request-example"></a><span data-ttu-id="5a1e8-162">Exemple de requête UpdateInboxRules (supprimer la règle)</span><span class="sxs-lookup"><span data-stu-id="5a1e8-162">UpdateInboxRules (Delete Rule) request example</span></span>

<span data-ttu-id="5a1e8-163">Vous pouvez utiliser les Services Web Exchange pour supprimer une règle de boîte de réception dans la boîte aux lettres d’un utilisateur dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="5a1e8-163">You can use Exchange Web Services to delete an Inbox rule in a user's mailbox in the Exchange store.</span></span> <span data-ttu-id="5a1e8-164">Utiliser [UpdateInboxRules](updateinboxrules.md) en association avec l’élément [DeleteRuleOperation](deleteruleoperation.md) pour supprimer une règle.</span><span class="sxs-lookup"><span data-stu-id="5a1e8-164">Use the [UpdateInboxRules](updateinboxrules.md) in conjunction with the [DeleteRuleOperation](deleteruleoperation.md) element to delete a rule.</span></span> 
  
### <a name="description"></a><span data-ttu-id="5a1e8-165">Description</span><span class="sxs-lookup"><span data-stu-id="5a1e8-165">Description</span></span>

<span data-ttu-id="5a1e8-166">Le client construit la requête XML et l’envoie au serveur.</span><span class="sxs-lookup"><span data-stu-id="5a1e8-166">The client constructs the request XML and sends it to the server.</span></span>
  
### <a name="code"></a><span data-ttu-id="5a1e8-167">Code</span><span class="sxs-lookup"><span data-stu-id="5a1e8-167">Code</span></span>

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

### <a name="comments"></a><span data-ttu-id="5a1e8-168">Commentaires</span><span class="sxs-lookup"><span data-stu-id="5a1e8-168">Comments</span></span>

<span data-ttu-id="5a1e8-169">Cet exemple supprime la règle existante identifiée.</span><span class="sxs-lookup"><span data-stu-id="5a1e8-169">This example deletes the existing identified rule.</span></span>
  
### <a name="request-elements"></a><span data-ttu-id="5a1e8-170">Éléments de la demande</span><span class="sxs-lookup"><span data-stu-id="5a1e8-170">Request elements</span></span>

<span data-ttu-id="5a1e8-171">La demande **UpdateInboxRules** comprend les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="5a1e8-171">The **UpdateInboxRules** request includes the following elements:</span></span> 
  
- [<span data-ttu-id="5a1e8-172">MailboxSmtpAddress</span><span class="sxs-lookup"><span data-stu-id="5a1e8-172">MailboxSmtpAddress</span></span>](mailboxsmtpaddress.md)
    
- [<span data-ttu-id="5a1e8-173">RemoveOutlookRuleBlob</span><span class="sxs-lookup"><span data-stu-id="5a1e8-173">RemoveOutlookRuleBlob</span></span>](removeoutlookruleblob.md)
    
- [<span data-ttu-id="5a1e8-174">Opérations</span><span class="sxs-lookup"><span data-stu-id="5a1e8-174">Operations</span></span>](operations.md)
    
<span data-ttu-id="5a1e8-175">L’élément [opérations](operations.md) contient l’élément [DeleteRuleOperation](deleteruleoperation.md) pour supprimer une règle.</span><span class="sxs-lookup"><span data-stu-id="5a1e8-175">The [Operations](operations.md) element contains the [DeleteRuleOperation](deleteruleoperation.md) element to delete a rule.</span></span> 
  
## <a name="updateinboxrules-delete-rule-response-example"></a><span data-ttu-id="5a1e8-176">Exemple de réponse UpdateInboxRules (supprimer la règle)</span><span class="sxs-lookup"><span data-stu-id="5a1e8-176">UpdateInboxRules (Delete Rule) response example</span></span>

### <a name="description"></a><span data-ttu-id="5a1e8-177">Description</span><span class="sxs-lookup"><span data-stu-id="5a1e8-177">Description</span></span>

<span data-ttu-id="5a1e8-178">L’exemple de corps Simple Object Access Protocol (SOAP) suivant montre une réponse positive à la demande **UpdateInboxRules** qui supprime une règle.</span><span class="sxs-lookup"><span data-stu-id="5a1e8-178">The following Simple Object Access Protocol (SOAP) body example shows a successful response to the **UpdateInboxRules** request that deletes a rule.</span></span> 
  
### <a name="code"></a><span data-ttu-id="5a1e8-179">Code</span><span class="sxs-lookup"><span data-stu-id="5a1e8-179">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
        MinorVersion="1" 
        MajorBuildNumber="139" 
        MinorBuildNumber="0" 
        Version="Exchange2010_SP1" 
        xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <UpdateInboxRulesResponse ResponseClass="Success" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
    </UpdateInboxRulesResponse>
  </s:Body>
</s:Envelope>

```

### <a name="successful-response-elements"></a><span data-ttu-id="5a1e8-180">Éléments de réponse réussie</span><span class="sxs-lookup"><span data-stu-id="5a1e8-180">Successful response elements</span></span>

<span data-ttu-id="5a1e8-181">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="5a1e8-181">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="5a1e8-182">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="5a1e8-182">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="5a1e8-183">UpdateInboxRulesResponse</span><span class="sxs-lookup"><span data-stu-id="5a1e8-183">UpdateInboxRulesResponse</span></span>](updateinboxrulesresponse.md)
    
- [<span data-ttu-id="5a1e8-184">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="5a1e8-184">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="5a1e8-185">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="5a1e8-185">ResponseCode</span></span>](responsecode.md)
    
## <a name="see-also"></a><span data-ttu-id="5a1e8-186">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="5a1e8-186">See also</span></span>



[<span data-ttu-id="5a1e8-187">Opération de GetInboxRules</span><span class="sxs-lookup"><span data-stu-id="5a1e8-187">GetInboxRules operation</span></span>](getinboxrules-operation.md)

