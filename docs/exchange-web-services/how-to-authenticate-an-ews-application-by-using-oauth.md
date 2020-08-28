---
title: Authentifier une application EWS à l’aide d’OAuth
manager: sethgros
ms.date: 05/17/2019
ms.audience: Developer
ms.assetid: 1d8d57f9-4df5-4f21-9bbb-a89e0e259052
description: Apprendre à utiliser l’authentification OAuth avec vos applications EWS Managed API.
localization_priority: Priority
ms.openlocfilehash: 795cbcc3dd1c895850086ebf0e23da905c1c99b7
ms.sourcegitcommit: 636c05a929279812c6ef87d75b01c166a4a05584
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/26/2020
ms.locfileid: "47254964"
---
<!-- markdownlint-disable MD025 -->
# <a name="authenticate-an-ews-application-by-using-oauth"></a>Authentifier une application EWS à l’aide d’OAuth
<!-- markdownlint-enable MD025 -->

Apprendre à utiliser l’authentification OAuth avec vos applications EWS Managed API.

Vous pouvez utiliser le service d’authentification OAuth fourni par Azure Active Directory pour permettre à vos applications EWS Managed API d’accéder à Exchange Online dans Office 365. Pour utiliser OAuth avec votre application, vous devrez :

1. [Inscrire votre application](#register-your-application) dans Azure Active Directory.

2. [Ajouter un code pour obtenir un jeton d’authentification](#add-code-to-get-an-authentication-token) afin d’obtenir un jeton d’authentification à partir d’un serveur de jetons.

3. [Ajouter un jeton d’authentification aux demandes EWS](#add-an-authentication-token-to-ews-requests) que vous envoyez.

> [!NOTE]
> L’authentification OAuth pour EWS est disponible uniquement dans Exchange dans le cadre d’Office 365. Les applications EWS qui utilisent OAuth doivent être inscrites auprès d’Azure Active Directory.

Pour utiliser le code dans cet article, vous devrez avoir accès aux éléments suivants :

- Un compte Office 365 avec une boîte aux lettres Exchange Online. Si vous n’avez pas de compte Office 365, vous pouvez [vous inscrire au programme pour les développeurs Office 365](https://developer.microsoft.com/office/dev-program) pour obtenir un abonnement gratuit à Office 365.

- La [bibliothèque d’authentification Microsoft pour .NET](/dotnet/api/microsoft.identity.client?view=azure-dotnet).

- L’ [API gérée EWS](https://github.com/officedev/ews-managed-api).


Deux types d’autorisations OAuth peuvent être utilisés pour accéder aux API EWS dans Exchange Online. Avant de commencer le tutoriel, vous devrez choisir le type de permission spécifique à utiliser.

* Des **autorisations déléguées** sont utilisées par les applications qui ont un utilisateur connecté. Pour ces applications, l’utilisateur ou un administrateur consent aux autorisations demandées par l’application, et l’application peut agir en tant qu’utilisateur connecté lors des appels API. 
* Des **autorisations d’application** sont utilisées par les applications qui s’exécutent sans utilisateur connecté ; par exemple, les applications qui s’exécutent en tant que démons ou services d’arrière-plan et qui peuvent accéder à plusieurs boîtes aux lettres.

## <a name="register-your-application"></a>Inscription de votre application

Pour utiliser OAuth, une application doit avoir une ID d’application émise par Azure Active Directory. Dans ce tutoriel, l’application est supposée être une application console, alors vous devez enregistrer votre application en tant que client public à l’aide d’Azure Active Directory.

1. Ouvrez un navigateur, accédez au [Centre d’administration Azure Active Directory ](https://aad.portal.azure.com) et connectez-vous à l’aide d’un **compte personnel** (ou compte Microsoft) ou d’un **compte professionnel ou scolaire**.

1. Sélectionnez **Azure Active Directory** dans le volet de navigation gauche, puis sélectionnez **Inscriptions d’applications** sous **Gérer**.

1. Sélectionnez **Nouvelle inscription**. Sur la page **Inscrire une application**, définissez les valeurs comme suit.

    - Définissez **Nom**pour un nom convivial de votre application.
    - Définissez **types de comptes pris en charge** pour le choix adapté à votre scénario.
    - Pour **Rediriger URI**, remplacez la liste déroulante par **client public (mobile & bureau)** et définissez la valeur sur `urn:ietf:wg:oauth:2.0:oob`.

1. Choisissez **Inscrire**. Sur la page suivante, copiez la valeur de l’**ID (client) de l’application** et enregistrez-la, vous en aurez besoin ultérieurement.

1. Sélectionnez **Autorisations de l’API** dans le volet de navigation gauche sous **Gérer**. 

1. Sélectionnez **Ajouter une autorisation**. Sur la page **Demander des autorisations** API, sélectionnez **Échanger** sous **API héritées prises en charge**. 

1. Pour utiliser les autorisations déléguées, sélectionnez **autorisations déléguées** puis sélectionnez **EWS.AccessAsUser.All** sous **EWS**. Cliquez sur **Ajouter des autorisations**. 

Pour utiliser les autorisations des applications, suivez ces étapes supplémentaires.

1. Sélectionnez **autorisations d’application** puis sélectionnez **full_access_as_app**. Cliquez sur **Ajouter des autorisations**.

1. Sélectionnez **Accorder l’autorisation d’administrateur pour l'entreprise** puis acceptez la boîte de dialogue de consentement. 

1. Sélectionnez **Certificats et clés secrètes** dans le volet de navigation gauche sous **Gérer**. 

1. Sélectionnez **Secret nouveau client**, entrez une courte description, puis sélectionnez **Ajouter**.

1. Copiez la **Valeur** du nouveau secret client ajouté et enregistrez-le. vous en aurez besoin plus tard. 

## <a name="add-code-to-get-an-authentication-token"></a>Ajouter un code pour obtenir un jeton d’authentification

Les extraits de code suivants montrent comment utiliser la bibliothèque d’authentification Microsoft pour obtenir des jetons d’authentification pour les autorisations déléguées et les autorisations d’application. Ces extraits de code partent du principe que les informations requises pour effectuer la demande d’authentification sont stockées dans le fichier **App. config** de l’application. Ces exemples ne comprennent pas la vérification des erreurs, voir les [exemples de code](#code-samples) pour le code complet.

### <a name="delegated-permissions"></a>Autorisations déléguées

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

### <a name="application-permissions"></a>Autorisations de l’application

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

## <a name="add-an-authentication-token-to-ews-requests"></a>Ajouter un jeton d’authentification aux demandes EWS

Une fois que vous avez reçu l’objet **RésultatAuthentification** vous pouvez utiliser la propriété du**Jetond’Accès** pour obtenir le jeton émis par le service d’émission de jeton.

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

### <a name="delegated-permissions"></a>Autorisations déléguées

Ce qui suit est l’échantillon de code complet qui démontre qu’une demande EWS authentifiée OAuth utilise les autorisations déléguées.

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

### <a name="application-permissions"></a>Autorisations de l’application

Ce qui suit est l’échantillon de code complet qui démontre qu’une demande EWS authentifiée OAuth utilise les autorisations d’application.

> [!NOTE]
> Lorsque vous utilisez l’emprunt d’identité, vous devez toujours utiliser l’en-tête de demande X-AnchorMailbox, qui doit être défini sur le SMTP de la boîte aux lettres empruntée.

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

                //Include x-anchormailbox header
                ewsClient.HttpHeaders.Add("X-AnchorMailbox", "test@demotenant.onmicrosoft.com");

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
    <!-- If you registered your app to support only users in your organization, change the value
           of this key to your tenant ID -->
    <add key="tenantId" value="common"/>
    <!-- The application's client secret from your app registration. Needed for application permission access -->
    <add key="clientSecret" value="YOUR_CLIENT_SECRET_HERE"/>
  </appSettings>
</configuration>
```

## <a name="see-also"></a>Voir aussi

- [Authentification et EWS dans Exchange](authentication-and-ews-in-exchange.md)
