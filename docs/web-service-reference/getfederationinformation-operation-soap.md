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
description: L’opération GetFederationInformation fournit des informations sur l’état de la fédération de l’organisation, telles que l’URI à utiliser lors de la demande de jetons sont destinés à cette organisation et les autres domaines que l’organisation a également cible fédérés.
ms.openlocfilehash: bf38b2f2b3db3e38b9b0157d1677efe4fc274e1b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756618"
---
# <a name="getfederationinformation-operation-soap"></a><span data-ttu-id="28952-103">Opération GetFederationInformation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="28952-103">GetFederationInformation operation (SOAP)</span></span>

<span data-ttu-id="28952-104">L’opération **GetFederationInformation** fournit des informations sur l’état de la fédération de l’organisation, telles que la cible URI à utiliser lors de la demande de jetons qui sont destinés à cette organisation et les autres domaines qui l’organisation a également fédérés.</span><span class="sxs-lookup"><span data-stu-id="28952-104">The **GetFederationInformation** operation provides information about the federation status of the organization, such as the target URI to be used when requesting tokens that are targeted at this organization, and the other domains that the organization has also federated.</span></span> 
  
<span data-ttu-id="28952-105">Les organisations fédérées uniquement peuvent partager Calendrier, des contacts et des messages aux utilisateurs externes.</span><span class="sxs-lookup"><span data-stu-id="28952-105">Only federated organizations can share calendar, contacts, and messages to external users.</span></span>
  
## <a name="getfederationinformation-request-example"></a><span data-ttu-id="28952-106">Exemple de requête GetFederationInformation</span><span class="sxs-lookup"><span data-stu-id="28952-106">GetFederationInformation request example</span></span>

### <a name="description"></a><span data-ttu-id="28952-107">Description</span><span class="sxs-lookup"><span data-stu-id="28952-107">Description</span></span>

<span data-ttu-id="28952-108">L’exemple suivant d’une demande **GetFederationInformation** montre une demande d’informations sur la fédération d’un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="28952-108">The following example of a **GetFederationInformation** request shows a request for a user's federation information.</span></span> <span data-ttu-id="28952-109">Le client envoie cette demande au serveur.</span><span class="sxs-lookup"><span data-stu-id="28952-109">The client sends this request to the server.</span></span> 
  
### <a name="code"></a><span data-ttu-id="28952-110">Code</span><span class="sxs-lookup"><span data-stu-id="28952-110">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?> 
<soap:Envelope xmlns:exm="http://schemas.microsoft.com/exchange/services/2006/messages"
           xmlns:ext="http://schemas.microsoft.com/exchange/services/2006/types"
           xmlns:a="http://www.w3.org/2005/08/addressing"
           xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema"> 
    <soap:Header> 
        <a:MessageID>urn:uuid:6389558d-9e05-465e-ade9-aae14c4bcd10</a:MessageID> 
        <a:Action soap:mustUnderstand="1">http://schemas.microsoft.com/
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
            xmlns="http://schemas.microsoft.com/exchange/2010/Autodiscover"> 
            <Request> 
                <Domain>contoso.com</Domain> 
            </Request> 
        </GetFederationInformationRequestMessage>
    </soap:Body> 
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="28952-111">Éléments de la demande</span><span class="sxs-lookup"><span data-stu-id="28952-111">Request elements</span></span>

<span data-ttu-id="28952-112">Les éléments suivants sont utilisés dans la demande :</span><span class="sxs-lookup"><span data-stu-id="28952-112">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="28952-113">GetFederationInformationRequestMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="28952-113">GetFederationInformationRequestMessage (SOAP)</span></span>](getfederationinformationrequestmessage-soap.md)
    
- [<span data-ttu-id="28952-114">Demande (SOAP)</span><span class="sxs-lookup"><span data-stu-id="28952-114">Request (SOAP)</span></span>](request-soap.md)
    
- [<span data-ttu-id="28952-115">Domaine (SOAP)</span><span class="sxs-lookup"><span data-stu-id="28952-115">Domain (SOAP)</span></span>](domain-soap.md)
    
## <a name="getfederationinformation-response-example"></a><span data-ttu-id="28952-116">Exemple de réponse GetFederationInformation</span><span class="sxs-lookup"><span data-stu-id="28952-116">GetFederationInformation response example</span></span>

### <a name="description"></a><span data-ttu-id="28952-117">Description</span><span class="sxs-lookup"><span data-stu-id="28952-117">Description</span></span>

<span data-ttu-id="28952-118">L’exemple suivant montre une réponse positive à la demande **GetFederationInformation** que le serveur envoie au client.</span><span class="sxs-lookup"><span data-stu-id="28952-118">The following example shows a successful response to the **GetFederationInformation** request that the server sends to the client.</span></span> 
  
### <a name="code"></a><span data-ttu-id="28952-119">Code</span><span class="sxs-lookup"><span data-stu-id="28952-119">Code</span></span>

```XML
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/" 
xmlns:a="http://www.w3.org/2005/08/addressing"> 
    <s:Header> 
        <a:Action s:mustUnderstand="1">
            http://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetFederationInformationResponse
        </a:Action> 
        <a:RelatesTo>urn:uuid:6389558d-9e05-465e-ade9-aae14c4bcd10</a:RelatesTo> 
    </s:Header> 
    <s:Body> 
        <GetFederationInformationResponseMessage xmlns="http://schemas.microsoft.com/exchange/2010/Autodiscover"> 
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

### <a name="response-elements"></a><span data-ttu-id="28952-120">Éléments de réponse</span><span class="sxs-lookup"><span data-stu-id="28952-120">Response elements</span></span>

<span data-ttu-id="28952-121">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="28952-121">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="28952-122">GetFederationInformationResponseMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="28952-122">GetFederationInformationResponseMessage (SOAP)</span></span>](getfederationinformationresponsemessage-soap.md)
    
- [<span data-ttu-id="28952-123">Réponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="28952-123">Response (SOAP)</span></span>](response-soap.md)
    
- [<span data-ttu-id="28952-124">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="28952-124">ErrorCode (SOAP)</span></span>](errorcode-soap.md)
    
- [<span data-ttu-id="28952-125">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="28952-125">ErrorMessage (SOAP)</span></span>](errormessage-soap.md)
    
- [<span data-ttu-id="28952-126">ApplicationUri (SOAP)</span><span class="sxs-lookup"><span data-stu-id="28952-126">ApplicationUri (SOAP)</span></span>](applicationuri-soap.md)
    
- [<span data-ttu-id="28952-127">Domaines (SOAP)</span><span class="sxs-lookup"><span data-stu-id="28952-127">Domains (SOAP)</span></span>](domains-soap.md)
    
- [<span data-ttu-id="28952-128">Domaine (SOAP)</span><span class="sxs-lookup"><span data-stu-id="28952-128">Domain (SOAP)</span></span>](domain-soap.md)
    
## <a name="see-also"></a><span data-ttu-id="28952-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="28952-129">See also</span></span>

- [<span data-ttu-id="28952-130">Opération GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="28952-130">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
- [<span data-ttu-id="28952-131">Opération GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="28952-131">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

