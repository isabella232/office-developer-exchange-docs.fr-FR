---
title: Gestion des messages d’erreur de découverte automatique
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: e5939ec2-1100-4174-8a88-5a6e09b60b23
description: Découvrez les différents types d’erreurs de découverte automatique et que faire avec eux.
ms.openlocfilehash: fcafc799f4d35e92159d2913845474ecf7bc5657
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754782"
---
# <a name="handling-autodiscover-error-messages"></a><span data-ttu-id="d73e6-103">Gestion des messages d’erreur de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="d73e6-103">Handling Autodiscover error messages</span></span>

<span data-ttu-id="d73e6-104">Découvrez les différents types d’erreurs de découverte automatique et que faire avec eux.</span><span class="sxs-lookup"><span data-stu-id="d73e6-104">Learn about the different types of Autodiscover errors and what to do with them.</span></span>
  
<span data-ttu-id="d73e6-105">Découverte automatique permet à vos applications récupérer les informations de configuration automatiquement, et il fonctionne très.</span><span class="sxs-lookup"><span data-stu-id="d73e6-105">Autodiscover enables your applications to retrieve configuration information automatically, and it works great.</span></span> <span data-ttu-id="d73e6-106">Toutefois, tout ne se passe toujours en fonction du plan.</span><span class="sxs-lookup"><span data-stu-id="d73e6-106">However, things don't always go according to plan.</span></span> <span data-ttu-id="d73e6-107">Examinons les erreurs courants qui peuvent se produire et comment vous pouvez gérer les afin de réduire la nécessité d’inviter l’utilisateur à configurer manuellement votre client.</span><span class="sxs-lookup"><span data-stu-id="d73e6-107">Let's look at the common errors that might occur and how you can handle them to minimize the need to prompt your user to manually configure your client.</span></span>
  
## <a name="http-status-errors"></a><span data-ttu-id="d73e6-108">Erreurs d’état HTTP</span><span class="sxs-lookup"><span data-stu-id="d73e6-108">HTTP status errors</span></span>
<span data-ttu-id="d73e6-109"><a name="bk_HttpErrors"> </a></span><span class="sxs-lookup"><span data-stu-id="d73e6-109"></span></span>

<span data-ttu-id="d73e6-110">Le premier type d’erreur que vous pouvez rencontrer lors de l’envoi de demandes de découverte automatique est l’état HTTP.</span><span class="sxs-lookup"><span data-stu-id="d73e6-110">The first type of error you might encounter when sending Autodiscover requests is the HTTP status.</span></span> <span data-ttu-id="d73e6-111">Si l’état HTTP dans votre réponse n’est pas 200 (OK), la charge utile de réponse ne contient pas la réponse de découverte automatique que vous recherchez.</span><span class="sxs-lookup"><span data-stu-id="d73e6-111">If the HTTP status in your response is anything other than 200 (OK), the response payload doesn't contain the Autodiscover response you were looking for.</span></span> <span data-ttu-id="d73e6-112">Par souci de simplicité, nous pouvons grouper les codes d’état non 200 en trois catégories.</span><span class="sxs-lookup"><span data-stu-id="d73e6-112">For simplicity, we can group non-200 status codes into three categories.</span></span>
  
<span data-ttu-id="d73e6-113">**Le tableau 1. Codes d’état HTTP**</span><span class="sxs-lookup"><span data-stu-id="d73e6-113">**Table 1. HTTP status codes**</span></span>

