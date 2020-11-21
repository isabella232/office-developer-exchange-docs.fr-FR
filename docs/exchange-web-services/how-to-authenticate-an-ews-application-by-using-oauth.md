---
title: Authentifier une application EWS à l’aide d’OAuth
manager: sethgros
ms.date: 11/19/2020
ms.audience: Developer
ms.assetid: 1d8d57f9-4df5-4f21-9bbb-a89e0e259052
description: Apprendre à utiliser l’authentification OAuth avec vos applications EWS Managed API.
localization_priority: Priority
ms.openlocfilehash: c52b254f14cadd287a709bb68f8464e7cfe1837a
ms.sourcegitcommit: 2d16ba247a8cb4b6c8ca9941cb079f75202aae1e
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/19/2020
ms.locfileid: "49356492"
---
<!-- markdownlint-disable MD025 -->
# <a name="authenticate-an-ews-application-by-using-oauth"></a><span data-ttu-id="793ea-103">Authentifier une application EWS à l’aide d’OAuth</span><span class="sxs-lookup"><span data-stu-id="793ea-103">Authenticate an EWS application by using OAuth</span></span>
<!-- markdownlint-enable MD025 -->

<span data-ttu-id="793ea-104">Apprendre à utiliser l’authentification OAuth avec vos applications EWS Managed API.</span><span class="sxs-lookup"><span data-stu-id="793ea-104">Learn how to use OAuth authentication with your EWS Managed API applications.</span></span>

<span data-ttu-id="793ea-105">Vous pouvez utiliser le service d’authentification OAuth fourni par Azure Active Directory pour permettre à vos applications EWS Managed API d’accéder à Exchange Online dans Office 365.</span><span class="sxs-lookup"><span data-stu-id="793ea-105">You can use the OAuth authentication service provided by Azure Active Directory to enable your EWS Managed API applications to access Exchange Online in Office 365.</span></span> <span data-ttu-id="793ea-106">Pour utiliser OAuth avec votre application, vous devrez :</span><span class="sxs-lookup"><span data-stu-id="793ea-106">To use OAuth with your application you will need to:</span></span>

