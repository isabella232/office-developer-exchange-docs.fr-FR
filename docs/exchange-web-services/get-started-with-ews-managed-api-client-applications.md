---
title: Prise en main des applications clientes d'API managée EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: c2267733-6f4f-49e5-9614-1e4a24c3af1a
description: Développer une application cliente de messagerie Hello World simple pour Exchange à l'aide de l'API managée EWS.
ms.openlocfilehash: dafc8cbbf172ad725ab83c93553464ba96ef33b8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754794"
---
# <a name="get-started-with-ews-managed-api-client-applications"></a><span data-ttu-id="5be8a-103">Prise en main des applications clientes d'API managée EWS</span><span class="sxs-lookup"><span data-stu-id="5be8a-103">Get started with EWS Managed API client applications</span></span>

<span data-ttu-id="5be8a-104">Ce document peut contenir des informations liées aux fonctionnalités ou produits préliminaires qui sont sujettes à modifications avant la sortie de la version définitive. Ce document est fourni "tel quel" à titre indicatif et Microsoft exclut toute garantie, expresse ou implicite, en ce qui concerne ce document. Développer une application cliente de messagerie Hello World simple pour Exchange à l'aide de l'API managée EWS.</span><span class="sxs-lookup"><span data-stu-id="5be8a-104">Develop a simple Hello World email client application for Exchange by using the EWS Managed API.</span></span> 
  
