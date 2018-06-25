---
title: Opération GetClientAccessToken
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 086876cc-e22c-4e89-89f9-19e78af51217
description: Opération de recherche plus d’informations sur la GetClientAccessToken EWS.
ms.openlocfilehash: afa9a315a8421f31c345c9547a5d80bed41e9fbc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756539"
---
# <a name="getclientaccesstoken-operation"></a><span data-ttu-id="e5226-103">Opération GetClientAccessToken</span><span class="sxs-lookup"><span data-stu-id="e5226-103">GetClientAccessToken operation</span></span>

<span data-ttu-id="e5226-104">Trouvez des informations sur l’opération EWS **GetClientAccessToken** .</span><span class="sxs-lookup"><span data-stu-id="e5226-104">Find information about the **GetClientAccessToken** EWS operation.</span></span> 
  
<span data-ttu-id="e5226-105">L’opération **GetClientAccessToken** Obtient un accès au client jeton pour une application de messagerie pour Outlook.</span><span class="sxs-lookup"><span data-stu-id="e5226-105">The **GetClientAccessToken** operation gets a client access token for a mail app for Outlook.</span></span> 
  
<span data-ttu-id="e5226-106">Cette opération est une nouveauté d’Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="e5226-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getclientaccesstoken-operation"></a><span data-ttu-id="e5226-107">Utilisation de l’opération GetClientAccessToken</span><span class="sxs-lookup"><span data-stu-id="e5226-107">Using the GetClientAccessToken operation</span></span>

<span data-ttu-id="e5226-108">La requête d’opération **GetClientAccessToken** accepte deux arguments requis : l’identificateur de l’application et le type de jeton.</span><span class="sxs-lookup"><span data-stu-id="e5226-108">The **GetClientAccessToken** operation request takes two required arguments: the identifier of the app, and the token type.</span></span> <span data-ttu-id="e5226-109">Vous pouvez utiliser l' [opération GetAppManifests](getappmanifests-operation.md) pour demander l’identificateur de l’application.</span><span class="sxs-lookup"><span data-stu-id="e5226-109">You can use the [GetAppManifests operation](getappmanifests-operation.md) to request the app identifier.</span></span> 
  
### <a name="getclientaccesstoken-operation-soap-headers"></a><span data-ttu-id="e5226-110">En-têtes SOAP GetClientAccessToken opération</span><span class="sxs-lookup"><span data-stu-id="e5226-110">GetClientAccessToken operation SOAP headers</span></span>

<span data-ttu-id="e5226-111">L’opération **GetClientAccessToken** permettre utiliser les en-têtes SOAP qui sont répertoriés dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="e5226-111">The **GetClientAccessToken** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="e5226-112">**Nom de l'en-tête**</span><span class="sxs-lookup"><span data-stu-id="e5226-112">**Header name**</span></span>|<span data-ttu-id="e5226-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e5226-113">**Element**</span></span>|<span data-ttu-id="e5226-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="e5226-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="e5226-115">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="e5226-115">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="e5226-116">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="e5226-116">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="e5226-117">Identifie la version du schéma pour la requête d’opération.</span><span class="sxs-lookup"><span data-stu-id="e5226-117">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="e5226-118">Cet en-tête est applicable à une demande.</span><span class="sxs-lookup"><span data-stu-id="e5226-118">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="e5226-119">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="e5226-119">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="e5226-120">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="e5226-120">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="e5226-121">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="e5226-121">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="e5226-122">Cet en-tête est applicable à une réponse.</span><span class="sxs-lookup"><span data-stu-id="e5226-122">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getclientaccesstoken-operation-request-example-get-a-caller-identity-token"></a><span data-ttu-id="e5226-123">Exemple de requête d’opération GetClientAccessToken : obtenir le jeton une identité de l’appelant</span><span class="sxs-lookup"><span data-stu-id="e5226-123">GetClientAccessToken operation request example: Get a caller identity token</span></span>

