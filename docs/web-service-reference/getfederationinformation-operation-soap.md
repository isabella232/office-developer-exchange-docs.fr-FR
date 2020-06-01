---
title: Opération GetFederationInformation (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: c6666a42-a18f-4e4b-beb6-b25ff62cfcc5
description: L’opération GetFederationInformation fournit des informations sur l’état de la Fédération de l’organisation, telles que l’URI cible à utiliser lors de la demande de jetons ciblés dans cette organisation, ainsi que sur les autres domaines que l’organisation a également fédérés.
ms.openlocfilehash: 533b2f6d282e3287f4945df56b169f5bc93ff445
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455624"
---
# <a name="getfederationinformation-operation-soap"></a><span data-ttu-id="44b65-103">Opération GetFederationInformation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="44b65-103">GetFederationInformation operation (SOAP)</span></span>

<span data-ttu-id="44b65-104">L’opération **GetFederationInformation** fournit des informations sur l’état de la Fédération de l’organisation, telles que l’URI cible à utiliser lors de la demande de jetons ciblés dans cette organisation, ainsi que sur les autres domaines que l’organisation a également fédérés.</span><span class="sxs-lookup"><span data-stu-id="44b65-104">The **GetFederationInformation** operation provides information about the federation status of the organization, such as the target URI to be used when requesting tokens that are targeted at this organization, and the other domains that the organization has also federated.</span></span> 
  
<span data-ttu-id="44b65-105">Seules les organisations fédérées peuvent partager du calendrier, des contacts et des messages avec des utilisateurs externes.</span><span class="sxs-lookup"><span data-stu-id="44b65-105">Only federated organizations can share calendar, contacts, and messages to external users.</span></span>
  
## <a name="getfederationinformation-request-example"></a><span data-ttu-id="44b65-106">Exemple de requête GetFederationInformation</span><span class="sxs-lookup"><span data-stu-id="44b65-106">GetFederationInformation request example</span></span>

### <a name="description"></a><span data-ttu-id="44b65-107">Description</span><span class="sxs-lookup"><span data-stu-id="44b65-107">Description</span></span>

<span data-ttu-id="44b65-108">L’exemple suivant de requête **GetFederationInformation** affiche une demande d’informations de Fédération d’un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="44b65-108">The following example of a **GetFederationInformation** request shows a request for a user's federation information.</span></span> <span data-ttu-id="44b65-109">Le client envoie cette demande au serveur.</span><span class="sxs-lookup"><span data-stu-id="44b65-109">The client sends this request to the server.</span></span> 
  
### <a name="code"></a><span data-ttu-id="44b65-110">Code</span><span class="sxs-lookup"><span data-stu-id="44b65-110">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?> 
<soap:Envelope xmlns:exm="https://schemas.microsoft.com/exchange/services/2006/messages"
           xmlns:ext="https://schemas.microsoft.com/exchange/services/2006/types"
           xmlns:a="http://www.w3.org/2005/08/addressing"
           xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema"> 
    <soap:Header> 
        <a:MessageID>urn:uuid:6389558d-9e05-465e-ade9-aae14c4bcd10</a:MessageID> 
        <a:Action soap:mustUnderstand="1">https://schemas.microsoft.com/
            exchange/2010/Autodiscover/Autodiscover/GetFederationInformation
        </a:Action> 
        <a:To soap:mustUnderstand="1">https://autodiscover.byfcxu-
            dom.extest.microsoft.com/autodiscover/autodiscover.svc</a:To> 
        <a:ReplyTo>
            <a:Address>http://www.w3.org/2005/08/addressing/anonymous</a:Address> 
        </a:ReplyTo> 
    </soap:Header> 
    <soap:Body> 
        <GetFederationInformationRequestMessage 
            xmlns="https://schemas.microsoft.com/exchange/2010/Autodiscover"> 
            <Request> 
                <Domain>contoso.com</Domain> 
            </Request> 
        </GetFederationInformationRequestMessage>
    </soap:Body> 
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="44b65-111">Demander des éléments</span><span class="sxs-lookup"><span data-stu-id="44b65-111">Request elements</span></span>

<span data-ttu-id="44b65-112">Les éléments suivants sont utilisés dans la demande :</span><span class="sxs-lookup"><span data-stu-id="44b65-112">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="44b65-113">GetFederationInformationRequestMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="44b65-113">GetFederationInformationRequestMessage (SOAP)</span></span>](getfederationinformationrequestmessage-soap.md)
    
