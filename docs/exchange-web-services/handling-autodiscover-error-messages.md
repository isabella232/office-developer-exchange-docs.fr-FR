---
title: Gestion des messages d'erreur de découverte automatique
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: e5939ec2-1100-4174-8a88-5a6e09b60b23
description: Découvrez les différents types d’erreurs de découverte automatique et la marche à suivre.
localization_priority: Priority
ms.openlocfilehash: 0cba7e54cb251a9775e0971826560e277dcd9d2d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455960"
---
# <a name="handling-autodiscover-error-messages"></a><span data-ttu-id="8a6fb-103">Gestion des messages d'erreur de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="8a6fb-103">Handling Autodiscover error messages</span></span>

<span data-ttu-id="8a6fb-104">Découvrez les différents types d’erreurs de découverte automatique et la marche à suivre.</span><span class="sxs-lookup"><span data-stu-id="8a6fb-104">Learn about the different types of Autodiscover errors and what to do with them.</span></span>
  
<span data-ttu-id="8a6fb-105">La découverte automatique permet à vos applications de récupérer automatiquement les informations de configuration et elle fonctionne parfaitement.</span><span class="sxs-lookup"><span data-stu-id="8a6fb-105">Autodiscover enables your applications to retrieve configuration information automatically, and it works great.</span></span> <span data-ttu-id="8a6fb-106">Toutefois, les choses ne sont pas toujours conformes à la planification.</span><span class="sxs-lookup"><span data-stu-id="8a6fb-106">However, things don't always go according to plan.</span></span> <span data-ttu-id="8a6fb-107">Examinons les erreurs courantes susceptibles de se produire et vous pouvez les gérer afin de réduire le besoin d’inviter votre utilisateur à configurer manuellement votre client.</span><span class="sxs-lookup"><span data-stu-id="8a6fb-107">Let's look at the common errors that might occur and how you can handle them to minimize the need to prompt your user to manually configure your client.</span></span>
  
## <a name="http-status-errors"></a><span data-ttu-id="8a6fb-108">Erreurs d’état HTTP</span><span class="sxs-lookup"><span data-stu-id="8a6fb-108">HTTP status errors</span></span>
<span data-ttu-id="8a6fb-109"><a name="bk_HttpErrors"> </a></span><span class="sxs-lookup"><span data-stu-id="8a6fb-109"><a name="bk_HttpErrors"> </a></span></span>

<span data-ttu-id="8a6fb-110">Le premier type d’erreur que vous pouvez rencontrer lors de l’envoi de demandes de découverte automatique est l’état HTTP.</span><span class="sxs-lookup"><span data-stu-id="8a6fb-110">The first type of error you might encounter when sending Autodiscover requests is the HTTP status.</span></span> <span data-ttu-id="8a6fb-111">Si l’état HTTP de votre réponse est autre que 200 (OK), la charge utile de la réponse ne contient pas la réponse de découverte automatique que vous recherchez.</span><span class="sxs-lookup"><span data-stu-id="8a6fb-111">If the HTTP status in your response is anything other than 200 (OK), the response payload doesn't contain the Autodiscover response you were looking for.</span></span> <span data-ttu-id="8a6fb-112">Par souci de simplicité, nous pouvons regrouper les codes d’État non 200 en trois catégories.</span><span class="sxs-lookup"><span data-stu-id="8a6fb-112">For simplicity, we can group non-200 status codes into three categories.</span></span>
  
<span data-ttu-id="8a6fb-113">**Tableau 1. Codes d’état HTTP**</span><span class="sxs-lookup"><span data-stu-id="8a6fb-113">**Table 1. HTTP status codes**</span></span>