<span data-ttu-id="5be8a-p101">L'[API managée EWS](http://aka.ms/ews-managed-api-readme) fournit un modèle objet intuitif et facile à utiliser pour envoyer et recevoir des messages du service web à partir d'applications clientes, d'applications de portail et d'applications de service. Vous pouvez accéder à presque toutes les informations stockées dans une boîte aux lettres de serveur Exchange Online, Exchange Online dans le cadre d'Office 365 ou Exchange à l'aide de l'API managée EWS. Vous pouvez utiliser les informations de cet article pour développer votre première application cliente d'API managée EWS.</span><span class="sxs-lookup"><span data-stu-id="5be8a-p101">The [EWS Managed API](http://aka.ms/ews-managed-api-readme) provides an intuitive, easy-to-use object model for sending and receiving web service messages from client applications, portal applications, and service applications. You can access almost all the information stored in an Exchange Online, Exchange Online as part of Office 365, or an Exchange server mailbox by using the EWS Managed API. You can use the information in this article to help you develop your first EWS Managed API client application.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="5be8a-p102"> L'API managée EWS est maintenant disponible en tant que projet open source sur [GitHub](https://github.com/officedev/ews-managed-api). Vous pouvez utiliser la bibliothèque open source afin de : >  participer aux résolutions de bogues et aux améliorations apportées à l'API ; >  obtenir des correctifs et des améliorations avant qu'ils soient disponibles dans une version officielle ; >  accéder à l'implémentation la plus complète et la plus à jour de l'API, afin de l'utiliser comme référence ou pour créer des bibliothèques sur de nouvelles plateformes. >  Vos [contributions](https://github.com/OfficeDev/ews-managed-api/blob/master/CONTRIBUTING.md) via GitHub sont les bienvenues.</span><span class="sxs-lookup"><span data-stu-id="5be8a-p102">The EWS Managed API is now available as an open source project on [GitHub](https://github.com/officedev/ews-managed-api). You can use the open source library to: >  Contribute bug fixes and enhancements to the API. >  Get fixes and enhancements before they are available in an official release. >  Access the most comprehensive and up-to-date implementation of the API, to use as a reference or to create new libraries on new platforms. >  We welcome your [contributions](https://github.com/OfficeDev/ews-managed-api/blob/master/CONTRIBUTING.md) via GitHub.</span></span> 
  
## <a name="youll-need-an-exchange-server"></a><span data-ttu-id="5be8a-113">Besoin d'un serveur Exchange</span><span class="sxs-lookup"><span data-stu-id="5be8a-113">You'll need an Exchange server</span></span>
<span data-ttu-id="5be8a-114"><a name="NeedExchange"> </a></span><span class="sxs-lookup"><span data-stu-id="5be8a-114"></span></span>

<span data-ttu-id="5be8a-p103">Si vous avez déjà un compte de boîte aux lettres Exchange, vous pouvez ignorer cette section. Dans le cas contraire, vous pouvez configurer une boîte aux lettres Exchange pour votre première application cliente EWS par le biais des méthodes suivantes :</span><span class="sxs-lookup"><span data-stu-id="5be8a-p103">If you already have an Exchange mailbox account, you can skip this section. Otherwise, you have the following options for setting up an Exchange mailbox for your first EWS client application:</span></span>
  
- <span data-ttu-id="5be8a-p104">En obtenant un [site de développement Office 365](http://msdn.microsoft.com/fr-fr/library/office/fp179924.aspx) (recommandé). Il s'agit de la manière la plus rapide de configurer une boîte aux lettres Exchange.</span><span class="sxs-lookup"><span data-stu-id="5be8a-p104">Get an [Office 365 Developer Site](http://msdn.microsoft.com/fr-fr/library/office/fp179924.aspx) (recommended). This is the quickest way for you to set up an Exchange mailbox.</span></span> 
    
- <span data-ttu-id="5be8a-119">En téléchargeant [Exchange Server](http://office.microsoft.com/en-us/exchange/microsoft-exchange-try-or-buy-exchange-we-can-help-you-decide-FX103746846.aspx?WT%2Eintid1=ODC%5FENUS%5FFX103472230%5FXT103965589).</span><span class="sxs-lookup"><span data-stu-id="5be8a-119">Download [Exchange Server](http://office.microsoft.com/en-us/exchange/microsoft-exchange-try-or-buy-exchange-we-can-help-you-decide-FX103746846.aspx?WT%2Eintid1=ODC%5FENUS%5FFX103472230%5FXT103965589).</span></span>
    
<span data-ttu-id="5be8a-p105">Après avoir vérifié que vous pouvez envoyer et recevoir des messages électroniques à partir d'Exchange, vous êtes prêt à configurer votre environnement de développement. Vous pouvez utiliser le client web Exchange [Outlook Web App](http://technet.microsoft.com/fr-fr/library/jj657718%28v=exchg.150%29.aspx) pour vérifier que vous pouvez envoyer des messages électroniques.</span><span class="sxs-lookup"><span data-stu-id="5be8a-p105">After you have verified that you can send and receive email from Exchange, you are ready to set up your development environment. You can use the Exchange web client [Outlook Web App](http://technet.microsoft.com/fr-fr/library/jj657718%28v=exchg.150%29.aspx) to verify that you can send email.</span></span> 
  
## <a name="set-up-your-development-environment"></a><span data-ttu-id="5be8a-122">Configuration de votre environnement de développement</span><span class="sxs-lookup"><span data-stu-id="5be8a-122">Set up your development environment</span></span>
<span data-ttu-id="5be8a-123"><a name="Setup"> </a></span><span class="sxs-lookup"><span data-stu-id="5be8a-123"></span></span>

<span data-ttu-id="5be8a-124">Assurez-vous que vous avez accès aux éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="5be8a-124">Make sure that you have access to the following:</span></span>
  
- <span data-ttu-id="5be8a-p106">Toute version de [Visual Studio](http://www.visualstudio.com/en-us/downloads/download-visual-studio-vs.aspx) prenant en charge .NET Framework 4. Nous vous recommandons d'utiliser Visual Studio même si vous n'en avez pas techniquement besoin (car vous pouvez utiliser un compilateur C#).</span><span class="sxs-lookup"><span data-stu-id="5be8a-p106">Any version of [Visual Studio](http://www.visualstudio.com/en-us/downloads/download-visual-studio-vs.aspx) that supports the .NET Framework 4. Although technically, you don't need Visual Studio because you can use any C# compiler, we recommend that you use it.</span></span> 
    
- <span data-ttu-id="5be8a-p107">L'[API managée EWS](http://aka.ms/ews-managed-api-readme). Vous pouvez utiliser la version 32 ou 64 bits, en fonction de votre système. Utilisez l'emplacement d'installation par défaut.</span><span class="sxs-lookup"><span data-stu-id="5be8a-p107">The [EWS Managed API](http://aka.ms/ews-managed-api-readme). You can use either the 64-bit or 32-bit version, depending on your system. Use the default installation location.</span></span> 
    
## <a name="create-your-first-ews-managed-api-application"></a><span data-ttu-id="5be8a-130">Création de votre première application d'API managée EWS</span><span class="sxs-lookup"><span data-stu-id="5be8a-130">Create your first EWS Managed API application</span></span>
<span data-ttu-id="5be8a-131"><a name="Create"> </a></span><span class="sxs-lookup"><span data-stu-id="5be8a-131"></span></span>

<span data-ttu-id="5be8a-p108">Ces étapes supposent que vous configurez un site de développement Office 365. Si vous avez téléchargé et installé Exchange, vous devez [installer un certificat valide](http://technet.microsoft.com/fr-fr/library/bb310769%28v=exchg.141%29.aspx) sur votre serveur Exchange, ou [implémenter un rappel de validation de certificat](how-to-validate-a-server-certificate-for-the-ews-managed-api.md) pour un certificat auto-signé fourni par défaut. Notez également que ces étapes peuvent varier légèrement selon la version de Visual Studio que vous utilisez.</span><span class="sxs-lookup"><span data-stu-id="5be8a-p108">These steps assume that you set up an Office 365 Developer Site. If you downloaded and installed Exchange, you will need to [install a valid certificate](http://technet.microsoft.com/fr-fr/library/bb310769%28v=exchg.141%29.aspx) on your Exchange server or [implement a certificate validation](how-to-validate-a-server-certificate-for-the-ews-managed-api.md) callback for a self-signed certificate that is provided by default. Also note that these steps might vary slightly depending on the version of Visual Studio that you are using.</span></span> 
  
### <a name="step-1-create-a-project-in-visual-studio"></a><span data-ttu-id="5be8a-135">Étape 1 : création d'un projet dans Visual Studio</span><span class="sxs-lookup"><span data-stu-id="5be8a-135">Step 1: Create a project in Visual Studio</span></span>

1. <span data-ttu-id="5be8a-p109">Dans Visual Studio, dans le menu **Fichier**, sélectionnez **Nouveau**, puis **Projet**. La boîte de dialogue **Nouveau projet** s'ouvre.</span><span class="sxs-lookup"><span data-stu-id="5be8a-p109">In Visual Studio, on the **File** menu, choose **New**, and then choose **Project**. The **New Project** dialog box opens.</span></span> 
    
2. <span data-ttu-id="5be8a-p110">Créez une **application console C#**. Dans le volet **Modèles**, choisissez **Visual C#**, puis **Application console**.</span><span class="sxs-lookup"><span data-stu-id="5be8a-p110">Create a **C# Console Application**. From the **Templates** pane, choose **Visual C#**, and then choose **Console Application**.</span></span> 
    
3. <span data-ttu-id="5be8a-140">Nommez le projet HelloWorld, puis cliquez sur **OK**.</span><span class="sxs-lookup"><span data-stu-id="5be8a-140">Name the project HelloWorld, and then choose **OK**.</span></span>
    
<span data-ttu-id="5be8a-141">Visual Studio crée le projet et ouvre la fenêtre de document de code Program.cs.</span><span class="sxs-lookup"><span data-stu-id="5be8a-141">Visual Studio creates the project and opens the Program.cs code document window.</span></span>

### <a name="step-2-add-a-reference-to-the-ews-managed-api"></a><span data-ttu-id="5be8a-142">Étape 2 : ajout d'une référence à l'API managée EWS</span><span class="sxs-lookup"><span data-stu-id="5be8a-142">Step 2: Add a reference to the EWS Managed API</span></span>

1. <span data-ttu-id="5be8a-p111">Si la fenêtre **Explorateur de solutions** est déjà ouverte, ignorez cette étape et passez à l'étape 2. Pour ouvrir la fenêtre **Explorateur de solutions**, sous le menu **Affichage**, choisissez **Explorateur de solutions**.</span><span class="sxs-lookup"><span data-stu-id="5be8a-p111">If the **Solution Explorer** window is already open, skip this step and proceed to step 2. To open the **Solution Explorer** window, on the **View** menu, choose **Solution Explorer**.</span></span> 
    
2. <span data-ttu-id="5be8a-p112">Dans l' **Explorateur de solutions** et le projet **HelloWorld**, ouvrez le menu contextuel (clic droit) de **Références** et choisissez **Ajouter une référence**. Une boîte de dialogue pour la gestion des références du projet s'ouvre.</span><span class="sxs-lookup"><span data-stu-id="5be8a-p112">In the **Solution Explorer** and the **HelloWorld** project, open the shortcut menu (right-click) for **References** and choose **Add Reference** from the context menu. A dialog box for managing project references will open.</span></span> 
    
3. <span data-ttu-id="5be8a-p113">Choisissez l'option **Parcourir**. Accédez à l'emplacement dans lequel vous avez installé le DLL d'API managée EWS. Le chemin par défaut défini par l'installateur est le suivant : C:\Program Files\Microsoft\Exchange\Web Services\<version>\. Le chemin peut varier en fonction de la version de Microsoft.Exchange.WebServices.dll que vous avez téléchargée (32 ou 64 bits). Choisissez **Microsoft.Exchange.WebServices.dll** et sélectionnez **OK** ou **Ajouter**. Cette action permet d'ajouter la référence d'API managée EWS à votre projet.</span><span class="sxs-lookup"><span data-stu-id="5be8a-p113">Choose the **Browse** option. Browse to the location where you installed the EWS Managed API DLL. The default path set by the installer is the following: C:\Program Files\Microsoft\Exchange\Web Services\<version>\. The path can vary based on whether you download the 32 or 64 bit version of the Microsoft.Exchange.WebServices.dll. Choose **Microsoft.Exchange.WebServices.dll** and select **OK** or **Add**. This adds the EWS Managed API reference to your project.</span></span> 
    
4. <span data-ttu-id="5be8a-p114">Si vous utilisez API managée EWS 2.0, modifiez le projet HelloWorld de façon à ce qu'il cible .NET Framework 4. D'autres versions de l'API managée EWS peuvent utiliser une version cible différente de .NET Framework.</span><span class="sxs-lookup"><span data-stu-id="5be8a-p114">If you are using EWS Managed API 2.0, change the HelloWorld project to target the .NET Framework 4. Other versions of the EWS Managed API might use a different target version of the .NET Framework.</span></span>
    
5. <span data-ttu-id="5be8a-p115">Vérifiez que vous utilisez la version cible appropriée de .NET Framework. Ouvrez le menu contextuel (clic droit) pour votre projet **HelloWorld** dans l' **Explorateur de solutions**, puis choisissez **Propriétés**. Vérifiez que **.NET Framework 4** est sélectionné dans la zone de liste déroulante **Version cible de .NET Framework**.</span><span class="sxs-lookup"><span data-stu-id="5be8a-p115">Confirm that you are using the correct target version of the .NET Framework. Open the shortcut menu (right-click) for your **HelloWorld** project in the **Solution Explorer**, and choose **Properties**. Verify that the **.NET Framework 4** is selected in the **Target framework** drop-down box.</span></span> 
    
<span data-ttu-id="5be8a-158">Maintenant que votre projet est configuré et que vous avez créé une référence à l'API managée EWS, vous êtes prêt à créer votre première application.</span><span class="sxs-lookup"><span data-stu-id="5be8a-158">Now that you have your project set up and you created a reference to the EWS Managed API, you are ready to create your first application.</span></span> <span data-ttu-id="5be8a-159">Pour simplifier les choses, ajoutez votre code au fichier Program.cs.</span><span class="sxs-lookup"><span data-stu-id="5be8a-159">To keep things simple, add your code to the Program.cs file.</span></span> <span data-ttu-id="5be8a-160">Lire la [référence l’assembly d’API managées](how-to-reference-the-ews-managed-api-assembly.md) pour plus d’informations sur la référence à l’API managée EWS.</span><span class="sxs-lookup"><span data-stu-id="5be8a-160">Read [Reference the EWS Managed API assembly](how-to-reference-the-ews-managed-api-assembly.md) for more information about referencing the EWS Managed API.</span></span> <span data-ttu-id="5be8a-161">À l'étape suivante, vous allez développer le code de base pour écrire la plupart des applications clientes d'API managée EWS.</span><span class="sxs-lookup"><span data-stu-id="5be8a-161">In the next step, you will develop the basic code to write most EWS Managed API client applications.</span></span> 
### <a name="step-3-set-up-url-redirection-validation-for-autodiscover"></a><span data-ttu-id="5be8a-162">Étape 3 : configuration de la validation de la redirection d'URL pour la découverte automatique</span><span class="sxs-lookup"><span data-stu-id="5be8a-162">Step 3: Set up URL redirection validation for Autodiscover</span></span>

- <span data-ttu-id="5be8a-p117">Ajoutez la méthode de rappel de validation de redirection suivante après la méthode **Main(string[] args)**. Cette action permet de vérifier si les URL redirigées renvoyées par la [découverte automatique](autodiscover-for-exchange.md) représentent un point de terminaison HTTPS.</span><span class="sxs-lookup"><span data-stu-id="5be8a-p117">Add the following redirection validation callback method after the **Main(string[] args)** method. This validates whether redirected URLs returned by [Autodiscover](autodiscover-for-exchange.md) represent an HTTPS endpoint.</span></span> 
    
  ```cs
  private static bool RedirectionUrlValidationCallback(string redirectionUrl)
  {
     // The default for the validation callback is to reject the URL.
     bool result = false;
     Uri redirectionUri = new Uri(redirectionUrl);
     // Validate the contents of the redirection URL. In this simple validation
     // callback, the redirection URL is considered valid if it is using HTTPS
     // to encrypt the authentication credentials. 
     if (redirectionUri.Scheme == "https")
     {
        result = true;
     }
     return result;
  }
  ```

<span data-ttu-id="5be8a-p118">Ce rappel de validation est transmis à l'objet **ExchangeService** à l'étape 4. Vous en avez besoin de façon à ce que votre application approuve et suive les redirections de la découverte automatique. Les résultats de la redirection de la découverte automatique fournissent le point de terminaison EWS de votre application.</span><span class="sxs-lookup"><span data-stu-id="5be8a-p118">This validation callback will be passed to the **ExchangeService** object in step 4. You need this so that your application will trust and follow Autodiscover redirects - the results of the Autodiscover redirect provides the EWS endpoint for our application.</span></span> 

### <a name="step-4-prepare-the-exchangeservice-object"></a><span data-ttu-id="5be8a-167">Étape 4 : préparation de l'objet ExchangeService</span><span class="sxs-lookup"><span data-stu-id="5be8a-167">Step 4: Prepare the ExchangeService object</span></span>

1. <span data-ttu-id="5be8a-p119">Ajoutez une référence de directive **using** à l'API managée EWS. Ajoutez le code suivant après la dernière directive **using** dans la partie supérieure de Program.cs.</span><span class="sxs-lookup"><span data-stu-id="5be8a-p119">Add a **using** directive reference to the EWS Managed API. Add the following code after the last **using** directive at the top of Program.cs.</span></span> 
    
   ```cs
    using Microsoft.Exchange.WebServices.Data;
   ```

2. <span data-ttu-id="5be8a-p120">Dans la méthode **Main**, instanciez l'objet [ExchangeService](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) avec la version de service que vous souhaitez cibler. Cet exemple cible la version la plus ancienne du schéma EWS.</span><span class="sxs-lookup"><span data-stu-id="5be8a-p120">In the **Main** method, instantiate the [ExchangeService](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object with the service version you intend to target. This example targets the earliest version of the EWS schema.</span></span> 
    
   ```cs
    ExchangeService service = new ExchangeService(ExchangeVersion.Exchange2007_SP1);
   ```

3. <span data-ttu-id="5be8a-p121">Si vous ciblez un serveur Exchange local et que votre client est joint au domaine, passez à l'étape 4. Si votre client cible une boîte aux lettres de site de développement Office 365 ou Exchange Online, vous devez transmettre des informations d'identification explicites. Ajoutez le code suivant après l'instanciation de l'objet **ExchangeService** et définissez les informations d'identification de votre compte de boîte aux lettres. Le nom d'utilisateur doit être le nom de l'utilisateur principal. Passez à l'étape 5.</span><span class="sxs-lookup"><span data-stu-id="5be8a-p121">If you are targeting an on-premises Exchange server and your client is domain joined, proceed to step 4. If you client is targeting an Exchange Online or Office 365 Developer Site mailbox, you have to pass explicit credentials. Add the following code after the instantiation of the **ExchangeService** object and set the credentials for your mailbox account. The user name should be the user principal name. Proceed to step 5.</span></span> 
    
   ```cs
    service.Credentials = new WebCredentials("user1@contoso.com", "password");
   ```

4. <span data-ttu-id="5be8a-p122">Les clients joints au domaine qui ciblent un serveur Exchange local peuvent utiliser les informations d'identification par défaut de l'utilisateur connecté, en supposant que les informations d'identification sont associées à une boîte aux lettres. Ajoutez le code suivant après l'instanciation de l'objet **ExchangeService**.</span><span class="sxs-lookup"><span data-stu-id="5be8a-p122">Domain-joined clients that target an on-premises Exchange server can use the default credentials of the user who is logged on, assuming the credentials are associated with a mailbox. Add the following code after the instantiation of the **ExchangeService** object.</span></span> 
    
   ```cs
    service.UseDefaultCredentials = true;
   ```

   <span data-ttu-id="5be8a-p123">Si votre client cible une boîte aux lettres de site de développement Exchange Online ou Office 365, vérifiez que l'élément [UseDefaultCredentials](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservicebase.usedefaultcredentials%28v=exchg.80%29.aspx) est défini sur **false**, qui est la valeur par défaut. Votre client est prêt à effectuer le premier appel vers le service de découverte automatique pour obtenir l'URL de service pour les appels vers le service EWS.</span><span class="sxs-lookup"><span data-stu-id="5be8a-p123">If your client targets an Exchange Online or Office 365 Developer Site mailbox, verify that [UseDefaultCredentials](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservicebase.usedefaultcredentials%28v=exchg.80%29.aspx) is set to **false**, which is the default value. Your client is ready to make the first call to the Autodiscover service to get the service URL for calls to the EWS service.</span></span>
    
5. <span data-ttu-id="5be8a-p124">La méthode **AutodiscoverUrl** sur l'objet **ExchangeService** effectue une série d'appels vers le service de découverte automatique pour obtenir l'URL de service. Si cet appel de méthode aboutit, la propriété d'URL sur l'objet **ExchangeService** sera définie avec l'URL de service. Transmettez l'adresse de messagerie de l'utilisateur et l'élément **RedirectionUrlValidationCallback** à la méthode **AutodiscoverUrl**. Ajoutez le code suivant après la spécification des informations d'identification à l'étape 3 ou 4. Remplacez  `user1@contoso.com` par votre adresse électronique afin que le service de découverte automatique détecte votre point de terminaison EWS.</span><span class="sxs-lookup"><span data-stu-id="5be8a-p124">The **AutodiscoverUrl** method on the **ExchangeService** object performs a series of calls to the Autodiscover service to get the service URL. If this method call is successful, the URL property on the **ExchangeService** object will be set with the service URL. Pass the user's email address and the **RedirectionUrlValidationCallback** to the **AutodiscoverUrl** method. Add the following code after the credentials have been specified in step 3 or 4. Change  `user1@contoso.com` to your email address so that the Autodiscover service finds your EWS endpoint.</span></span> 
    
   ```cs
    service.AutodiscoverUrl("user1@contoso.com", RedirectionUrlValidationCallback);
   ```

<span data-ttu-id="5be8a-186">À ce stade, votre client est configuré pour émettre des appels à EWS pour accéder aux données de boîtes aux lettres.</span><span class="sxs-lookup"><span data-stu-id="5be8a-186">At this point, your client is set up to make calls to EWS to access mailbox data.</span></span> <span data-ttu-id="5be8a-187">Si vous exécutez votre code maintenant, vous pouvez vérifier que l'appel de méthode **AutodiscoverUrl** a fonctionné en examinant le contenu de la propriété [ExchangeService.Url](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="5be8a-187">If you run your code now, you can verify that the **AutodiscoverUrl** method call worked by examining the contents of the [ExchangeService.Url](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) property.</span></span> <span data-ttu-id="5be8a-188">Si cette propriété contient une URL, votre appel a abouti.</span><span class="sxs-lookup"><span data-stu-id="5be8a-188">If this property contains a URL, your call was a success!</span></span> <span data-ttu-id="5be8a-189">Cela signifie que votre application s'est correctement authentifiée auprès du service et qu'elle a découvert le point de terminaison EWS de votre boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="5be8a-189">This means that your application successfully authenticated with the service and discovered the EWS endpoint for your mailbox.</span></span> <span data-ttu-id="5be8a-190">Vous êtes maintenant prêt à émettre vos premiers appels vers EWS.</span><span class="sxs-lookup"><span data-stu-id="5be8a-190">Now you are ready to make your first calls to EWS.</span></span> <span data-ttu-id="5be8a-191">Pour plus d’informations sur la définition de l’URL EWS, lisez [la valeur de l’URL du service à l’aide de l’API managées EWS](how-to-set-the-ews-service-url-by-using-the-ews-managed-api.md) .</span><span class="sxs-lookup"><span data-stu-id="5be8a-191">Read [Set the EWS service URL by using the EWS Managed API](how-to-set-the-ews-service-url-by-using-the-ews-managed-api.md) for more information about setting the EWS URL.</span></span> 

### <a name="step-6-create-your-first-hello-world-email-message"></a><span data-ttu-id="5be8a-192">Étape 6 : création de votre premier message électronique Hello World</span><span class="sxs-lookup"><span data-stu-id="5be8a-192">Step 6: Create your first Hello World email message</span></span>

1. <span data-ttu-id="5be8a-193">Après l'appel de méthode **AutodiscoverUrl**, instanciez un nouvel objet **EmailMessage** et transmettez l'objet de service que vous avez créé.</span><span class="sxs-lookup"><span data-stu-id="5be8a-193">After the **AutodiscoverUrl** method call, instantiate a new **EmailMessage** object and pass in the service object you created.</span></span> 
    
   ```cs
    EmailMessage email = new EmailMessage(service);
   ```

   <span data-ttu-id="5be8a-p126">Vous disposez désormais d'un message électronique sur lequel la liaison de service est définie. Les appels émis sur l'objet **EmailMessage** sont destinés à ce service.</span><span class="sxs-lookup"><span data-stu-id="5be8a-p126">You now have an email message on which the service binding is set. Any calls initiated on the **EmailMessage** object will be targeted at the service.</span></span> 
    
2. <span data-ttu-id="5be8a-p127">À présent, définissez la ligne du destinataire du message électronique (To:). Pour ce faire, modifiez l'élément  `user1@contoso.com` afin d'utiliser votre adresse SMTP.</span><span class="sxs-lookup"><span data-stu-id="5be8a-p127">Now set the To: line recipient of the email message. To do this, change  `user1@contoso.com` to use your SMTP address.</span></span> 
    
   ```cs
    email.ToRecipients.Add("user1@contoso.com");
   ```

3. <span data-ttu-id="5be8a-198">Définissez l'objet et le corps du message électronique.</span><span class="sxs-lookup"><span data-stu-id="5be8a-198">Set the subject and the body of the email message.</span></span>
    
   ```cs
    email.Subject = "HelloWorld";
    email.Body = new MessageBody("This is the first email I've sent by using the EWS Managed API.");
   ```

4. <span data-ttu-id="5be8a-199">Vous êtes maintenant prêt à envoyer votre premier message électronique à l'aide de l'API managée EWS.</span><span class="sxs-lookup"><span data-stu-id="5be8a-199">You are now ready to send your first email message by using the EWS Managed API.</span></span> <span data-ttu-id="5be8a-200">La méthode **Send** appelle le service et soumet le message électronique pour livraison.</span><span class="sxs-lookup"><span data-stu-id="5be8a-200">The **Send** method will call the service and submit the email message for delivery.</span></span> <span data-ttu-id="5be8a-201">Lisez [communiquer avec EWS à l’aide de l’API managée EWS](how-to-communicate-with-ews-by-using-the-ews-managed-api.md) pour en savoir plus sur les autres méthodes que vous pouvez utiliser pour communiquer avec Exchange.</span><span class="sxs-lookup"><span data-stu-id="5be8a-201">Read [Communicate with EWS by using the EWS Managed API](how-to-communicate-with-ews-by-using-the-ews-managed-api.md) to learn about other methods you can use to communicate with Exchange.</span></span> 
    
   ```cs
    email.Send();
   ```

5. <span data-ttu-id="5be8a-p129">Vous êtes prêt à exécuter votre application Hello World. Dans Visual Studio, sélectionnez **F5**. Une fenêtre de console vide s'ouvre. Vous ne verrez rien dans la fenêtre de console le temps que votre application s'authentifie, suive les redirections de la découverte automatique et effectue son premier appel pour créer un message électronique que vous envoyez à vous-même. Si vous souhaitez voir les appels en cours, ajoutez les deux lignes suivantes de code avant d'appeler la méthode **AutodiscoverUrl**. Appuyez ensuite sur F5. Cette action permet de [transmettre les requêtes et les réponses EWS](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md) dans la fenêtre de console.</span><span class="sxs-lookup"><span data-stu-id="5be8a-p129">You are ready to run your Hello World application. In Visual Studio, select **F5**. A blank console window will open. You will not see anything in the console window while your application authenticates, follows Autodiscover redirections, and then makes its first call to create an email message that you send to yourself. If you want to see the calls being made, add the following two lines of code before the **AutodiscoverUrl** method is called. Then press F5. This will [trace out the EWS requests and responses](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md) to the console window.</span></span> 
    
   ```cs
    service.TraceEnabled = true;
    service.TraceFlags = TraceFlags.All;
   ```

<span data-ttu-id="5be8a-p130">Vous disposez maintenant d'une application cliente d'API managée EWS qui fonctionne. Pour plus de commodité, l'exemple suivant comporte l'intégralité du code que vous avez ajouté à Program.cs pour créer votre application Hello World.</span><span class="sxs-lookup"><span data-stu-id="5be8a-p130">You now have a working EWS Managed API client application. For your convenience, the following example shows all the code that you added to Program.cs to create your Hello World application.</span></span>

```cs
using System;
using Microsoft.Exchange.WebServices.Data;
namespace HelloWorld
{
  class Program
  {
    static void Main(string[] args)
    {
      ExchangeService service = new ExchangeService(ExchangeVersion.Exchange2007_SP1);
      service.Credentials = new WebCredentials("user1@contoso.com", "password");
      service.TraceEnabled = true;
      service.TraceFlags = TraceFlags.All;
      service.AutodiscoverUrl("user1@contoso.com", RedirectionUrlValidationCallback);
      EmailMessage email = new EmailMessage(service);
      email.ToRecipients.Add("user1@contoso.com");
      email.Subject = "HelloWorld";
      email.Body = new MessageBody("This is the first email I've sent by using the EWS Managed API");
      email.Send();
    }
    private static bool RedirectionUrlValidationCallback(string redirectionUrl)
    {
      // The default for the validation callback is to reject the URL.
      bool result = false;
      Uri redirectionUri = new Uri(redirectionUrl);
      // Validate the contents of the redirection URL. In this simple validation
      // callback, the redirection URL is considered valid if it is using HTTPS
      // to encrypt the authentication credentials. 
      if (redirectionUri.Scheme == "https")
      {
        result = true;
      }
      return result;
    }
  }
}
```

## <a name="next-steps"></a><span data-ttu-id="5be8a-211">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="5be8a-211">Next steps</span></span>
<span data-ttu-id="5be8a-212"><a name="Next"> </a></span><span class="sxs-lookup"><span data-stu-id="5be8a-212"></span></span>

<span data-ttu-id="5be8a-213">Si vous êtes prêt à aller plus loin avec votre première application cliente d'API managée EWS, consultez les ressources suivantes :</span><span class="sxs-lookup"><span data-stu-id="5be8a-213">If you're ready to do more with your first EWS Managed API client application, explore the following resources:</span></span>
  
- [<span data-ttu-id="5be8a-214">Exchange 2013 : 101 exemples de code</span><span class="sxs-lookup"><span data-stu-id="5be8a-214">Exchange 2013: 101 code samples</span></span>](http://code.msdn.microsoft.com/exchange/Exchange-2013-101-Code-3c38582c)
    
- [<span data-ttu-id="5be8a-215">Dossiers et éléments</span><span class="sxs-lookup"><span data-stu-id="5be8a-215">Folders and items</span></span>](folders-and-items-in-ews-in-exchange.md)
    
- [<span data-ttu-id="5be8a-216">EWSEditor</span><span class="sxs-lookup"><span data-stu-id="5be8a-216">EWSEditor</span></span>](http://ewseditor.codeplex.com/)
    
<span data-ttu-id="5be8a-217">Si vous rencontrez des problèmes avec votre application, [publiez une question ou un commentaire dans le forum](http://social.technet.microsoft.com/Forums/exchange/en-US/home?forum=exchangesvrdevelopment) (et n'oubliez pas de lire la meilleure publication).</span><span class="sxs-lookup"><span data-stu-id="5be8a-217">If you run into any issues with your application, [try posting a question or comment in the forum](http://social.technet.microsoft.com/Forums/exchange/en-US/home?forum=exchangesvrdevelopment) (and don't forget to read the top post).</span></span> 
  
## <a name="in-this-section"></a><span data-ttu-id="5be8a-218">Dans cette section</span><span class="sxs-lookup"><span data-stu-id="5be8a-218">In this section</span></span>
<span data-ttu-id="5be8a-219"><a name="Next"> </a></span><span class="sxs-lookup"><span data-stu-id="5be8a-219"></span></span>

- [<span data-ttu-id="5be8a-220">Référence de l’assembly de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="5be8a-220">Reference the EWS Managed API assembly</span></span>](how-to-reference-the-ews-managed-api-assembly.md)
    
- [<span data-ttu-id="5be8a-221">Définir l’URL du service EWS à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="5be8a-221">Set the EWS service URL by using the EWS Managed API</span></span>](how-to-set-the-ews-service-url-by-using-the-ews-managed-api.md)
    
- [<span data-ttu-id="5be8a-222">Communiquer avec EWS à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="5be8a-222">Communicate with EWS by using the EWS Managed API</span></span>](how-to-communicate-with-ews-by-using-the-ews-managed-api.md)
    
## <a name="see-also"></a><span data-ttu-id="5be8a-223">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="5be8a-223">See also</span></span>

- [<span data-ttu-id="5be8a-224">Commencer à utiliser les services web dans Exchange</span><span class="sxs-lookup"><span data-stu-id="5be8a-224">Start using web services in Exchange</span></span>](start-using-web-services-in-exchange.md)    
- [<span data-ttu-id="5be8a-225">Vue d'ensemble de la conception client EWS pour Exchange</span><span class="sxs-lookup"><span data-stu-id="5be8a-225">EWS client design overview for Exchange</span></span>](ews-client-design-overview-for-exchange.md)    
- [<span data-ttu-id="5be8a-226">Développer des clients de service web pour Exchange</span><span class="sxs-lookup"><span data-stu-id="5be8a-226">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)   
- [<span data-ttu-id="5be8a-227">Suivi des demandes et réponses pour dépanner les applications de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="5be8a-227">Trace requests and responses to troubleshoot EWS Managed API applications</span></span>](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md)
    

