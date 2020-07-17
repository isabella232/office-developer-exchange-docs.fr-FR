---
title: Authentification d’une connexion IMAP, POP ou SMTP à l’aide du protocole OAuth
description: Découvrez comment utiliser l’authentification OAuth avec vos applications IMAP, POP et SMTP.
author: svpsiva
ms.date: 02/19/2020
ms.audience: Developer
ms.openlocfilehash: f83a932790cde558e741ece1e87403103aff18fd
ms.sourcegitcommit: eeda51cb037aa25566adb293f25574674fdb2d9e
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/01/2020
ms.locfileid: "45012558"
---
# <a name="authenticate-an-imap-pop-or-smtp-connection-using-oauth"></a><span data-ttu-id="2a9a7-103">Authentification d’une connexion IMAP, POP ou SMTP à l’aide du protocole OAuth</span><span class="sxs-lookup"><span data-stu-id="2a9a7-103">Authenticate an IMAP, POP or SMTP connection using OAuth</span></span>

<span data-ttu-id="2a9a7-104">Découvrez comment utiliser l’authentification OAuth pour vous connecter à des protocoles IMAP, POP ou SMTP et accéder aux données de courrier électronique pour les utilisateurs d’Office 365.</span><span class="sxs-lookup"><span data-stu-id="2a9a7-104">Learn how to use OAuth authentication to connect with IMAP, POP or SMTP protocols and access email data for Office 365 users.</span></span>

> <span data-ttu-id="2a9a7-105">La prise en charge OAuth2 pour IMAP, POP, les protocoles SMTP, comme décrit ci-dessous, n’est pas prise en charge pour les utilisateurs de Outlook.com.</span><span class="sxs-lookup"><span data-stu-id="2a9a7-105">OAuth2 support for IMAP, POP, SMTP protocols as described below is not supported for Outlook.com users.</span></span>

<span data-ttu-id="2a9a7-106">Si vous n’êtes pas familiarisé avec OAuth 2,0, lisez la [rubrique vue d’ensemble de la plateforme d’identité Microsoft (v 2.0)](/azure/active-directory/develop/v2-overview).</span><span class="sxs-lookup"><span data-stu-id="2a9a7-106">If you're not familiar with OAuth 2.0, start by reading the [Microsoft identity platform (v2.0) overview](/azure/active-directory/develop/v2-overview).</span></span> <span data-ttu-id="2a9a7-107">Ce document présente les différents composants de la plateforme d’identité Microsoft, y compris les kits de développement logiciel (SDK).</span><span class="sxs-lookup"><span data-stu-id="2a9a7-107">That document introduces you to different components of Microsoft identity platform, including SDKs.</span></span>

<span data-ttu-id="2a9a7-108">Vous pouvez utiliser le service d’authentification OAuth fourni par Azure Active Directory pour permettre à votre application de se connecter à des protocoles IMAP, POP ou SMTP pour accéder à Exchange Online dans Office 365.</span><span class="sxs-lookup"><span data-stu-id="2a9a7-108">You can use the OAuth authentication service provided by Azure Active Directory to enable your application to connect with IMAP, POP or SMTP protocols to access Exchange Online in Office 365.</span></span> <span data-ttu-id="2a9a7-109">Pour utiliser OAuth avec votre application, vous devez :</span><span class="sxs-lookup"><span data-stu-id="2a9a7-109">To use OAuth with your application you need to:</span></span>

