---
title: Opération GetUserSettings (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 758d965c-ef63-4de4-9120-e293abf14ff8
description: L’opération GetUserSettings contient une requête pour la configuration de l’accès au client de l’utilisateur.
ms.openlocfilehash: e274fd4e1ca954ea25ea91a52e363c9a434b290a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466142"
---
# <a name="getusersettings-operation-soap"></a><span data-ttu-id="07bfd-103">Opération GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="07bfd-103">GetUserSettings operation (SOAP)</span></span>

<span data-ttu-id="07bfd-104">L’opération **GetUserSettings** contient une requête pour la configuration de l’accès au client de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="07bfd-104">The **GetUserSettings** operation contains a query for users' client access configuration.</span></span> 
  
## <a name="getusersettings-request-example"></a><span data-ttu-id="07bfd-105">Exemple de requête GetUserSettings</span><span class="sxs-lookup"><span data-stu-id="07bfd-105">GetUserSettings request example</span></span>

### <a name="description"></a><span data-ttu-id="07bfd-106">Description</span><span class="sxs-lookup"><span data-stu-id="07bfd-106">Description</span></span>

<span data-ttu-id="07bfd-107">L’exemple de code XML suivant montre un corps de demande de découverte automatique qui demande le nom d’affichage, le nom unique, l’ID de déploiement, le serveur de boîtes aux lettres, le nom unique de la boîte aux lettres, le serveur Active Directory, la version du serveur d’accès au client et les schémas des services Web Exchange pris en charge.</span><span class="sxs-lookup"><span data-stu-id="07bfd-107">The following XML example shows an Autodiscover request body that requests a user's display name, distinguished name, deployment ID, mailbox server, mailbox distinguished name, Active Directory server, Client Access server version, and supported Exchange Web Services schemas.</span></span>
  
### <a name="code"></a><span data-ttu-id="07bfd-108">Code</span><span class="sxs-lookup"><span data-stu-id="07bfd-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:a="https://schemas.microsoft.com/exchange/2010/Autodiscover"      
               xmlns:wsa="http://www.w3.org/2005/08/addressing" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"      
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <a:RequestedServerVersion>Exchange2010</a:RequestedServerVersion>
    <wsa:Action>https://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetUserSettings</wsa:Action>
    <wsa:To>https://myserver.contoso.com/autodiscover/autodiscover.svc</wsa:To>
  </soap:Header>
  <soap:Body>
    <a:GetUserSettingsRequestMessage xmlns:a="https://schemas.microsoft.com/exchange/2010/Autodiscover">
      <a:Request>
        <a:Users>
          <a:User>
            <a:Mailbox>UserName@domain.contoso.com</a:Mailbox>
          </a:User>
        </a:Users>
        <a:RequestedSettings>
          <a:Setting>UserDisplayName</a:Setting>
          <a:Setting>UserDN</a:Setting>
          <a:Setting>UserDeploymentId</a:Setting>
          <a:Setting>InternalMailboxServer</a:Setting>
          <a:Setting>MailboxDN</a:Setting>
          <a:Setting>ActiveDirectoryServer</a:Setting>
          <a:Setting>CasVersion</a:Setting>
          <a:Setting>EwsSupportedSchemas</a:Setting>
        </a:RequestedSettings>
      </a:Request>
    </a:GetUserSettingsRequestMessage>
  </soap:Body>
</soap:Envelope>

```

### <a name="request-elements"></a><span data-ttu-id="07bfd-109">Demander des éléments</span><span class="sxs-lookup"><span data-stu-id="07bfd-109">Request elements</span></span>

<span data-ttu-id="07bfd-110">Les éléments suivants sont utilisés dans le corps de la demande :</span><span class="sxs-lookup"><span data-stu-id="07bfd-110">The following elements are used in the request body:</span></span>
  
- [<span data-ttu-id="07bfd-111">GetUserSettingsRequestMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="07bfd-111">GetUserSettingsRequestMessage (SOAP)</span></span>](getusersettingsrequestmessage-soap.md)
    
- [<span data-ttu-id="07bfd-112">Boîte aux lettres (SOAP)</span><span class="sxs-lookup"><span data-stu-id="07bfd-112">Mailbox (SOAP)</span></span>](mailbox-soap.md)
    
- [<span data-ttu-id="07bfd-113">Demande (SOAP)</span><span class="sxs-lookup"><span data-stu-id="07bfd-113">Request (SOAP)</span></span>](request-soap.md)
    
- [<span data-ttu-id="07bfd-114">RequestedServerVersion (SOAP)</span><span class="sxs-lookup"><span data-stu-id="07bfd-114">RequestedServerVersion (SOAP)</span></span>](requestedserverversion-soap.md)
    
- [<span data-ttu-id="07bfd-115">RequestedSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="07bfd-115">RequestedSettings (SOAP)</span></span>](requestedsettings-soap.md)
    
- [<span data-ttu-id="07bfd-116">Paramètre (SOAP)</span><span class="sxs-lookup"><span data-stu-id="07bfd-116">Setting (SOAP)</span></span>](setting-soap.md)
    
- [<span data-ttu-id="07bfd-117">Utilisateur (SOAP)</span><span class="sxs-lookup"><span data-stu-id="07bfd-117">User (SOAP)</span></span>](user-soap.md)
    
- [<span data-ttu-id="07bfd-118">Utilisateurs (SOAP)</span><span class="sxs-lookup"><span data-stu-id="07bfd-118">Users (SOAP)</span></span>](users-soap.md)
    
## <a name="getusersettings-response-example"></a><span data-ttu-id="07bfd-119">Exemple de réponse GetUserSettings</span><span class="sxs-lookup"><span data-stu-id="07bfd-119">GetUserSettings response example</span></span>

### <a name="description"></a><span data-ttu-id="07bfd-120">Description</span><span class="sxs-lookup"><span data-stu-id="07bfd-120">Description</span></span>

<span data-ttu-id="07bfd-121">L’exemple suivant montre une réponse **GetUserSettings** réussie.</span><span class="sxs-lookup"><span data-stu-id="07bfd-121">The following example shows a successful **GetUserSettings** response.</span></span> 
  
### <a name="code"></a><span data-ttu-id="07bfd-122">Code</span><span class="sxs-lookup"><span data-stu-id="07bfd-122">Code</span></span>

```XML
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/" xmlns:a="http://www.w3.org/2005/08/addressing">
  <s:Header>
    <a:Action s:mustUnderstand="1">https://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetUserSettingsResponse</a:Action>
  </s:Header>
  <s:Body>
  <GetUserSettingsResponseMessage xmlns="https://schemas.microsoft.com/exchange/2010/Autodiscover">
      <Response xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
        <ErrorCode>NoError</ErrorCode>
        <ErrorMessage />
        <UserResponses>
          <UserResponse>
            <ErrorCode>NoError</ErrorCode>
            <ErrorMessage>No error.</ErrorMessage>
            <RedirectTarget i:nil="true" />
            <UserSettingErrors />
            <UserSettings>
              <UserSetting i:type="StringSetting">
                <Name>UserDisplayName</Name>
                <Value>UserDisplayName</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>UserDN</Name>
                <Value>/o=First Organization/ou=Exchange Administrative Group (SDASDASDJ)/cn=Recipients/cn=UserDisplayName</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>UserDeploymentId</Name>
                <Value>a40E2742-21c6-4050-8Ed2-d41f100c22b8</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>CasVersion</Name>
                <Value>14.00.0478.000</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>EwsSupportedSchemas</Name>
                <Value>Exchange2007,  Exchange2010</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>InternalMailboxServer</Name>
                <Value>machinename.domain.contoso.com</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>ActiveDirectoryServer</Name>
                <Value>machinename.domain.contoso.com</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>MailboxDN</Name>
                <Value>/o=First Organization/ou=Exchange Administrative Group (SDASDASDJ)/cn=Configuration/cn=Servers/cn=server/cn=Contoso Pri MDB</Value>
              </UserSetting>
            </UserSettings>
          </UserResponse>
        </UserResponses>
      </Response>
    </GetUserSettingsResponseMessage>
  </s:Body>
</s:Envelope>
```

### <a name="response-elements"></a><span data-ttu-id="07bfd-123">Éléments Response</span><span class="sxs-lookup"><span data-stu-id="07bfd-123">Response elements</span></span>

<span data-ttu-id="07bfd-124">Les éléments suivants sont utilisés dans le corps de la réponse :</span><span class="sxs-lookup"><span data-stu-id="07bfd-124">The following elements are used in the response body:</span></span>
  
- [<span data-ttu-id="07bfd-125">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="07bfd-125">ErrorCode (SOAP)</span></span>](errorcode-soap.md)
    
- [<span data-ttu-id="07bfd-126">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="07bfd-126">ErrorMessage (SOAP)</span></span>](errormessage-soap.md)
    
- [<span data-ttu-id="07bfd-127">GetUserSettingsResponseMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="07bfd-127">GetUserSettingsResponseMessage (SOAP)</span></span>](getusersettingsresponsemessage-soap.md)
    
- [<span data-ttu-id="07bfd-128">Nom (SOAP)</span><span class="sxs-lookup"><span data-stu-id="07bfd-128">Name (SOAP)</span></span>](name-soap.md)
    
- [<span data-ttu-id="07bfd-129">RedirectTarget (SOAP)</span><span class="sxs-lookup"><span data-stu-id="07bfd-129">RedirectTarget (SOAP)</span></span>](redirecttarget-soap.md)
    
- [<span data-ttu-id="07bfd-130">Réponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="07bfd-130">Response (SOAP)</span></span>](response-soap.md)
    
- [<span data-ttu-id="07bfd-131">UserResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="07bfd-131">UserResponse (SOAP)</span></span>](userresponse-soap.md)
    
- [<span data-ttu-id="07bfd-132">UserResponses (SOAP)</span><span class="sxs-lookup"><span data-stu-id="07bfd-132">UserResponses (SOAP)</span></span>](userresponses-soap.md)
    
- [<span data-ttu-id="07bfd-133">UserSetting (SOAP)</span><span class="sxs-lookup"><span data-stu-id="07bfd-133">UserSetting (SOAP)</span></span>](usersetting-soap.md)
    
- [<span data-ttu-id="07bfd-134">UserSettingErrors (SOAP)</span><span class="sxs-lookup"><span data-stu-id="07bfd-134">UserSettingErrors (SOAP)</span></span>](usersettingerrors-soap.md)
    
- [<span data-ttu-id="07bfd-135">UserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="07bfd-135">UserSettings (SOAP)</span></span>](usersettings-soap.md)
    
- [<span data-ttu-id="07bfd-136">Valeur (SOAP)</span><span class="sxs-lookup"><span data-stu-id="07bfd-136">Value (SOAP)</span></span>](value-soap.md)
    
## <a name="see-also"></a><span data-ttu-id="07bfd-137">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="07bfd-137">See also</span></span>



[<span data-ttu-id="07bfd-138">Opération GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="07bfd-138">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)
  
[<span data-ttu-id="07bfd-139">Opération GetFederationInformation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="07bfd-139">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)


[<span data-ttu-id="07bfd-140">Éléments XML de découverte automatique SOAP pour Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="07bfd-140">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

