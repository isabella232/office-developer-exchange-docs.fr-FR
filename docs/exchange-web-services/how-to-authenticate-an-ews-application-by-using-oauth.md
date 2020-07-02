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
# <a name="authenticate-an-ews-application-by-using-oauth"></a>Authentifier une application EWS à l’aide d’OAuth
<!-- markdownlint-enable MD025 -->

Découvrez comment utiliser l’authentification OAuth avec vos applications d’API managée EWS.

Vous pouvez utiliser le service d’authentification OAuth fourni par Azure Active Directory pour permettre à vos applications d’API managée EWS d’accéder à Exchange Online dans Office 365. Pour utiliser OAuth avec votre application, vous devez :

1. [Enregistrez votre application](#register-your-application) auprès d’Azure Active Directory.

2. [Ajoutez du code pour obtenir un jeton d’authentification](#add-code-to-get-an-authentication-token) afin d’obtenir un jeton d’authentification à partir d’un serveur de jetons.

3. [Ajoutez un jeton d’authentification aux requêtes EWS](#add-an-authentication-token-to-ews-requests) que vous envoyez.

> [!NOTE]
> L’authentification OAuth pour EWS est disponible uniquement dans Exchange dans le cadre d’Office 365. Les applications EWS qui utilisent OAuth doivent être inscrites auprès d’Azure Active Directory.

Pour utiliser le code de cet article, vous devez avoir accès à ce qui suit :

- Un compte Office 365 avec une boîte aux lettres Exchange Online. Si vous ne disposez pas d’un compte Office 365, vous pouvez vous [inscrire au programme pour les développeurs office 365](https://developer.microsoft.com/office/dev-program) pour obtenir un abonnement gratuit à Office 365.

- La [bibliothèque d’authentification Microsoft pour .net](/dotnet/api/microsoft.identity.client?view=azure-dotnet).

- L'[API managée EWS](https://github.com/officedev/ews-managed-api).


Il existe deux types d’autorisations OAuth qui peuvent être utilisées pour accéder aux API EWS dans Exchange Online. Avant de passer au didacticiel, vous devrez choisir le type d’autorisation spécifique à utiliser.

* Les **autorisations déléguées** sont utilisées par les applications qui ont un utilisateur connecté. Pour ces applications, l’utilisateur ou un administrateur accepte les autorisations demandées par l’application et l’application peut agir en tant qu’utilisateur connecté lors de la réalisation d’appels d’API. 
* Les **autorisations d’application** sont utilisées par les applications qui s’exécutent sans utilisateur connecté présent ; par exemple, les applications qui s’exécutent en tant que services ou démons d’arrière-plan et peuvent accéder à plusieurs boîtes aux lettres.

## <a name="register-your-application"></a>Inscrire votre application

Pour utiliser OAuth, une application doit avoir un ID d’application émis par Azure Active Directory. Dans ce didacticiel, il est supposé que l’application est une application console ; vous devez donc enregistrer votre application en tant que client public avec Azure Active Directory.

1. Ouvrez un navigateur, accédez au [Centre d’administration Azure Active Directory ](https://aad.portal.azure.com) et connectez-vous à l’aide d’un **compte personnel** (ou compte Microsoft) ou d’un **compte professionnel ou scolaire**.

1. Sélectionnez **Azure Active Directory** dans le volet de navigation gauche, puis sélectionnez **Inscriptions d’applications** sous **Gérer**.

1. Sélectionnez **Nouvelle inscription**. Sur la page **Inscrire une application**, définissez les valeurs comme suit.

    - Définissez **nom** sur un nom convivial pour votre application.
    - Définissez les **types de comptes pris en charge** sur le choix adapté à votre scénario.
    - Pour l' **URI de redirection**, définissez la liste déroulante sur **client Public (mobile & Desktop)** et définissez la valeur sur `urn:ietf:wg:oauth:2.0:oob` .

1. Choisissez **Inscrire**. Sur la page suivante, copiez la valeur de l' **ID d’application (client)** et enregistrez-la, vous en aurez besoin plus tard.

1. Sélectionnez **autorisations d’API** dans le volet de navigation de gauche sous **gérer**. 

1. Sélectionnez **Ajouter une autorisation**. Sur la page autorisations de l' **API de demande** , sélectionnez **Exchange** sous les **API héritées prises en charge**. 

1. Pour utiliser des autorisations déléguées, sélectionnez **autorisations déléguées** , puis **EWS. AccessAsUser. All** sous **EWS**. Cliquez sur **Ajouter des autorisations**. 

Pour utiliser les autorisations d’application, suivez ces étapes supplémentaires.

1. Sélectionnez **autorisations d’application** , puis **full_access_as_app**. Cliquez sur **Ajouter des autorisations**.

1. Sélectionnez **accorder le consentement de l’administrateur pour org** et acceptez la boîte de dialogue de consentement. 

1. Sélectionnez **certificats & secrets** dans le volet de navigation de gauche sous **gérer**. 

1. Sélectionnez **nouvelle clé secrète client**, entrez une brève description et sélectionnez **Ajouter**.

1. Copiez la **valeur** de la clé secrète client nouvellement ajoutée et enregistrez-la, vous en aurez besoin plus tard. 

## <a name="add-code-to-get-an-authentication-token"></a>Ajouter du code pour obtenir un jeton d’authentification

Les extraits de code suivants montrent comment utiliser la bibliothèque d’authentification Microsoft pour obtenir des jetons d’authentification pour les autorisations déléguées et les autorisations d’application. Ces extraits de code supposent que les informations requises pour effectuer la demande d’authentification sont stockées dans le fichier **App.config** de l’application. Ces exemples n’incluent pas la vérification des erreurs, reportez-vous aux [exemples de code](#code-samples) pour le code complet.

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

## <a name="add-an-authentication-token-to-ews-requests"></a>Ajouter un jeton d’authentification aux requêtes EWS

Une fois que vous avez reçu l’objet **AuthenticationResult** , vous pouvez utiliser la propriété **AccessToken** pour obtenir le jeton émis par le service de jetons.

```cs
// Configure the ExchangeService with the access token
var ewsClient = new ExchangeService();
ewsClient.Url = new Uri("https://outlook.office365.com/EWS/Exchange.asmx");
ewsClient.Credentials = new OAuthCredentials(authResult.AccessToken);
```

Pour utiliser des autorisations d’application, vous devez également emprunter explicitement l’identité d’une boîte aux lettres à laquelle vous souhaitez accéder. 

```cs
//Impersonate the mailbox you'd like to access.
ewsClient.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.SmtpAddress, "test@demotenant.onmicrosoft.com");
```

## <a name="code-samples"></a>Exemples de code

### <a name="delegated-permissions"></a>Autorisations déléguées

Voici l’exemple de code complet qui montre comment effectuer une demande EWS authentifiée OAuth à l’aide d’autorisations déléguées.

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

Voici l’exemple de code complet qui montre comment effectuer une demande EWS authentifiée OAuth à l’aide d’autorisations d’application.

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

Dans les deux cas, l’exemple de code requiert un fichier **App.config** avec les entrées suivantes :

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

## <a name="see-also"></a>Consultez aussi

- [Authentification et EWS dans Exchange](authentication-and-ews-in-exchange.md)