1. <span data-ttu-id="2a9a7-110">[Enregistrez votre application](#register-your-application) auprès d’Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="2a9a7-110">[Register your application](#register-your-application) with Azure Active Directory.</span></span>
1. <span data-ttu-id="2a9a7-111">[Configurez votre application](#configure-your-application) dans Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="2a9a7-111">[Configure your application](#configure-your-application) in Azure Active Directory.</span></span>
1. <span data-ttu-id="2a9a7-112">[Obtenir un jeton d’accès](#get-an-access-token) à partir d’un serveur de jetons.</span><span class="sxs-lookup"><span data-stu-id="2a9a7-112">[Get an access token](#get-an-access-token) from a token server.</span></span>
1. <span data-ttu-id="2a9a7-113">[Authentifier les demandes de connexion](#authenticate-connection-requests) avec un jeton d’accès.</span><span class="sxs-lookup"><span data-stu-id="2a9a7-113">[Authenticate connection requests](#authenticate-connection-requests) with an access token.</span></span>

## <a name="register-your-application"></a><span data-ttu-id="2a9a7-114">Inscrire votre application</span><span class="sxs-lookup"><span data-stu-id="2a9a7-114">Register your application</span></span>

<span data-ttu-id="2a9a7-115">Pour utiliser OAuth, une application doit être inscrite auprès d’Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="2a9a7-115">To use OAuth, an application must be registered with Azure Active Directory.</span></span>

<span data-ttu-id="2a9a7-116">Suivez les instructions indiquées dans [enregistrer une application avec la plateforme d’identité Microsoft](/azure/active-directory/develop/quickstart-register-app) pour créer une application.</span><span class="sxs-lookup"><span data-stu-id="2a9a7-116">Follow the instructions listed in [Register an application with the Microsoft identity platform](/azure/active-directory/develop/quickstart-register-app) to create a new application.</span></span>

## <a name="configure-your-application"></a><span data-ttu-id="2a9a7-117">Configurer votre application</span><span class="sxs-lookup"><span data-stu-id="2a9a7-117">Configure your application</span></span>

<span data-ttu-id="2a9a7-118">Suivez les instructions indiquées dans la [configuration d’une application cliente pour accéder aux API Web](/azure/active-directory/develop/quickstart-configure-app-access-web-apis) .</span><span class="sxs-lookup"><span data-stu-id="2a9a7-118">Follow the instructions listed in [Configure a client application to access web APIs](/azure/active-directory/develop/quickstart-configure-app-access-web-apis)</span></span>

<span data-ttu-id="2a9a7-119">Assurez-vous d’ajouter une ou plusieurs des étendues d’autorisation suivantes qui correspondent aux protocoles que vous souhaitez intégrer.</span><span class="sxs-lookup"><span data-stu-id="2a9a7-119">Make sure to add one or more of the following permission scopes that correspond to the protocols you would like to integrate with.</span></span> <span data-ttu-id="2a9a7-120">Dans l’Assistant **Ajouter une autorisation** , sélectionnez **Microsoft Graph** , puis **autorisations déléguées** pour trouver les étendues d’autorisation suivantes.</span><span class="sxs-lookup"><span data-stu-id="2a9a7-120">In the **Add a permission** wizard, select **Microsoft Graph** and then **Delegated permissions** to find the following permission scopes listed.</span></span>

| <span data-ttu-id="2a9a7-121">Protocole</span><span class="sxs-lookup"><span data-stu-id="2a9a7-121">Protocol</span></span>  | <span data-ttu-id="2a9a7-122">Étendue d’autorisation</span><span class="sxs-lookup"><span data-stu-id="2a9a7-122">Permission scope</span></span>        |
|-----------|-------------------------|
| <span data-ttu-id="2a9a7-123">IMAP</span><span class="sxs-lookup"><span data-stu-id="2a9a7-123">IMAP</span></span>      | `IMAP.AccessAsUser.All` |
| <span data-ttu-id="2a9a7-124">POP</span><span class="sxs-lookup"><span data-stu-id="2a9a7-124">POP</span></span>       | `POP.AccessAsUser.All`  |
| <span data-ttu-id="2a9a7-125">AUTHENTIFICATION SMTP</span><span class="sxs-lookup"><span data-stu-id="2a9a7-125">SMTP AUTH</span></span> | `SMTP.Send`             |

## <a name="get-an-access-token"></a><span data-ttu-id="2a9a7-126">Obtenir un jeton d’accès</span><span class="sxs-lookup"><span data-stu-id="2a9a7-126">Get an access token</span></span>

<span data-ttu-id="2a9a7-127">Vous pouvez utiliser l’une de nos [bibliothèques clientes MSAL](/azure/active-directory/develop/msal-overview) pour récupérer un jeton d’accès à partir de votre application cliente.</span><span class="sxs-lookup"><span data-stu-id="2a9a7-127">You can use one of our [MSAL client libraries](/azure/active-directory/develop/msal-overview) to fetch an access token from your client application.</span></span>

<span data-ttu-id="2a9a7-128">Vous pouvez également sélectionner un flux approprié dans la liste suivante et suivre les étapes correspondantes pour appeler les API REST de la plateforme d’identité sous-jacente et récupérer un jeton d’accès.</span><span class="sxs-lookup"><span data-stu-id="2a9a7-128">Alternatively, you can select an appropriate flow from the following list and follow the corresponding steps to call the underlying identity platform REST APIs and retrieve an access token.</span></span>

1. [<span data-ttu-id="2a9a7-129">Flux de code d’autorisation OAuth2</span><span class="sxs-lookup"><span data-stu-id="2a9a7-129">OAuth2 authorization code flow</span></span>](/azure/active-directory/develop/v2-oauth2-auth-code-flow)
1. [<span data-ttu-id="2a9a7-130">Flux d’octroi d’autorisation d’appareil OAuth2</span><span class="sxs-lookup"><span data-stu-id="2a9a7-130">OAuth2 Device authorization grant flow</span></span>](/azure/active-directory/develop/v2-oauth2-device-code)

<span data-ttu-id="2a9a7-131">L’accès OAuth aux protocoles IMAP, POP et SMTP AUTH via le flux d’octroi d’informations d’identification du client OAuth2 n’est pas pris en charge.</span><span class="sxs-lookup"><span data-stu-id="2a9a7-131">OAuth access to IMAP, POP, SMTP AUTH protocols via OAuth2 client credentials grant flow is not supported.</span></span> <span data-ttu-id="2a9a7-132">Si votre application a besoin d’un accès permanent à toutes les boîtes aux lettres dans une organisation Microsoft 365, nous vous recommandons d’utiliser les API Microsoft Graph autorisant l’accès sans utilisateur, d’activer des autorisations granulaires et de permettre aux administrateurs d’étendre ce type d’accès à un ensemble spécifique de boîtes aux lettres.</span><span class="sxs-lookup"><span data-stu-id="2a9a7-132">If your application needs persistent access to all mailboxes in a Microsoft 365 organization, we recommend that you use the Microsoft Graph APIs which allow access without a user, enable granular permissions and let administrators scope such access to a specific set of mailboxes.</span></span>

<span data-ttu-id="2a9a7-133">Veillez à spécifier les étendues complètes, y compris les URL de ressource Outlook, lorsque vous autorisez votre application et que vous demandez un jeton d’accès.</span><span class="sxs-lookup"><span data-stu-id="2a9a7-133">Make sure to specify the full scopes, including Outlook resource URLs, when authorizing your application and requesting an access token.</span></span>

| <span data-ttu-id="2a9a7-134">Protocole</span><span class="sxs-lookup"><span data-stu-id="2a9a7-134">Protocol</span></span>  | <span data-ttu-id="2a9a7-135">Chaîne d’étendue d’autorisation</span><span class="sxs-lookup"><span data-stu-id="2a9a7-135">Permission scope string</span></span> |
|-----------|-------------------------|
| <span data-ttu-id="2a9a7-136">IMAP</span><span class="sxs-lookup"><span data-stu-id="2a9a7-136">IMAP</span></span>      | `https://outlook.office.com/IMAP.AccessAsUser.All` |
| <span data-ttu-id="2a9a7-137">POP</span><span class="sxs-lookup"><span data-stu-id="2a9a7-137">POP</span></span>       | `https://outlook.office.com/POP.AccessAsUser.All`  |
| <span data-ttu-id="2a9a7-138">AUTHENTIFICATION SMTP</span><span class="sxs-lookup"><span data-stu-id="2a9a7-138">SMTP AUTH</span></span> | `https://outlook.office.com/SMTP.Send`             |

<span data-ttu-id="2a9a7-139">En outre, vous pouvez demander une étendue [offline_access](/azure/active-directory/develop/v2-permissions-and-consent#offline_access) .</span><span class="sxs-lookup"><span data-stu-id="2a9a7-139">In addition, you can request for [offline_access](/azure/active-directory/develop/v2-permissions-and-consent#offline_access) scope.</span></span> <span data-ttu-id="2a9a7-140">Lorsqu’un utilisateur approuve l’étendue offline_access, votre application peut recevoir des jetons d’actualisation à partir du point de terminaison du jeton de plateforme d’identité Microsoft.</span><span class="sxs-lookup"><span data-stu-id="2a9a7-140">When a user approves the offline_access scope, your app can receive refresh tokens from the Microsoft identity platform token endpoint.</span></span> <span data-ttu-id="2a9a7-141">Les jetons d’actualisation sont à durée de vie longue.</span><span class="sxs-lookup"><span data-stu-id="2a9a7-141">Refresh tokens are long-lived.</span></span> <span data-ttu-id="2a9a7-142">Votre application peut obtenir de nouveaux jetons d’accès car les plus anciens arrivent à expiration.</span><span class="sxs-lookup"><span data-stu-id="2a9a7-142">Your app can get new access tokens as older ones expire.</span></span>

## <a name="authenticate-connection-requests"></a><span data-ttu-id="2a9a7-143">Authentifier les demandes de connexion</span><span class="sxs-lookup"><span data-stu-id="2a9a7-143">Authenticate connection requests</span></span>

<span data-ttu-id="2a9a7-144">Vous pouvez établir une connexion aux serveurs de messagerie Office 365 à l’aide des [paramètres de messagerie IMAP et pop pour Office 365](https://support.office.com/article/pop-and-imap-email-settings-for-outlook-8361e398-8af4-4e97-b147-6c6c4ac95353).</span><span class="sxs-lookup"><span data-stu-id="2a9a7-144">You can initiate a connection to Office 365 mail servers using the [IMAP and POP email settings for Office 365](https://support.office.com/article/pop-and-imap-email-settings-for-outlook-8361e398-8af4-4e97-b147-6c6c4ac95353).</span></span>

### <a name="sasl-xoauth2"></a><span data-ttu-id="2a9a7-145">XOAUTH2 SASL</span><span class="sxs-lookup"><span data-stu-id="2a9a7-145">SASL XOAUTH2</span></span>

<span data-ttu-id="2a9a7-146">L’intégration OAuth avec nécessite que votre application utilise le format SASL XOAUTH2 pour coder et transmettre le jeton d’accès.</span><span class="sxs-lookup"><span data-stu-id="2a9a7-146">OAuth integration with requires your application to use SASL XOAUTH2 format for encoding and transmitting the access token.</span></span> <span data-ttu-id="2a9a7-147">SASL XOAUTH2 encode le nom d’utilisateur, le jeton d’accès au format suivant :</span><span class="sxs-lookup"><span data-stu-id="2a9a7-147">SASL XOAUTH2 encodes the username, access token together in the following format:</span></span>

```text
base64("user=" + userName + "^Aauth=Bearer " + accessToken + "^A^A")
```

<span data-ttu-id="2a9a7-148">`^A`représente un **contrôle**  +  **a** ( `%x01` ).</span><span class="sxs-lookup"><span data-stu-id="2a9a7-148">`^A` represents a **Control** + **A** (`%x01`).</span></span>

<span data-ttu-id="2a9a7-149">Par exemple, le format XOAUTH2 SASL pour accéder à un `test@contoso.onmicrosoft.com` jeton d’accès `EwBAAl3BAAUFFpUAo7J3Ve0bjLBWZWCclRC3EoAA` est le suivant :</span><span class="sxs-lookup"><span data-stu-id="2a9a7-149">For example, the SASL XOAUTH2 format to access `test@contoso.onmicrosoft.com` with access token `EwBAAl3BAAUFFpUAo7J3Ve0bjLBWZWCclRC3EoAA` is:</span></span>

```text
base64("user=test@contoso.onmicrosoft.com^Aauth=Bearer EwBAAl3BAAUFFpUAo7J3Ve0bjLBWZWCclRC3EoAA^A^A")
```

<span data-ttu-id="2a9a7-150">Après le codage Base64, cela traduit la chaîne suivante.</span><span class="sxs-lookup"><span data-stu-id="2a9a7-150">After base64 encoding, this translates to the following string.</span></span> <span data-ttu-id="2a9a7-151">Notez que les sauts de ligne sont insérés pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="2a9a7-151">Note that line breaks are inserted for readability.</span></span>

```text
dXNlcj10ZXN0QGNvbnRvc28ub25taWNyb3NvZnQuY29tAWF1dGg9QmVhcmVy
IEV3QkFBbDNCQUFVRkZwVUFvN0ozVmUwYmpMQldaV0NjbFJDM0VvQUEBAQ==
```

### <a name="sasl-xoauth2-authentication-for-shared-mailboxes-in-office-365"></a><span data-ttu-id="2a9a7-152">Authentification SASL XOAUTH2 pour les boîtes aux lettres partagées dans Office 365</span><span class="sxs-lookup"><span data-stu-id="2a9a7-152">SASL XOAUTH2 authentication for shared mailboxes in Office 365</span></span>

<span data-ttu-id="2a9a7-153">Dans le cas d’un accès partagé aux boîtes aux lettres à l’aide d’OAuth, l’application doit obtenir le jeton d’accès au nom d’un utilisateur, mais remplacer le champ nom d’utilisateur dans la chaîne codée SASL XOAUTH2 par l’adresse e-mail de la boîte aux lettres partagée.</span><span class="sxs-lookup"><span data-stu-id="2a9a7-153">In case of shared mailbox access using OAuth, application needs to obtain the access token on behalf of a user but replace the userName field in the SASL XOAUTH2 encoded string with the email address of the shared mailbox.</span></span> 

### <a name="imap-protocol-exchange"></a><span data-ttu-id="2a9a7-154">Échange de protocole IMAP</span><span class="sxs-lookup"><span data-stu-id="2a9a7-154">IMAP Protocol Exchange</span></span>

<span data-ttu-id="2a9a7-155">Pour authentifier une connexion de serveur IMAP, le client doit répondre par une `AUTHENTICATE` commande au format suivant :</span><span class="sxs-lookup"><span data-stu-id="2a9a7-155">To authenticate a IMAP server connection, the client will have to respond with an `AUTHENTICATE` command in the following format:</span></span>

```text
AUTHENTICATE XOAUTH2 <base64 string in XOAUTH2 format>
```

<span data-ttu-id="2a9a7-156">Exemple d’échange de messages client-serveur entraînant une réussite de l’authentification :</span><span class="sxs-lookup"><span data-stu-id="2a9a7-156">Sample client-server message exchange that results in an authentication success:</span></span>

```text
[connection begins]
C: C01 CAPABILITY
S: * CAPABILITY … AUTH=XOAUTH2
S: C01 OK Completed
C: A01 AUTHENTICATE XOAUTH2 dXNlcj1zb21ldXNlckBleGFtcGxlLmNvbQFhdXRoPUJlYXJlciB5YTI5LnZGOWRmdDRxbVRjMk52YjNSbGNrQmhkSFJoZG1semRHRXVZMjl0Q2cBAQ==
S: A01 OK AUTHENTICATE completed.
```

<span data-ttu-id="2a9a7-157">Exemple d’échange de messages client-serveur entraînant un échec d’authentification :</span><span class="sxs-lookup"><span data-stu-id="2a9a7-157">Sample client-server message exchange that results in an authentication failure:</span></span>

```text
[connection begins]
S: * CAPABILITY … AUTH=XOAUTH2
S: C01 OK Completed
C: A01 AUTHENTICATE XOAUTH2 dXNlcj1zb21ldXNlckBleGFtcGxlLmNvbQFhdXRoPUJlYXJlciB5YTI5LnZGOWRmdDRxbVRjMk52YjNSbGNrQmhkSFJoZG1semRHRXVZMjl0Q2cBAQ==
S: A01 NO AUTHENTICATE failed.
```

### <a name="pop-protocol-exchange"></a><span data-ttu-id="2a9a7-158">Échange de protocole POP</span><span class="sxs-lookup"><span data-stu-id="2a9a7-158">POP Protocol Exchange</span></span>

<span data-ttu-id="2a9a7-159">Pour authentifier une connexion de serveur POP, le client doit répondre par une `AUTH` commande divisée en deux lignes au format suivant :</span><span class="sxs-lookup"><span data-stu-id="2a9a7-159">To authenticate a POP server connection, the client will have to respond with an `AUTH` command split into two lines in the following format:</span></span>    

```text 
AUTH XOAUTH2 
<base64 string in XOAUTH2 format>   
``` 

<span data-ttu-id="2a9a7-160">Exemple d’échange de messages client-serveur entraînant une réussite de l’authentification :</span><span class="sxs-lookup"><span data-stu-id="2a9a7-160">Sample client-server message exchange that results in an authentication success:</span></span>    

```text 
[connection begins] 
C: AUTH XOAUTH2     
S: +    
C: dXNlcj1zb21ldXNlckBleGFtcGxlLmNvbQFhdXRoPUJlYX   
JlciB5YTI5LnZGOWRmdDRxbVRjMk52YjNSbGNrQmhkSFJoZG1semRHRXVZMjl0  
Q2cBAQ==    
S: +OK User successfully authenticated. 
[connection continues...]   
``` 

<span data-ttu-id="2a9a7-161">Exemple d’échange de messages client-serveur entraînant un échec d’authentification :</span><span class="sxs-lookup"><span data-stu-id="2a9a7-161">Sample client-server message exchange that results in an authentication failure:</span></span>    

```text 
[connection begins] 
C: AUTH XOAUTH2     
S: +    
C: dXNlcj1zb21ldXNlckBleGFtcGxlLmNvbQFhdXRoPUJlY    
XJlciB5YTI5LnZGOWRmdDRxbVRjMk52YjNSbGNrQmhkSFJoZG1semRHRXVZMj   
l0Q2cBAQ=   
S: -ERR Authentication failure: unknown user name or bad password.  
```

### <a name="smtp-protocol-exchange"></a><span data-ttu-id="2a9a7-162">Échange de protocole SMTP</span><span class="sxs-lookup"><span data-stu-id="2a9a7-162">SMTP Protocol Exchange</span></span>

<span data-ttu-id="2a9a7-163">Pour authentifier une connexion de serveur SMTP, le client doit répondre par une `AUTH` commande au format suivant :</span><span class="sxs-lookup"><span data-stu-id="2a9a7-163">To authenticate a SMTP server connection, the client will have to respond with an `AUTH` command in the following format:</span></span>

```text
AUTH XOAUTH2 <base64 string in XOAUTH2 format>
```

<span data-ttu-id="2a9a7-164">Exemple d’échange de messages client-serveur entraînant une réussite de l’authentification :</span><span class="sxs-lookup"><span data-stu-id="2a9a7-164">Sample client-server message exchange that results in an authentication success:</span></span>

```text
[connection begins]
C: auth xoauth2
S: 334
C: dXNlcj1zb21ldXNlckBleGFtcGxlLmNvbQFhdXRoPUJlY
XJlciB5YTI5LnZGOWRmdDRxbVRjMk52YjNSbGNrQmhkSFJoZG1semRHRXVZMj
l0Q2cBAQ==
S: 235 2.7.0 Authentication successful
[connection continues...]
```

<span data-ttu-id="2a9a7-165">Exemple d’échange de messages client-serveur entraînant un échec d’authentification :</span><span class="sxs-lookup"><span data-stu-id="2a9a7-165">Sample client-server message exchange that results in an authentication failure:</span></span>

```text
[connection begins]
C: auth xoauth2
S: 334
C: dXNlcj1zb21ldXNlckBleGFtcGxlLmNvbQFhdXRoPUJlY
XJlciB5YTI5LnZGOWRmdDRxbVRjMk52YjNSbGNrQmhkSFJoZG1semRHRXVZMj
l0Q2cBAQ==
S: 535 5.7.3 Authentication unsuccessful [SN2PR00CA0018.namprd00.prod.outlook.com]
```

## <a name="see-also"></a><span data-ttu-id="2a9a7-166">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="2a9a7-166">See also</span></span>

- [<span data-ttu-id="2a9a7-167">Authentification et EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="2a9a7-167">Authentication and EWS in Exchange</span></span>](../exchange-web-services/authentication-and-ews-in-exchange.md)
- [<span data-ttu-id="2a9a7-168">IMAP, paramètres de connexion POP</span><span class="sxs-lookup"><span data-stu-id="2a9a7-168">IMAP, POP Connection settings</span></span>](https://support.office.com/article/pop-and-imap-email-settings-for-outlook-8361e398-8af4-4e97-b147-6c6c4ac95353)
- [<span data-ttu-id="2a9a7-169">Internet Message Access Protocol</span><span class="sxs-lookup"><span data-stu-id="2a9a7-169">Internet Message Access Protocol</span></span>](https://tools.ietf.org/html/rfc3501)
- [<span data-ttu-id="2a9a7-170">Protocole post Office</span><span class="sxs-lookup"><span data-stu-id="2a9a7-170">Post Office Protocol</span></span>](https://tools.ietf.org/html/rfc1081)
- [<span data-ttu-id="2a9a7-171">Extension de service SMTP pour l’authentification</span><span class="sxs-lookup"><span data-stu-id="2a9a7-171">SMTP Service extension for Authentication</span></span>](https://tools.ietf.org/html/rfc4954)
