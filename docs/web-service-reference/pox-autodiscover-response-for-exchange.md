---
title: Réponse de découverte automatique variole pour Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 08c6c5a2-a67a-4141-a8bd-1b5d560b90a7
description: La réponse de découverte automatique contient une réponse à une demande de découverte automatique qui inclut une liste d’URL qui sont utilisées pour établir une liaison avec Exchange Web Services (EWS).
ms.openlocfilehash: d9f8a5cc86efaa4dceda7385164872ecc5409252
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828863"
---
# <a name="pox-autodiscover-response-for-exchange"></a><span data-ttu-id="55607-103">Réponse de découverte automatique variole pour Exchange</span><span class="sxs-lookup"><span data-stu-id="55607-103">POX Autodiscover response for Exchange</span></span>

<span data-ttu-id="55607-104">La réponse de découverte automatique contient une réponse à une demande de découverte automatique qui inclut une liste d’URL qui sont utilisées pour établir une liaison avec Exchange Web Services (EWS).</span><span class="sxs-lookup"><span data-stu-id="55607-104">The Autodiscover response contains a response to an Autodiscover request that includes a list of URLs that are used to establish a binding with Exchange Web Services (EWS).</span></span>
  
## <a name="autodiscover-response-example"></a><span data-ttu-id="55607-105">Exemple de réponse de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="55607-105">Autodiscover response example</span></span>

### <a name="description"></a><span data-ttu-id="55607-106">Description</span><span class="sxs-lookup"><span data-stu-id="55607-106">Description</span></span>

<span data-ttu-id="55607-107">L’exemple suivant montre une réponse positive de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="55607-107">The following example shows a successful Autodiscover response.</span></span>
  
### <a name="code"></a><span data-ttu-id="55607-108">Code</span><span class="sxs-lookup"><span data-stu-id="55607-108">Code</span></span>

```XML
<Autodiscover xmlns="http://schemas.microsoft.com/exchange/autodiscover/responseschema/2006">
  <Response xmlns="http://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a">
    <User>
      <DisplayName>First Last</DisplayName>
      <LegacyDN>/o=contoso/ou=First Administrative Group/cn=Recipients/cn=iuser885646</LegacyDN>
      <DeploymentId>644560b8-a1ce-429c-8ace-23395843f701</DeploymentId>
    </User>
    <Account>
      <AccountType>email</AccountType>
      <Action>settings</Action>
      <Protocol>
        <Type>EXCH</Type>
        <Server>MBX-SERVER.mail.internal.contoso.com</Server>
        <ServerDN>/o=contoso/ou=Exchange Administrative Group (FYDIBOHF23SPDLT)/cn=Configuration/cn=Servers/cn=MBX-SERVER</ServerDN>
        <ServerVersion>72008287</ServerVersion>
        <MdbDN>/o=contoso/ou=Exchange Administrative Group (FYDIBOHF23SPDLT)/cn=Configuration/cn=Servers/cn=MBX-SERVER/cn=Microsoft Private MDB</MdbDN>
        <ASUrl>https://mail.contoso.com/ews/exchange.asmx</ASUrl>
        <OOFUrl>https://mail.contoso.com/ews/exchange.asmx</OOFUrl>
        <UMUrl>https://mail.contoso.com/unifiedmessaging/service.asmx</UMUrl>
        <OABUrl>https://mail.contoso.com/OAB/d29844a9-724e-468c-8820-0f7b345b767b/</OABUrl>
      </Protocol>
      <Protocol>
        <Type>EXPR</Type>
        <Server>Exchange.contoso.com</Server>
        <ASUrl>https://mail.contoso.com/ews/exchange.asmx</ASUrl>
        <OOFUrl>https://mail.contoso.com/ews/exchange.asmx</OOFUrl>
        <UMUrl>https://mail.contoso.com/unifiedmessaging/service.asmx</UMUrl>
        <OABUrl>https://mail.contoso.com/OAB/d29844a9-724e-468c-8820-0f7b345b767b/</OABUrl>
      </Protocol>
      <Protocol>
        <Type>WEB</Type>
        <Internal>
          <OWAUrl AuthenticationMethod="Ntlm, WindowsIntegrated">https://cas-01-server.mail.internal.contoso.com/owa</OWAUrl>
          <OWAUrl AuthenticationMethod="Ntlm, WindowsIntegrated">https://cas-02-server.mail.internal.contoso.com/owa</OWAUrl>
          <OWAUrl AuthenticationMethod="Basic">https://cas-04-server.mail.internal.contoso.com/owa</OWAUrl>
          <OWAUrl AuthenticationMethod="Ntlm, WindowsIntegrated">https://cas-05-server.mail.internal.contoso.com/owa</OWAUrl>
        </Internal>
      </Protocol>
    </Account>
  </Response>
</Autodiscover>
```