- [<span data-ttu-id="44b65-114">Demande (SOAP)</span><span class="sxs-lookup"><span data-stu-id="44b65-114">Request (SOAP)</span></span>](request-soap.md)
    
- [<span data-ttu-id="44b65-115">Domaine (SOAP)</span><span class="sxs-lookup"><span data-stu-id="44b65-115">Domain (SOAP)</span></span>](domain-soap.md)
    
## <a name="getfederationinformation-response-example"></a><span data-ttu-id="44b65-116">Exemple de réponse GetFederationInformation</span><span class="sxs-lookup"><span data-stu-id="44b65-116">GetFederationInformation response example</span></span>

### <a name="description"></a><span data-ttu-id="44b65-117">Description</span><span class="sxs-lookup"><span data-stu-id="44b65-117">Description</span></span>

<span data-ttu-id="44b65-118">L’exemple suivant montre une réponse réussie à la demande **GetFederationInformation** que le serveur envoie au client.</span><span class="sxs-lookup"><span data-stu-id="44b65-118">The following example shows a successful response to the **GetFederationInformation** request that the server sends to the client.</span></span> 
  
### <a name="code"></a><span data-ttu-id="44b65-119">Code</span><span class="sxs-lookup"><span data-stu-id="44b65-119">Code</span></span>

```XML
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/" 
xmlns:a="http://www.w3.org/2005/08/addressing"> 
    <s:Header> 
        <a:Action s:mustUnderstand="1">
            https://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetFederationInformationResponse
        </a:Action> 
        <a:RelatesTo>urn:uuid:6389558d-9e05-465e-ade9-aae14c4bcd10</a:RelatesTo> 
    </s:Header> 
    <s:Body> 
        <GetFederationInformationResponseMessage xmlns="https://schemas.microsoft.com/exchange/2010/Autodiscover"> 
            <Response xmlns:i="http://www.w3.org/2001/XMLSchema-instance"> 
                <ErrorCode>NoError</ErrorCode> 
                <ErrorMessage/> 
                <ApplicationUri>BYFCXU-DOM.EXTEST.MICROSOFT.COM</ApplicationUri> 
                <Domains> 
                    <Domain>contoso.com</Domain> 
                    <Domain>europe.contoso.com</Domain> 
                    <Domain>americas.contoso.com</Domain> 
                    <Domain>contosolive.com</Domain> 
                </Domains> 
            </Response> 
        </GetFederationInformationResponseMessage> 
    </s:Body> 
</s:Envelope>
```

### <a name="response-elements"></a><span data-ttu-id="44b65-120">Éléments Response</span><span class="sxs-lookup"><span data-stu-id="44b65-120">Response elements</span></span>

<span data-ttu-id="44b65-121">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="44b65-121">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="44b65-122">GetFederationInformationResponseMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="44b65-122">GetFederationInformationResponseMessage (SOAP)</span></span>](getfederationinformationresponsemessage-soap.md)
    
- [<span data-ttu-id="44b65-123">Réponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="44b65-123">Response (SOAP)</span></span>](response-soap.md)
    
- [<span data-ttu-id="44b65-124">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="44b65-124">ErrorCode (SOAP)</span></span>](errorcode-soap.md)
    
- [<span data-ttu-id="44b65-125">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="44b65-125">ErrorMessage (SOAP)</span></span>](errormessage-soap.md)
    
- [<span data-ttu-id="44b65-126">ApplicationUri (SOAP)</span><span class="sxs-lookup"><span data-stu-id="44b65-126">ApplicationUri (SOAP)</span></span>](applicationuri-soap.md)
    
- [<span data-ttu-id="44b65-127">Domaines (SOAP)</span><span class="sxs-lookup"><span data-stu-id="44b65-127">Domains (SOAP)</span></span>](domains-soap.md)
    
- [<span data-ttu-id="44b65-128">Domaine (SOAP)</span><span class="sxs-lookup"><span data-stu-id="44b65-128">Domain (SOAP)</span></span>](domain-soap.md)
    
## <a name="see-also"></a><span data-ttu-id="44b65-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="44b65-129">See also</span></span>

- [<span data-ttu-id="44b65-130">Opération GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="44b65-130">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
- [<span data-ttu-id="44b65-131">Opération GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="44b65-131">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

