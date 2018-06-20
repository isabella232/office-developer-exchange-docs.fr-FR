---
title: Gérer les règles de boîte de réception à l’aide de EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 982ddb78-5606-44b0-8aba-dbffc60d6085
description: Découvrez comment obtenir, créer, mettre à jour et supprimer des règles de boîte de réception à l’aide de l’API managée EWS ou EWS dans Exchange.
ms.openlocfilehash: 85e166ba57d74c74382b257d01d9bff8f44bade1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19754876"
---
# <a name="manage-inbox-rules-by-using-ews-in-exchange"></a><span data-ttu-id="5335f-103">Gérer les règles de boîte de réception à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="5335f-103">Manage Inbox rules by using EWS in Exchange</span></span>

<span data-ttu-id="5335f-104">Découvrez comment obtenir, créer, mettre à jour et supprimer des règles de boîte de réception à l’aide de l’API managée EWS ou EWS dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="5335f-104">Find out how to get, create, update, and delete Inbox rules by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="5335f-105">Vous pouvez obtenir, créer, mettre à jour et supprimer des règles de boîte de réception à l’aide de l’API managée EWS ou EWS.</span><span class="sxs-lookup"><span data-stu-id="5335f-105">You can get, create, update, and delete Inbox rules by using the EWS Managed API or EWS.</span></span> <span data-ttu-id="5335f-106">Quelle que soit la technologie que vous utilisez, vous obtenez et modifier des règles de boîte de réception en tant que collection, et non individuellement.</span><span class="sxs-lookup"><span data-stu-id="5335f-106">Regardless of the technology you use, you get and modify Inbox rules as a collection, rather than individually.</span></span> <span data-ttu-id="5335f-107">Vous utilisez la méthode ou l’opération pour créer de nouvelles règles, mettre à jour les règles existantes et supprimer des règles.</span><span class="sxs-lookup"><span data-stu-id="5335f-107">You use the same method or operation to create new rules, update existing rules, and delete rules.</span></span> 
  
<span data-ttu-id="5335f-108">**Le tableau 1. Méthodes et opérations pour l’extraction et la modification des règles de boîte de réception**</span><span class="sxs-lookup"><span data-stu-id="5335f-108">**Table 1. Methods and operations for getting and modifying Inbox rules**</span></span>

|<span data-ttu-id="5335f-109">**Pour...**</span><span class="sxs-lookup"><span data-stu-id="5335f-109">**In order to…**</span></span>|<span data-ttu-id="5335f-110">**Méthode d'API managée EWS**</span><span class="sxs-lookup"><span data-stu-id="5335f-110">**EWS Managed API method**</span></span>|<span data-ttu-id="5335f-111">**Opération EWS**</span><span class="sxs-lookup"><span data-stu-id="5335f-111">**EWS operation**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="5335f-112">Obtention des règles de boîte de réception</span><span class="sxs-lookup"><span data-stu-id="5335f-112">Get Inbox rules</span></span>  <br/> |[<span data-ttu-id="5335f-113">ExchangeService.GetInboxRules</span><span class="sxs-lookup"><span data-stu-id="5335f-113">ExchangeService.GetInboxRules</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.getinboxrules%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="5335f-114">GetInboxRules</span><span class="sxs-lookup"><span data-stu-id="5335f-114">GetInboxRules</span></span>](http://msdn.microsoft.com/library/b4b2701a-4a23-4acc-8c75-19f7955ad7ae%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="5335f-115">Créer, mettre à jour ou supprimer des règles de boîte de réception</span><span class="sxs-lookup"><span data-stu-id="5335f-115">Create, update, or delete Inbox rules</span></span>  <br/> |[<span data-ttu-id="5335f-116">ExchangeService.UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="5335f-116">ExchangeService.UpdateInboxRules</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.updateinboxrules%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="5335f-117">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="5335f-117">UpdateInboxRules</span></span>](http://msdn.microsoft.com/library/f982a237-471e-45c5-a2b5-468cfc53150b%28Office.15%29.aspx) <br/> |
   