### <a name="comments"></a><span data-ttu-id="55607-109">Commentaires</span><span class="sxs-lookup"><span data-stu-id="55607-109">Comments</span></span>

<span data-ttu-id="55607-110">Pour lier aux Services Web Exchange, utilisez l’URL identifié par l’élément [ASUrl (POX)](asurl-pox.md) .</span><span class="sxs-lookup"><span data-stu-id="55607-110">To bind to Exchange Web Services, use the URL identified by the [ASUrl (POX)](asurl-pox.md) element.</span></span> 
  
### <a name="response-element"></a><span data-ttu-id="55607-111">Response, élément</span><span class="sxs-lookup"><span data-stu-id="55607-111">Response Element</span></span>

<span data-ttu-id="55607-112">Les éléments suivants sont utilisés dans le corps de réponse :</span><span class="sxs-lookup"><span data-stu-id="55607-112">The following elements are used in the response body:</span></span>
  
- [<span data-ttu-id="55607-113">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="55607-113">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
    
- [<span data-ttu-id="55607-114">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="55607-114">Response (POX)</span></span>](response-pox.md)
    
- [<span data-ttu-id="55607-115">Utilisateur (POX)</span><span class="sxs-lookup"><span data-stu-id="55607-115">User (POX)</span></span>](user-pox.md)
    
- [<span data-ttu-id="55607-116">DisplayName (POX)</span><span class="sxs-lookup"><span data-stu-id="55607-116">DisplayName (POX)</span></span>](displayname-pox.md)
    
- [<span data-ttu-id="55607-117">LegacyDN (POX)</span><span class="sxs-lookup"><span data-stu-id="55607-117">LegacyDN (POX)</span></span>](legacydn-pox.md)
    
- [<span data-ttu-id="55607-118">DeploymentId (POX)</span><span class="sxs-lookup"><span data-stu-id="55607-118">DeploymentId (POX)</span></span>](deploymentid-pox.md)
    
- [<span data-ttu-id="55607-119">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="55607-119">Account (POX)</span></span>](account-pox.md)
    
- [<span data-ttu-id="55607-120">AccountType (POX)</span><span class="sxs-lookup"><span data-stu-id="55607-120">AccountType (POX)</span></span>](accounttype-pox.md)
    
- [<span data-ttu-id="55607-121">Action (POX)</span><span class="sxs-lookup"><span data-stu-id="55607-121">Action (POX)</span></span>](action-pox.md)
    
- [<span data-ttu-id="55607-122">Protocole (POX)</span><span class="sxs-lookup"><span data-stu-id="55607-122">Protocol (POX)</span></span>](protocol-pox.md)
    
- [<span data-ttu-id="55607-123">Type (POX)</span><span class="sxs-lookup"><span data-stu-id="55607-123">Type (POX)</span></span>](type-pox.md)
    
- [<span data-ttu-id="55607-124">Serveur (POX)</span><span class="sxs-lookup"><span data-stu-id="55607-124">Server (POX)</span></span>](server-pox.md)
    
- [<span data-ttu-id="55607-125">ServerDN (POX)</span><span class="sxs-lookup"><span data-stu-id="55607-125">ServerDN (POX)</span></span>](serverdn-pox.md)
    
- [<span data-ttu-id="55607-126">ServerVersion (POX)</span><span class="sxs-lookup"><span data-stu-id="55607-126">ServerVersion (POX)</span></span>](serverversion-pox.md)
    
- [<span data-ttu-id="55607-127">MdbDN (POX)</span><span class="sxs-lookup"><span data-stu-id="55607-127">MdbDN (POX)</span></span>](mdbdn-pox.md)
    
- [<span data-ttu-id="55607-128">ASUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="55607-128">ASUrl (POX)</span></span>](asurl-pox.md)
    
- [<span data-ttu-id="55607-129">OOFUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="55607-129">OOFUrl (POX)</span></span>](oofurl-pox.md)
    
- [<span data-ttu-id="55607-130">UMUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="55607-130">UMUrl (POX)</span></span>](umurl-pox.md)
    
- [<span data-ttu-id="55607-131">OABUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="55607-131">OABUrl (POX)</span></span>](oaburl-pox.md)
    
- [<span data-ttu-id="55607-132">Interne (POX)</span><span class="sxs-lookup"><span data-stu-id="55607-132">Internal (POX)</span></span>](internal-pox.md)
    
- [<span data-ttu-id="55607-133">OWAUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="55607-133">OWAUrl (POX)</span></span>](owaurl-pox.md)
    
## <a name="autodiscover-error-response-example"></a><span data-ttu-id="55607-134">Exemple de réponse d’erreur de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="55607-134">Autodiscover Error response example</span></span>

### <a name="description"></a><span data-ttu-id="55607-135">Description</span><span class="sxs-lookup"><span data-stu-id="55607-135">Description</span></span>

<span data-ttu-id="55607-136">L’exemple suivant montre une réponse d’erreur de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="55607-136">The following example shows an Autodiscover error response.</span></span>
  
### <a name="code"></a><span data-ttu-id="55607-137">Code</span><span class="sxs-lookup"><span data-stu-id="55607-137">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<Autodiscover xmlns="http://schemas.microsoft.com/exchange/autodiscover/responseschema/2006">
  <Response xmlns="http://schemas.microsoft.com/exchange/autodiscover/responseschema/2006">
    <Error Time="21:25:04.8897083" Id="4130155072">
      <ErrorCode>600</ErrorCode>
      <Message>Invalid Request</Message>
      <DebugData />
    </Error>
  </Response>
</Autodiscover>
```

### <a name="error-response-element"></a><span data-ttu-id="55607-138">Élément de réponse d’erreur</span><span class="sxs-lookup"><span data-stu-id="55607-138">Error response element</span></span>

<span data-ttu-id="55607-139">Les éléments suivants sont utilisés dans le corps de réponse :</span><span class="sxs-lookup"><span data-stu-id="55607-139">The following elements are used in the response body:</span></span>
  
- [<span data-ttu-id="55607-140">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="55607-140">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
    
- [<span data-ttu-id="55607-141">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="55607-141">Response (POX)</span></span>](response-pox.md)
    
- [<span data-ttu-id="55607-142">Erreur (POX)</span><span class="sxs-lookup"><span data-stu-id="55607-142">Error (POX)</span></span>](error-pox.md)
    
- [<span data-ttu-id="55607-143">ErrorCode (POX)</span><span class="sxs-lookup"><span data-stu-id="55607-143">ErrorCode (POX)</span></span>](errorcode-pox.md)
    
- [<span data-ttu-id="55607-144">Message (POX)</span><span class="sxs-lookup"><span data-stu-id="55607-144">Message (POX)</span></span>](message-pox.md)
    
- [<span data-ttu-id="55607-145">DebugData (POX)</span><span class="sxs-lookup"><span data-stu-id="55607-145">DebugData (POX)</span></span>](debugdata-pox.md)
    
## <a name="see-also"></a><span data-ttu-id="55607-146">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="55607-146">See also</span></span>

- [<span data-ttu-id="55607-147">Demande de découverte automatique variole pour Exchange</span><span class="sxs-lookup"><span data-stu-id="55607-147">POX Autodiscover request for Exchange</span></span>](pox-autodiscover-request-for-exchange.md)
- [<span data-ttu-id="55607-148">Référence de service web variole découverte automatique pour Exchange</span><span class="sxs-lookup"><span data-stu-id="55607-148">POX Autodiscover web service reference for Exchange</span></span>](pox-autodiscover-web-service-reference-for-exchange.md) 
- [<span data-ttu-id="55607-149">Éléments du fichier XML Autodiscover variole pour Exchange</span><span class="sxs-lookup"><span data-stu-id="55607-149">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

