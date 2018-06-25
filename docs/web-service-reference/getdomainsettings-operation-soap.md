---
title: Opération GetDomainSettings (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: a6f4a53d-d7f6-4ad1-8afb-78745c500eaa
description: L’opération GetDomainSettings récupère les paramètres du domaine pour l’utilisateur spécifiés. Découverte automatique renvoie les domaines doivent être découvert et les paramètres requis de ces domaines.
ms.openlocfilehash: 09b1d610cd415d2d9d7d0098354521ece86f5184
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756591"
---
# <a name="getdomainsettings-operation-soap"></a><span data-ttu-id="f4e2b-104">Opération GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f4e2b-104">GetDomainSettings operation (SOAP)</span></span>

<span data-ttu-id="f4e2b-105">L’opération **GetDomainSettings** récupère les paramètres du domaine pour l’utilisateur spécifiés.</span><span class="sxs-lookup"><span data-stu-id="f4e2b-105">The **GetDomainSettings** operation retrieves the specified settings of the domain for the user.</span></span> <span data-ttu-id="f4e2b-106">Découverte automatique renvoie les domaines doivent être découvert et les paramètres requis de ces domaines.</span><span class="sxs-lookup"><span data-stu-id="f4e2b-106">Autodiscover returns the domains that are to be discovered and the requested settings of those domains.</span></span> 
  
## <a name="getdomainsettings-request-example"></a><span data-ttu-id="f4e2b-107">Exemple de requête GetDomainSettings</span><span class="sxs-lookup"><span data-stu-id="f4e2b-107">GetDomainSettings request example</span></span>

### <a name="description"></a><span data-ttu-id="f4e2b-108">Description</span><span class="sxs-lookup"><span data-stu-id="f4e2b-108">Description</span></span>

<span data-ttu-id="f4e2b-109">L’exemple suivant d’une demande **GetDomainSettings** illustre une demande pour les paramètres de domaine d’un utilisateur **ExternalEWSUrl** .</span><span class="sxs-lookup"><span data-stu-id="f4e2b-109">The following example of a **GetDomainSettings** request shows a request for a user's **ExternalEWSUrl** domain settings.</span></span> <span data-ttu-id="f4e2b-110">Le client envoie cette demande au serveur.</span><span class="sxs-lookup"><span data-stu-id="f4e2b-110">The client sends this request to the server.</span></span> 
  
### <a name="code"></a><span data-ttu-id="f4e2b-111">Code</span><span class="sxs-lookup"><span data-stu-id="f4e2b-111">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?> 
<soap:Envelope xmlns:a="http://schemas.microsoft.com/exchange/2010/Autodiscover"
               xmlns:wsa="http://www.w3.org/2005/08/addressing"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"> 
    <soap:Header> 
        <a:RequestedServerVersion>Exchange2010</a:RequestedServerVersion>
        <wsa:Action>http://schemas.microsoft.com/exchange/2010/
            Autodiscover/Autodiscover/GetDomainSettings</wsa:Action>
        <wsa:To>
            https://autodiscover.exchange.microsoft.com/autodiscover/autodiscover.svc
        </wsa:To>
    </soap:Header> 
    <soap:Body> 
        <a:GetDomainSettingsRequestMessage xmlns:a="http://schemas.microsoft.com
            /exchange/2010/Autodiscover"> 
            <a:Request> 
                <a:Domains> 
                    <a:Domain>contoso.com<</a:Domain> 
                </a:Domains> 
                <a:RequestedSettings> 
                    <a:Setting>ExternalEwsUrl</a:Setting> 
                </a:RequestedSettings> 
            </a:Request> 
        </a:GetDomainSettingsRequestMessage> 
    </soap:Body> 
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="f4e2b-112">Éléments de la demande</span><span class="sxs-lookup"><span data-stu-id="f4e2b-112">Request elements</span></span>

<span data-ttu-id="f4e2b-113">Les éléments suivants sont utilisés dans la demande :</span><span class="sxs-lookup"><span data-stu-id="f4e2b-113">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="f4e2b-114">GetDomainSettingsRequestMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f4e2b-114">GetDomainSettingsRequestMessage (SOAP)</span></span>](getdomainsettingsrequestmessage-soap.md)
    
- [<span data-ttu-id="f4e2b-115">Demande (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f4e2b-115">Request (SOAP)</span></span>](request-soap.md)
    
- [<span data-ttu-id="f4e2b-116">Domaines (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f4e2b-116">Domains (SOAP)</span></span>](domains-soap.md)
    
- [<span data-ttu-id="f4e2b-117">Domaine (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f4e2b-117">Domain (SOAP)</span></span>](domain-soap.md)
    
- [<span data-ttu-id="f4e2b-118">RequestedSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f4e2b-118">RequestedSettings (SOAP)</span></span>](requestedsettings-soap.md)
    
- [<span data-ttu-id="f4e2b-119">Paramètre (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f4e2b-119">Setting (SOAP)</span></span>](setting-soap.md)
    
## <a name="getdomainsettings-response-example"></a><span data-ttu-id="f4e2b-120">Exemple de réponse GetDomainSettings</span><span class="sxs-lookup"><span data-stu-id="f4e2b-120">GetDomainSettings response example</span></span>

### <a name="description"></a><span data-ttu-id="f4e2b-121">Description</span><span class="sxs-lookup"><span data-stu-id="f4e2b-121">Description</span></span>

<span data-ttu-id="f4e2b-122">L’exemple suivant montre une réponse positive à la demande **GetDomainSettings** que le serveur envoie au client.</span><span class="sxs-lookup"><span data-stu-id="f4e2b-122">The following example shows a successful response to the **GetDomainSettings** request that the server sends to the client.</span></span> 
  
### <a name="code"></a><span data-ttu-id="f4e2b-123">Code</span><span class="sxs-lookup"><span data-stu-id="f4e2b-123">Code</span></span>

```XML
//www.w3.org/2005/08/addressing"> 
    <s:Header> 
        <a:Action s:mustUnderstand="1">http://schemas.microsoft.com/exchange/2010/ 
            Autodiscover/Autodiscover/GetDomainSettingsResponse
        </a:Action> 
        <h:ServerVersionInfo xmlns:h="http://schemas.microsoft.com/exchange/2010/Autodiscover" 
            xmlns:i="http://www.w3.org/2001/XMLSchema-instance"> 
        <h:MajorVersion>14</h:MajorVersion> 
        <h:MinorVersion>0</h:MinorVersion> 
        <h:MajorBuildNumber>639</h:MajorBuildNumber> 
        <h:MinorBuildNumber>20</h:MinorBuildNumber> 
        <h:Version>Exchange2010</h:Version> 
        </h:ServerVersionInfo>
    </s:Header> 
    <s:Body> 
        <GetDomainSettingsResponseMessage xmlns="http://schemas.microsoft.com/exchange/2010/Autodiscover"> 
            <Response xmlns:i="http://www.w3.org/2001/XMLSchema-instance"> 
                <ErrorCode>NoError</ErrorCode> 
                <ErrorMessage /> 
                <DomainResponses> 
                    <DomainResponse> 
                        <ErrorCode>NoError</ErrorCode> 
                        <ErrorMessage>No error.</ErrorMessage> 
                        <DomainSettingErrors /> 
                        <DomainSettings> 
                            <DomainSetting i:type="DomainStringSetting"> 
                                <Name>ExternalEwsUrl</Name> 
                                <Value>https://emea.mail.microsoft.com/EWS/Exchange.asmx</Value> 
                            </DomainSetting> 
                        </DomainSettings> 
                        <RedirectTarget i:nil="true" /> 
                    </DomainResponse> 
                </DomainResponses> 
            </Response> 
        </GetDomainSettingsResponseMessage> 
    </s:Body> 
</s:Envelope>
```

### <a name="response-elements"></a><span data-ttu-id="f4e2b-124">Éléments de réponse</span><span class="sxs-lookup"><span data-stu-id="f4e2b-124">Response elements</span></span>

<span data-ttu-id="f4e2b-125">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="f4e2b-125">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="f4e2b-126">GetDomainSettingsResponseMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f4e2b-126">GetDomainSettingsResponseMessage (SOAP)</span></span>](getdomainsettingsresponsemessage-soap.md)
    
- [<span data-ttu-id="f4e2b-127">Réponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f4e2b-127">Response (SOAP)</span></span>](response-soap.md)
    
- [<span data-ttu-id="f4e2b-128">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f4e2b-128">ErrorCode (SOAP)</span></span>](errorcode-soap.md)
    
- [<span data-ttu-id="f4e2b-129">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f4e2b-129">ErrorMessage (SOAP)</span></span>](errormessage-soap.md)
    
- [<span data-ttu-id="f4e2b-130">DomainResponses (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f4e2b-130">DomainResponses (SOAP)</span></span>](domainresponses-soap.md)
    
- [<span data-ttu-id="f4e2b-131">DomainResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f4e2b-131">DomainResponse (SOAP)</span></span>](domainresponse-soap.md)
    
- [<span data-ttu-id="f4e2b-132">DomainSettingErrors (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f4e2b-132">DomainSettingErrors (SOAP)</span></span>](domainsettingerrors-soap.md)
    
- [<span data-ttu-id="f4e2b-133">DomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f4e2b-133">DomainSettings (SOAP)</span></span>](domainsettings-soap.md)
    
- [<span data-ttu-id="f4e2b-134">DomainSetting (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f4e2b-134">DomainSetting (SOAP)</span></span>](domainsetting-soap.md)
    
- [<span data-ttu-id="f4e2b-135">Nom (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f4e2b-135">Name (SOAP)</span></span>](name-soap.md)
    
- [<span data-ttu-id="f4e2b-136">Valeur (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f4e2b-136">Value (SOAP)</span></span>](value-soap.md)
    
- [<span data-ttu-id="f4e2b-137">RedirectTarget (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f4e2b-137">RedirectTarget (SOAP)</span></span>](redirecttarget-soap.md)
    
## <a name="see-also"></a><span data-ttu-id="f4e2b-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f4e2b-138">See also</span></span>



[<span data-ttu-id="f4e2b-139">Opération GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f4e2b-139">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
  
[<span data-ttu-id="f4e2b-140">Opération GetFederationInformation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f4e2b-140">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)

