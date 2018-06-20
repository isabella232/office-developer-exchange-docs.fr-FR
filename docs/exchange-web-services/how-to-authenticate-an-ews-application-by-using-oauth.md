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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19754803"
---
# <a name="authenticate-an-ews-application-by-using-oauth"></a><span data-ttu-id="d8a11-103">Authentifier une demande EWS à l’aide d’OAuth</span><span class="sxs-lookup"><span data-stu-id="d8a11-103">Authenticate an EWS application by using OAuth</span></span>

<span data-ttu-id="d8a11-104">Découvrez comment utiliser l’authentification OAuth avec vos applications d’API managées.</span><span class="sxs-lookup"><span data-stu-id="d8a11-104">Learn how to use OAuth authentication with your EWS Managed API applications.</span></span>
  
<span data-ttu-id="d8a11-105">Vous pouvez utiliser le service d’authentification OAuth fourni par Azure Active Directory pour intégrer vos applications d’API managées avec le même modèle d’authentification utilisé par l’API REST d’Office 365.</span><span class="sxs-lookup"><span data-stu-id="d8a11-105">You can use the OAuth authentication service provided by Azure Active Directory to integrate your EWS Managed API applications with the same authentication model used by the Office 365 REST APIs.</span></span> <span data-ttu-id="d8a11-106">Pour utiliser OAuth avec votre application, que vous devez :</span><span class="sxs-lookup"><span data-stu-id="d8a11-106">To use OAuth with your application you will need to:</span></span>
  
