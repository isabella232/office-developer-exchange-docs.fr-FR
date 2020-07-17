---
title: Authentifier une application EWS à l’aide d’OAuth
manager: sethgros
ms.date: 05/17/2019
ms.audience: Developer
ms.assetid: 1d8d57f9-4df5-4f21-9bbb-a89e0e259052
description: Découvrez comment utiliser l’authentification OAuth avec vos applications d’API managée EWS.
localization_priority: Priority
ms.openlocfilehash: 0375095faac918859354da026118ea4ccfd6792b
ms.sourcegitcommit: eeda51cb037aa25566adb293f25574674fdb2d9e
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/01/2020
ms.locfileid: "45012565"
---
<!-- markdownlint-disable MD025 -->
# <a name="authenticate-an-ews-application-by-using-oauth"></a><span data-ttu-id="5ecc0-103">Authentifier une application EWS à l’aide d’OAuth</span><span class="sxs-lookup"><span data-stu-id="5ecc0-103">Authenticate an EWS application by using OAuth</span></span>
<!-- markdownlint-enable MD025 -->

<span data-ttu-id="5ecc0-104">Découvrez comment utiliser l’authentification OAuth avec vos applications d’API managée EWS.</span><span class="sxs-lookup"><span data-stu-id="5ecc0-104">Learn how to use OAuth authentication with your EWS Managed API applications.</span></span>

<span data-ttu-id="5ecc0-105">Vous pouvez utiliser le service d’authentification OAuth fourni par Azure Active Directory pour permettre à vos applications d’API managée EWS d’accéder à Exchange Online dans Office 365.</span><span class="sxs-lookup"><span data-stu-id="5ecc0-105">You can use the OAuth authentication service provided by Azure Active Directory to enable your EWS Managed API applications to access Exchange Online in Office 365.</span></span> <span data-ttu-id="5ecc0-106">Pour utiliser OAuth avec votre application, vous devez :</span><span class="sxs-lookup"><span data-stu-id="5ecc0-106">To use OAuth with your application you will need to:</span></span>

