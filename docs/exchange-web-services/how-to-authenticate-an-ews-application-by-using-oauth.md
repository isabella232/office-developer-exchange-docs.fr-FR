---
title: Authentifier une demande EWS à l’aide d’OAuth
manager: sethgros
ms.date: 1/15/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 1d8d57f9-4df5-4f21-9bbb-a89e0e259052
description: Découvrez comment utiliser l’authentification OAuth avec vos applications d’API managées.
ms.openlocfilehash: 66bbc0525ecf78407e853da0c8dcdec92791ca56
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754803"
---
# <a name="authenticate-an-ews-application-by-using-oauth"></a>Authentifier une demande EWS à l’aide d’OAuth

Découvrez comment utiliser l’authentification OAuth avec vos applications d’API managées.
  
Vous pouvez utiliser le service d’authentification OAuth fourni par Azure Active Directory pour intégrer vos applications d’API managées avec le même modèle d’authentification utilisé par l’API REST d’Office 365. Pour utiliser OAuth avec votre application, que vous devez :
  
1. [Inscrire votre application](#bk_register) avec Azure Active Directory. 
    
2. [Ajout de code pour obtenir un jeton d’authentification](#bk_getToken) obtenir le jeton d’authentification à partir d’un serveur de jetons. 
    
3. [Ajouter un jeton d’authentification pour les demandes EWS](#bk_useToken) que vous envoyez. 
    
> [!NOTE]
> Authentification OAuth pour EWS est disponible uniquement dans Exchange dans le cadre d’Office 365. Applications EWS requièrent l’autorisation « Accès complet à boîte aux lettres sa ». 
  
Pour utiliser le code dans cet article, vous devez avoir accès à ce qui suit :
  
- Un [compte de développeur Office 365](http://office.microsoft.com/compare-office-365-for-business-plans-FX102918419.aspx.aspx). Vous pouvez utiliser un compte d’évaluation pour tester votre application
    
- La [bibliothèque d’authentification Azure AD pour .NET](http://msdn.microsoft.com/en-us/library/office/jj573266.aspx.aspx).
    
- [L’API managée](https://github.com/officedev/ews-managed-api.aspx).

<a name="bk_register"> </a>

## <a name="register-your-application"></a>Inscrire votre application

Pour utiliser OAuth, une application doit avoir un identificateur de client et une application URI qui identifie l’application. Si vous n’avez pas encore inscrit votre application avec les Services Azure Active Directory, vous devez ajouter manuellement l’application en suivant les étapes indiquées sous [Enregistrer vous application](http://msdn.microsoft.com/en-us/office/office365/howto/test-and-deploy-apps.aspx).

<a name="bk_getToken"> </a>

## <a name="add-code-to-get-an-authentication-token"></a>Ajouter du code pour obtenir un jeton d’authentification

La bibliothèque de l’authentification Azure AD pour .NET simplifie l’obtention d’un jeton d’authentification d’Azure Active Directory afin que vous puissiez utiliser le jeton dans votre application. Vous devez fournir les quatre éléments d’information pour obtenir le jeton :
  
1. L’URI du serveur de jeton. Le serveur de jetons est l' **autorité** qui authentifie l’utilisateur et retourne un jeton que votre application peut utiliser pour accéder aux EWS. 
    
2. L’ID client d’application créé lorsque vous avez enregistré votre application avec Azure Active Directory.
    
3. Client de l’application créé lors de l’inscription de votre application avec Azure Active Directory.
    
4. L’URI du serveur EWS et l’URI du point de terminaison EWS. Pour Exchange dans le cadre d’Office 365, il s’agit de `https://<server name>/ews/exchange.asmx`.
    
Le code suivant montre comment utiliser la bibliothèque de l’authentification Azure AD pour obtenir un jeton d’authentification. Il suppose que les informations nécessaires pour effectuer la demande d’authentification sont stockées dans le fichier App.config de l’application. Cet exemple montre comment ne pas inclure la vérification des erreurs, consultez l' [exemple de Code](#bk_codeSample) pour le code complet. 
  
```cs
string authority = ConfigurationManager.AppSettings["authority"];
string clientID = ConfigurationManager.AppSettings["clientID"];
Uri clientAppUri = new Uri(ConfigurationManager.AppSettings["clientAppUri"];
string serverName = ConfigurationManager.AppSettings["serverName"];
AuthenticationContext authenticationContext = new AuthenticationContext(authority, false);
AuthenticationResult authenticationResult = authenticationContext.AcquireToken(serverName, clientId, clientAppUri);

```

<a name="bk_useToken"> </a>

## <a name="add-an-authentication-token-to-ews-requests"></a>Ajouter un jeton d’authentification pour les demandes EWS

Une fois que vous avez reçu l’objet **AuthenticationResult** , vous pouvez utiliser la propriété **AccessToken** pour obtenir le jeton émis par le service d’émission de jeton. 
  
```cs
ExchangeService exchangeService = new ExchangeService(ExchangeVersion.Exchange2013);
exchangeService.Url = new Uri(ConfigurationManager.AppSettings["serverName"]+"ews/exchange.asmx");
exchangeService.TraceEnabled = true;
exchangeService.TraceFlags = TraceFlags.All;
exchangeService.Credentials = new OAuthCredentials(authenticationResult.AccessToken));
exchangeService.FindFolders(WellKnownFolderName.Root, new Folderview(10));
```

<a name="bk_codeSample"> </a>

## <a name="code-sample"></a>Exemple de code

Voici l’exemple de code complet qui montre émet une demande EWS OAuth authentifié.
  
```cs
using System;
using System.Collections.Generic;
using System.Configuration;
using System.Globalization;
using System.Linq;
using System.Text;
using System.Threading;
using System.Threading.Tasks;
using System.Web.Script.Serialization;
using Microsoft.Exchange.WebServices.Autodiscover;
using Microsoft.Exchange.WebServices.Data;
using Microsoft.IdentityModel.Clients.ActiveDirectory;
namespace TestV1App
{
    class Program
    {
        static void Main(string[] args)
        {
            var t = new Thread(Run);
            t.SetApartmentState(ApartmentState.STA);
            t.Start();
            t.Join();
        }
        static void Run()
        {
           string authority = ConfigurationManager.AppSettings["authority"];
           string clientID = ConfigurationManager.AppSettings["clientID"];
           Uri clientAppUri = new Uri(ConfigurationManager.AppSettings["clientAppUri"];
           string serverName = ConfigurationManager.AppSettings["serverName"];
            AuthenticationResult authenticationResult = null;
            AuthenticationContext authenticationContext = new AuthenticationContext(authority, false);
            
            string errorMessage = null;
            try
            {
                Console.WriteLine("Trying to acquire token");
                authenticationResult = authenticationContext.AcquireToken(serverName, clientId, clientAppUri);
            }
                catch (AdalException ex)
            {
                errorMessage = ex.Message;
                if (ex.InnerException != null)
                {
                    errorMessage += "\nInnerException : " + ex.InnerException.Message;
                }
            }
            catch (ArgumentException ex)
            {
                errorMessage = ex.Message;
            }
            if (!string.IsNullOrEmpty(errorMessage))
            {
                Console.WriteLine("Failed: {0}" + errorMessage);
                return;
            }
            Console.WriteLine("\nMaking the protocol call\n");
            ExchangeService exchangeService = new ExchangeService(ExchangeVersion.Exchange2013);
            exchangeService.Url = new Uri(resource + "ews/exchange.asmx");
            exchangeService.TraceEnabled = true;
            exchangeService.TraceFlags = TraceFlags.All;
            exchangeService.Credentials = new OAuthCredentials(authenticationResult.AccessToken);
            exchangeService.FindFolders(WellKnownFolderName.Root, new FolderView(10));
        }
    }
}

```

L’exemple de code requiert un fichier App.config avec les entrées suivantes :
  
```xml
<?xml version="1.0" encoding="utf-8" ?>
<configuration>
  <startup>
    <supportedRuntime version="v4.0" sku=".NETFramework,Version=v4.5" />
  </startup>
  <appSettings>
    <add key="authority" value="http://login.windows.net/<devAccountName>.onmicrosoft.com" />
    <add key="clientId" value="<ID generated by Azure Active Directory"/>
    <add key="clientAppUri" value="<URI registered with Azure Active Directory"/>
    <add key="serverName" value="outlook.office365.com" />
  </appSettings>
</configuration>
```

## <a name="see-also"></a>Voir aussi

- [L’authentification et les services EWS d’Exchange](authentication-and-ews-in-exchange.md)    
- [Tester et déployer des applications Office 365](http://msdn.microsoft.com/en-us/office/office365/howto/test-and-deploy-apps.aspx)
    