1. <span data-ttu-id="d8a11-107">[Inscrire votre application](#bk_register) avec Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d8a11-107">[Register your application](#bk_register) with Azure Active Directory.</span></span> 
    
2. <span data-ttu-id="d8a11-108">[Ajout de code pour obtenir un jeton d’authentification](#bk_getToken) obtenir le jeton d’authentification à partir d’un serveur de jetons.</span><span class="sxs-lookup"><span data-stu-id="d8a11-108">[Add code to get an authentication token](#bk_getToken) to get an authentication token from a token server.</span></span> 
    
3. <span data-ttu-id="d8a11-109">[Ajouter un jeton d’authentification pour les demandes EWS](#bk_useToken) que vous envoyez.</span><span class="sxs-lookup"><span data-stu-id="d8a11-109">[Add an authentication token to EWS requests](#bk_useToken) that you send.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="d8a11-110">Authentification OAuth pour EWS est disponible uniquement dans Exchange dans le cadre d’Office 365.</span><span class="sxs-lookup"><span data-stu-id="d8a11-110">OAuth authentication for EWS is only available in Exchange as part of Office 365.</span></span> <span data-ttu-id="d8a11-111">Applications EWS requièrent l’autorisation « Accès complet à boîte aux lettres sa ».</span><span class="sxs-lookup"><span data-stu-id="d8a11-111">EWS applications require the "Full access to user's mailbox" permission.</span></span> 
  
<span data-ttu-id="d8a11-112">Pour utiliser le code dans cet article, vous devez avoir accès à ce qui suit :</span><span class="sxs-lookup"><span data-stu-id="d8a11-112">To use the code in this article, you will need to have access to the following:</span></span>
  
- <span data-ttu-id="d8a11-113">Un [compte de développeur Office 365](http://office.microsoft.com/compare-office-365-for-business-plans-FX102918419.aspx.aspx).</span><span class="sxs-lookup"><span data-stu-id="d8a11-113">An [Office 365 developer account](http://office.microsoft.com/compare-office-365-for-business-plans-FX102918419.aspx.aspx).</span></span> <span data-ttu-id="d8a11-114">Vous pouvez utiliser un compte d’évaluation pour tester votre application</span><span class="sxs-lookup"><span data-stu-id="d8a11-114">You can use a trial account to test your application</span></span>
    
- <span data-ttu-id="d8a11-115">La [bibliothèque d’authentification Azure AD pour .NET](http://msdn.microsoft.com/en-us/library/office/jj573266.aspx.aspx).</span><span class="sxs-lookup"><span data-stu-id="d8a11-115">The [Azure AD Authentication Library for .NET](http://msdn.microsoft.com/en-us/library/office/jj573266.aspx.aspx).</span></span>
    
- <span data-ttu-id="d8a11-116">[L’API managée](https://github.com/officedev/ews-managed-api.aspx).</span><span class="sxs-lookup"><span data-stu-id="d8a11-116">[The EWS Managed API](https://github.com/officedev/ews-managed-api.aspx).</span></span>

<span data-ttu-id="d8a11-117"><a name="bk_register"> </a></span><span class="sxs-lookup"><span data-stu-id="d8a11-117"></span></span>

## <a name="register-your-application"></a><span data-ttu-id="d8a11-118">Inscrire votre application</span><span class="sxs-lookup"><span data-stu-id="d8a11-118">Register your application</span></span>

<span data-ttu-id="d8a11-119">Pour utiliser OAuth, une application doit avoir un identificateur de client et une application URI qui identifie l’application.</span><span class="sxs-lookup"><span data-stu-id="d8a11-119">To use OAuth, an application must have a client identifier and an application URI that identifies the application.</span></span> <span data-ttu-id="d8a11-120">Si vous n’avez pas encore inscrit votre application avec les Services Azure Active Directory, vous devez ajouter manuellement l’application en suivant les étapes indiquées sous [Enregistrer vous application](http://msdn.microsoft.com/en-us/office/office365/howto/test-and-deploy-apps.aspx).</span><span class="sxs-lookup"><span data-stu-id="d8a11-120">If you have not yet registered your application with Azure Active Directory Services, you'll need to manually add your application by following the steps under [Register you app](http://msdn.microsoft.com/en-us/office/office365/howto/test-and-deploy-apps.aspx).</span></span>

<span data-ttu-id="d8a11-121"><a name="bk_getToken"> </a></span><span class="sxs-lookup"><span data-stu-id="d8a11-121"></span></span>

## <a name="add-code-to-get-an-authentication-token"></a><span data-ttu-id="d8a11-122">Ajouter du code pour obtenir un jeton d’authentification</span><span class="sxs-lookup"><span data-stu-id="d8a11-122">Add code to get an authentication token</span></span>

<span data-ttu-id="d8a11-123">La bibliothèque de l’authentification Azure AD pour .NET simplifie l’obtention d’un jeton d’authentification d’Azure Active Directory afin que vous puissiez utiliser le jeton dans votre application.</span><span class="sxs-lookup"><span data-stu-id="d8a11-123">The Azure AD Authentication Library for .NET simplifies getting an authentication token from Azure Active Directory so that you can use the token in your application.</span></span> <span data-ttu-id="d8a11-124">Vous devez fournir les quatre éléments d’information pour obtenir le jeton :</span><span class="sxs-lookup"><span data-stu-id="d8a11-124">You need to provide four pieces of information to get the token:</span></span>
  
1. <span data-ttu-id="d8a11-125">L’URI du serveur de jeton.</span><span class="sxs-lookup"><span data-stu-id="d8a11-125">The URI of the token server.</span></span> <span data-ttu-id="d8a11-126">Le serveur de jetons est l' **autorité** qui authentifie l’utilisateur et retourne un jeton que votre application peut utiliser pour accéder aux EWS.</span><span class="sxs-lookup"><span data-stu-id="d8a11-126">The token server is the **authority** that authenticates the user and returns a token that your application can use to access EWS.</span></span> 
    
2. <span data-ttu-id="d8a11-127">L’ID client d’application créé lorsque vous avez enregistré votre application avec Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d8a11-127">The application client ID created when you registered your application with Azure Active Directory.</span></span>
    
3. <span data-ttu-id="d8a11-128">Client de l’application créé lors de l’inscription de votre application avec Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d8a11-128">The application client URI created when you registered your application with Azure Active Directory.</span></span>
    
4. <span data-ttu-id="d8a11-129">L’URI du serveur EWS et l’URI du point de terminaison EWS.</span><span class="sxs-lookup"><span data-stu-id="d8a11-129">The URI of the EWS server and the URI of the EWS endpoint.</span></span> <span data-ttu-id="d8a11-130">Pour Exchange dans le cadre d’Office 365, il s’agit de `https://<server name>/ews/exchange.asmx`.</span><span class="sxs-lookup"><span data-stu-id="d8a11-130">For Exchange as part of Office 365, this will be  `https://<server name>/ews/exchange.asmx`.</span></span>
    
<span data-ttu-id="d8a11-131">Le code suivant montre comment utiliser la bibliothèque de l’authentification Azure AD pour obtenir un jeton d’authentification.</span><span class="sxs-lookup"><span data-stu-id="d8a11-131">The following code shows how to use the Azure AD Authentication Library to get an authentication token.</span></span> <span data-ttu-id="d8a11-132">Il suppose que les informations nécessaires pour effectuer la demande d’authentification sont stockées dans le fichier App.config de l’application.</span><span class="sxs-lookup"><span data-stu-id="d8a11-132">It assumes that the information required to make the authentication request is stored in the application's App.config file.</span></span> <span data-ttu-id="d8a11-133">Cet exemple montre comment ne pas inclure la vérification des erreurs, consultez l' [exemple de Code](#bk_codeSample) pour le code complet.</span><span class="sxs-lookup"><span data-stu-id="d8a11-133">This example does not include error checking, see the [Code sample](#bk_codeSample) for the complete code.</span></span> 
  
```cs
string authority = ConfigurationManager.AppSettings["authority"];
string clientID = ConfigurationManager.AppSettings["clientID"];
Uri clientAppUri = new Uri(ConfigurationManager.AppSettings["clientAppUri"];
string serverName = ConfigurationManager.AppSettings["serverName"];
AuthenticationContext authenticationContext = new AuthenticationContext(authority, false);
AuthenticationResult authenticationResult = authenticationContext.AcquireToken(serverName, clientId, clientAppUri);

```

<span data-ttu-id="d8a11-134"><a name="bk_useToken"> </a></span><span class="sxs-lookup"><span data-stu-id="d8a11-134"></span></span>

## <a name="add-an-authentication-token-to-ews-requests"></a><span data-ttu-id="d8a11-135">Ajouter un jeton d’authentification pour les demandes EWS</span><span class="sxs-lookup"><span data-stu-id="d8a11-135">Add an authentication token to EWS requests</span></span>

<span data-ttu-id="d8a11-136">Une fois que vous avez reçu l’objet **AuthenticationResult** , vous pouvez utiliser la propriété **AccessToken** pour obtenir le jeton émis par le service d’émission de jeton.</span><span class="sxs-lookup"><span data-stu-id="d8a11-136">After you've received the **AuthenticationResult** object you can use the **AccessToken** property to get the token issued by the token service.</span></span> 
  
```cs
ExchangeService exchangeService = new ExchangeService(ExchangeVersion.Exchange2013);
exchangeService.Url = new Uri(ConfigurationManager.AppSettings["serverName"]+"ews/exchange.asmx");
exchangeService.TraceEnabled = true;
exchangeService.TraceFlags = TraceFlags.All;
exchangeService.Credentials = new OAuthCredentials(authenticationResult.AccessToken));
exchangeService.FindFolders(WellKnownFolderName.Root, new Folderview(10));
```

<span data-ttu-id="d8a11-137"><a name="bk_codeSample"> </a></span><span class="sxs-lookup"><span data-stu-id="d8a11-137"></span></span>

## <a name="code-sample"></a><span data-ttu-id="d8a11-138">Exemple de code</span><span class="sxs-lookup"><span data-stu-id="d8a11-138">Code sample</span></span>

<span data-ttu-id="d8a11-139">Voici l’exemple de code complet qui montre émet une demande EWS OAuth authentifié.</span><span class="sxs-lookup"><span data-stu-id="d8a11-139">The following is the complete code sample that demonstrates making an OAuth-authenticated EWS request.</span></span>
  
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

<span data-ttu-id="d8a11-140">L’exemple de code requiert un fichier App.config avec les entrées suivantes :</span><span class="sxs-lookup"><span data-stu-id="d8a11-140">The sample code requires an App.config file with the following entries:</span></span>
  
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

## <a name="see-also"></a><span data-ttu-id="d8a11-141">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d8a11-141">See also</span></span>

- [<span data-ttu-id="d8a11-142">L’authentification et les services EWS d’Exchange</span><span class="sxs-lookup"><span data-stu-id="d8a11-142">Authentication and EWS in Exchange</span></span>](authentication-and-ews-in-exchange.md)    
- [<span data-ttu-id="d8a11-143">Tester et déployer des applications Office 365</span><span class="sxs-lookup"><span data-stu-id="d8a11-143">Test and deploy Office 365 apps</span></span>](http://msdn.microsoft.com/en-us/office/office365/howto/test-and-deploy-apps.aspx)
    