1. <span data-ttu-id="5ecc0-107">[Enregistrez votre application](#register-your-application) auprès d’Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="5ecc0-107">[Register your application](#register-your-application) with Azure Active Directory.</span></span>

2. <span data-ttu-id="5ecc0-108">[Ajoutez du code pour obtenir un jeton d’authentification](#add-code-to-get-an-authentication-token) afin d’obtenir un jeton d’authentification à partir d’un serveur de jetons.</span><span class="sxs-lookup"><span data-stu-id="5ecc0-108">[Add code to get an authentication token](#add-code-to-get-an-authentication-token) to get an authentication token from a token server.</span></span>

3. <span data-ttu-id="5ecc0-109">[Ajoutez un jeton d’authentification aux requêtes EWS](#add-an-authentication-token-to-ews-requests) que vous envoyez.</span><span class="sxs-lookup"><span data-stu-id="5ecc0-109">[Add an authentication token to EWS requests](#add-an-authentication-token-to-ews-requests) that you send.</span></span>

> [!NOTE]
> <span data-ttu-id="5ecc0-110">L’authentification OAuth pour EWS est disponible uniquement dans Exchange dans le cadre d’Office 365.</span><span class="sxs-lookup"><span data-stu-id="5ecc0-110">OAuth authentication for EWS is only available in Exchange as part of Office 365.</span></span> <span data-ttu-id="5ecc0-111">Les applications EWS qui utilisent OAuth doivent être inscrites auprès d’Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="5ecc0-111">EWS applications that use OAuth must be registered with Azure Active Directory.</span></span>

<span data-ttu-id="5ecc0-112">Pour utiliser le code de cet article, vous devez avoir accès à ce qui suit :</span><span class="sxs-lookup"><span data-stu-id="5ecc0-112">To use the code in this article, you will need to have access to the following:</span></span>

- <span data-ttu-id="5ecc0-113">Un compte Office 365 avec une boîte aux lettres Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="5ecc0-113">An Office 365 account with an Exchange Online mailbox.</span></span> <span data-ttu-id="5ecc0-114">Si vous ne disposez pas d’un compte Office 365, vous pouvez vous [inscrire au programme pour les développeurs office 365](https://developer.microsoft.com/office/dev-program) pour obtenir un abonnement gratuit à Office 365.</span><span class="sxs-lookup"><span data-stu-id="5ecc0-114">If you do not have an Office 365 account, you can [sign up for the Office 365 Developer Program](https://developer.microsoft.com/office/dev-program) to get a free Office 365 subscription.</span></span>

- <span data-ttu-id="5ecc0-115">La [bibliothèque d’authentification Microsoft pour .net](/dotnet/api/microsoft.identity.client?view=azure-dotnet).</span><span class="sxs-lookup"><span data-stu-id="5ecc0-115">The [Microsoft Authentication Library for .NET](/dotnet/api/microsoft.identity.client?view=azure-dotnet).</span></span>

- <span data-ttu-id="5ecc0-116">L'[API managée EWS](https://github.com/officedev/ews-managed-api).</span><span class="sxs-lookup"><span data-stu-id="5ecc0-116">The [EWS Managed API](https://github.com/officedev/ews-managed-api).</span></span>


<span data-ttu-id="5ecc0-117">Il existe deux types d’autorisations OAuth qui peuvent être utilisées pour accéder aux API EWS dans Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="5ecc0-117">There are two types of OAuth permissions that can be used to access EWS APIs in Exchange Online.</span></span> <span data-ttu-id="5ecc0-118">Avant de passer au didacticiel, vous devrez choisir le type d’autorisation spécifique à utiliser.</span><span class="sxs-lookup"><span data-stu-id="5ecc0-118">Before you proceed with the tutorial, you will need to choose the specific permission type to use.</span></span>

* <span data-ttu-id="5ecc0-119">Les **autorisations déléguées** sont utilisées par les applications qui ont un utilisateur connecté.</span><span class="sxs-lookup"><span data-stu-id="5ecc0-119">**Delegated permissions** are used by apps that have a signed-in user present.</span></span> <span data-ttu-id="5ecc0-120">Pour ces applications, l’utilisateur ou un administrateur accepte les autorisations demandées par l’application et l’application peut agir en tant qu’utilisateur connecté lors de la réalisation d’appels d’API.</span><span class="sxs-lookup"><span data-stu-id="5ecc0-120">For these apps, either the user or an administrator consents to the permissions that the app requests and the app can act as the signed-in user when making API calls.</span></span> 
* <span data-ttu-id="5ecc0-121">Les **autorisations d’application** sont utilisées par les applications qui s’exécutent sans utilisateur connecté présent ; par exemple, les applications qui s’exécutent en tant que services ou démons d’arrière-plan et peuvent accéder à plusieurs boîtes aux lettres.</span><span class="sxs-lookup"><span data-stu-id="5ecc0-121">**Application permissions** are used by apps that run without a signed-in user present; for example, apps that run as background services or daemons and can access multiple mailboxes.</span></span>

## <a name="register-your-application"></a><span data-ttu-id="5ecc0-122">Inscrire votre application</span><span class="sxs-lookup"><span data-stu-id="5ecc0-122">Register your application</span></span>

<span data-ttu-id="5ecc0-123">Pour utiliser OAuth, une application doit avoir un ID d’application émis par Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="5ecc0-123">To use OAuth, an application must have an application ID issued by Azure Active Directory.</span></span> <span data-ttu-id="5ecc0-124">Dans ce didacticiel, il est supposé que l’application est une application console ; vous devez donc enregistrer votre application en tant que client public avec Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="5ecc0-124">In this tutorial, it is assumed that the application is a console application, so you need to register your application as a public client with Azure Active Directory.</span></span>

1. <span data-ttu-id="5ecc0-125">Ouvrez un navigateur, accédez au [Centre d’administration Azure Active Directory ](https://aad.portal.azure.com) et connectez-vous à l’aide d’un **compte personnel** (ou compte Microsoft) ou d’un **compte professionnel ou scolaire**.</span><span class="sxs-lookup"><span data-stu-id="5ecc0-125">Open a browser and navigate to the [Azure Active Directory admin center](https://aad.portal.azure.com) and login using a **personal account** (aka: Microsoft Account) or **Work or School Account**.</span></span>

1. <span data-ttu-id="5ecc0-126">Sélectionnez **Azure Active Directory** dans le volet de navigation gauche, puis sélectionnez **Inscriptions d’applications** sous **Gérer**.</span><span class="sxs-lookup"><span data-stu-id="5ecc0-126">Select **Azure Active Directory** in the left-hand navigation, then select **App registrations** under **Manage**.</span></span>

1. <span data-ttu-id="5ecc0-127">Sélectionnez **Nouvelle inscription**.</span><span class="sxs-lookup"><span data-stu-id="5ecc0-127">Select **New registration**.</span></span> <span data-ttu-id="5ecc0-128">Sur la page **Inscrire une application**, définissez les valeurs comme suit.</span><span class="sxs-lookup"><span data-stu-id="5ecc0-128">On the **Register an application** page, set the values as follows.</span></span>

    - <span data-ttu-id="5ecc0-129">Définissez **nom** sur un nom convivial pour votre application.</span><span class="sxs-lookup"><span data-stu-id="5ecc0-129">Set **Name** to a friendly name for your app.</span></span>
    - <span data-ttu-id="5ecc0-130">Définissez les **types de comptes pris en charge** sur le choix adapté à votre scénario.</span><span class="sxs-lookup"><span data-stu-id="5ecc0-130">Set **Supported account types** to the choice that makes sense for your scenario.</span></span>
    - <span data-ttu-id="5ecc0-131">Pour l' **URI de redirection**, définissez la liste déroulante sur **client Public (mobile & Desktop)** et définissez la valeur sur `urn:ietf:wg:oauth:2.0:oob` .</span><span class="sxs-lookup"><span data-stu-id="5ecc0-131">For **Redirect URI**, change the dropdown to **Public client (mobile & desktop)** and set the value to `urn:ietf:wg:oauth:2.0:oob`.</span></span>

1. <span data-ttu-id="5ecc0-132">Choisissez **Inscrire**.</span><span class="sxs-lookup"><span data-stu-id="5ecc0-132">Choose **Register**.</span></span> <span data-ttu-id="5ecc0-133">Sur la page suivante, copiez la valeur de l' **ID d’application (client)** et enregistrez-la, vous en aurez besoin plus tard.</span><span class="sxs-lookup"><span data-stu-id="5ecc0-133">On the next page, copy the value of the **Application (client) ID** and save it, you will need it later.</span></span>

1. <span data-ttu-id="5ecc0-134">Sélectionnez **autorisations d’API** dans le volet de navigation de gauche sous **gérer**.</span><span class="sxs-lookup"><span data-stu-id="5ecc0-134">Select **API permissions** in the left-hand navigation under **Manage**.</span></span> 

1. <span data-ttu-id="5ecc0-135">Sélectionnez **Ajouter une autorisation**.</span><span class="sxs-lookup"><span data-stu-id="5ecc0-135">Select **Add a permission**.</span></span> <span data-ttu-id="5ecc0-136">Sur la page autorisations de l' **API de demande** , sélectionnez **Exchange** sous les **API héritées prises en charge**.</span><span class="sxs-lookup"><span data-stu-id="5ecc0-136">On the **Request API permissions** page, select **Exchange** under **Supported legacy APIs**.</span></span> 

1. <span data-ttu-id="5ecc0-137">Pour utiliser des autorisations déléguées, sélectionnez **autorisations déléguées** , puis **EWS. AccessAsUser. All** sous **EWS**.</span><span class="sxs-lookup"><span data-stu-id="5ecc0-137">To use Delegated permissions, select **Delegated permissions** and then select **EWS.AccessAsUser.All** under **EWS**.</span></span> <span data-ttu-id="5ecc0-138">Cliquez sur **Ajouter des autorisations**.</span><span class="sxs-lookup"><span data-stu-id="5ecc0-138">Click on **Add permissions**.</span></span> 

<span data-ttu-id="5ecc0-139">Pour utiliser les autorisations d’application, suivez ces étapes supplémentaires.</span><span class="sxs-lookup"><span data-stu-id="5ecc0-139">To use Application permissions, follow these additional steps.</span></span>

1. <span data-ttu-id="5ecc0-140">Sélectionnez **autorisations d’application** , puis **full_access_as_app**.</span><span class="sxs-lookup"><span data-stu-id="5ecc0-140">Select **Application permissions** and then select **full_access_as_app**.</span></span> <span data-ttu-id="5ecc0-141">Cliquez sur **Ajouter des autorisations**.</span><span class="sxs-lookup"><span data-stu-id="5ecc0-141">Click on **Add permissions**.</span></span>

1. <span data-ttu-id="5ecc0-142">Sélectionnez **accorder le consentement de l’administrateur pour org** et acceptez la boîte de dialogue de consentement.</span><span class="sxs-lookup"><span data-stu-id="5ecc0-142">Select **Grant admin consent for org** and accept the consent dialog.</span></span> 

1. <span data-ttu-id="5ecc0-143">Sélectionnez **certificats & secrets** dans le volet de navigation de gauche sous **gérer**.</span><span class="sxs-lookup"><span data-stu-id="5ecc0-143">Select **Certificates & Secrets** in the left-hand navigation under **Manage**.</span></span> 

1. <span data-ttu-id="5ecc0-144">Sélectionnez **nouvelle clé secrète client**, entrez une brève description et sélectionnez **Ajouter**.</span><span class="sxs-lookup"><span data-stu-id="5ecc0-144">Select **New client secret**, enter a short description and select **Add**.</span></span>

1. <span data-ttu-id="5ecc0-145">Copiez la **valeur** de la clé secrète client nouvellement ajoutée et enregistrez-la, vous en aurez besoin plus tard.</span><span class="sxs-lookup"><span data-stu-id="5ecc0-145">Copy the **Value** of the newly added client secret and save it, you will need it later.</span></span> 

## <a name="add-code-to-get-an-authentication-token"></a><span data-ttu-id="5ecc0-146">Ajouter du code pour obtenir un jeton d’authentification</span><span class="sxs-lookup"><span data-stu-id="5ecc0-146">Add code to get an authentication token</span></span>

<span data-ttu-id="5ecc0-147">Les extraits de code suivants montrent comment utiliser la bibliothèque d’authentification Microsoft pour obtenir des jetons d’authentification pour les autorisations déléguées et les autorisations d’application.</span><span class="sxs-lookup"><span data-stu-id="5ecc0-147">The following code snippets show how to use the Microsoft Authentication Library to get authentication tokens for delegated permissions and application permissions.</span></span> <span data-ttu-id="5ecc0-148">Ces extraits de code supposent que les informations requises pour effectuer la demande d’authentification sont stockées dans le fichier **App.config** de l’application.</span><span class="sxs-lookup"><span data-stu-id="5ecc0-148">These snippets assume that the information required to make the authentication request is stored in the application's **App.config** file.</span></span> <span data-ttu-id="5ecc0-149">Ces exemples n’incluent pas la vérification des erreurs, reportez-vous aux [exemples de code](#code-samples) pour le code complet.</span><span class="sxs-lookup"><span data-stu-id="5ecc0-149">These examples do not include error checking, see the [Code samples](#code-samples) for the complete code.</span></span>

### <a name="delegated-permissions"></a><span data-ttu-id="5ecc0-150">Autorisations déléguées</span><span class="sxs-lookup"><span data-stu-id="5ecc0-150">Delegated permissions</span></span>

```cs
// Configure the MSAL client to get tokens
var pcaOptions = new PublicClientApplicationOptions
{
    ClientId = ConfigurationManager.AppSettings["appId"],
    TenantId = ConfigurationManager.AppSettings["tenantId"]
};

var pca = PublicClientApplicationBuilder
    .CreateWithApplicationOptions(pcaOptions).Build();

// The permission scope required for EWS access
var ewsScopes = new string[] { "https://outlook.office.com/EWS.AccessAsUser.All" };

// Make the interactive token request
var authResult = await pca.AcquireTokenInteractive(ewsScopes).ExecuteAsync();
```

### <a name="application-permissions"></a><span data-ttu-id="5ecc0-151">Autorisations de l’application</span><span class="sxs-lookup"><span data-stu-id="5ecc0-151">Application permissions</span></span>

```cs
// Configure the MSAL client to get tokens
var app = ConfidentialClientApplicationBuilder
    .Create(ConfigurationManager.AppSettings["appId"])
    .WithAuthority(AzureCloudInstance.AzurePublic, ConfigurationManager.AppSettings["tenantId"])
    .WithClientSecret(ConfigurationManager.AppSettings["clientSecret"]).Build();

// The permission scope required for EWS access
var ewsScopes = new string[] { "https://outlook.office.com/.default" };

//Make the token request
AuthenticationResult authResult = await app.AcquireTokenForClient(ewsScopes).ExecuteAsync();

```

## <a name="add-an-authentication-token-to-ews-requests"></a><span data-ttu-id="5ecc0-152">Ajouter un jeton d’authentification aux requêtes EWS</span><span class="sxs-lookup"><span data-stu-id="5ecc0-152">Add an authentication token to EWS requests</span></span>

<span data-ttu-id="5ecc0-153">Une fois que vous avez reçu l’objet **AuthenticationResult** , vous pouvez utiliser la propriété **AccessToken** pour obtenir le jeton émis par le service de jetons.</span><span class="sxs-lookup"><span data-stu-id="5ecc0-153">After you've received the **AuthenticationResult** object you can use the **AccessToken** property to get the token issued by the token service.</span></span>

```cs
// Configure the ExchangeService with the access token
var ewsClient = new ExchangeService();
ewsClient.Url = new Uri("https://outlook.office365.com/EWS/Exchange.asmx");
ewsClient.Credentials = new OAuthCredentials(authResult.AccessToken);
```

<span data-ttu-id="5ecc0-154">Pour utiliser des autorisations d’application, vous devez également emprunter explicitement l’identité d’une boîte aux lettres à laquelle vous souhaitez accéder.</span><span class="sxs-lookup"><span data-stu-id="5ecc0-154">To use Application permissions, you will also need to explictly impersonate a mailbox that you would like to access.</span></span> 

```cs
//Impersonate the mailbox you'd like to access.
ewsClient.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.SmtpAddress, "test@demotenant.onmicrosoft.com");
```

## <a name="code-samples"></a><span data-ttu-id="5ecc0-155">Exemples de code</span><span class="sxs-lookup"><span data-stu-id="5ecc0-155">Code samples</span></span>

### <a name="delegated-permissions"></a><span data-ttu-id="5ecc0-156">Autorisations déléguées</span><span class="sxs-lookup"><span data-stu-id="5ecc0-156">Delegated permissions</span></span>

<span data-ttu-id="5ecc0-157">Voici l’exemple de code complet qui montre comment effectuer une demande EWS authentifiée OAuth à l’aide d’autorisations déléguées.</span><span class="sxs-lookup"><span data-stu-id="5ecc0-157">The following is the complete code sample that demonstrates making an OAuth-authenticated EWS request using Delegated permissions.</span></span>

```cs
using Microsoft.Exchange.WebServices.Data;
using Microsoft.Identity.Client;
using System;
using System.Configuration;

namespace EwsOAuth
{
    class Program
    {
        static void Main(string[] args)
        {
            MainAsync(args).Wait();

            if (System.Diagnostics.Debugger.IsAttached)
            {
                Console.WriteLine("Hit any key to exit...");
                Console.ReadKey();
            }
        }

        static async System.Threading.Tasks.Task MainAsync(string[] args)
        {
            // Configure the MSAL client to get tokens
            var pcaOptions = new PublicClientApplicationOptions
            {
                ClientId = ConfigurationManager.AppSettings["appId"],
                TenantId = ConfigurationManager.AppSettings["tenantId"]
            };

            var pca = PublicClientApplicationBuilder
                .CreateWithApplicationOptions(pcaOptions).Build();

            var ewsScopes = new string[] { "https://outlook.office.com/EWS.AccessAsUser.All" };

            try
            {
                // Make the interactive token request
                var authResult = await pca.AcquireTokenInteractive(ewsScopes).ExecuteAsync();

                // Configure the ExchangeService with the access token
                var ewsClient = new ExchangeService();
                ewsClient.Url = new Uri("https://outlook.office365.com/EWS/Exchange.asmx");
                ewsClient.Credentials = new OAuthCredentials(authResult.AccessToken);

                // Make an EWS call
                var folders = ewsClient.FindFolders(WellKnownFolderName.MsgFolderRoot, new FolderView(10));
                foreach(var folder in folders)
                {
                    Console.WriteLine($"Folder: {folder.DisplayName}");
                }
            }
            catch (MsalException ex)
            {
                Console.WriteLine($"Error acquiring access token: {ex.ToString()}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.ToString()}");
            }
        }
    }
}
```

### <a name="application-permissions"></a><span data-ttu-id="5ecc0-158">Autorisations de l’application</span><span class="sxs-lookup"><span data-stu-id="5ecc0-158">Application permissions</span></span>

<span data-ttu-id="5ecc0-159">Voici l’exemple de code complet qui montre comment effectuer une demande EWS authentifiée OAuth à l’aide d’autorisations d’application.</span><span class="sxs-lookup"><span data-stu-id="5ecc0-159">The following is the complete code sample that demonstrates making an OAuth-authenticated EWS request using Application permissions.</span></span>

```cs
using System;
using System.Configuration;
using Microsoft.Exchange.WebServices.Data;
using Microsoft.Identity.Client;

namespace ews_oauth_samples
{
    class Program
    {
        static void Main(string[] args)
        {
            MainAsync(args).Wait();

            if (System.Diagnostics.Debugger.IsAttached)
            {
                Console.WriteLine("Hit any key to exit...");
                Console.ReadKey();
            }
        }
        
        static async System.Threading.Tasks.Task MainAsync(string[] args)
        {
            // Configure the MSAL client to get tokens
            var ewsScopes = new string[] { "https://outlook.office.com/.default" };

            var app = ConfidentialClientApplicationBuilder.Create(ConfigurationManager.AppSettings["appId"])
                .WithAuthority(AzureCloudInstance.AzurePublic, ConfigurationManager.AppSettings["tenantId"])
                .WithClientSecret(ConfigurationManager.AppSettings["clientSecret"])
                .Build();

            AuthenticationResult result = null;

            try
            {
                // Make the interactive token request
                result = await app.AcquireTokenForClient(ewsScopes)
                    .ExecuteAsync();

                // Configure the ExchangeService with the access token
                var ewsClient = new ExchangeService();
                ewsClient.Url = new Uri("https://outlook.office365.com/EWS/Exchange.asmx");
                ewsClient.Credentials = new OAuthCredentials(result.AccessToken);

                //Impersonate the mailbox you'd like to access.
                ewsClient.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.SmtpAddress, "test@demotenant.onmicrosoft.com");

                // Make an EWS call
                var folders = ewsClient.FindFolders(WellKnownFolderName.MsgFolderRoot, new FolderView(10));
                foreach (var folder in folders)
                {
                    Console.WriteLine($"Folder: {folder.DisplayName}");
                }
            }
            catch (MsalException ex)
            {
                Console.WriteLine($"Error acquiring access token: {ex.ToString()}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.ToString()}");
            }
        }
    }
}
```

<span data-ttu-id="5ecc0-160">Dans les deux cas, l’exemple de code requiert un fichier **App.config** avec les entrées suivantes :</span><span class="sxs-lookup"><span data-stu-id="5ecc0-160">The sample code in both cases requires an **App.config** file with the following entries:</span></span>

```xml
<?xml version="1.0" encoding="utf-8" ?>
<configuration>
  <startup>
    <supportedRuntime version="v4.0" sku=".NETFramework,Version=v4.7.2" />
  </startup>
  <appSettings>
    <!-- The application ID from your app registration -->
    <add key="appId" value="YOUR_APP_ID_HERE" />
    <!-- If you registered your app to support only users in your organization, change the value
           of this key to your tenant ID -->
    <add key="tenantId" value="common"/>
    <!-- The application's client secret from your app registration. Needed for application permission access -->
    <add key="clientSecret" value="YOUR_CLIENT_SECRET_HERE"/>
  </appSettings>
</configuration>
```

## <a name="see-also"></a><span data-ttu-id="5ecc0-161">Consultez aussi</span><span class="sxs-lookup"><span data-stu-id="5ecc0-161">See also</span></span>

- [<span data-ttu-id="5ecc0-162">Authentification et EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="5ecc0-162">Authentication and EWS in Exchange</span></span>](authentication-and-ews-in-exchange.md)