<span data-ttu-id="e5226-124">Une demande d’opération **GetClientAccessToken** l’exemple suivant montre comment obtenir une identité de l’appelant jeton pour une application.</span><span class="sxs-lookup"><span data-stu-id="e5226-124">The following example of a **GetClientAccessToken** operation request shows how to get a caller identity token for an app.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:GetClientAccessToken>
         <m:TokenRequests>
            <t:TokenRequest>
               <t:Id>1C50226D-04B5-4AB2-9FCD-42E236B59E4B</t:Id>
               <t:TokenType>CallerIdentity</t:TokenType>
            </t:TokenRequest>
         </m:TokenRequests>
      </m:GetClientAccessToken>
   </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="e5226-125">La demande SOAP body contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="e5226-125">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="e5226-126">GetClientAccessToken</span><span class="sxs-lookup"><span data-stu-id="e5226-126">GetClientAccessToken</span></span>](getclientaccesstoken.md)
    
- [<span data-ttu-id="e5226-127">TokenRequests</span><span class="sxs-lookup"><span data-stu-id="e5226-127">TokenRequests</span></span>](tokenrequests.md)
    
- [<span data-ttu-id="e5226-128">TokenRequest</span><span class="sxs-lookup"><span data-stu-id="e5226-128">TokenRequest</span></span>](tokenrequest.md)
    
- [<span data-ttu-id="e5226-129">ID (chaîne)</span><span class="sxs-lookup"><span data-stu-id="e5226-129">ID (String)</span></span>](id-string.md)
    
- [<span data-ttu-id="e5226-130">TokenType</span><span class="sxs-lookup"><span data-stu-id="e5226-130">TokenType</span></span>](tokentype.md)
    
## <a name="successful-getclientaccesstoken-operation-response"></a><span data-ttu-id="e5226-131">Réponse d’opération GetClientAccessToken réussie</span><span class="sxs-lookup"><span data-stu-id="e5226-131">Successful GetClientAccessToken operation response</span></span>

<span data-ttu-id="e5226-132">L’exemple suivant montre une réponse positive à une demande d’opération **GetClientAccessToken** pour obtenir une identité de l’appelant jeton pour une application.</span><span class="sxs-lookup"><span data-stu-id="e5226-132">The following example shows a successful response to a **GetClientAccessToken** operation request to get a caller identity token for an app.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="e5226-133">Les valeurs de jeton dans cet article ont été réduits afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="e5226-133">The token values in this article have been shortened to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="14" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:GetClientAccessTokenResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:GetClientAccessTokenResponseMessage ResponseClass="Success">
               <m:ResponseCode>NoError</m:ResponseCode>
               <m:Token>
                  <t:Id>1C50226D-04B5-4AB2-9FCD-42E236B59E4B</t:Id>
                  <t:TokenType>CallerIdentity</t:TokenType>
                  <t:TokenValue>eyJ0eXAmv0QitaJg</t:TokenValue>
                  <t:TTL>479</t:TTL>
               </m:Token>
            </m:GetClientAccessTokenResponseMessage>
         </m:ResponseMessages>
      </m:GetClientAccessTokenResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="e5226-134">La réponse SOAP body contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="e5226-134">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="e5226-135">GetClientAccessTokenResponse</span><span class="sxs-lookup"><span data-stu-id="e5226-135">GetClientAccessTokenResponse</span></span>](getclientaccesstokenresponse.md)
    
- [<span data-ttu-id="e5226-136">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="e5226-136">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="e5226-137">GetClientAccessTokenResponseMessage</span><span class="sxs-lookup"><span data-stu-id="e5226-137">GetClientAccessTokenResponseMessage</span></span>](getclientaccesstokenresponsemessage.md)
    
- [<span data-ttu-id="e5226-138">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="e5226-138">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="e5226-139">Jeton (ClientAccessTokenType)</span><span class="sxs-lookup"><span data-stu-id="e5226-139">Token (ClientAccessTokenType)</span></span>](token-clientaccesstokentype.md)
    
