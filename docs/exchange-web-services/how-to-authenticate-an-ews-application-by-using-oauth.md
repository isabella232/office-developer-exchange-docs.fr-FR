---
title: Authentifier une application EWS à l’aide d’OAuth
manager: sethgros
ms.date: 11/25/2020
ms.audience: Developer
ms.assetid: 1d8d57f9-4df5-4f21-9bbb-a89e0e259052
description: Apprendre à utiliser l’authentification OAuth avec vos applications EWS Managed API.
localization_priority: Priority
ms.openlocfilehash: a7b1d2a099cf5f3c95f8453605363de12ff33c54
ms.sourcegitcommit: 843a2e030a94b12aec70c553ca4e06e39ac02d82
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/09/2020
ms.locfileid: "49603826"
---
<!-- markdownlint-disable MD025 -->
# <a name="authenticate-an-ews-application-by-using-oauth"></a>Authentifier une application EWS à l’aide d’OAuth
<!-- markdownlint-enable MD025 -->

Apprendre à utiliser l’authentification OAuth avec vos applications EWS Managed API.

Vous pouvez utiliser le service d’authentification OAuth fourni par Azure Active Directory pour permettre à vos applications EWS Managed API d’accéder à Exchange Online dans Office 365. Pour utiliser OAuth avec votre application, vous devrez :