|<span data-ttu-id="8a6fb-114">**Code d’état**</span><span class="sxs-lookup"><span data-stu-id="8a6fb-114">**Status code**</span></span>|<span data-ttu-id="8a6fb-115">**Type d’erreur**</span><span class="sxs-lookup"><span data-stu-id="8a6fb-115">**Type of error**</span></span>|<span data-ttu-id="8a6fb-116">**Pour gérer...**</span><span class="sxs-lookup"><span data-stu-id="8a6fb-116">**To handle…**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="8a6fb-117">301 ou 302</span><span class="sxs-lookup"><span data-stu-id="8a6fb-117">301 or 302</span></span>  <br/> |<span data-ttu-id="8a6fb-118">Erreur de redirection</span><span class="sxs-lookup"><span data-stu-id="8a6fb-118">Redirect error</span></span>  <br/> |<span data-ttu-id="8a6fb-119">Renvoyez votre requête à l’URI contenu dans l’en-tête de réponse HTTP « location ».</span><span class="sxs-lookup"><span data-stu-id="8a6fb-119">Resend your request to the URI contained in the "Location" HTTP response header.</span></span> <span data-ttu-id="8a6fb-120">Pour plus d’informations, consultez [la rubrique gestion des erreurs de redirection](#bk_HandlingRedirects).</span><span class="sxs-lookup"><span data-stu-id="8a6fb-120">For details, see [Handling redirect errors](#bk_HandlingRedirects).</span></span>  <br/> |
|<span data-ttu-id="8a6fb-121">401</span><span class="sxs-lookup"><span data-stu-id="8a6fb-121">401</span></span>  <br/> |<span data-ttu-id="8a6fb-122">Erreur non autorisée</span><span class="sxs-lookup"><span data-stu-id="8a6fb-122">Unauthorized error</span></span>  <br/> |<span data-ttu-id="8a6fb-123">Étant donné que le [processus de découverte automatique](autodiscover-for-exchange.md) implique de tenter plusieurs URL potentielles, vous pouvez obtenir cette URL sur une seule URL pour qu’elle accepte vos informations d’identification.</span><span class="sxs-lookup"><span data-stu-id="8a6fb-123">Because the [Autodiscover process](autodiscover-for-exchange.md) involves trying multiple potential URLs, you could get this on one URL only to have the next one accept your credentials.</span></span> <span data-ttu-id="8a6fb-124">Pour cette raison, vous ne devez pas prendre en compte une seule erreur 401 pour indiquer que les informations d’identification ne sont pas valides.</span><span class="sxs-lookup"><span data-stu-id="8a6fb-124">For this reason, you shouldn't consider a single 401 error to indicate that the credentials are invalid.</span></span> <span data-ttu-id="8a6fb-125">Toutefois, si vous recevez des erreurs 401 à partir de plusieurs URL, vous pouvez inviter l’utilisateur à entrer de nouveau son mot de passe (le cas échéant).</span><span class="sxs-lookup"><span data-stu-id="8a6fb-125">However, if you receive 401 errors from multiple URLs, you might want to prompt the user to reenter their password (if possible).</span></span>  <br/> |
|<span data-ttu-id="8a6fb-126">Tout autre État autre qu' 200</span><span class="sxs-lookup"><span data-stu-id="8a6fb-126">Any other non-200 status</span></span>  <br/> |<span data-ttu-id="8a6fb-127">Erreur de point de terminaison de découverte automatique non valide</span><span class="sxs-lookup"><span data-stu-id="8a6fb-127">Invalid Autodiscover endpoint error</span></span>  <br/> |<span data-ttu-id="8a6fb-128">Considérez l’URL qui renvoie tout autre code d’État non 200 comme non valide et continuez à essayer l’URL suivante dans votre liste.</span><span class="sxs-lookup"><span data-stu-id="8a6fb-128">Consider the URL that returns any other non-200 status code to be invalid, and continue trying the next URL in your list.</span></span>  <br/> |
   
## <a name="autodiscover-errors"></a><span data-ttu-id="8a6fb-129">Erreurs de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="8a6fb-129">Autodiscover errors</span></span>
<span data-ttu-id="8a6fb-130"><a name="bk_AutodiscoverErrors"> </a></span><span class="sxs-lookup"><span data-stu-id="8a6fb-130"><a name="bk_AutodiscoverErrors"> </a></span></span>

<span data-ttu-id="8a6fb-131">Même si vous obtenez un code d’état 200 (OK) après avoir envoyé une demande de découverte automatique, cela ne signifie pas que le serveur a envoyé les informations dont vous avez besoin.</span><span class="sxs-lookup"><span data-stu-id="8a6fb-131">Even if you get a 200 (OK) status code after sending an Autodiscover request, that doesn't mean that the server sent the information you need.</span></span> <span data-ttu-id="8a6fb-132">L’état 200 uniquement signifie que vous avez une réponse de découverte automatique et que cette réponse peut contenir une erreur au sein de la charge utile.</span><span class="sxs-lookup"><span data-stu-id="8a6fb-132">The 200 status only means that you have an Autodiscover response, and that response might contain an error within the payload.</span></span> <span data-ttu-id="8a6fb-133">L’emplacement des informations relatives à l’erreur diffère selon que le format est SOAP ou POX.</span><span class="sxs-lookup"><span data-stu-id="8a6fb-133">The location of the error information differs depending on whether the format is SOAP or POX.</span></span>
  
### <a name="soap-autodiscover-errors"></a><span data-ttu-id="8a6fb-134">Erreurs de découverte automatique SOAP</span><span class="sxs-lookup"><span data-stu-id="8a6fb-134">SOAP Autodiscover errors</span></span>

<span data-ttu-id="8a6fb-135">Pour la découverte automatique SOAP, la réponse peut contenir un ou plusieurs éléments [ErrorCode (SOAP)](https://msdn.microsoft.com/library/5e5ec861-0191-4ecb-a906-47ce8ed96381%28Office.15%29.aspx) , à différents endroits.</span><span class="sxs-lookup"><span data-stu-id="8a6fb-135">For SOAP Autodiscover, the response can contain one or more [ErrorCode (SOAP)](https://msdn.microsoft.com/library/5e5ec861-0191-4ecb-a906-47ce8ed96381%28Office.15%29.aspx) elements, in different places.</span></span> <span data-ttu-id="8a6fb-136">En règle générale, vous pouvez vous attendre à ce qu’il s’agit d’un élément enfant de l’élément de [réponse (SOAP)](https://msdn.microsoft.com/library/4c2bcdeb-95ce-4ffa-bd83-118af53b534f%28Office.15%29.aspx) et de l’autre en tant qu’enfant de chaque élément [UserResponse (SOAP)](https://msdn.microsoft.com/library/5007b1ba-bfcc-40d7-b1cb-e32fbaf54ffd%28Office.15%29.aspx) dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="8a6fb-136">Typically you can expect one as a child element of the [Response (SOAP)](https://msdn.microsoft.com/library/4c2bcdeb-95ce-4ffa-bd83-118af53b534f%28Office.15%29.aspx) element, and one as a child of each [UserResponse (SOAP)](https://msdn.microsoft.com/library/5007b1ba-bfcc-40d7-b1cb-e32fbaf54ffd%28Office.15%29.aspx) element in the response.</span></span> <span data-ttu-id="8a6fb-137">Vous pouvez également rencontrer un élément enfant d’un élément [UserSettingError (SOAP)](https://msdn.microsoft.com/library/abb175c5-4f38-4dcc-81e3-b511686862eb%28Office.15%29.aspx) , s’il en existe une.</span><span class="sxs-lookup"><span data-stu-id="8a6fb-137">You might also encounter one as a child of a [UserSettingError (SOAP)](https://msdn.microsoft.com/library/abb175c5-4f38-4dcc-81e3-b511686862eb%28Office.15%29.aspx) element, if one is present.</span></span> <span data-ttu-id="8a6fb-138">Le contexte de l’erreur dépend de l’emplacement de l’élément **ErrorCode** , comme suit :</span><span class="sxs-lookup"><span data-stu-id="8a6fb-138">The context of the error depends on where the **ErrorCode** element is located, as follows:</span></span> 
  
- <span data-ttu-id="8a6fb-139">En tant qu’élément enfant de l’élément **Response** , l’élément **ErrorCode** représente une erreur qui s’applique à l’ensemble de la requête.</span><span class="sxs-lookup"><span data-stu-id="8a6fb-139">As a child element of the **Response** element, the **ErrorCode** element represents an error that applies to the entire request.</span></span> 
    
- <span data-ttu-id="8a6fb-140">En tant qu’enfant de l’élément **UserResponse** , il représente une erreur qui s’applique uniquement à cet utilisateur spécifique.</span><span class="sxs-lookup"><span data-stu-id="8a6fb-140">As a child of the **UserResponse** element, it represents an error that applies just to that specific user.</span></span> 
    
- <span data-ttu-id="8a6fb-141">En tant qu’enfant d’un élément **UserSettingError** , il représente une erreur qui s’applique à un paramètre spécifique qui a été demandé.</span><span class="sxs-lookup"><span data-stu-id="8a6fb-141">As a child of a **UserSettingError** element, it represents an error that applies to a specific setting that was requested.</span></span> 
    
<span data-ttu-id="8a6fb-142">Examinons un exemple de réponse.</span><span class="sxs-lookup"><span data-stu-id="8a6fb-142">Let's take a look at an example of a response.</span></span> <span data-ttu-id="8a6fb-143">Dans cet exemple, l’élément **ErrorCode** sous l’élément **Response** a la valeur « NOERROR », ce qui indique une réussite globale.</span><span class="sxs-lookup"><span data-stu-id="8a6fb-143">In this example, the **ErrorCode** element under the **Response** element has a value of "NoError", which indicates overall success.</span></span> <span data-ttu-id="8a6fb-144">Toutefois, l’élément **ErrorCode** sous l’élément **UserResponse** a la valeur « RedirectAddress », ce qui indique qu’une erreur s’est produite pour cet utilisateur particulier.</span><span class="sxs-lookup"><span data-stu-id="8a6fb-144">However, the **ErrorCode** element under the **UserResponse** element has a value of "RedirectAddress", which indicates that an error occurred for that particular user.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/" 
    xmlns:a="http://www.w3.org/2005/08/addressing">
  <s:Header>
    <a:Action s:mustUnderstand="1">https://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetUserSettingsResponse</a:Action>
    <h:ServerVersionInfo xmlns:h="https://schemas.microsoft.com/exchange/2010/Autodiscover" 
        xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
      <h:MajorVersion>14</h:MajorVersion>
      <h:MinorVersion>3</h:MinorVersion>
      <h:MajorBuildNumber>136</h:MajorBuildNumber>
      <h:MinorBuildNumber>1</h:MinorBuildNumber>
      <h:Version>Exchange2010_SP2</h:Version>
    </h:ServerVersionInfo>
  </s:Header>
  <s:Body>
    <GetUserSettingsResponseMessage xmlns="https://schemas.microsoft.com/exchange/2010/Autodiscover">
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

<span data-ttu-id="8a6fb-145">L’article [ErrorCode (SOAP)](https://msdn.microsoft.com/library/5e5ec861-0191-4ecb-a906-47ce8ed96381%28Office.15%29.aspx) contient la liste complète des erreurs possibles.</span><span class="sxs-lookup"><span data-stu-id="8a6fb-145">The [ErrorCode (SOAP)](https://msdn.microsoft.com/library/5e5ec861-0191-4ecb-a906-47ce8ed96381%28Office.15%29.aspx) article contains a full list of possible errors.</span></span> <span data-ttu-id="8a6fb-146">La plupart de ces éléments indiquent une erreur irrécupérable, mais quelques mérites de gestion spéciale.</span><span class="sxs-lookup"><span data-stu-id="8a6fb-146">Most of these indicate an unrecoverable error, but a few warrant special handling.</span></span> 
  
<span data-ttu-id="8a6fb-147">**Tableau 2. Valeurs de code d’découverte automatique SOAP**</span><span class="sxs-lookup"><span data-stu-id="8a6fb-147">**Table 2. SOAP Autodisover ErrorCode values**</span></span>

|<span data-ttu-id="8a6fb-148">**Valeur ErrorCode**</span><span class="sxs-lookup"><span data-stu-id="8a6fb-148">**ErrorCode value**</span></span>|<span data-ttu-id="8a6fb-149">**Pour gérer...**</span><span class="sxs-lookup"><span data-stu-id="8a6fb-149">**To handle…**</span></span>|
|:-----|:-----|
|<span data-ttu-id="8a6fb-150">RedirectAddress</span><span class="sxs-lookup"><span data-stu-id="8a6fb-150">RedirectAddress</span></span>  <br/> |<span data-ttu-id="8a6fb-151">Redémarrage de la [découverte automatique avec une nouvelle adresse de messagerie](#bk_RestartAutodiscover) avec l’adresse de messagerie dans l’élément [RedirectTarget (SOAP)](https://msdn.microsoft.com/library/f8162724-cf9a-4543-a1ad-5846c8b10bfa%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="8a6fb-151">[Restarting Autodiscover with a new email address](#bk_RestartAutodiscover) with the email address in the [RedirectTarget (SOAP)](https://msdn.microsoft.com/library/f8162724-cf9a-4543-a1ad-5846c8b10bfa%28Office.15%29.aspx) element.</span></span>  <br/> |
|<span data-ttu-id="8a6fb-152">RedirectUrl</span><span class="sxs-lookup"><span data-stu-id="8a6fb-152">RedirectUrl</span></span>  <br/> |<span data-ttu-id="8a6fb-153">[Renvoi de votre requête à une nouvelle URL](#bk_ResendRequest) vers l’URL dans l’élément **RedirectTarget** .</span><span class="sxs-lookup"><span data-stu-id="8a6fb-153">[Resending your request to a new URL](#bk_ResendRequest) to the URL in the **RedirectTarget** element.</span></span>  <br/> |
|<span data-ttu-id="8a6fb-154">ServerBusy</span><span class="sxs-lookup"><span data-stu-id="8a6fb-154">ServerBusy</span></span>  <br/> |<span data-ttu-id="8a6fb-155">Renouvelez cette URL après un petit délai.</span><span class="sxs-lookup"><span data-stu-id="8a6fb-155">Retry this URL after a small delay.</span></span> <span data-ttu-id="8a6fb-156">Vous pouvez patienter pendant un laps de temps défini ou simplement déplacer cette URL à la fin de la liste des URL à essayer.</span><span class="sxs-lookup"><span data-stu-id="8a6fb-156">You might wait a set amount of time or simply move this URL to the end of your list of URLs to try.</span></span> <span data-ttu-id="8a6fb-157">Si vous recevez cette erreur plusieurs fois à partir d’une URL, vous devez considérer que l’URL n’est pas valide.</span><span class="sxs-lookup"><span data-stu-id="8a6fb-157">If you receive this error multiple times from a URL, you should consider the URL to be invalid.</span></span>  <br/> |
   
### <a name="pox-autodiscover-errors"></a><span data-ttu-id="8a6fb-158">Erreurs de découverte automatique POX</span><span class="sxs-lookup"><span data-stu-id="8a6fb-158">POX Autodiscover errors</span></span>

<span data-ttu-id="8a6fb-159">Le service de découverte automatique POX signale les erreurs un peu différemment.</span><span class="sxs-lookup"><span data-stu-id="8a6fb-159">The POX Autodiscover service reports errors a little differently.</span></span> <span data-ttu-id="8a6fb-160">Les erreurs non récupérables sont contenues dans l’élément [Error (POX)](https://msdn.microsoft.com/library/91c63b62-ab68-4c32-a2f7-5a87c188335b%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="8a6fb-160">Non-recoverable errors are contained in the [Error (POX)](https://msdn.microsoft.com/library/91c63b62-ab68-4c32-a2f7-5a87c188335b%28Office.15%29.aspx) element.</span></span> <span data-ttu-id="8a6fb-161">L’article [ErrorCode (POX)](https://msdn.microsoft.com/library/064d73e4-45b7-4797-828e-9df590830db8%28Office.15%29.aspx) contient la liste complète des codes d’erreur possibles.</span><span class="sxs-lookup"><span data-stu-id="8a6fb-161">The [ErrorCode (POX)](https://msdn.microsoft.com/library/064d73e4-45b7-4797-828e-9df590830db8%28Office.15%29.aspx) article contains a full list of possible error codes.</span></span> 
  
<span data-ttu-id="8a6fb-162">Les erreurs de redirection sont contenues dans l’élément [action (POX)](https://msdn.microsoft.com/library/a3462c6b-453c-462a-830d-f29ee4a2babb%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="8a6fb-162">Redirect errors are contained in the [Action (POX)](https://msdn.microsoft.com/library/a3462c6b-453c-462a-830d-f29ee4a2babb%28Office.15%29.aspx) element.</span></span> <span data-ttu-id="8a6fb-163">Toute valeur de l’élément **action** autre que « paramètres » indique une erreur de redirection.</span><span class="sxs-lookup"><span data-stu-id="8a6fb-163">Any value of the **Action** element other than "settings" indicates a redirect error.</span></span> 
  
<span data-ttu-id="8a6fb-164">**Tableau 3. Valeurs ErrorCode découverte automatique ErrorCode**</span><span class="sxs-lookup"><span data-stu-id="8a6fb-164">**Table 3. POX Autodisover ErrorCode values**</span></span>

|<span data-ttu-id="8a6fb-165">**Valeur de l’action**</span><span class="sxs-lookup"><span data-stu-id="8a6fb-165">**Action value**</span></span>|<span data-ttu-id="8a6fb-166">**Pour gérer...**</span><span class="sxs-lookup"><span data-stu-id="8a6fb-166">**To handle…**</span></span>|
|:-----|:-----|
|<span data-ttu-id="8a6fb-167">redirectAddr</span><span class="sxs-lookup"><span data-stu-id="8a6fb-167">redirectAddr</span></span>  <br/> |<span data-ttu-id="8a6fb-168">Redémarrage de la [découverte automatique avec une nouvelle adresse de messagerie](#bk_RestartAutodiscover) avec l’adresse de messagerie dans l' [RedirectAddr (POX)](https://msdn.microsoft.com/library/0e9fa6b6-7991-4dc1-a59a-48e5f8e041e4%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="8a6fb-168">[Restarting Autodiscover with a new email address](#bk_RestartAutodiscover) with the email address in the [RedirectAddr (POX)](https://msdn.microsoft.com/library/0e9fa6b6-7991-4dc1-a59a-48e5f8e041e4%28Office.15%29.aspx) element.</span></span>  <br/> |
|<span data-ttu-id="8a6fb-169">redirectUrl</span><span class="sxs-lookup"><span data-stu-id="8a6fb-169">redirectUrl</span></span>  <br/> |<span data-ttu-id="8a6fb-170">[Renvoi de votre requête à une nouvelle URL](#bk_ResendRequest) vers l’URL dans l’élément [redirectUrl (POX)](https://msdn.microsoft.com/library/c54f310f-8c99-4c37-8e73-ac87722b6229%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="8a6fb-170">[Resending your request to a new URL](#bk_ResendRequest) to the URL in the [RedirectUrl (POX)](https://msdn.microsoft.com/library/c54f310f-8c99-4c37-8e73-ac87722b6229%28Office.15%29.aspx) element.</span></span>  <br/> |
   
<span data-ttu-id="8a6fb-171">Dans cet exemple, l’élément **action** a la valeur « redirectAddr », ce qui indique qu’une nouvelle demande doit être envoyée avec la nouvelle adresse e-mail contenue dans l’élément **redirectAddr** .</span><span class="sxs-lookup"><span data-stu-id="8a6fb-171">In this example, the **Action** element has a value of "redirectAddr", which indicates that a new request should be sent with the new email address contained in the **RedirectAddr** element.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<Autodiscover xmlns="https://schemas.microsoft.com/exchange/autodiscover/responseschema/2006">
  <Response xmlns="https://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a">
    <Account>
      <Action>redirectAddr</Action>
      <RedirectAddr>elvin@mail.contoso.com</RedirectAddr>
    </Account>
  </Response>
</Autodiscover>
```

## <a name="handling-redirect-errors"></a><span data-ttu-id="8a6fb-172">Gestion des erreurs de redirection</span><span class="sxs-lookup"><span data-stu-id="8a6fb-172">Handling redirect errors</span></span>
<span data-ttu-id="8a6fb-173"><a name="bk_HandlingRedirects"> </a></span><span class="sxs-lookup"><span data-stu-id="8a6fb-173"><a name="bk_HandlingRedirects"> </a></span></span>

<span data-ttu-id="8a6fb-174">Vous pouvez gérer les scénarios d’erreur de redirection de deux manières :</span><span class="sxs-lookup"><span data-stu-id="8a6fb-174">You can handle redirect error scenarios in two ways:</span></span>
  
- <span data-ttu-id="8a6fb-175">En redémarrant la découverte automatique avec une nouvelle adresse de messagerie.</span><span class="sxs-lookup"><span data-stu-id="8a6fb-175">By restarting Autodiscover with a new email address.</span></span>
    
- <span data-ttu-id="8a6fb-176">En renvoyant votre demande à une nouvelle URL.</span><span class="sxs-lookup"><span data-stu-id="8a6fb-176">By resending your request to a new URL.</span></span>
    
<span data-ttu-id="8a6fb-177">Les deux scénarios nécessitent une validation avant de continuer.</span><span class="sxs-lookup"><span data-stu-id="8a6fb-177">Both scenarios require some validation before proceeding.</span></span>
  
### <a name="restarting-autodiscover-with-a-new-email-address"></a><span data-ttu-id="8a6fb-178">Redémarrage de la découverte automatique avec une nouvelle adresse de messagerie</span><span class="sxs-lookup"><span data-stu-id="8a6fb-178">Restarting Autodiscover with a new email address</span></span>
<span data-ttu-id="8a6fb-179"><a name="bk_RestartAutodiscover"> </a></span><span class="sxs-lookup"><span data-stu-id="8a6fb-179"><a name="bk_RestartAutodiscover"> </a></span></span>

<span data-ttu-id="8a6fb-180">Lorsque vous obtenez une nouvelle adresse de messagerie dans une réponse de redirection de découverte automatique, vérifiez d’abord que la nouvelle adresse de messagerie fournie dans la réponse d’erreur de redirection n’est pas la même adresse que celle que vous avez envoyée dans la demande ayant provoqué l’erreur.</span><span class="sxs-lookup"><span data-stu-id="8a6fb-180">When you get a new email address in an Autodiscover redirect response, first verify that the new email address that was provided in the redirect error response is not the same address that you sent in the request that resulted in the error.</span></span> <span data-ttu-id="8a6fb-181">Si c’est le cas, ne redémarrez pas la découverte automatique et considérez plutôt l’URL qui a généré la réponse pour qu’elle ne soit pas valide.</span><span class="sxs-lookup"><span data-stu-id="8a6fb-181">If it is, you should not restart Autodiscover and instead consider the URL that generated the response to be invalid.</span></span>
  
<span data-ttu-id="8a6fb-182">Si la nouvelle adresse de messagerie est différente, ignorez votre liste existante d’URL de point de terminaison de découverte automatique potentielles et générez une nouvelle liste basée sur la nouvelle adresse de messagerie.</span><span class="sxs-lookup"><span data-stu-id="8a6fb-182">If the new email address is different, discard your existing list of potential Autodiscover endpoint URLs and generate a new list based on the new email address.</span></span>
  
### <a name="resending-your-request-to-a-new-url"></a><span data-ttu-id="8a6fb-183">Renvoi de votre requête à une nouvelle URL</span><span class="sxs-lookup"><span data-stu-id="8a6fb-183">Resending your request to a new URL</span></span>
<span data-ttu-id="8a6fb-184"><a name="bk_ResendRequest"> </a></span><span class="sxs-lookup"><span data-stu-id="8a6fb-184"><a name="bk_ResendRequest"> </a></span></span>

<span data-ttu-id="8a6fb-185">Lorsque vous obtenez une nouvelle URL dans une réponse de redirection de découverte automatique, vous devez d’abord valider l’URL comme suit :</span><span class="sxs-lookup"><span data-stu-id="8a6fb-185">When you get a new URL in an Autodiscover redirect response, you should first validate the URL as follows:</span></span>
  
- <span data-ttu-id="8a6fb-186">Vérifiez que l’URL est une URL HTTPs.</span><span class="sxs-lookup"><span data-stu-id="8a6fb-186">Verify that the URL is an HTTPS URL.</span></span>
    
- <span data-ttu-id="8a6fb-187">Vérifiez que vous n’avez pas reçu une erreur de cette URL avec l’adresse de messagerie actuelle.</span><span class="sxs-lookup"><span data-stu-id="8a6fb-187">Verify that you have not received an error from this URL with the current email address before.</span></span>
    
- <span data-ttu-id="8a6fb-188">Si applicable à votre application, Informez l’utilisateur de la redirection et demandez-lui l’autorisation de suivre la redirection.</span><span class="sxs-lookup"><span data-stu-id="8a6fb-188">If applicable to your application, inform the user of the redirection and get their permission to follow the redirect.</span></span>
    
- <span data-ttu-id="8a6fb-189">Envoyez une demande à l’URL et [Vérifiez que le certificat SSL présenté par le serveur est valide](how-to-validate-a-server-certificate-for-the-ews-managed-api.md).</span><span class="sxs-lookup"><span data-stu-id="8a6fb-189">Send a request to the URL and [verify that the SSL certificate presented by the server is valid](how-to-validate-a-server-certificate-for-the-ews-managed-api.md).</span></span>
    
<span data-ttu-id="8a6fb-190">Si l’URL réussit la validation, renvoyez la demande à cette nouvelle URL.</span><span class="sxs-lookup"><span data-stu-id="8a6fb-190">If the URL passes validation, resend the request to this new URL.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="8a6fb-191">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="8a6fb-191">See also</span></span>


- [<span data-ttu-id="8a6fb-192">Découverte automatique pour Exchange</span><span class="sxs-lookup"><span data-stu-id="8a6fb-192">Autodiscover for Exchange</span></span>](autodiscover-for-exchange.md)
    
- [<span data-ttu-id="8a6fb-193">Trouver des points de terminaison de découverte automatique à l’aide de la recherche SCP dans Exchange</span><span class="sxs-lookup"><span data-stu-id="8a6fb-193">Find Autodiscover endpoints by using SCP lookup in Exchange</span></span>](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md)
    
- [<span data-ttu-id="8a6fb-194">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8a6fb-194">ErrorCode (SOAP)</span></span>](https://msdn.microsoft.com/library/5e5ec861-0191-4ecb-a906-47ce8ed96381%28Office.15%29.aspx)
    
- [<span data-ttu-id="8a6fb-195">ErrorCode (POX)</span><span class="sxs-lookup"><span data-stu-id="8a6fb-195">ErrorCode (POX)</span></span>](https://msdn.microsoft.com/library/064d73e4-45b7-4797-828e-9df590830db8%28Office.15%29.aspx)
    