<span data-ttu-id="5335f-118">Afin de créer, mettre à jour ou supprimer des règles de boîte de réception à l’aide de l’API managée EWS ou EWS, vous devez supprimer la règle Outlook, si elle existe.</span><span class="sxs-lookup"><span data-stu-id="5335f-118">In order to create, update, or delete Inbox rules by using the EWS Managed API or EWS, you must remove the Outlook rule, if it exists.</span></span> <span data-ttu-id="5335f-119">Si vous utilisez l’API managée EWS, cela en définissant le paramètre **removeOutlookRulesBlob** sur **true** dans l’appel de méthode **ExchangeService.UpdateInboxRules** .</span><span class="sxs-lookup"><span data-stu-id="5335f-119">If you're using the EWS Managed API, you do this by setting the **removeOutlookRulesBlob** parameter to **true** in the **ExchangeService.UpdateInboxRules** method call.</span></span> <span data-ttu-id="5335f-120">Si vous utilisez EWS, vous définissez la valeur de l’élément [RemoveOutlookRuleBlob](http://msdn.microsoft.com/library/69614475-8bd3-4475-b988-614fe9cad8ef%28Office.15%29.aspx) **true** dans l’opération **UpdateInboxRules** .</span><span class="sxs-lookup"><span data-stu-id="5335f-120">If you're using EWS, you set the value of the [RemoveOutlookRuleBlob](http://msdn.microsoft.com/library/69614475-8bd3-4475-b988-614fe9cad8ef%28Office.15%29.aspx) element to **true** in the **UpdateInboxRules** operation.</span></span> <span data-ttu-id="5335f-121">Il est recommandé que votre à cocher application la propriété [RuleCollection.OutlookRuleBlobExists](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.rulecollection.outlookruleblobexists%28v=exchg.80%29.aspx) (si vous utilisez l’API managée EWS), ou de l’élément [OutlookRuleBlobExists](http://msdn.microsoft.com/library/ae1bc448-deb9-4b5b-ab38-4b276abcb650%28Office.15%29.aspx) (si vous utilisez EWS) avant la mise à jour des règles de boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="5335f-121">We recommend that your application check the [RuleCollection.OutlookRuleBlobExists](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.rulecollection.outlookruleblobexists%28v=exchg.80%29.aspx) property (if you are using the EWS Managed API), or the [OutlookRuleBlobExists](http://msdn.microsoft.com/library/ae1bc448-deb9-4b5b-ab38-4b276abcb650%28Office.15%29.aspx) element (if you're using EWS) before updating Inbox rules.</span></span> <span data-ttu-id="5335f-122">Si cette propriété ou un élément a la valeur **true**, votre application doit avertir l’utilisateur que toutes les règles désactivés perdues dans le cadre de la mise à jour et passez uniquement avec l’autorisation.</span><span class="sxs-lookup"><span data-stu-id="5335f-122">If this property or element has a value of **true**, your application should alert the user that any disabled rules will be lost as part of the update, and only proceed with their permission.</span></span>
  
<span data-ttu-id="5335f-123">Lorsque vous appelez la méthode **UpdateInboxRules** , EWS supprime les règles d’envoi côté client.</span><span class="sxs-lookup"><span data-stu-id="5335f-123">When you call the **UpdateInboxRules** method, EWS deletes client-side send rules.</span></span> <span data-ttu-id="5335f-124">Règles d’envoi côté client sont stockées sur le client dans la règle de Message dossier associé informations (FAI) et nulle part ailleurs.</span><span class="sxs-lookup"><span data-stu-id="5335f-124">Client-side send rules are stored on the client in the rule Folder Associated Information (FAI) Message and nowhere else.</span></span> <span data-ttu-id="5335f-125">EWS supprime cette règle message FAI par défaut, en fonction de l’attente qu’Outlook va le recréer.</span><span class="sxs-lookup"><span data-stu-id="5335f-125">EWS deletes this rule FAI message by default, based on the expectation that Outlook will recreate it.</span></span> <span data-ttu-id="5335f-126">Toutefois, Outlook ne peut pas recréer les règles qui n’existent pas également en tant qu’une règle d’étendue, et les règles côté client send n’existent pas sous forme de règles d’étendue.</span><span class="sxs-lookup"><span data-stu-id="5335f-126">However, Outlook can't recreate rules that don't also exist as an extended rule, and client-side send rules don't exist as extended rules.</span></span> <span data-ttu-id="5335f-127">Par conséquent, ces règles sont perdues.</span><span class="sxs-lookup"><span data-stu-id="5335f-127">As a result, these rules are lost.</span></span> <span data-ttu-id="5335f-128">Nous vous suggérons Voici lors de la conception de votre solution.</span><span class="sxs-lookup"><span data-stu-id="5335f-128">We suggest you consider this when designing your solution.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="5335f-129">Les exemples de code d’API managées dans cet article utilisent un [ensemble commun de méthodes utilitaires](how-to-manage-inbox-rules-by-using-ews-in-exchange.md#bk_UtilitySource).</span><span class="sxs-lookup"><span data-stu-id="5335f-129">The EWS Managed API code examples in this article use a [common set of utility methods](how-to-manage-inbox-rules-by-using-ews-in-exchange.md#bk_UtilitySource).</span></span> <span data-ttu-id="5335f-130">Ces méthodes sont tous deux omis dans les exemples de code par souci de concision.</span><span class="sxs-lookup"><span data-stu-id="5335f-130">These methods are omitted from the code samples for brevity.</span></span> 
  
## <a name="get-inbox-rules-by-using-the-ews-managed-api"></a><span data-ttu-id="5335f-131">Obtention des règles de boîte de réception à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="5335f-131">Get Inbox rules by using the EWS Managed API</span></span>
<span data-ttu-id="5335f-132"><a name="bk_GetRulesEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="5335f-132"></span></span>

<span data-ttu-id="5335f-133">Pour obtenir les règles de boîte de réception en cours, utilisez la méthode [ExchangeService.GetInboxRules](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.getinboxrules%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="5335f-133">To get the current Inbox rules, use the [ExchangeService.GetInboxRules](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.getinboxrules%28v=exchg.80%29.aspx) method.</span></span> <span data-ttu-id="5335f-134">Cette méthode renvoie un objet [RuleCollection](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.rulecollection%28v=exchg.80%29.aspx) qui contient toutes les règles de boîte de réception en cours.</span><span class="sxs-lookup"><span data-stu-id="5335f-134">This method returns a [RuleCollection](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.rulecollection%28v=exchg.80%29.aspx) object that contains all the current Inbox rules.</span></span> 
  
<span data-ttu-id="5335f-135">Dans cet exemple, chaque règle dans la boîte de réception en cours est transmis à une fonction d’assistance ( **ParseRuleDetails** ) pour afficher les détails de la règle.</span><span class="sxs-lookup"><span data-stu-id="5335f-135">In this example, each rule in the current Inbox is passed to a helper function ( **ParseRuleDetails** ) to display the details of the rule.</span></span> 
  
```cs
using System;
using System.Collections.Generic;
using Microsoft.Exchange.WebServices.Data;
private static void GetInboxRules(ExchangeService service, string emailAddress)
{
    RuleCollection inboxRules = null;
    Console.WriteLine("Retrieving inbox rules...");
    // Get the rules from the user's Inbox.
    try
    {
        inboxRules = service.GetInboxRules(emailAddress);
    }
    catch (ServiceResponseException ex)
    {
        Console.WriteLine("Error getting inbox rules: {0}", ex.ErrorCode.ToString());
        return;
    }
    // Loop through the rules and print out the details of each.
    foreach (Rule rule in inboxRules)
    {
        Console.WriteLine("\n***************************************************************");
        Console.WriteLine("Rule: {0}", rule.DisplayName);
        Console.WriteLine("Rule ID: {0}", rule.Id);
        Console.WriteLine("Priority: {0}", rule.Priority);
        Console.WriteLine("Enabled: {0}", rule.IsEnabled.ToString());
        Console.WriteLine("Error: {0}", rule.IsInError.ToString());
        Console.WriteLine("Supported: {0}", (!rule.IsNotSupported).ToString());
        ParseRuleDetails(service, rule);
    }
}
```

## <a name="get-inbox-rules-by-using-ews"></a><span data-ttu-id="5335f-136">Obtention des règles de boîte de réception à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="5335f-136">Get Inbox rules by using EWS</span></span>
<span data-ttu-id="5335f-137"><a name="bk_GetRulesEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="5335f-137"></span></span>

<span data-ttu-id="5335f-138">La demande SOAP EWS suivante utilise l' [opération GetInboxRules](http://msdn.microsoft.com/library/b4b2701a-4a23-4acc-8c75-19f7955ad7ae%28Office.15%29.aspx) pour récupérer les règles de boîte de réception pour sadie@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="5335f-138">The following EWS SOAP request uses the [GetInboxRules operation](http://msdn.microsoft.com/library/b4b2701a-4a23-4acc-8c75-19f7955ad7ae%28Office.15%29.aspx) to retrieve the Inbox rules for sadie@contoso.com.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
<soap:Header>
  <t:RequestServerVersion Version="Exchange2013" />
</soap:Header>
<soap:Body>
  <m:GetInboxRules>
    <m:MailboxSmtpAddress>sadie@contoso.com</m:MailboxSmtpAddress>
  </m:GetInboxRules>
</soap:Body>
</soap:Envelope>
```

<span data-ttu-id="5335f-139">La réponse SOAP EWS suivante contient les règles de boîte de réception en cours de sadie@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="5335f-139">The following EWS SOAP response contains the current Inbox rules for sadie@contoso.com.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
<s:Header>
  <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="712" MinorBuildNumber="22" Version="V2_3" 
      xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
      xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
      xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
      xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
</s:Header>
<s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <GetInboxRulesResponse ResponseClass="Success" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
    <ResponseCode>NoError</ResponseCode>
    <OutlookRuleBlobExists>false</OutlookRuleBlobExists>
    <InboxRules>
      <Rule xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
        <RuleId>AQAAAAAAASY=</RuleId>
        <DisplayName>Alfred</DisplayName>
        <Priority>1</Priority>
        <IsEnabled>true</IsEnabled>
        <Conditions>
          <FromAddresses>
            <Address>
              <Name>Alfred Welker</Name>
              <EmailAddress>/o=First Organization/ou=Exchange Administrative Group (FYDIBOHF23SPDLT)/cn=Recipients/cn=9a83e6380cae41918c71e7921d960b5a-Alfre</EmailAddress>
              <RoutingType>EX</RoutingType>
            </Address>
          </FromAddresses>
        </Conditions>
        <Actions>
          <MoveToFolder>
            <FolderId Id="AAMkADg1OWUwODcyLTg4M2MtNDAyMS05YjI0LTI5ZGM5OTU4Njk3YwAuAAAAAADPriAxh444TpHj2GoQxWQNAQAN+VjmVZl5Rq1ymCq5eFKOAAAAABSyAAA=" ChangeKey="AQAAAA==" />
          </MoveToFolder>
          <StopProcessingRules>true</StopProcessingRules>
        </Actions>
      </Rule>
      <Rule xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
        <RuleId>AQAAAAAAASQ=</RuleId>
        <DisplayName>Important</DisplayName>
        <Priority>2</Priority>
        <IsEnabled>true</IsEnabled>
        <Conditions>
          <ContainsSubjectStrings>
            <String>Urgent</String>
          </ContainsSubjectStrings>
          <FromAddresses>
            <Address>
              <Name>Hope Gross</Name>
              <EmailAddress>/o=First Organization/ou=Exchange Administrative Group (FYDIBOHF23SPDLT)/cn=Recipients/cn=9b55e4100c064d9d8c5f72ff36802ed3-Hope</EmailAddress>
              <RoutingType>EX</RoutingType>
            </Address>
          </FromAddresses>
        </Conditions>
        <Actions>
          <MarkImportance>High</MarkImportance>
          <StopProcessingRules>true</StopProcessingRules>
        </Actions>
      </Rule>
    </InboxRules>
  </GetInboxRulesResponse>
</s:Body>
</s:Envelope>
```

## <a name="create-inbox-rules-by-using-the-ews-managed-api"></a><span data-ttu-id="5335f-140">Créer des règles de boîte de réception à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="5335f-140">Create Inbox rules by using the EWS Managed API</span></span>
<span data-ttu-id="5335f-141"><a name="bk_CreateRulesEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="5335f-141"></span></span>

<span data-ttu-id="5335f-142">Pour créer une règle, incluez un objet [CreateRuleOperation](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.createruleoperation%28v=exchg.80%29.aspx) dans la collection d’objets [RuleOperation](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.ruleoperation%28v=exchg.80%29.aspx) transmis à la méthode [ExchangeService.UpdateInboxRules](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.updateinboxrules%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="5335f-142">To create a rule, include a [CreateRuleOperation](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.createruleoperation%28v=exchg.80%29.aspx) object in the collection of [RuleOperation](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.ruleoperation%28v=exchg.80%29.aspx) objects passed to the [ExchangeService.UpdateInboxRules](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.updateinboxrules%28v=exchg.80%29.aspx) method.</span></span> 
  
<span data-ttu-id="5335f-143">Dans cet exemple, une nouvelle règle est créée pour déplacer des messages envoyés vers une liste de distribution nommée « Sales » dans un sous-dossier de la boîte de réception, également appelés « Sales ».</span><span class="sxs-lookup"><span data-stu-id="5335f-143">In this example, a new rule is created to move mail sent to a distribution list called "Sales" to a subfolder of the Inbox, also called "Sales".</span></span>
  
```cs
using System;
using System.Collections.Generic;
using Microsoft.Exchange.WebServices.Data;
private static void CreateInboxRule(ExchangeService service, string emailAddress)
{
    // Before modifying the rules on the server, determine
    // whether an Outlook rules BLOB exists. Updating rules
    // via EWS requires removal of the Outlook BLOB. This can
    // result in any rules that the user has disabled via the Outlook
    // UI to be lost.
    RuleCollection currentRules = null;
    try
    {
        currentRules = service.GetInboxRules(emailAddress);
    }
    catch (ServiceResponseException ex)
    {
        Console.WriteLine("Error getting inbox rules: {0}", ex.ErrorCode.ToString());
    }
    if (currentRules != null &amp;&amp; currentRules.OutlookRuleBlobExists)
    {
        Console.WriteLine("WARNING: Adding a new rule will delete the Outlook rule BLOB.");
        Console.WriteLine("This can lead to a loss of any disabled rules.");
        Console.Write("Hit Y to proceed (any other key to cancel): ");
        ConsoleKeyInfo cki = Console.ReadKey();
        if (cki.KeyChar != 'Y' &amp;&amp; cki.KeyChar != 'y')
        {
            Console.WriteLine("\nCanceling addition of new rule...");
            return;
        }
        Console.WriteLine();
    }
    Console.WriteLine("Adding \"Sales\" rule.");
    Rule newRule = new Rule();
    // Creating a rule called "Sales"
    newRule.DisplayName = "Sales";
    // Conditions
    // When messages are sent to the "Sales" address (sales@contoso.com),
    newRule.Conditions.SentToAddresses.Add("Sales", "sales@contoso.com");
    FolderId moveToFolderId = GetFolderIdByName(service, WellKnownFolderName.Inbox, "Sales");
    if (moveToFolderId == null)
    {
        throw new ArgumentException("Invalid subfolder specified");
    }
    // Actions
    // Move the message to the "Sales" folder
    newRule.Actions.MoveToFolder = moveToFolderId;
    // And stop processing more rules
    newRule.Actions.StopProcessingRules = true;
    // Exceptions
    // Except if the message is from Hope Gross (hope@contoso.com).
    newRule.Exceptions.FromAddresses.Add("Hope Gross", "hope@contoso.com");
    Console.WriteLine("Rule: {0}", newRule.DisplayName);
    ParseRuleDetails(service, newRule);
    // Add the new rule to the CreateRule operation.
    CreateRuleOperation createMoveIfFromSalesRule = new CreateRuleOperation(newRule);
    try
    {
        // Update rules. Note that this method can accept
        // an array of rule operations, enabling you to batch
        // updates.
        service.UpdateInboxRules(new RuleOperation[] { createMoveIfFromSalesRule }, true);
    }
    catch (UpdateInboxRulesException ex)
    {
        Console.WriteLine("Error updating Inbox rules: {0}", ex.ErrorCode.ToString());
        return;
    }
    Console.WriteLine("Rule added.");
}
```

## <a name="create-inbox-rules-by-using-ews"></a><span data-ttu-id="5335f-144">Créer des règles de boîte de réception à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="5335f-144">Create Inbox rules by using EWS</span></span>
<span data-ttu-id="5335f-145"><a name="bk_CreateRulesEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="5335f-145"></span></span>

<span data-ttu-id="5335f-146">La demande SOAP EWS suivante crée la règle « Sales » dans la boîte de réception de sadie@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="5335f-146">The following EWS SOAP request creates the "Sales" rule in sadie@contoso.com's Inbox.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
  <soap:Body>
    <m:UpdateInboxRules>
      <m:RemoveOutlookRuleBlob>true</m:RemoveOutlookRuleBlob>
      <m:Operations>
        <t:CreateRuleOperation>
          <t:Rule>
            <t:DisplayName>Sales</t:DisplayName>
            <t:Priority>1</t:Priority>
            <t:IsEnabled>true</t:IsEnabled>
            <t:IsInError>false</t:IsInError>
            <t:Conditions>
              <t:SentToAddresses>
                <t:Address>
                  <t:Name>Sales</t:Name>
                  <t:EmailAddress>sales@contoso.com</t:EmailAddress>
                </t:Address>
              </t:SentToAddresses>
            </t:Conditions>
            <t:Exceptions>
              <t:FromAddresses>
                <t:Address>
                  <t:Name>Hope Gross</t:Name>
                  <t:EmailAddress>hope@contoso.com</t:EmailAddress>
                </t:Address>
              </t:FromAddresses>
            </t:Exceptions>
            <t:Actions>
              <t:MoveToFolder>
                <t:FolderId Id="AAMkADg1OWUwODcyLTg4M2MtNDAyMS05YjI0LTI5ZGM5OTU4Njk3YwAuAAAAAADPriAxh444TpHj2GoQxWQNAQAN+VjmVZl5Rq1ymCq5eFKOAAAAABSxAAA=" 
                    ChangeKey="AQAAABYAAAAN+VjmVZl5Rq1ymCq5eFKOAAAAABTZ" />
              </t:MoveToFolder>
              <t:StopProcessingRules>true</t:StopProcessingRules>
            </t:Actions>
          </t:Rule>
        </t:CreateRuleOperation>
      </m:Operations>
    </m:UpdateInboxRules>
  </soap:Body>
</soap:Envelope>
```

## <a name="update-inbox-rules-by-using-the-ews-managed-api"></a><span data-ttu-id="5335f-147">Mise à jour des règles de boîte de réception à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="5335f-147">Update Inbox rules by using the EWS Managed API</span></span>
<span data-ttu-id="5335f-148"><a name="bk_UpdateRulesEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="5335f-148"></span></span>

<span data-ttu-id="5335f-149">Pour mettre à jour une règle, inclure un objet [SetRuleOperation](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.setruleoperation%28v=exchg.80%29.aspx) dans la collection d’objets **RuleOperation** transmis à la méthode **UpdateInboxRules** .</span><span class="sxs-lookup"><span data-stu-id="5335f-149">To update a rule, include a [SetRuleOperation](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.setruleoperation%28v=exchg.80%29.aspx) object in the collection of **RuleOperation** objects passed to the **UpdateInboxRules** method.</span></span> 
  
<span data-ttu-id="5335f-150">Dans cet exemple, la règle « Sales » est mis à jour pour ajouter une exception.</span><span class="sxs-lookup"><span data-stu-id="5335f-150">In this example, the "Sales" rule is updated to add an exception.</span></span> <span data-ttu-id="5335f-151">Si l’objet contient le mot « Urgent », les messages ne seront pas déplacées vers le sous-dossier « Sales ».</span><span class="sxs-lookup"><span data-stu-id="5335f-151">If the subject contains the word "Urgent", the messages will not be moved to the "Sales" subfolder.</span></span>
  
```cs
using System;
using System.Collections.Generic;
using Microsoft.Exchange.WebServices.Data;
private static void UpdateInboxRule(ExchangeService service, string emailAddress)
{
    // Before modifying the rules on the server, determine
    // whether an Outlook rules BLOB exists. Updating rules
    // via EWS requires removal of the Outlook BLOB. This can
    // result in any rules that the user has disabled via the Outlook
    // UI to be lost.
    RuleCollection currentRules = null;
    try
    {
        currentRules = service.GetInboxRules(emailAddress);
    }
    catch (ServiceResponseException ex)
    {
        Console.WriteLine("Error getting inbox rules: {0}", ex.ErrorCode.ToString());
    }
    if (currentRules != null &amp;&amp; currentRules.OutlookRuleBlobExists)
    {
        Console.WriteLine("WARNING: Updating an existing rule will delete the Outlook rule BLOB.");
        Console.WriteLine("This can lead to a loss of any disabled rules.");
        Console.Write("Hit Y to proceed (any other key to cancel): ");
        ConsoleKeyInfo cki = Console.ReadKey();
        if (cki.KeyChar != 'Y' &amp;&amp; cki.KeyChar != 'y')
        {
            Console.WriteLine("\nCanceling update of rule...");
            return;
        }
        Console.WriteLine();
    }
    // Look for the rule called "Sales" and modify it
    // to add an exception if "Urgent" is in the subject.
    Console.WriteLine("Updating rule \"Sales\"...");
    Rule ruleToUpdate = null;
    foreach (Rule rule in currentRules)
    {
        if (rule.DisplayName == "Sales")
        {
            ruleToUpdate = rule;
            break;
        }
    }
    if (ruleToUpdate == null)
    {
        Console.WriteLine("Could not find a rule called \"Sales\", canceling update.");
        return;
    }
    // Add the exception.
    ruleToUpdate.Exceptions.ContainsSubjectStrings.Add("Urgent");
    SetRuleOperation setRuleOperation = new SetRuleOperation(ruleToUpdate);
    try
    {
        // Update rules. Note that this method can accept
        // an array of rule operations, enabling you to batch
        // updates.
        service.UpdateInboxRules(new RuleOperation[] { setRuleOperation }, true);
    }
    catch (UpdateInboxRulesException ex)
    {
        Console.WriteLine("Error updating Inbox rules: {0}", ex.ErrorCode.ToString());
        return;
    }
    Console.WriteLine("Rule updated.");
}
```

## <a name="update-inbox-rules-by-using-ews"></a><span data-ttu-id="5335f-152">Mise à jour des règles de boîte de réception à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="5335f-152">Update Inbox rules by using EWS</span></span>
<span data-ttu-id="5335f-153"><a name="bk_UpdateRulesEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="5335f-153"></span></span>

<span data-ttu-id="5335f-154">La demande SOAP EWS suivante met à jour la règle « Sales » dans la boîte de réception de sadie@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="5335f-154">The following EWS SOAP request updates the "Sales" rule in sadie@contoso.com's Inbox.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
  <soap:Body>
    <m:UpdateInboxRules>
      <m:RemoveOutlookRuleBlob>true</m:RemoveOutlookRuleBlob>
      <m:Operations>
        <t:SetRuleOperation>
          <t:Rule>
            <t:RuleId>AQAAAATnzOA=</t:RuleId>
            <t:DisplayName>Sales</t:DisplayName>
            <t:Priority>1</t:Priority>
            <t:IsEnabled>true</t:IsEnabled>
            <t:IsInError>false</t:IsInError>
            <t:Conditions>
              <t:SentToAddresses>
                <t:Address>
                  <t:Name>Sales</t:Name>
                  <t:EmailAddress>sales@contoso.com</t:EmailAddress>
                  <t:RoutingType>SMTP</t:RoutingType>
                </t:Address>
              </t:SentToAddresses>
            </t:Conditions>
            <t:Exceptions>
              <t:ContainsSubjectStrings>
                <t:String>Urgent</t:String>
              </t:ContainsSubjectStrings>
              <t:FromAddresses>
                <t:Address>
                  <t:Name>Hope Gross</t:Name>
                  <t:EmailAddress>hope@contoso.com</t:EmailAddress>
                  <t:RoutingType>SMTP</t:RoutingType>
                </t:Address>
              </t:FromAddresses>
            </t:Exceptions>
            <t:Actions>
              <t:MoveToFolder>
                <t:FolderId Id="AAMkADg1OWUwODcyLTg4M2MtNDAyMS05YjI0LTI5ZGM5OTU4Njk3YwAuAAAAAADPriAxh444TpHj2GoQxWQNAQAN+VjmVZl5Rq1ymCq5eFKOAAAAABSxAAA=" 
                    ChangeKey="AQAAAA==" />
              </t:MoveToFolder>
              <t:StopProcessingRules>true</t:StopProcessingRules>
            </t:Actions>
          </t:Rule>
        </t:SetRuleOperation>
      </m:Operations>
    </m:UpdateInboxRules>
  </soap:Body>
</soap:Envelope>
```

## <a name="delete-inbox-rules-by-using-the-ews-managed-api"></a><span data-ttu-id="5335f-155">Supprimer des règles de boîte de réception à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="5335f-155">Delete Inbox rules by using the EWS Managed API</span></span>
<span data-ttu-id="5335f-156"><a name="bk_DeleteRulesEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="5335f-156"></span></span>

<span data-ttu-id="5335f-157">Pour supprimer une règle, inclure un objet [DeleteRuleOperation](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.deleteruleoperation%28v=exchg.80%29.aspx) dans la collection d’objets **RuleOperation** transmis à la méthode **UpdateInboxRules** .</span><span class="sxs-lookup"><span data-stu-id="5335f-157">To delete a rule, include a [DeleteRuleOperation](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.deleteruleoperation%28v=exchg.80%29.aspx) object in the collection of **RuleOperation** objects passed to the **UpdateInboxRules** method.</span></span> 
  
<span data-ttu-id="5335f-158">Dans cet exemple, la règle « Sales » est supprimée.</span><span class="sxs-lookup"><span data-stu-id="5335f-158">In this example, the "Sales" rule is deleted.</span></span>
  
```cs
using System;
using System.Collections.Generic;
using Microsoft.Exchange.WebServices.Data;
private static void DeleteInboxRule(ExchangeService service, string emailAddress)
{
    // Before modifying the rules on the server, determine
    // whether an Outlook rules BLOB exists. Updating rules
    // via EWS requires removal of the Outlook BLOB. This can
    // result in any rules that the user has disabled via the Outlook
    // UI to be lost.
    RuleCollection currentRules = null;
    try
    {
        currentRules = service.GetInboxRules(emailAddress);
    }
    catch (ServiceResponseException ex)
    {
        Console.WriteLine("Error getting inbox rules: {0}", ex.ErrorCode.ToString());
    }
    if (currentRules != null &amp;&amp; currentRules.OutlookRuleBlobExists)
    {
        Console.WriteLine("WARNING: Deleting a rule will delete the Outlook rule BLOB.");
        Console.WriteLine("This can lead to a loss of any disabled rules.");
        Console.Write("Hit Y to proceed (any other key to cancel): ");
        ConsoleKeyInfo cki = Console.ReadKey();
        if (cki.KeyChar != 'Y' &amp;&amp; cki.KeyChar != 'y')
        {
            Console.WriteLine("\nCancelling deletion of new rule...");
            return;
        }
        Console.WriteLine();
    }
    // Look for the rule called "Sales" and delete it.
    Console.WriteLine("Deleting rule \"Sales\"...");
    string ruleId = string.Empty;
    foreach (Rule rule in currentRules)
    {
        if (rule.DisplayName == "Sales")
        {
            ruleId = rule.Id;
            break;
        }
    }
    if (string.IsNullOrEmpty(ruleId))
    {
        Console.WriteLine("Could not find a rule called \"Sales\", canceling delete.");
        return;
    }
    DeleteRuleOperation deleteRuleOperation = new DeleteRuleOperation(ruleId);
    try
    {
        // Update rules. Note that this method can accept
        // an array of rule operations, enabling you to batch
        // updates.
        service.UpdateInboxRules(new RuleOperation[] { deleteRuleOperation }, true);
    }
    catch (UpdateInboxRulesException ex)
    {
        Console.WriteLine("Error updating Inbox rules: {0}", ex.ErrorCode.ToString());
        return;
    }
    Console.WriteLine("Rule deleted.");
}
```

## <a name="delete-inbox-rules-by-using-ews"></a><span data-ttu-id="5335f-159">Supprimer des règles de boîte de réception à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="5335f-159">Delete Inbox rules by using EWS</span></span>
<span data-ttu-id="5335f-160"><a name="bk_DeleteRulesEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="5335f-160"></span></span>

<span data-ttu-id="5335f-161">La demande SOAP EWS suivante supprime les règles de « Sales » à partir de la boîte de réception de sadie@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="5335f-161">The following EWS SOAP request deletes the "Sales" rules from sadie@contoso.com's inbox.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
  <soap:Body>
    <m:UpdateInboxRules>
      <m:RemoveOutlookRuleBlob>true</m:RemoveOutlookRuleBlob>
      <m:Operations>
        <t:DeleteRuleOperation>
          <t:RuleId>AQAAAATnzOA=</t:RuleId>
        </t:DeleteRuleOperation>
      </m:Operations>
    </m:UpdateInboxRules>
  </soap:Body>
</soap:Envelope>
```

## <a name="source-for-sample-utility-methods"></a><span data-ttu-id="5335f-162">Source pour les méthodes de l’utilitaire exemple</span><span class="sxs-lookup"><span data-stu-id="5335f-162">Source for sample utility methods</span></span>
<span data-ttu-id="5335f-163"><a name="bk_UtilitySource"> </a></span><span class="sxs-lookup"><span data-stu-id="5335f-163"></span></span>

<span data-ttu-id="5335f-164">Les exemples d’API managées dans cet article utilisent les méthodes utilitaires inclus dans l’exemple suivant.</span><span class="sxs-lookup"><span data-stu-id="5335f-164">The EWS Managed API examples in this article use the utility methods included in the following example.</span></span>
  
```cs
private static void ParseRuleDetails(ExchangeService service, Rule rule)
{
    // Conditions
    string conditions = ParseRulePredicates(rule.Conditions, false);
    if (!string.IsNullOrEmpty(conditions))
    {
        Console.WriteLine("When a message:");
        Console.WriteLine(conditions);
    }
    // Actions
    string actions = ParseRuleActions(service, rule.Actions);
    if (!string.IsNullOrEmpty(actions))
    {
        Console.WriteLine("Take the following action(s):");
        Console.WriteLine(actions);
    }
    // Exceptions
    string exceptions = ParseRulePredicates(rule.Exceptions, true);
    if (!string.IsNullOrEmpty(exceptions))
    {
        Console.WriteLine("Except when the message:");
        Console.WriteLine(exceptions);
    }
}
private static string ParseRulePredicates(RulePredicates predicates, bool isExceptions)
{
    string humanReadablePredicates = string.Empty;
    foreach (string category in predicates.Categories)
    {
        humanReadablePredicates = AppendToHumanReadableString(humanReadablePredicates,
            "has the category \"" + category + "\"", isExceptions);
    }
    foreach (string bodyString in predicates.ContainsBodyStrings)
    {
        humanReadablePredicates = AppendToHumanReadableString(humanReadablePredicates,
            "has \"" + bodyString + "\" in the body", isExceptions);
    }
    foreach (string headerString in predicates.ContainsHeaderStrings)
    {
        humanReadablePredicates = AppendToHumanReadableString(humanReadablePredicates,
            "has \"" + headerString + "\" in the headers", isExceptions);
    }
    foreach (string recipientString in predicates.ContainsRecipientStrings)
    {
        humanReadablePredicates = AppendToHumanReadableString(humanReadablePredicates,
            "has \"" + recipientString + "\" in the recipient's address", isExceptions);
    }
    foreach (string senderString in predicates.ContainsSenderStrings)
    {
        humanReadablePredicates = AppendToHumanReadableString(humanReadablePredicates,
            "has \"" + senderString + "\" in the sender's address", isExceptions);
    }
    foreach (string subjectOrBodyString in predicates.ContainsSubjectOrBodyStrings)
    {
        humanReadablePredicates = AppendToHumanReadableString(humanReadablePredicates,
            "has \"" + subjectOrBodyString + "\" in the subject or body", isExceptions);
    }
    foreach (string subjectString in predicates.ContainsSubjectStrings)
    {
        humanReadablePredicates = AppendToHumanReadableString(humanReadablePredicates,
            "has \"" + subjectString + "\" in the subject", isExceptions);
    }
    if (predicates.FlaggedForAction != null)
    {
        humanReadablePredicates = AppendToHumanReadableString(humanReadablePredicates,
            "is flagged for \"" + predicates.FlaggedForAction.Value + "\" action", isExceptions);
    }
    foreach (EmailAddress fromAddress in predicates.FromAddresses)
    {
        humanReadablePredicates = AppendToHumanReadableString(humanReadablePredicates,
            "is from " + fromAddress.Name + " (" + fromAddress.Address + ")", isExceptions);
    }
    foreach (string fromConnectedAccount in predicates.FromConnectedAccounts)
    {
        humanReadablePredicates = AppendToHumanReadableString(humanReadablePredicates,
            "is from the \"" + fromConnectedAccount + "\" account", isExceptions);
    }
    if (predicates.HasAttachments)
    {
        humanReadablePredicates = AppendToHumanReadableString(humanReadablePredicates,
            "has an attachment", isExceptions);
    }
    if (predicates.Importance != null)
    {
        humanReadablePredicates = AppendToHumanReadableString(humanReadablePredicates,
            "is marked as " + predicates.Importance.Value + " importance", isExceptions);
    }
    if (predicates.IsApprovalRequest)
    {
        humanReadablePredicates = AppendToHumanReadableString(humanReadablePredicates,
            "is an approval request", isExceptions);
    }
    if (predicates.IsAutomaticForward)
    {
        humanReadablePredicates = AppendToHumanReadableString(humanReadablePredicates,
            "is an automatic forward", isExceptions);
    }
    if (predicates.IsAutomaticReply)
    {
        humanReadablePredicates = AppendToHumanReadableString(humanReadablePredicates,
            "is an automatic reply", isExceptions);
    }
    if (predicates.IsEncrypted)
    {
        humanReadablePredicates = AppendToHumanReadableString(humanReadablePredicates,
            "is encrypted", isExceptions);
    }
    if (predicates.IsMeetingRequest)
    {
        humanReadablePredicates = AppendToHumanReadableString(humanReadablePredicates,
            "is a meeting request", isExceptions);
    }
    if (predicates.IsMeetingResponse)
    {
        humanReadablePredicates = AppendToHumanReadableString(humanReadablePredicates,
            "is a meeting response", isExceptions);
    }
    if (predicates.IsNonDeliveryReport)
    {
        humanReadablePredicates = AppendToHumanReadableString(humanReadablePredicates,
            "is a non-delivery report", isExceptions);
    }
    if (predicates.IsPermissionControlled)
    {
        humanReadablePredicates = AppendToHumanReadableString(humanReadablePredicates,
            "is a rights-managed message", isExceptions);
    }
    if (predicates.IsReadReceipt)
    {
        humanReadablePredicates = AppendToHumanReadableString(humanReadablePredicates,
            "is a read receipt", isExceptions);
    }
    if (predicates.IsSigned)
    {
        humanReadablePredicates = AppendToHumanReadableString(humanReadablePredicates,
            "is signed", isExceptions);
    }
    if (predicates.IsVoicemail)
    {
        humanReadablePredicates = AppendToHumanReadableString(humanReadablePredicates,
            "is a voicemail", isExceptions);
    }
    foreach (string messageClass in predicates.ItemClasses)
    {
        humanReadablePredicates = AppendToHumanReadableString(humanReadablePredicates,
            "has a message class of \"" + messageClass + "\"", isExceptions);
    }
    foreach (string messageClassification in predicates.MessageClassifications)
    {
        humanReadablePredicates = AppendToHumanReadableString(humanReadablePredicates,
            "has a classification of \"" + messageClassification + "\"", isExceptions);
    }
    if (predicates.NotSentToMe)
    {
        humanReadablePredicates = AppendToHumanReadableString(humanReadablePredicates,
            "is not sent to me", isExceptions);
    }
    if (predicates.Sensitivity != null)
    {
        humanReadablePredicates = AppendToHumanReadableString(humanReadablePredicates,
            "has a sensitivity of \"" + predicates.Sensitivity.Value + "\"", isExceptions);
    }
    if (predicates.SentCcMe)
    {
        humanReadablePredicates = AppendToHumanReadableString(humanReadablePredicates,
            "has me on the CC line", isExceptions);
    }
    if (predicates.SentOnlyToMe)
    {
        humanReadablePredicates = AppendToHumanReadableString(humanReadablePredicates,
            "is sent ONLY to me", isExceptions);
    }
    foreach (EmailAddress sentToAddress in predicates.SentToAddresses)
    {
        humanReadablePredicates = AppendToHumanReadableString(humanReadablePredicates,
            "is sent to " + sentToAddress.Name + " (" + sentToAddress.Address + ")", isExceptions);
    }
    if (predicates.SentToMe)
    {
        humanReadablePredicates = AppendToHumanReadableString(humanReadablePredicates,
            "has me on the To line", isExceptions);
    }
    if (predicates.SentToOrCcMe)
    {
        humanReadablePredicates = AppendToHumanReadableString(humanReadablePredicates,
            "has me on the To or CC line", isExceptions);
    }
    if (predicates.WithinDateRange != null)
    {
        if (predicates.WithinDateRange.Start != null)
        {
            humanReadablePredicates = AppendToHumanReadableString(humanReadablePredicates,
                "was received after " + predicates.WithinDateRange.Start.ToString(), isExceptions);
        }
        if (predicates.WithinDateRange.End != null)
        {
            humanReadablePredicates = AppendToHumanReadableString(humanReadablePredicates,
                "was recieved before " + predicates.WithinDateRange.End.ToString(), isExceptions);
        }
    }
    if (predicates.WithinSizeRange != null)
    {
        if (predicates.WithinSizeRange.MinimumSize != null)
        {
            humanReadablePredicates = AppendToHumanReadableString(humanReadablePredicates,
                "is larger than " + predicates.WithinSizeRange.MinimumSize + " kb", isExceptions);
        }
        if (predicates.WithinSizeRange.MaximumSize != null)
        {
            humanReadablePredicates = AppendToHumanReadableString(humanReadablePredicates,
                "is smaller than " + predicates.WithinSizeRange.MaximumSize + " kb", isExceptions);
        }
    }
    return humanReadablePredicates;
}
private static string ParseRuleActions(ExchangeService service, RuleActions actions)
{
    string humanReadableActions = string.Empty;
    foreach (string category in actions.AssignCategories)
    {
        humanReadableActions = AppendToHumanReadableString(humanReadableActions,
            "assign the \"" + category + "\" category", false);
    }
    if (actions.CopyToFolder != null)
    {
        humanReadableActions = AppendToHumanReadableString(humanReadableActions,
            "move to the \"" + GetFolderNameFromId(service, actions.CopyToFolder) + "\" folder", false);
    }
    if (actions.Delete)
    {
        humanReadableActions = AppendToHumanReadableString(humanReadableActions,
            "delete the message", false);
    }
    foreach (EmailAddress forwardAddress in actions.ForwardAsAttachmentToRecipients)
    {
        humanReadableActions = AppendToHumanReadableString(humanReadableActions,
            "forward as an attachment to " + forwardAddress.Name + " (" +
            forwardAddress.Address + ")", false);
    }
    foreach (EmailAddress forwardAddress in actions.ForwardToRecipients)
    {
        humanReadableActions = AppendToHumanReadableString(humanReadableActions,
            "forward to " + forwardAddress.Name + " (" + forwardAddress.Address + ")", false);
    }
    if (actions.MarkAsRead)
    {
        humanReadableActions = AppendToHumanReadableString(humanReadableActions,
            "mark the message as read", false);
    }
    if (actions.MarkImportance != null)
    {
        humanReadableActions = AppendToHumanReadableString(humanReadableActions,
            "mark the message with " + actions.MarkImportance.Value + " importance", false);
    }
    if (actions.MoveToFolder != null)
    {
        humanReadableActions = AppendToHumanReadableString(humanReadableActions,
            "move the message to the \"" + GetFolderNameFromId(service, actions.MoveToFolder) + "\" folder", false);
    }
    if (actions.PermanentDelete)
    {
        humanReadableActions = AppendToHumanReadableString(humanReadableActions,
            "permanently delete the message", false);
    }
    foreach (EmailAddress redirectAddress in actions.RedirectToRecipients)
    {
        humanReadableActions = AppendToHumanReadableString(humanReadableActions,
            "redirect the message to " + redirectAddress.Name + " (" +
            redirectAddress.Address + ")", false);
    }
    foreach (MobilePhone smsRecipient in actions.SendSMSAlertToRecipients)
    {
        humanReadableActions = AppendToHumanReadableString(humanReadableActions,
            "send SMS alert to " + smsRecipient.Name + " (" +
            smsRecipient.PhoneNumber + ")", false);
    }
    if (actions.ServerReplyWithMessage != null)
    {
        humanReadableActions = AppendToHumanReadableString(humanReadableActions,
            "have the server reply with a template message, ID=" +
            actions.ServerReplyWithMessage.UniqueId, false);
    }
    if (actions.StopProcessingRules)
    {
        humanReadableActions = AppendToHumanReadableString(humanReadableActions,
            "stop processing more rules", false);
    }
    return humanReadableActions;
}
private static string AppendToHumanReadableString(string humanReadableString, string appendString, bool isExceptions)
{
    // Conditions and Actions are AND'ed together
    string logicalOperator = "AND";
    if (isExceptions)
    {
        // Exceptions are OR'ed
        logicalOperator = "OR";
    }
    if (!string.IsNullOrEmpty(humanReadableString))
    {
        // There's already an item in the list, so we need to
        // add the operator
        humanReadableString += "\n  " + logicalOperator + " ";
    }
    else
    {
        humanReadableString += "  ";
    }
    humanReadableString += appendString;
    return humanReadableString;
}
private static string GetFolderNameFromId(ExchangeService service, FolderId folderId)
{
    string folderName = string.Empty;
    Folder folder = null;
    try
    {
        folder = Folder.Bind(service, folderId);
    }
    catch (ServiceResponseException)
    {
        Console.WriteLine("Unable to bind to the folder specified.");
    }
    if (folder != null)
        folderName = folder.DisplayName;
    return folderName;
}
private static FolderId GetFolderIdByName(ExchangeService service, WellKnownFolderName parentWellKnownFolder, string subFolderName)
{
    FolderId returnId = null;
    Folder parentFolder = null;
    try
    {
        parentFolder = Folder.Bind(service, parentWellKnownFolder);
    }
    catch (ServiceResponseException)
    {
        Console.WriteLine("Unable to bind to the {} folder.", parentWellKnownFolder.ToString());
    }
    if (parentFolder == null)
        return null;
    SearchFilter searchFilter = new SearchFilter.IsEqualTo(FolderSchema.DisplayName, subFolderName);
    FolderView view = new FolderView(10);
    view.PropertySet = new PropertySet(BasePropertySet.IdOnly);
    view.PropertySet.Add(FolderSchema.DisplayName);
    view.Traversal = FolderTraversal.Shallow;
    FindFoldersResults searchResults = null;
    try
    {
        searchResults = parentFolder.FindFolders(searchFilter, view);
    }
    catch (ServiceResponseException ex)
    {
        Console.WriteLine("Error searching for {0} folder: {1}", subFolderName,
            ex.ErrorCode.ToString());
    }
    foreach (Folder subFolder in searchResults.Folders)
    {
        if (subFolder.DisplayName == subFolderName)
            returnId = subFolder.Id;
        break;
    }
    return returnId;
}
```

## <a name="see-also"></a><span data-ttu-id="5335f-165">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="5335f-165">See also</span></span>


- [<span data-ttu-id="5335f-166">Gestion de la boîte de réception et EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="5335f-166">Inbox management and EWS in Exchange</span></span>](inbox-management-and-ews-in-exchange.md)
    
- [<span data-ttu-id="5335f-167">Méthode ExchangeService.GetInboxRules</span><span class="sxs-lookup"><span data-stu-id="5335f-167">ExchangeService.GetInboxRules method</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.getinboxrules%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="5335f-168">Méthode ExchangeService.UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="5335f-168">ExchangeService.UpdateInboxRules method</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.updateinboxrules%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="5335f-169">Opération de GetInboxRules</span><span class="sxs-lookup"><span data-stu-id="5335f-169">GetInboxRules operation</span></span>](http://msdn.microsoft.com/library/b4b2701a-4a23-4acc-8c75-19f7955ad7ae%28Office.15%29.aspx)
    
- [<span data-ttu-id="5335f-170">Opération de UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="5335f-170">UpdateInboxRules operation</span></span>](http://msdn.microsoft.com/library/f982a237-471e-45c5-a2b5-468cfc53150b%28Office.15%29.aspx)
    