|<span data-ttu-id="d73e6-114">**Code d’état**</span><span class="sxs-lookup"><span data-stu-id="d73e6-114">**Status code**</span></span>|<span data-ttu-id="d73e6-115">**Type d’erreur**</span><span class="sxs-lookup"><span data-stu-id="d73e6-115">**Type of error**</span></span>|<span data-ttu-id="d73e6-116">**Pour gérer...**</span><span class="sxs-lookup"><span data-stu-id="d73e6-116">**To handle…**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="d73e6-117">301 ou 302</span><span class="sxs-lookup"><span data-stu-id="d73e6-117">301 or 302</span></span>  <br/> |<span data-ttu-id="d73e6-118">Erreur de redirection</span><span class="sxs-lookup"><span data-stu-id="d73e6-118">Redirect error</span></span>  <br/> |<span data-ttu-id="d73e6-119">Renvoyer votre demande à l’URI contenue dans l’en-tête de réponse HTTP ligne « emplacement ».</span><span class="sxs-lookup"><span data-stu-id="d73e6-119">Resend your request to the URI contained in the "Location" HTTP response header.</span></span> <span data-ttu-id="d73e6-120">Pour plus d’informations, voir [Gestion des erreurs de redirection](#bk_HandlingRedirects).</span><span class="sxs-lookup"><span data-stu-id="d73e6-120">For details, see [Handling redirect errors](#bk_HandlingRedirects).</span></span>  <br/> |
|<span data-ttu-id="d73e6-121">401</span><span class="sxs-lookup"><span data-stu-id="d73e6-121">401</span></span>  <br/> |<span data-ttu-id="d73e6-122">Erreur non autorisée</span><span class="sxs-lookup"><span data-stu-id="d73e6-122">Unauthorized error</span></span>  <br/> |<span data-ttu-id="d73e6-123">Le [processus de découverte automatique](autodiscover-for-exchange.md) implique la tentative de plusieurs URL potentiels, vous pouvez obtenir cette sur une seule URL que suivant accepte vos informations d’identification.</span><span class="sxs-lookup"><span data-stu-id="d73e6-123">Because the [Autodiscover process](autodiscover-for-exchange.md) involves trying multiple potential URLs, you could get this on one URL only to have the next one accept your credentials.</span></span> <span data-ttu-id="d73e6-124">Pour cette raison, vous ne devez pas tenir compte une seule erreur 401 pour indiquer que les informations d’identification ne sont pas valides.</span><span class="sxs-lookup"><span data-stu-id="d73e6-124">For this reason, you shouldn't consider a single 401 error to indicate that the credentials are invalid.</span></span> <span data-ttu-id="d73e6-125">Toutefois, si vous recevez des 401 erreurs à partir de plusieurs URL, vous souhaiterez invite l’utilisateur à entrer de nouveau leur mot de passe (si possible).</span><span class="sxs-lookup"><span data-stu-id="d73e6-125">However, if you receive 401 errors from multiple URLs, you might want to prompt the user to reenter their password (if possible).</span></span>  <br/> |
|<span data-ttu-id="d73e6-126">N’importe quel autre état non-200</span><span class="sxs-lookup"><span data-stu-id="d73e6-126">Any other non-200 status</span></span>  <br/> |<span data-ttu-id="d73e6-127">Erreur de point de terminaison de découverte automatique non valide</span><span class="sxs-lookup"><span data-stu-id="d73e6-127">Invalid Autodiscover endpoint error</span></span>  <br/> |<span data-ttu-id="d73e6-128">Prendre en compte l’URL qui renvoie un autre code d’état non 200 comme non valide et continue d’essayer de l’URL suivante dans votre liste.</span><span class="sxs-lookup"><span data-stu-id="d73e6-128">Consider the URL that returns any other non-200 status code to be invalid, and continue trying the next URL in your list.</span></span>  <br/> |
   
## <a name="autodiscover-errors"></a><span data-ttu-id="d73e6-129">Erreurs de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="d73e6-129">Autodiscover errors</span></span>
<span data-ttu-id="d73e6-130"><a name="bk_AutodiscoverErrors"> </a></span><span class="sxs-lookup"><span data-stu-id="d73e6-130"></span></span>

<span data-ttu-id="d73e6-131">Même si vous obtenez un code d’état 200 (OK) après l’envoi d’une demande de découverte automatique, cela ne signifie pas que le serveur a envoyé les informations que nécessaires.</span><span class="sxs-lookup"><span data-stu-id="d73e6-131">Even if you get a 200 (OK) status code after sending an Autodiscover request, that doesn't mean that the server sent the information you need.</span></span> <span data-ttu-id="d73e6-132">L’état de 200 signifie simplement que vous avez une réponse de découverte automatique et réponse peut contenir une erreur dans la charge utile.</span><span class="sxs-lookup"><span data-stu-id="d73e6-132">The 200 status only means that you have an Autodiscover response, and that response might contain an error within the payload.</span></span> <span data-ttu-id="d73e6-133">L’emplacement des informations d’erreur diffère selon que le format est SOAP ou variole.</span><span class="sxs-lookup"><span data-stu-id="d73e6-133">The location of the error information differs depending on whether the format is SOAP or POX.</span></span>
  
### <a name="soap-autodiscover-errors"></a><span data-ttu-id="d73e6-134">Erreurs de découverte automatique SOAP</span><span class="sxs-lookup"><span data-stu-id="d73e6-134">SOAP Autodiscover errors</span></span>

<span data-ttu-id="d73e6-135">Pour la découverte automatique SOAP, la réponse peut contenir un ou plusieurs éléments [ErrorCode (SOAP)](http://msdn.microsoft.com/library/5e5ec861-0191-4ecb-a906-47ce8ed96381%28Office.15%29.aspx) dans plusieurs emplacements.</span><span class="sxs-lookup"><span data-stu-id="d73e6-135">For SOAP Autodiscover, the response can contain one or more [ErrorCode (SOAP)](http://msdn.microsoft.com/library/5e5ec861-0191-4ecb-a906-47ce8ed96381%28Office.15%29.aspx) elements, in different places.</span></span> <span data-ttu-id="d73e6-136">En règle générale, vous pouvez tirer un élément enfant de l’élément de [Réponse (SOAP)](http://msdn.microsoft.com/library/4c2bcdeb-95ce-4ffa-bd83-118af53b534f%28Office.15%29.aspx) et un en tant qu’enfant de chaque élément de [Réponse utilisateur (SOAP)](http://msdn.microsoft.com/library/5007b1ba-bfcc-40d7-b1cb-e32fbaf54ffd%28Office.15%29.aspx) dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="d73e6-136">Typically you can expect one as a child element of the [Response (SOAP)](http://msdn.microsoft.com/library/4c2bcdeb-95ce-4ffa-bd83-118af53b534f%28Office.15%29.aspx) element, and one as a child of each [UserResponse (SOAP)](http://msdn.microsoft.com/library/5007b1ba-bfcc-40d7-b1cb-e32fbaf54ffd%28Office.15%29.aspx) element in the response.</span></span> <span data-ttu-id="d73e6-137">Vous pouvez également rencontrer un en tant qu’enfant d’un élément [UserSettingError (SOAP)](http://msdn.microsoft.com/library/abb175c5-4f38-4dcc-81e3-b511686862eb%28Office.15%29.aspx) , s’il est présent.</span><span class="sxs-lookup"><span data-stu-id="d73e6-137">You might also encounter one as a child of a [UserSettingError (SOAP)](http://msdn.microsoft.com/library/abb175c5-4f38-4dcc-81e3-b511686862eb%28Office.15%29.aspx) element, if one is present.</span></span> <span data-ttu-id="d73e6-138">Le contexte de l’erreur dépend de l’élément **ErrorCode** situe, comme suit :</span><span class="sxs-lookup"><span data-stu-id="d73e6-138">The context of the error depends on where the **ErrorCode** element is located, as follows:</span></span> 
  
- <span data-ttu-id="d73e6-139">Élément enfant de l’élément de **réponse** , l’élément **ErrorCode** représente une erreur qui s’applique à l’ensemble de la demande.</span><span class="sxs-lookup"><span data-stu-id="d73e6-139">As a child element of the **Response** element, the **ErrorCode** element represents an error that applies to the entire request.</span></span> 
    
- <span data-ttu-id="d73e6-140">En tant qu’enfant de l’élément de **réponse utilisateur** , elle représente une erreur qui s’applique uniquement à un utilisateur spécifique.</span><span class="sxs-lookup"><span data-stu-id="d73e6-140">As a child of the **UserResponse** element, it represents an error that applies just to that specific user.</span></span> 
    
- <span data-ttu-id="d73e6-141">En tant qu’enfant d’un élément **UserSettingError** , il représente une erreur qui s’applique à un paramètre spécifique qui a été demandé.</span><span class="sxs-lookup"><span data-stu-id="d73e6-141">As a child of a **UserSettingError** element, it represents an error that applies to a specific setting that was requested.</span></span> 
    
<span data-ttu-id="d73e6-142">Examinons un exemple d’une réponse.</span><span class="sxs-lookup"><span data-stu-id="d73e6-142">Let's take a look at an example of a response.</span></span> <span data-ttu-id="d73e6-143">Dans cet exemple, l’élément **ErrorCode** sous l’élément de **réponse** a une valeur de « NoError », ce qui indique la réussite.</span><span class="sxs-lookup"><span data-stu-id="d73e6-143">In this example, the **ErrorCode** element under the **Response** element has a value of "NoError", which indicates overall success.</span></span> <span data-ttu-id="d73e6-144">Toutefois, l’élément **ErrorCode** sous l’élément de **réponse utilisateur** a une valeur de « RedirectAddress », ce qui indique qu’une erreur s’est produite pour cet utilisateur spécifique.</span><span class="sxs-lookup"><span data-stu-id="d73e6-144">However, the **ErrorCode** element under the **UserResponse** element has a value of "RedirectAddress", which indicates that an error occurred for that particular user.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/" 
    xmlns:a="http://www.w3.org/2005/08/addressing">
  <s:Header>
    <a:Action s:mustUnderstand="1">http://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetUserSettingsResponse</a:Action>
    <h:ServerVersionInfo xmlns:h="http://schemas.microsoft.com/exchange/2010/Autodiscover" 
        xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
      <h:MajorVersion>14</h:MajorVersion>
      <h:MinorVersion>3</h:MinorVersion>
      <h:MajorBuildNumber>136</h:MajorBuildNumber>
      <h:MinorBuildNumber>1</h:MinorBuildNumber>
      <h:Version>Exchange2010_SP2</h:Version>
    </h:ServerVersionInfo>
  </s:Header>
  <s:Body>
    <GetUserSettingsResponseMessage xmlns="http://schemas.microsoft.com/exchange/2010/Autodiscover">
      <Response xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
        <ErrorCode>NoError</ErrorCode>
        <ErrorMessage />
        <UserResponses>
          <UserResponse>
            <ErrorCode>RedirectAddress</ErrorCode>
            <ErrorMessage>Redirection address.</ErrorMessage>
            <RedirectTarget>elvin@mail.contoso.com</RedirectTarget>
            <UserSettingErrors />
            <UserSettings />
          </UserResponse>
        </UserResponses>
      </Response>
    </GetUserSettingsResponseMessage>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="d73e6-145">L’article [ErrorCode (SOAP)](http://msdn.microsoft.com/library/5e5ec861-0191-4ecb-a906-47ce8ed96381%28Office.15%29.aspx) contient une liste complète des erreurs possibles.</span><span class="sxs-lookup"><span data-stu-id="d73e6-145">The [ErrorCode (SOAP)](http://msdn.microsoft.com/library/5e5ec861-0191-4ecb-a906-47ce8ed96381%28Office.15%29.aspx) article contains a full list of possible errors.</span></span> <span data-ttu-id="d73e6-146">La plupart de ces indique une erreur irrécupérable, mais quelques justifient une gestion spéciale.</span><span class="sxs-lookup"><span data-stu-id="d73e6-146">Most of these indicate an unrecoverable error, but a few warrant special handling.</span></span> 
  
<span data-ttu-id="d73e6-147">**Le tableau 2. Valeurs Autodisover ErrorCode SOAP**</span><span class="sxs-lookup"><span data-stu-id="d73e6-147">**Table 2. SOAP Autodisover ErrorCode values**</span></span>

|<span data-ttu-id="d73e6-148">**Valeur de code d’erreur**</span><span class="sxs-lookup"><span data-stu-id="d73e6-148">**ErrorCode value**</span></span>|<span data-ttu-id="d73e6-149">**Pour gérer...**</span><span class="sxs-lookup"><span data-stu-id="d73e6-149">**To handle…**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d73e6-150">RedirectAddress</span><span class="sxs-lookup"><span data-stu-id="d73e6-150">RedirectAddress</span></span>  <br/> |<span data-ttu-id="d73e6-151">[Le redémarrage de la découverte automatique avec une nouvelle adresse de messagerie](#bk_RestartAutodiscover) avec l’adresse de messagerie dans l’élément [RedirectTarget (SOAP)](http://msdn.microsoft.com/library/f8162724-cf9a-4543-a1ad-5846c8b10bfa%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="d73e6-151">[Restarting Autodiscover with a new email address](#bk_RestartAutodiscover) with the email address in the [RedirectTarget (SOAP)](http://msdn.microsoft.com/library/f8162724-cf9a-4543-a1ad-5846c8b10bfa%28Office.15%29.aspx) element.</span></span>  <br/> |
|<span data-ttu-id="d73e6-152">RedirectUrl</span><span class="sxs-lookup"><span data-stu-id="d73e6-152">RedirectUrl</span></span>  <br/> |<span data-ttu-id="d73e6-153">[Renvoi de votre demande vers une nouvelle URL](#bk_ResendRequest) à l’URL dans l’élément **RedirectTarget** .</span><span class="sxs-lookup"><span data-stu-id="d73e6-153">[Resending your request to a new URL](#bk_ResendRequest) to the URL in the **RedirectTarget** element.</span></span>  <br/> |
|<span data-ttu-id="d73e6-154">ServerBusy</span><span class="sxs-lookup"><span data-stu-id="d73e6-154">ServerBusy</span></span>  <br/> |<span data-ttu-id="d73e6-155">Réessayez cette URL après un court délai.</span><span class="sxs-lookup"><span data-stu-id="d73e6-155">Retry this URL after a small delay.</span></span> <span data-ttu-id="d73e6-156">Vous pouvez attendre un laps de temps ou simplement déplacer cette URL à la fin de la liste d’URL pour essayer.</span><span class="sxs-lookup"><span data-stu-id="d73e6-156">You might wait a set amount of time or simply move this URL to the end of your list of URLs to try.</span></span> <span data-ttu-id="d73e6-157">Si vous recevez cette erreur plusieurs fois à partir d’une URL, vous devez envisager l’URL non valide.</span><span class="sxs-lookup"><span data-stu-id="d73e6-157">If you receive this error multiple times from a URL, you should consider the URL to be invalid.</span></span>  <br/> |
   
### <a name="pox-autodiscover-errors"></a><span data-ttu-id="d73e6-158">Erreurs de découverte automatique POX</span><span class="sxs-lookup"><span data-stu-id="d73e6-158">POX Autodiscover errors</span></span>

<span data-ttu-id="d73e6-159">Le service de découverte automatique variole signale les erreurs un peu différemment.</span><span class="sxs-lookup"><span data-stu-id="d73e6-159">The POX Autodiscover service reports errors a little differently.</span></span> <span data-ttu-id="d73e6-160">Erreurs non récupérables sont contenues dans l’élément [Erreur (POX)](http://msdn.microsoft.com/library/91c63b62-ab68-4c32-a2f7-5a87c188335b%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="d73e6-160">Non-recoverable errors are contained in the [Error (POX)](http://msdn.microsoft.com/library/91c63b62-ab68-4c32-a2f7-5a87c188335b%28Office.15%29.aspx) element.</span></span> <span data-ttu-id="d73e6-161">L’article [ErrorCode (POX)](http://msdn.microsoft.com/library/064d73e4-45b7-4797-828e-9df590830db8%28Office.15%29.aspx) contient une liste complète des codes d’erreur possibles.</span><span class="sxs-lookup"><span data-stu-id="d73e6-161">The [ErrorCode (POX)](http://msdn.microsoft.com/library/064d73e4-45b7-4797-828e-9df590830db8%28Office.15%29.aspx) article contains a full list of possible error codes.</span></span> 
  
<span data-ttu-id="d73e6-162">Erreurs de redirection sont contenues dans l’élément [Action (POX)](http://msdn.microsoft.com/library/a3462c6b-453c-462a-830d-f29ee4a2babb%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="d73e6-162">Redirect errors are contained in the [Action (POX)](http://msdn.microsoft.com/library/a3462c6b-453c-462a-830d-f29ee4a2babb%28Office.15%29.aspx) element.</span></span> <span data-ttu-id="d73e6-163">N’importe quelle valeur de l’élément **Action** autres que « paramètres » indique une erreur de redirection.</span><span class="sxs-lookup"><span data-stu-id="d73e6-163">Any value of the **Action** element other than "settings" indicates a redirect error.</span></span> 
  
<span data-ttu-id="d73e6-164">**Le tableau 3. Valeurs Autodisover ErrorCode POX**</span><span class="sxs-lookup"><span data-stu-id="d73e6-164">**Table 3. POX Autodisover ErrorCode values**</span></span>

|<span data-ttu-id="d73e6-165">**Valeur d’action**</span><span class="sxs-lookup"><span data-stu-id="d73e6-165">**Action value**</span></span>|<span data-ttu-id="d73e6-166">**Pour gérer...**</span><span class="sxs-lookup"><span data-stu-id="d73e6-166">**To handle…**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d73e6-167">redirectAddr</span><span class="sxs-lookup"><span data-stu-id="d73e6-167">redirectAddr</span></span>  <br/> |<span data-ttu-id="d73e6-168">[Le redémarrage de la découverte automatique avec une nouvelle adresse de messagerie](#bk_RestartAutodiscover) avec l’adresse de messagerie dans l’élément [RedirectAddr (POX)](http://msdn.microsoft.com/library/0e9fa6b6-7991-4dc1-a59a-48e5f8e041e4%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="d73e6-168">[Restarting Autodiscover with a new email address](#bk_RestartAutodiscover) with the email address in the [RedirectAddr (POX)](http://msdn.microsoft.com/library/0e9fa6b6-7991-4dc1-a59a-48e5f8e041e4%28Office.15%29.aspx) element.</span></span>  <br/> |
|<span data-ttu-id="d73e6-169">redirectUrl</span><span class="sxs-lookup"><span data-stu-id="d73e6-169">redirectUrl</span></span>  <br/> |<span data-ttu-id="d73e6-170">[Renvoi de votre demande vers une nouvelle URL](#bk_ResendRequest) à l’URL dans l’élément [RedirectUrl (POX)](http://msdn.microsoft.com/library/c54f310f-8c99-4c37-8e73-ac87722b6229%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="d73e6-170">[Resending your request to a new URL](#bk_ResendRequest) to the URL in the [RedirectUrl (POX)](http://msdn.microsoft.com/library/c54f310f-8c99-4c37-8e73-ac87722b6229%28Office.15%29.aspx) element.</span></span>  <br/> |
   
<span data-ttu-id="d73e6-171">Dans cet exemple, l’élément **Action** a la valeur « redirectAddr », ce qui indique qu’une nouvelle demande doit être envoyée avec la nouvelle adresse de messagerie contenue dans l’élément **RedirectAddr** .</span><span class="sxs-lookup"><span data-stu-id="d73e6-171">In this example, the **Action** element has a value of "redirectAddr", which indicates that a new request should be sent with the new email address contained in the **RedirectAddr** element.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<Autodiscover xmlns="http://schemas.microsoft.com/exchange/autodiscover/responseschema/2006">
  <Response xmlns="http://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a">
    <Account>
      <Action>redirectAddr</Action>
      <RedirectAddr>elvin@mail.contoso.com</RedirectAddr>
    </Account>
  </Response>
</Autodiscover>
```

## <a name="handling-redirect-errors"></a><span data-ttu-id="d73e6-172">Gestion des erreurs de redirection</span><span class="sxs-lookup"><span data-stu-id="d73e6-172">Handling redirect errors</span></span>
<span data-ttu-id="d73e6-173"><a name="bk_HandlingRedirects"> </a></span><span class="sxs-lookup"><span data-stu-id="d73e6-173"></span></span>

<span data-ttu-id="d73e6-174">Vous pouvez gérer des scénarios de redirection d’erreur de deux manières :</span><span class="sxs-lookup"><span data-stu-id="d73e6-174">You can handle redirect error scenarios in two ways:</span></span>
  
- <span data-ttu-id="d73e6-175">En redémarrant la découverte automatique avec une nouvelle adresse de messagerie.</span><span class="sxs-lookup"><span data-stu-id="d73e6-175">By restarting Autodiscover with a new email address.</span></span>
    
- <span data-ttu-id="d73e6-176">Par le renvoi de votre demande vers une nouvelle URL.</span><span class="sxs-lookup"><span data-stu-id="d73e6-176">By resending your request to a new URL.</span></span>
    
<span data-ttu-id="d73e6-177">Les deux scénarios nécessitent une validation avant de continuer.</span><span class="sxs-lookup"><span data-stu-id="d73e6-177">Both scenarios require some validation before proceeding.</span></span>
  
### <a name="restarting-autodiscover-with-a-new-email-address"></a><span data-ttu-id="d73e6-178">Redémarrage du service de découverte automatique avec une nouvelle adresse de messagerie</span><span class="sxs-lookup"><span data-stu-id="d73e6-178">Restarting Autodiscover with a new email address</span></span>
<span data-ttu-id="d73e6-179"><a name="bk_RestartAutodiscover"> </a></span><span class="sxs-lookup"><span data-stu-id="d73e6-179"></span></span>

<span data-ttu-id="d73e6-180">Lorsque vous participez à une nouvelle adresse de messagerie une découverte automatique rediriger réponse, tout d’abord vérifier que la nouvelle adresse de messagerie qui a été fournie dans la réponse d’erreur de redirection n’est pas la même adresse que vous avez envoyé dans la demande qui a provoqué l’erreur.</span><span class="sxs-lookup"><span data-stu-id="d73e6-180">When you get a new email address in an Autodiscover redirect response, first verify that the new email address that was provided in the redirect error response is not the same address that you sent in the request that resulted in the error.</span></span> <span data-ttu-id="d73e6-181">Si tel est le cas, vous ne devez pas redémarrer le service de découverte automatique et prendre en compte à la place de l’URL qui a généré la réponse comme non valide.</span><span class="sxs-lookup"><span data-stu-id="d73e6-181">If it is, you should not restart Autodiscover and instead consider the URL that generated the response to be invalid.</span></span>
  
<span data-ttu-id="d73e6-182">Si la nouvelle adresse de messagerie est différente, annuler votre liste existante d’URL de point de terminaison de découverte automatique potentiels et générer une nouvelle liste en fonction de la nouvelle adresse de messagerie.</span><span class="sxs-lookup"><span data-stu-id="d73e6-182">If the new email address is different, discard your existing list of potential Autodiscover endpoint URLs and generate a new list based on the new email address.</span></span>
  
### <a name="resending-your-request-to-a-new-url"></a><span data-ttu-id="d73e6-183">Renvoi de votre demande vers une nouvelle URL</span><span class="sxs-lookup"><span data-stu-id="d73e6-183">Resending your request to a new URL</span></span>
<span data-ttu-id="d73e6-184"><a name="bk_ResendRequest"> </a></span><span class="sxs-lookup"><span data-stu-id="d73e6-184"></span></span>

<span data-ttu-id="d73e6-185">Lorsque vous recevez une nouvelle URL dans une réponse de redirection de découverte automatique, vous devez tout d’abord valider l’URL comme suit :</span><span class="sxs-lookup"><span data-stu-id="d73e6-185">When you get a new URL in an Autodiscover redirect response, you should first validate the URL as follows:</span></span>
  
- <span data-ttu-id="d73e6-186">Vérifiez que l’URL est une URL HTTPS.</span><span class="sxs-lookup"><span data-stu-id="d73e6-186">Verify that the URL is an HTTPS URL.</span></span>
    
- <span data-ttu-id="d73e6-187">Vérifiez que vous n’avez pas reçu une erreur à partir de cette URL avec l’adresse de messagerie actuelle avant.</span><span class="sxs-lookup"><span data-stu-id="d73e6-187">Verify that you have not received an error from this URL with the current email address before.</span></span>
    
- <span data-ttu-id="d73e6-188">Le cas échéant à votre application, informer l’utilisateur de la redirection et obtenez leur autorisation pour suivre la redirection.</span><span class="sxs-lookup"><span data-stu-id="d73e6-188">If applicable to your application, inform the user of the redirection and get their permission to follow the redirect.</span></span>
    
- <span data-ttu-id="d73e6-189">Envoyer une requête à l’URL et [Vérifiez que le certificat SSL présenté par le serveur est valid](how-to-validate-a-server-certificate-for-the-ews-managed-api.md).</span><span class="sxs-lookup"><span data-stu-id="d73e6-189">Send a request to the URL and [verify that the SSL certificate presented by the server is valid](how-to-validate-a-server-certificate-for-the-ews-managed-api.md).</span></span>
    
<span data-ttu-id="d73e6-190">Si l’URL est validé, renvoyez la demande à cette nouvelle URL.</span><span class="sxs-lookup"><span data-stu-id="d73e6-190">If the URL passes validation, resend the request to this new URL.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="d73e6-191">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d73e6-191">See also</span></span>


- [<span data-ttu-id="d73e6-192">Découverte automatique pour Exchange</span><span class="sxs-lookup"><span data-stu-id="d73e6-192">Autodiscover for Exchange</span></span>](autodiscover-for-exchange.md)
    
- [<span data-ttu-id="d73e6-193">Rechercher des points de terminaison de découverte automatique à l’aide de recherche SCP dans Exchange</span><span class="sxs-lookup"><span data-stu-id="d73e6-193">Find Autodiscover endpoints by using SCP lookup in Exchange</span></span>](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md)
    
- [<span data-ttu-id="d73e6-194">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d73e6-194">ErrorCode (SOAP)</span></span>](http://msdn.microsoft.com/library/5e5ec861-0191-4ecb-a906-47ce8ed96381%28Office.15%29.aspx)
    
- [<span data-ttu-id="d73e6-195">ErrorCode (POX)</span><span class="sxs-lookup"><span data-stu-id="d73e6-195">ErrorCode (POX)</span></span>](http://msdn.microsoft.com/library/064d73e4-45b7-4797-828e-9df590830db8%28Office.15%29.aspx)
    