1. [Inscrire votre application](#register-your-application) dans Azure Active Directory.
1. [Ajouter un code pour obtenir un jeton d’authentification](#add-code-to-get-an-authentication-token) afin d’obtenir un jeton d’authentification à partir d’un serveur de jetons.
1. [Ajouter un jeton d’authentification aux demandes EWS](#add-an-authentication-token-to-ews-requests) que vous envoyez.

> [!NOTE]
> L’authentification OAuth pour EWS est disponible uniquement dans Exchange dans le cadre d’Office 365. Les applications EWS qui utilisent OAuth doivent être inscrites auprès d’Azure Active Directory.

Pour utiliser le code dans cet article, vous devrez avoir accès aux éléments suivants :

- Un compte Office 365 avec une boîte aux lettres Exchange Online. Si vous n’avez pas de compte Office 365, vous pouvez [vous inscrire au programme pour les développeurs Office 365](https://developer.microsoft.com/microsoft-365/dev-program) pour obtenir un abonnement gratuit à Office 365.
- La [bibliothèque d’authentification Microsoft pour .NET](/dotnet/api/microsoft.identity.client).
- L’ [API gérée EWS](https://github.com/officedev/ews-managed-api).

Deux types d’autorisations OAuth peuvent être utilisés pour accéder aux API EWS dans Exchange Online. Avant de commencer le tutoriel, vous devrez choisir le type de permission spécifique à utiliser.

- Des **autorisations déléguées** sont utilisées par les applications qui ont un utilisateur connecté. Pour ces applications, l’utilisateur ou un administrateur consent aux autorisations demandées par l’application, et l’application peut agir en tant qu’utilisateur connecté lors des appels API.
- Des **autorisations d’application** sont utilisées par les applications qui s’exécutent sans utilisateur connecté ; par exemple, les applications qui s’exécutent en tant que démons ou services d’arrière-plan et qui peuvent accéder à plusieurs boîtes aux lettres.

## <a name="register-your-application"></a>Inscription de votre application

Pour utiliser OAuth, une application doit avoir une ID d’application émise par Azure Active Directory. Dans ce tutoriel, l’application est supposée être une application console, alors vous devez enregistrer votre application en tant que client public à l’aide d’Azure Active Directory. Vous pouvez inscrire une application dans le centre d’administration Azure Active Directory ou à l’aide de Microsoft Graph.

1. Ouvrez un navigateur, accédez au [Centre d’administration Azure Active Directory](https://aad.portal.azure.com) et connectez-vous à l’aide d’un **compte personnel** (ou compte Microsoft) ou d’un **compte professionnel ou scolaire**.

1. Sélectionnez **Azure Active Directory** dans le volet de navigation gauche, puis sélectionnez **Inscriptions d’applications** sous **Gérer**.

1. Sélectionnez **Nouvelle inscription**. Sur la page **Inscrire une application**, définissez les valeurs comme suit.

    - Définissez **Nom** pour un nom convivial de votre application.
    - Définissez **types de comptes pris en charge** pour le choix adapté à votre scénario.
    - Pour **Rediriger URI**, remplacez la liste déroulante par **client public (mobile & bureau)** et définissez la valeur sur `urn:ietf:wg:oauth:2.0:oob`.

1. Choisissez **Inscrire**. Sur la page Application console Graph, copiez les valeurs de **l’ID de l’application (client)** et de **l’ID du répertoire (client)**  ; vous en aurez besoin plus loin dans cet exercice.

### <a name="configure-for-delegated-authentication"></a>Configurer pour l’authentification déléguée

Si votre application utilise l’authentification déléguée, aucune configuration ultérieure n’est requise. La [Platforme d’identites Microsoft pour développeurs](/azure/active-directory/develop/v2-overview) permet aux applications de demander des autorisations de façon dynamique, de sorte que vous n’avez pas à configurer préalablement les autorisations sur l’inscription de l’application. Toutefois, dans certains scénarios (par exemples, [au nom du flux](/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow)), la configuration préalable des autorisations est requise. Suivez les étapes ci-dessous pour préconfigurer les autorisations EWS.

1. Sélectionnez **Autorisations de l’API** dans le volet de navigation gauche sous **Gérer**.

1. Recherchez la propriété `requiredResourceAccess` dans le manifeste, puis ajoutez les éléments suivants à l’intérieur des crochets (`[]`) :

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

1. Sélectionnez **Enregistrer**.

1. Sélectionnez **Autorisations de l’API** dans le volet de navigation gauche sous **Gérer**. Vérifiez que l’autorisation **EWS.AccessAsUser.All** est répertoriée.

### <a name="configure-for-app-only-authentication"></a>Configurer pour l’authentification de l’application uniquement

Pour utiliser les autorisations des applications, suivez ces étapes supplémentaires.

1. Sélectionnez **Autorisations de l’API** dans le volet de navigation gauche sous **Gérer**.

1. Recherchez la propriété `requiredResourceAccess` dans le manifeste, puis ajoutez les éléments suivants à l’intérieur des crochets (`[]`) :

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

1. Sélectionnez **Enregistrer**.

1. Sélectionnez **Autorisations de l’API** dans le volet de navigation gauche sous **Gérer**. Vérifiez que l’autorisation **full_access_as_app** est répertoriée.

1. Sélectionnez **Accorder l’autorisation d’administrateur pour l'entreprise** puis acceptez la boîte de dialogue de consentement.

1. Sélectionnez **Certificats et clés secrètes** dans le volet de navigation gauche sous **Gérer**.

1. Sélectionnez **Secret nouveau client**, entrez une courte description, puis sélectionnez **Ajouter**.

1. Copiez la **Valeur** du nouveau secret client ajouté et enregistrez-le. vous en aurez besoin plus tard.

## <a name="add-code-to-get-an-authentication-token"></a>Ajouter un code pour obtenir un jeton d’authentification

Les extraits de code suivants montrent comment utiliser la bibliothèque d’authentification Microsoft pour obtenir des jetons d’authentification pour les autorisations déléguées et les autorisations d’application. Ces extraits de code partent du principe que les informations requises pour effectuer la demande d’authentification sont stockées dans le fichier **App. config** de l’application. Ces exemples ne comprennent pas la vérification des erreurs, voir les [exemples de code](#code-samples) pour le code complet.

### <a name="get-a-token-with-delegated-auth"></a>Obtenir un jeton avec l’authentification déléguée

```cs
// Using Microsoft.Identity.Client 4.22.0

// Configure the MSAL client to get tokens
var pcaOptions = new PublicClientApplicationOptions
{
    ClientId = ConfigurationManager.AppSettings["appId"],
    TenantId = ConfigurationManager.AppSettings["tenantId"]
};

var pca = PublicClientApplicationBuilder
    .CreateWithApplicationOptions(pcaOptions).Build();

// The permission scope required for EWS access
var ewsScopes = new string[] { "https://outlook.office365.com/EWS.AccessAsUser.All" };

// Make the interactive token request
var authResult = await pca.AcquireTokenInteractive(ewsScopes).ExecuteAsync();
```

### <a name="get-a-token-with-app-only-auth"></a>Obtenir un jeton avec l’authentification de l’application uniquement

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
var authResult = await cca.AcquireTokenForClient(ewsScopes).ExecuteAsync();
```

## <a name="add-an-authentication-token-to-ews-requests"></a>Ajouter un jeton d’authentification aux demandes EWS

Une fois que vous avez reçu l’objet **RésultatAuthentification** vous pouvez utiliser la propriété du **Jetond’Accès** pour obtenir le jeton émis par le service d’émission de jeton.

```cs
// Configure the ExchangeService with the access token
var ewsClient = new ExchangeService();
ewsClient.Url = new Uri("https://outlook.office365.com/EWS/Exchange.asmx");
ewsClient.Credentials = new OAuthCredentials(authResult.AccessToken);
```

Pour utiliser les autorisations d’application, vous devez également emprunter explicitement une boîte aux lettres à laquelle vous voulez accéder.

```cs
//Impersonate the mailbox you'd like to access.
ewsClient.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.SmtpAddress, "test@demotenant.onmicrosoft.com");
```

## <a name="code-samples"></a>Exemples de code

### <a name="delegated-authentication"></a>Authentification déléguée

Ce qui suit est l’échantillon de code complet qui démontre qu’une demande EWS authentifiée OAuth utilise les autorisations d’application.

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

            // Configure the MSAL client to get tokens
            var pcaOptions = new PublicClientApplicationOptions
            {
                ClientId = ConfigurationManager.AppSettings["appId"],
                TenantId = ConfigurationManager.AppSettings["tenantId"]
            };

            var pca = PublicClientApplicationBuilder
                .CreateWithApplicationOptions(pcaOptions).Build();

            // The permission scope required for EWS access
            var ewsScopes = new string[] { "https://outlook.office365.com/EWS.AccessAsUser.All" };

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

### <a name="app-only-authentication"></a>Authentification de l'application uniquement

Ce qui suit est l’échantillon de code complet qui démontre qu’une demande EWS authentifiée OAuth utilise les autorisations d’application.

> [!NOTE]
> Lorsque vous utilisez l’emprunt d’identité, vous devez toujours utiliser l’en-tête de demande X-AnchorMailbox, qui doit être défini sur le SMTP de la boîte aux lettres empruntée.

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

Le code échantillon dans les deux cas nécessite un **fichier App.config** avec les entrées suivantes :

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

## <a name="see-also"></a>Voir aussi

- [Authentification et EWS dans Exchange](authentication-and-ews-in-exchange.md)