- [<span data-ttu-id="e5226-140">ID (chaîne)</span><span class="sxs-lookup"><span data-stu-id="e5226-140">ID (String)</span></span>](id-string.md)
    
- [<span data-ttu-id="e5226-141">TokenType (ClientAccessTokenType)</span><span class="sxs-lookup"><span data-stu-id="e5226-141">TokenType (ClientAccessTokenType)</span></span>](tokentype-clientaccesstokentype.md)
    
- [<span data-ttu-id="e5226-142">TokenValue</span><span class="sxs-lookup"><span data-stu-id="e5226-142">TokenValue</span></span>](tokenvalue.md)
    
- [<span data-ttu-id="e5226-143">TTL (ClientAccessTokenTypeType)</span><span class="sxs-lookup"><span data-stu-id="e5226-143">TTL (ClientAccessTokenTypeType)</span></span>](ttl-clientaccesstokentypetype.md)
    
## <a name="getclientaccesstoken-operation-error-response"></a><span data-ttu-id="e5226-144">Réponse d’erreur d’opération GetClientAccessToken</span><span class="sxs-lookup"><span data-stu-id="e5226-144">GetClientAccessToken operation error response</span></span>

<span data-ttu-id="e5226-145">L’exemple suivant montre une réponse d’erreur à une demande d’opération **GetClientAccessToken** .</span><span class="sxs-lookup"><span data-stu-id="e5226-145">The following example shows an error response to a **GetClientAccessToken** operation request.</span></span> <span data-ttu-id="e5226-146">Il s’agit d’une réponse à une demande pour obtenir un rappel d’extension jeton sans les autorisations appropriées.</span><span class="sxs-lookup"><span data-stu-id="e5226-146">This is a response to a request to get an extension callback token without the appropriate permissions.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="14" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:GetClientAccessTokenResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:GetClientAccessTokenResponseMessage ResponseClass="Error">
               <m:MessageText>The caller does not have enough permission for this token request.</m:MessageText>
               <m:ResponseCode>ErrorInvalidClientAccessTokenRequest</m:ResponseCode>
               <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
            </m:GetClientAccessTokenResponseMessage>
         </m:ResponseMessages>
      </m:GetClientAccessTokenResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="e5226-147">La réponse d’erreur corps SOAP contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="e5226-147">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="e5226-148">GetClientAccessTokenResponse</span><span class="sxs-lookup"><span data-stu-id="e5226-148">GetClientAccessTokenResponse</span></span>](getclientaccesstokenresponse.md)
    
- [<span data-ttu-id="e5226-149">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="e5226-149">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="e5226-150">GetClientAccessTokenResponseMessage</span><span class="sxs-lookup"><span data-stu-id="e5226-150">GetClientAccessTokenResponseMessage</span></span>](getclientaccesstokenresponsemessage.md)
    
- [<span data-ttu-id="e5226-151">MessageText</span><span class="sxs-lookup"><span data-stu-id="e5226-151">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="e5226-152">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="e5226-152">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="e5226-153">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="e5226-153">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="e5226-154">Pour les codes d’erreur générique à EWS, spécifiques à cette opération, consultez la rubrique [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="e5226-154">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="e5226-155">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e5226-155">See also</span></span>

- [<span data-ttu-id="e5226-156">Opérations EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="e5226-156">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="e5226-157">Opération GetAppManifests</span><span class="sxs-lookup"><span data-stu-id="e5226-157">GetAppManifests operation</span></span>](getappmanifests-operation.md)
    
- [<span data-ttu-id="e5226-158">Compléments Outlook</span><span class="sxs-lookup"><span data-stu-id="e5226-158">Outlook add-ins</span></span>](http://msdn.microsoft.com/library/71e64bc9-e347-4f5d-8948-0a47b5dd93e6%28Office.15%29.aspx)
    