1. <span data-ttu-id="793ea-107">[Inscrire votre application](#register-your-application) dans Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="793ea-107">[Register your application](#register-your-application) with Azure Active Directory.</span></span>
1. <span data-ttu-id="793ea-108">[Ajouter un code pour obtenir un jeton d’authentification](#add-code-to-get-an-authentication-token) afin d’obtenir un jeton d’authentification à partir d’un serveur de jetons.</span><span class="sxs-lookup"><span data-stu-id="793ea-108">[Add code to get an authentication token](#add-code-to-get-an-authentication-token) to get an authentication token from a token server.</span></span>
1. <span data-ttu-id="793ea-109">[Ajouter un jeton d’authentification aux demandes EWS](#add-an-authentication-token-to-ews-requests) que vous envoyez.</span><span class="sxs-lookup"><span data-stu-id="793ea-109">[Add an authentication token to EWS requests](#add-an-authentication-token-to-ews-requests) that you send.</span></span>

> [!NOTE]
> <span data-ttu-id="793ea-110">L’authentification OAuth pour EWS est disponible uniquement dans Exchange dans le cadre d’Office 365.</span><span class="sxs-lookup"><span data-stu-id="793ea-110">OAuth authentication for EWS is only available in Exchange Online as part of Microsoft 365.</span></span> <span data-ttu-id="793ea-111">Les applications EWS qui utilisent OAuth doivent être inscrites auprès d’Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="793ea-111">EWS applications that use OAuth must be registered with Azure Active Directory.</span></span>

<span data-ttu-id="793ea-112">Pour utiliser le code dans cet article, vous devrez avoir accès aux éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="793ea-112">To use the code in this article, you will need to have access to the following:</span></span>

- <span data-ttu-id="793ea-113">Un compte Office 365 avec une boîte aux lettres Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="793ea-113">A Microsoft 365 account with an Exchange Online mailbox.</span></span> <span data-ttu-id="793ea-114">Si vous n’avez pas de compte Office 365, vous pouvez [vous inscrire au programme pour les développeurs Office 365](https://developer.microsoft.com/microsoft-365/dev-program) pour obtenir un abonnement gratuit à Office 365.</span><span class="sxs-lookup"><span data-stu-id="793ea-114">If you do not have a Microsoft 365 account, you can [sign up for the Microsoft 365 Developer Program](https://developer.microsoft.com/microsoft-365/dev-program) to get a free Microsoft 365 subscription.</span></span>
- <span data-ttu-id="793ea-115">La [bibliothèque d’authentification Microsoft pour .NET](/dotnet/api/microsoft.identity.client).</span><span class="sxs-lookup"><span data-stu-id="793ea-115">The [Microsoft Authentication Library for .NET](/dotnet/api/microsoft.identity.client).</span></span>
- <span data-ttu-id="793ea-116">L’ [API gérée EWS](https://github.com/officedev/ews-managed-api).</span><span class="sxs-lookup"><span data-stu-id="793ea-116">The [EWS Managed API](https://github.com/officedev/ews-managed-api).</span></span>

<span data-ttu-id="793ea-117">Deux types d’autorisations OAuth peuvent être utilisés pour accéder aux API EWS dans Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="793ea-117">There are two types of OAuth permissions that can be used to access EWS APIs in Exchange Online.</span></span> <span data-ttu-id="793ea-118">Avant de commencer le tutoriel, vous devrez choisir le type de permission spécifique à utiliser.</span><span class="sxs-lookup"><span data-stu-id="793ea-118">Before you proceed with the tutorial, you will need to choose the specific permission type to use.</span></span>

- <span data-ttu-id="793ea-119">Des **autorisations déléguées** sont utilisées par les applications qui ont un utilisateur connecté.</span><span class="sxs-lookup"><span data-stu-id="793ea-119">**Delegated permissions** are used by apps that have a signed-in user present.</span></span> <span data-ttu-id="793ea-120">Pour ces applications, l’utilisateur ou un administrateur consent aux autorisations demandées par l’application, et l’application peut agir en tant qu’utilisateur connecté lors des appels API.</span><span class="sxs-lookup"><span data-stu-id="793ea-120">For these apps, either the user or an administrator consents to the permissions that the app requests and the app can act as the signed-in user when making API calls.</span></span>
- <span data-ttu-id="793ea-121">Des **autorisations d’application** sont utilisées par les applications qui s’exécutent sans utilisateur connecté ; par exemple, les applications qui s’exécutent en tant que démons ou services d’arrière-plan et qui peuvent accéder à plusieurs boîtes aux lettres.</span><span class="sxs-lookup"><span data-stu-id="793ea-121">**Application permissions** are used by apps that run without a signed-in user present; for example, apps that run as background services or daemons and can access multiple mailboxes.</span></span>

## <a name="register-your-application"></a><span data-ttu-id="793ea-122">Inscription de votre application</span><span class="sxs-lookup"><span data-stu-id="793ea-122">Register your application</span></span>

<span data-ttu-id="793ea-123">Pour utiliser OAuth, une application doit avoir une ID d’application émise par Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="793ea-123">To use OAuth, an application must have an application ID issued by Azure Active Directory.</span></span> <span data-ttu-id="793ea-124">Dans ce tutoriel, l’application est supposée être une application console, alors vous devez enregistrer votre application en tant que client public à l’aide d’Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="793ea-124">In this tutorial, it is assumed that the application is a console application, so you need to register your application as a public client with Azure Active Directory.</span></span> <span data-ttu-id="793ea-125">Vous pouvez inscrire une application dans le centre d’administration Azure Active Directory ou à l’aide de Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="793ea-125">You can register an application in the Azure Active Directory admin center or by using Microsoft Graph.</span></span>

1. <span data-ttu-id="793ea-126">Ouvrez un navigateur, accédez au [Centre d’administration Azure Active Directory](https://aad.portal.azure.com) et connectez-vous à l’aide d’un **compte personnel** (ou compte Microsoft) ou d’un **compte professionnel ou scolaire**.</span><span class="sxs-lookup"><span data-stu-id="793ea-126">Open a browser and navigate to the [Azure Active Directory admin center](https://aad.portal.azure.com) and login using a **personal account** (aka: Microsoft Account) or **Work or School Account**.</span></span>

1. <span data-ttu-id="793ea-127">Sélectionnez **Azure Active Directory** dans le volet de navigation gauche, puis sélectionnez **Inscriptions d’applications** sous **Gérer**.</span><span class="sxs-lookup"><span data-stu-id="793ea-127">Select **Azure Active Directory** in the left-hand navigation, then select **App registrations** under **Manage**.</span></span>

1. <span data-ttu-id="793ea-128">Sélectionnez **Nouvelle inscription**.</span><span class="sxs-lookup"><span data-stu-id="793ea-128">Select **New registration**.</span></span> <span data-ttu-id="793ea-129">Sur la page **Inscrire une application**, définissez les valeurs comme suit.</span><span class="sxs-lookup"><span data-stu-id="793ea-129">On the **Register an application** page, set the values as follows.</span></span>

    - <span data-ttu-id="793ea-130">Définissez **Nom** pour un nom convivial de votre application.</span><span class="sxs-lookup"><span data-stu-id="793ea-130">Set **Name** to a friendly name for your app.</span></span>
    - <span data-ttu-id="793ea-131">Définissez **types de comptes pris en charge** pour le choix adapté à votre scénario.</span><span class="sxs-lookup"><span data-stu-id="793ea-131">Set **Supported account types** to the choice that makes sense for your scenario.</span></span>
    - <span data-ttu-id="793ea-132">Pour **Rediriger URI**, remplacez la liste déroulante par **client public (mobile & bureau)** et définissez la valeur sur `urn:ietf:wg:oauth:2.0:oob`.</span><span class="sxs-lookup"><span data-stu-id="793ea-132">For **Redirect URI**, change the dropdown to **Public client (mobile & desktop)** and set the value to `urn:ietf:wg:oauth:2.0:oob`.</span></span>

1. <span data-ttu-id="793ea-133">Choisissez **Inscrire**.</span><span class="sxs-lookup"><span data-stu-id="793ea-133">Choose **Register**.</span></span> <span data-ttu-id="793ea-134">Sur la page Application console Graph, copiez les valeurs de **l’ID de l’application (client)** et de **l’ID du répertoire (client)**  ; vous en aurez besoin plus loin dans cet exercice.</span><span class="sxs-lookup"><span data-stu-id="793ea-134">On the next page, copy the values of the **Application (client) ID** and **Directory (tenant) ID** and save them, you will need them later.</span></span>

### <a name="configure-for-delegated-authentication"></a><span data-ttu-id="793ea-135">Configurer pour l’authentification déléguée</span><span class="sxs-lookup"><span data-stu-id="793ea-135">Configure for delegated authentication</span></span>

<span data-ttu-id="793ea-136">Si votre application utilise l’authentification déléguée, aucune configuration ultérieure n’est requise.</span><span class="sxs-lookup"><span data-stu-id="793ea-136">If your application uses delegated authentication, no further configuration is required.</span></span> <span data-ttu-id="793ea-137">La [Microsoft Identity Platform] permet aux applications de demander des autorisations de façon dynamique, de sorte que vous n’avez pas à configurer préalablement les autorisations sur l’inscription de l’application.</span><span class="sxs-lookup"><span data-stu-id="793ea-137">The [Microsoft identity platform] allows apps to request permissions dynamically, so you do not have to pre-configure permissions on the app registration.</span></span> <span data-ttu-id="793ea-138">Toutefois, dans certains scénarios (par exemples, [au nom du flux](/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow)), la configuration préalable des autorisations est requise.</span><span class="sxs-lookup"><span data-stu-id="793ea-138">However, in some scenarios (like the [on-behalf-of flow](/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow)) pre-configuring permissions is required.</span></span> <span data-ttu-id="793ea-139">Suivez les étapes ci-dessous pour préconfigurer les autorisations EWS.</span><span class="sxs-lookup"><span data-stu-id="793ea-139">Use the following steps to pre-configure EWS permissions.</span></span>

1. <span data-ttu-id="793ea-140">Sélectionnez **Autorisations de l’API** dans le volet de navigation gauche sous **Gérer**.</span><span class="sxs-lookup"><span data-stu-id="793ea-140">Select **Manifest** in the left-hand navigation under **Manage**.</span></span>

1. <span data-ttu-id="793ea-141">Recherchez la propriété `requiredResourceAccess` dans le manifeste, puis ajoutez les éléments suivants à l’intérieur des crochets (`[]`) :</span><span class="sxs-lookup"><span data-stu-id="793ea-141">Locate the `requiredResourceAccess` property in the manifest, and add the following inside the square brackets (`[]`):</span></span>

    ```json
    {
        "resourceAppId": "00000002-0000-0ff1-ce00-000000000000",
        "resourceAccess": [
            {
                "id": "3b5f3d61-589b-4a3c-a359-5dd4b5ee5bd5",
                "type": "Scope"
            }
        ]
    }
    ```

1. <span data-ttu-id="793ea-142">Sélectionnez **Enregistrer**.</span><span class="sxs-lookup"><span data-stu-id="793ea-142">Select **Save**.</span></span>

1. <span data-ttu-id="793ea-143">Sélectionnez **Autorisations de l’API** dans le volet de navigation gauche sous **Gérer**.</span><span class="sxs-lookup"><span data-stu-id="793ea-143">Select **API permissions** under **Manage**.</span></span> <span data-ttu-id="793ea-144">Vérifiez que l’autorisation **EWS.AccessAsUser.All** est répertoriée.</span><span class="sxs-lookup"><span data-stu-id="793ea-144">Confirm that the **EWS.AccessAsUser.All** permission is listed.</span></span>

### <a name="configure-for-app-only-authentication"></a><span data-ttu-id="793ea-145">Configurer pour l’authentification de l’application uniquement</span><span class="sxs-lookup"><span data-stu-id="793ea-145">Configure for app-only authentication</span></span>

<span data-ttu-id="793ea-146">Pour utiliser les autorisations des applications, suivez ces étapes supplémentaires.</span><span class="sxs-lookup"><span data-stu-id="793ea-146">To use application permissions, follow these additional steps.</span></span>

1. <span data-ttu-id="793ea-147">Sélectionnez **Autorisations de l’API** dans le volet de navigation gauche sous **Gérer**.</span><span class="sxs-lookup"><span data-stu-id="793ea-147">Select **Manifest** in the left-hand navigation under **Manage**.</span></span>

1. <span data-ttu-id="793ea-148">Recherchez la propriété `requiredResourceAccess` dans le manifeste, puis ajoutez les éléments suivants à l’intérieur des crochets (`[]`) :</span><span class="sxs-lookup"><span data-stu-id="793ea-148">Locate the `requiredResourceAccess` property in the manifest, and add the following inside the square brackets (`[]`):</span></span>

    ```json
    {
        "resourceAppId": "00000002-0000-0ff1-ce00-000000000000",
        "resourceAccess": [
            {
                "id": "dc890d15-9560-4a4c-9b7f-a736ec74ec40",
                "type": "Role"
            }
        ]
    }
    ```

1. <span data-ttu-id="793ea-149">Sélectionnez **Enregistrer**.</span><span class="sxs-lookup"><span data-stu-id="793ea-149">Select **Save**.</span></span>

1. <span data-ttu-id="793ea-150">Sélectionnez **Autorisations de l’API** dans le volet de navigation gauche sous **Gérer**.</span><span class="sxs-lookup"><span data-stu-id="793ea-150">Select **API permissions** under **Manage**.</span></span> <span data-ttu-id="793ea-151">Vérifiez que l’autorisation **full_access_as_app** est répertoriée.</span><span class="sxs-lookup"><span data-stu-id="793ea-151">Confirm that the **full_access_as_app** permission is listed.</span></span>

1. <span data-ttu-id="793ea-152">Sélectionnez **Accorder l’autorisation d’administrateur pour l'entreprise** puis acceptez la boîte de dialogue de consentement.</span><span class="sxs-lookup"><span data-stu-id="793ea-152">Select **Grant admin consent for org** and accept the consent dialog.</span></span>

1. <span data-ttu-id="793ea-153">Sélectionnez **Certificats et clés secrètes** dans le volet de navigation gauche sous **Gérer**.</span><span class="sxs-lookup"><span data-stu-id="793ea-153">Select **Certificates & Secrets** in the left-hand navigation under **Manage**.</span></span>

1. <span data-ttu-id="793ea-154">Sélectionnez **Secret nouveau client**, entrez une courte description, puis sélectionnez **Ajouter**.</span><span class="sxs-lookup"><span data-stu-id="793ea-154">Select **New client secret**, enter a short description and select **Add**.</span></span>

1. <span data-ttu-id="793ea-155">Copiez la **Valeur** du nouveau secret client ajouté et enregistrez-le. vous en aurez besoin plus tard.</span><span class="sxs-lookup"><span data-stu-id="793ea-155">Copy the **Value** of the newly added client secret and save it, you will need it later.</span></span>

## <a name="add-code-to-get-an-authentication-token"></a><span data-ttu-id="793ea-156">Ajouter un code pour obtenir un jeton d’authentification</span><span class="sxs-lookup"><span data-stu-id="793ea-156">Add code to get an authentication token</span></span>

<span data-ttu-id="793ea-157">Les extraits de code suivants montrent comment utiliser la bibliothèque d’authentification Microsoft pour obtenir des jetons d’authentification pour les autorisations déléguées et les autorisations d’application.</span><span class="sxs-lookup"><span data-stu-id="793ea-157">The following code snippets show how to use the Microsoft Authentication Library to get authentication tokens for delegated permissions and application permissions.</span></span> <span data-ttu-id="793ea-158">Ces extraits de code partent du principe que les informations requises pour effectuer la demande d’authentification sont stockées dans le fichier **App. config** de l’application.</span><span class="sxs-lookup"><span data-stu-id="793ea-158">These snippets assume that the information required to make the authentication request is stored in the application's **App.config** file.</span></span> <span data-ttu-id="793ea-159">Ces exemples ne comprennent pas la vérification des erreurs, voir les [exemples de code](#code-samples) pour le code complet.</span><span class="sxs-lookup"><span data-stu-id="793ea-159">These examples do not include error checking, see the [Code samples](#code-samples) for the complete code.</span></span>

### <a name="get-a-token-with-delegated-auth"></a><span data-ttu-id="793ea-160">Obtenir un jeton avec l’authentification déléguée</span><span class="sxs-lookup"><span data-stu-id="793ea-160">Get a token with delegated auth</span></span>

```cs
// Using Microsoft.Identity.Client 4.22.0
var pca = PublicClientApplicationBuilder
    .Create(ConfigurationManager.AppSettings["appId"])
    .Build();

// The permission scope required for EWS access
var ewsScopes = new string[] { "EWS.AccessAsUser.All" };

// Make the interactive token request
var authResult = await pca.AcquireTokenInteractive(ewsScopes).ExecuteAsync();
```

### <a name="get-a-token-with-app-only-auth"></a><span data-ttu-id="793ea-161">Obtenir un jeton avec l’authentification de l’application uniquement</span><span class="sxs-lookup"><span data-stu-id="793ea-161">Get a token with app-only auth</span></span>

```cs
// Using Microsoft.Identity.Client 4.22.0
var cca = ConfidentialClientApplicationBuilder
    .Create(ConfigurationManager.AppSettings["appId"])
    .WithClientSecret(ConfigurationManager.AppSettings["clientSecret"])
    .WithTenantId(ConfigurationManager.AppSettings["tenantId"])
    .Build();

// The permission scope required for EWS access
var ewsScopes = new string[] { "https://outlook.office365.com/.default" };

//Make the token request
var authResult = await app.AcquireTokenForClient(ewsScopes).ExecuteAsync();
```

## <a name="add-an-authentication-token-to-ews-requests"></a><span data-ttu-id="793ea-162">Ajouter un jeton d’authentification aux demandes EWS</span><span class="sxs-lookup"><span data-stu-id="793ea-162">Add an authentication token to EWS requests</span></span>

<span data-ttu-id="793ea-163">Une fois que vous avez reçu l’objet **RésultatAuthentification** vous pouvez utiliser la propriété du **Jetond’Accès** pour obtenir le jeton émis par le service d’émission de jeton.</span><span class="sxs-lookup"><span data-stu-id="793ea-163">After you've received the **AuthenticationResult** object you can use the **AccessToken** property to get the token issued by the token service.</span></span>

```cs
// Configure the ExchangeService with the access token
var ewsClient = new ExchangeService();
ewsClient.Url = new Uri("https://outlook.office365.com/EWS/Exchange.asmx");
ewsClient.Credentials = new OAuthCredentials(authResult.AccessToken);
```

<span data-ttu-id="793ea-164">Pour utiliser les autorisations d’application, vous devez également emprunter explicitement une boîte aux lettres à laquelle vous voulez accéder.</span><span class="sxs-lookup"><span data-stu-id="793ea-164">To use application permissions, you will also need to explicitly impersonate a mailbox that you would like to access.</span></span>

```cs
//Impersonate the mailbox you'd like to access.
ewsClient.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.SmtpAddress, "test@demotenant.onmicrosoft.com");
```

## <a name="code-samples"></a><span data-ttu-id="793ea-165">Exemples de code</span><span class="sxs-lookup"><span data-stu-id="793ea-165">Code samples</span></span>

### <a name="delegated-authentication"></a><span data-ttu-id="793ea-166">Authentification déléguée</span><span class="sxs-lookup"><span data-stu-id="793ea-166">Delegated authentication</span></span>

<span data-ttu-id="793ea-167">Ce qui suit est l’échantillon de code complet qui démontre qu’une demande EWS authentifiée OAuth utilise les autorisations d’application.</span><span class="sxs-lookup"><span data-stu-id="793ea-167">The following is the complete code sample that demonstrates making an OAuth-authenticated EWS request using delegated authentication.</span></span>

```cs
using Microsoft.Exchange.WebServices.Data;
using Microsoft.Identity.Client;
using System;
using System.Configuration;

namespace EwsOAuth
{
    class Program
    {
        static async System.Threading.Tasks.Task Main(string[] args)
        {
            // Using Microsoft.Identity.Client 4.22.0
            var pca = PublicClientApplicationBuilder
                .Create(ConfigurationManager.AppSettings["appId"])
                .Build();

            var ewsScopes = new string[] { "EWS.AccessAsUser.All" };

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
                Console.WriteLine($"Error acquiring access token: {ex}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex}");
            }

            if (System.Diagnostics.Debugger.IsAttached)
            {
                Console.WriteLine("Hit any key to exit...");
                Console.ReadKey();
            }
        }
    }
}
```

### <a name="app-only-authentication"></a><span data-ttu-id="793ea-168">Authentification de l'application uniquement</span><span class="sxs-lookup"><span data-stu-id="793ea-168">App-only authentication</span></span>

<span data-ttu-id="793ea-169">Ce qui suit est l’échantillon de code complet qui démontre qu’une demande EWS authentifiée OAuth utilise les autorisations d’application.</span><span class="sxs-lookup"><span data-stu-id="793ea-169">The following is the complete code sample that demonstrates making an OAuth-authenticated EWS request using app-only authentication.</span></span>

> [!NOTE]
> <span data-ttu-id="793ea-170">Lorsque vous utilisez l’emprunt d’identité, vous devez toujours utiliser l’en-tête de demande X-AnchorMailbox, qui doit être défini sur le SMTP de la boîte aux lettres empruntée.</span><span class="sxs-lookup"><span data-stu-id="793ea-170">When using impersonation you must always use the X-AnchorMailbox request header, which should be set to the SMTP address of the impersonated mailbox.</span></span>

```cs
using Microsoft.Exchange.WebServices.Data;
using Microsoft.Identity.Client;
using System;
using System.Configuration;

namespace EwsOAuth
{
    class Program
    {
        static async System.Threading.Tasks.Task Main(string[] args)
        {
            // Using Microsoft.Identity.Client 4.22.0
            var cca = ConfidentialClientApplicationBuilder
                .Create(ConfigurationManager.AppSettings["appId"])
                .WithClientSecret(ConfigurationManager.AppSettings["clientSecret"])
                .WithTenantId(ConfigurationManager.AppSettings["tenantId"])
                .Build();

            var ewsScopes = new string[] { "https://outlook.office365.com/.default" };

            try
            {
                var authResult = await cca.AcquireTokenForClient(ewsScopes)
                    .ExecuteAsync();

                // Configure the ExchangeService with the access token
                var ewsClient = new ExchangeService();
                ewsClient.Url = new Uri("https://outlook.office365.com/EWS/Exchange.asmx");
                ewsClient.Credentials = new OAuthCredentials(authResult.AccessToken);
                ewsClient.ImpersonatedUserId =
                    new ImpersonatedUserId(ConnectingIdType.SmtpAddress, "meganb@contoso.onmicrosoft.com");

                //Include x-anchormailbox header
                ewsClient.HttpHeaders.Add("X-AnchorMailbox", "meganb@contoso.onmicrosoft.com");

                // Make an EWS call
                var folders = ewsClient.FindFolders(WellKnownFolderName.MsgFolderRoot, new FolderView(10));
                foreach(var folder in folders)
                {
                    Console.WriteLine($"Folder: {folder.DisplayName}");
                }
            }
            catch (MsalException ex)
            {
                Console.WriteLine($"Error acquiring access token: {ex}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex}");
            }

            if (System.Diagnostics.Debugger.IsAttached)
            {
                Console.WriteLine("Hit any key to exit...");
                Console.ReadKey();
            }
        }
    }
}
```

<span data-ttu-id="793ea-171">Le code échantillon dans les deux cas nécessite un **fichier App.config** avec les entrées suivantes :</span><span class="sxs-lookup"><span data-stu-id="793ea-171">The sample code in both cases requires an **App.config** file with the following entries:</span></span>

```xml
<?xml version="1.0" encoding="utf-8" ?>
<configuration>
  <startup>
    <supportedRuntime version="v4.0" sku=".NETFramework,Version=v4.7.2" />
  </startup>
  <appSettings>
    <!-- The application ID from your app registration -->
    <add key="appId" value="YOUR_APP_ID_HERE" />
    <!-- The tenant ID copied from your app registration -->
    <add key="tenantId" value="YOUR_TENANT_ID_HERE"/>
    <!-- The application's client secret from your app registration. Needed for application permission access -->
    <add key="clientSecret" value="YOUR_CLIENT_SECRET_HERE"/>
  </appSettings>
</configuration>
```

## <a name="see-also"></a><span data-ttu-id="793ea-172">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="793ea-172">See also</span></span>

- [<span data-ttu-id="793ea-173">Authentification et EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="793ea-173">Authentication and EWS in Exchange</span></span>](authentication-and-ews-in-exchange.md)
