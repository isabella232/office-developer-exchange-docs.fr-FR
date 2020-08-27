---
title: Prise en main des applications clientes EWS
manager: sethgros
ms.date: 8/26/2020
ms.audience: Developer
ms.assetid: e6fd5c23-0ba5-4a7b-bdde-4a553447069f
description: Créez votre première application en utilisant Exchange Web Services (EWS) dans Exchange.
localization_priority: Priority
ms.openlocfilehash: 81d4cb69d20f17945658ab4ad16c9fe3a47d4eec
ms.sourcegitcommit: 636c05a929279812c6ef87d75b01c166a4a05584
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/26/2020
ms.locfileid: "47254978"
---
# <a name="get-started-with-ews-client-applications"></a><span data-ttu-id="95c55-103">Prise en main des applications clientes EWS</span><span class="sxs-lookup"><span data-stu-id="95c55-103">Get started with EWS client applications</span></span>

<span data-ttu-id="95c55-104">Créez votre première application en utilisant Exchange Web Services (EWS) dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="95c55-104">Create your first application by using Exchange Web Services (EWS) in Exchange.</span></span>
  
<span data-ttu-id="95c55-p101">EWS est un service complet que vos applications peuvent utiliser pour accéder à presque toutes les informations stockées dans une boîte aux lettres Exchange Online, Exchange Online dans le cadre d'Office 365 ou Exchange en local. EWS utilise les protocoles web standard pour fournir un accès à un serveur Exchange ; les bibliothèques telles que l'[API managée EWS](get-started-with-ews-managed-api-client-applications.md) encapsulent les opérations EWS pour fournir une interface orientée objet. Une fois que vous aurez exécuté les exemples de cet article, vous maîtriserez les concepts de base d'EWS.</span><span class="sxs-lookup"><span data-stu-id="95c55-p101">EWS is a comprehensive service that your applications can use to access almost all the information stored in an Exchange Online, Exchange Online as part of Office 365, or Exchange on-premises mailbox. EWS uses standard web protocols to provide access to an Exchange server; libraries like the [EWS Managed API](get-started-with-ews-managed-api-client-applications.md) wrap the EWS operations to provide an object-oriented interface. After you've run the examples in this article, you will have a basic understanding of what you can do with EWS.</span></span> 
  
<span data-ttu-id="95c55-p102">Vous pouvez appeler les opérations EWS à partir de n'importe quel système d'exploitation ou langage, car les requêtes et réponses EWS utilisent le protocole SOAP. Les exemples de cet article sont écrits à l'aide de C# et utilisent .NET Framework [HttpWebRequest](https://msdn.microsoft.com/library/System.Net.HttpWebRequest.aspx) et [HttpWebResponse](https://msdn.microsoft.com/library/System.Net.HttpWebResponse.aspx) des objets ; toutefois, la partie importante du code est le code XML utilisé pour établir la demande EWS et la réponse XML renvoyée par le serveur. Les exemples de code mettent en évidence les transactions XML et ne traitent pas le code XML.</span><span class="sxs-lookup"><span data-stu-id="95c55-p102">You can call EWS operations from any operating system or language, because the EWS requests and responses use the SOAP protocol. The examples in this article are written using C# and make use of the .NET Framework [HttpWebRequest](https://msdn.microsoft.com/library/System.Net.HttpWebRequest.aspx) and [HttpWebResponse](https://msdn.microsoft.com/library/System.Net.HttpWebResponse.aspx) objects; however, the important part of the code is the XML used to make the EWS request and the XML response returned from the server. The code examples emphasize the XML transactions and not processing the XML.</span></span> 
  
## <a name="youll-need-an-exchange-server"></a><span data-ttu-id="95c55-111">Besoin d'un serveur Exchange</span><span class="sxs-lookup"><span data-stu-id="95c55-111">You'll need an Exchange server</span></span>

<span data-ttu-id="95c55-p103">Si vous avez déjà un compte de boîte aux lettres Exchange, vous pouvez ignorer cette étape. Dans le cas contraire, vous pouvez configurer une boîte aux lettres Exchange pour votre première application EWS par le biais des méthodes suivantes :</span><span class="sxs-lookup"><span data-stu-id="95c55-p103">If you already have an Exchange mailbox account, you can skip this step. Otherwise, you have the following options for setting up an Exchange mailbox for your first EWS application:</span></span>
  
- <span data-ttu-id="95c55-p104">En obtenant un [site de développement Office 365](https://developer.microsoft.com/microsoft-365/dev-program) (recommandé). Il s'agit de la manière la plus rapide d'obtenir une boîte aux lettres Exchange.</span><span class="sxs-lookup"><span data-stu-id="95c55-p104">[Get an Office 365 Developer Site ](https://developer.microsoft.com/microsoft-365/dev-program)(recommended). This is the quickest way for you to get an Exchange mailbox.</span></span>
    
- <span data-ttu-id="95c55-116">En téléchargeant [Exchange Server](https://office.microsoft.com/exchange/microsoft-exchange-try-or-buy-exchange-we-can-help-you-decide-FX103746846.aspx?WT%2Eintid1=ODC%5FENUS%5FFX103472230%5FXT103965589).</span><span class="sxs-lookup"><span data-stu-id="95c55-116">Download [Exchange Server](https://office.microsoft.com/exchange/microsoft-exchange-try-or-buy-exchange-we-can-help-you-decide-FX103746846.aspx?WT%2Eintid1=ODC%5FENUS%5FFX103472230%5FXT103965589).</span></span>

    
<span data-ttu-id="95c55-p105">Après avoir vérifié que vous pouvez envoyer et recevoir des messages électroniques à partir de votre serveur Exchange, vous êtes prêt à configurer votre environnement de développement. Vous pouvez utiliser l'application web Outlook pour vérifier que vous pouvez envoyer des messages électroniques.</span><span class="sxs-lookup"><span data-stu-id="95c55-p105">After you've verified that you can send and receive email from your Exchange server you are ready to set up your development environment. You can use Outlook Web App to verify that you can send email.</span></span>
  
<span data-ttu-id="95c55-p106">Vous devez également connaître l'URL du point de terminaison EWS du serveur. Dans une application de production, vous devez utiliser la [découverte automatique](autodiscover-for-exchange.md) pour déterminer l'URL EWS. Les exemples de cet article utilisent l'URL du point de terminaison Office 365 EWS, `https://outlook.office365.com/EWS/Exchange.asmx`. La section [Étapes suivantes](#bk_next) comporte des liens vers des informations complémentaires sur la découverte automatique que vous pouvez consulter lorsque vous êtes prêt.</span><span class="sxs-lookup"><span data-stu-id="95c55-p106">You'll also need to know the URL of the EWS endpoint for your server. In a production application, you'd use [Autodiscover](autodiscover-for-exchange.md) to determine the EWS URL. The examples in this article use the Office 365 EWS endpoint URL, `https://outlook.office365.com/EWS/Exchange.asmx`. The [Next steps](#bk_next) section has links to more information about Autodiscover when you're ready.</span></span> 
  
<span data-ttu-id="95c55-123">Si vous testez votre application à l'aide d'un serveur Exchange qui comporte le certificat auto-signé par défaut, vous devez créer une [méthode de validation de certificats](how-to-validate-a-server-certificate-for-the-ews-managed-api.md) répondant aux exigences de sécurité de votre organisation.</span><span class="sxs-lookup"><span data-stu-id="95c55-123">If you are testing your application using an Exchange server that has the default self-signed certificate, you'll need to create a [certificate validation method](how-to-validate-a-server-certificate-for-the-ews-managed-api.md) that meets the security requirements of your organization.</span></span> 
  
## <a name="set-up-your-development-environment"></a><span data-ttu-id="95c55-124">Configuration de votre environnement de développement</span><span class="sxs-lookup"><span data-stu-id="95c55-124">Set up your development environment</span></span>

<span data-ttu-id="95c55-p107">Les outils que vous utilisez pour créer votre première application EWS dépendent de votre système d'exploitation et de votre langage, selon vos goûts personnels principalement. Si vous voulez suivre les exemples C# de cet article, vous avez besoin des éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="95c55-p107">The tools that you use to create your first EWS application depend on the operating system and language that you use, and are mostly a matter of taste. If you want to follow along with the C# examples in this article, you'll need:</span></span> 
  
- <span data-ttu-id="95c55-127">Toute version de Visual Studio qui prend en charge .NET Framework 4.0.</span><span class="sxs-lookup"><span data-stu-id="95c55-127">Any version of Visual Studio that supports the .NET Framework 4.0.</span></span> 
    
- <span data-ttu-id="95c55-p108">Une connexion Internet que votre ordinateur de développement peut utiliser pour contacter votre serveur Exchange. Si vous pouvez utiliser Outlook Web App avec un nom DNS plutôt qu’avec une adresse IP pour vous connecter à votre serveur Exchange, la configuration est opérationnelle.</span><span class="sxs-lookup"><span data-stu-id="95c55-p108">An Internet connection that your development machine can use to contact your Exchange server. If you can use Outlook Web App with a DNS name rather than an IP address to connect to your Exchange server, you are set up.</span></span>
    
## <a name="create-your-first-ews-application"></a><span data-ttu-id="95c55-130">Création de votre première application EWS</span><span class="sxs-lookup"><span data-stu-id="95c55-130">Create your first EWS application</span></span>

<span data-ttu-id="95c55-131">L’application EWS que vous allez créer illustre deux scénarios courants d’utilisation d’EWS :</span><span class="sxs-lookup"><span data-stu-id="95c55-131">The EWS application that you will create shows two typical scenarios for using EWS:</span></span>
  
1. <span data-ttu-id="95c55-132">Obtenir des informations à partir d'une boîte aux lettres Exchange et afficher ces informations à l'utilisateur.</span><span class="sxs-lookup"><span data-stu-id="95c55-132">Get information from an Exchange mailbox and display that information to the user.</span></span>
    
2. <span data-ttu-id="95c55-133">Effectuer une action, comme envoyer un courrier électronique et vérifier la réponse pour voir si l'action a réussi.</span><span class="sxs-lookup"><span data-stu-id="95c55-133">Perform an action, such as sending an email, and check the response to see if the action succeeded.</span></span>
    
<span data-ttu-id="95c55-134">Nous allons commencer.</span><span class="sxs-lookup"><span data-stu-id="95c55-134">Let's get started.</span></span>
  
### <a name="set-up-the-solution"></a><span data-ttu-id="95c55-135">Configurer la solution</span><span class="sxs-lookup"><span data-stu-id="95c55-135">Set up the solution</span></span>

<span data-ttu-id="95c55-p109">Commencez par créer une solution d’application console à l’aide de Visual Studio. Lorsque la solution est prête, créez un objet nommé Tracing.cs. Utilisez cet objet pour écrire des informations sur la console et un fichier journal afin de pouvoir consulter les résultats après l’exécution de votre code. Collez le code suivant dans le fichier Tracing.cs.</span><span class="sxs-lookup"><span data-stu-id="95c55-p109">First, create a new console application solution using Visual Studio. When the solution is ready, create a new object called Tracing.cs. Use this object to write information to both the console and a log file so that you can review the results after you run your code. Paste the following code into the Tracing.cs file.</span></span>
  
```cs
using System;
using System.IO;
namespace Microsoft.Exchange.Samples.EWS
{
  class Tracing
  {
    private static TextWriter logFileWriter = null;
    public static void OpenLog(string fileName)
    {
      logFileWriter = new StreamWriter(fileName);
    }
    public static void Write(string format, params object[] args)
    {
      Console.Write(format, args);
      if (logFileWriter != null)
      {
        logFileWriter.Write(format, args);
      }
    }
    public static void WriteLine(string format, params object[] args)
    {
      Console.WriteLine(format, args);
      if (logFileWriter != null)
      {
        logFileWriter.WriteLine(format, args);
      }
    }
    public static void CloseLog()
    {
      logFileWriter.Flush();
      logFileWriter.Close();
    }
  }
}
```

<span data-ttu-id="95c55-p110">Ouvrez ensuite le fichier Program.cs. Copiez le reste du code de l'exemple dans ce fichier.</span><span class="sxs-lookup"><span data-stu-id="95c55-p110">Next, open the Program.cs file. You will put the rest of the code for the example in this file.</span></span>
  
<span data-ttu-id="95c55-p111">Tout d'abord, configurez le shell du programme. Le programme :</span><span class="sxs-lookup"><span data-stu-id="95c55-p111">First, set up the shell of the program. The program will:</span></span> 
  
1. <span data-ttu-id="95c55-144">Crée un fichier journal afin que la demande et la réponse puissent être écrites sur le disque pour consultation ultérieure.</span><span class="sxs-lookup"><span data-stu-id="95c55-144">Create a log file so that the request and response can be written to disk for later study.</span></span>
    
2. <span data-ttu-id="95c55-145">Obtient l'adresse de messagerie et le mot de passe du compte auquel vous accédez.</span><span class="sxs-lookup"><span data-stu-id="95c55-145">Get the email address and password of the account that you'll access.</span></span>
    
3. <span data-ttu-id="95c55-146">Appelle les méthodes de l'échantillon.</span><span class="sxs-lookup"><span data-stu-id="95c55-146">Call the sample methods.</span></span>
    
<span data-ttu-id="95c55-147">Remplacez la méthode  `Main` dans Program.cs par le code suivant.</span><span class="sxs-lookup"><span data-stu-id="95c55-147">Replace the  `Main` method in the Program.cs with the following code.</span></span> 
  
```cs
    static void Main(string[] args)
    {
      // Start tracing to console and a log file.
      Tracing.OpenLog("./GetStartedWithEWS.log");
      Tracing.WriteLine("EWS sample application started.");
      var isValidEmailAddress = false;
      Console.Write("Enter an email address: ");
      var emailAddress = Console.ReadLine();
      
        isValidEmailAddress = (emailAddress.Contains("@") &amp;&amp; emailAddress.Contains("."));
      if (!isValidEmailAddress)
      {
        Tracing.WriteLine("Email address " + emailAddress + " is not a valid SMTP address. Closing program.");
        return;
      }
      SecureString password = GetPasswordFromConsole();
      if (password.Length == 0)
      {
        Tracing.WriteLine("Password empty, closing program.");
      }
      NetworkCredential userCredentials = new NetworkCredential(emailAddress, password);
      // These are the sample methods that demonstrate using EWS.
      // ShowNumberOfMessagesInInbox(userCredentials);
      // SendTestEmail(userCredentials);
     
      Tracing.WriteLine("EWS sample application ends.");
      Tracing.CloseLog();
      Console.WriteLine("Press enter to exit: ");
      Console.ReadLine();
    }
    // These method stubs will be filled in later.
    private static void ShowNumberOfMessagesInInbox(NetworkCredential userCredentials)
    {
    }
    private static void SendTestEmail(NetworkCredential userCredentials)
    {
    }
```

<span data-ttu-id="95c55-p112">La dernière chose que vous devez faire est d'ajouter la méthode statique  `GetPasswordFromConsole`. Cette méthode retourne un objet [SecureString](https://msdn.microsoft.com/library/System.Security.SecureString.aspx) qui contient un mot de passe tapé à la console.</span><span class="sxs-lookup"><span data-stu-id="95c55-p112">The last thing that you need to do is add the  `GetPasswordFromConsole` static method. This method returns a [SecureString](https://msdn.microsoft.com/library/System.Security.SecureString.aspx) object that contains a password typed at the console.</span></span> 
  
```cs
    private static SecureString GetPasswordFromConsole()
    {
      SecureString password = new SecureString();
      bool readingPassword = true;
      Console.Write("Enter password: ");
      while (readingPassword)
      {
        ConsoleKeyInfo userInput = Console.ReadKey(true);
        switch (userInput.Key)
        {
          case (ConsoleKey.Enter):
            readingPassword = false;
            break;
          case (ConsoleKey.Escape):
            password.Clear();
            readingPassword = false;
            break;
          case (ConsoleKey.Backspace):
            if (password.Length > 0)
            {
              password.RemoveAt(password.Length - 1);
              Console.SetCursorPosition(Console.CursorLeft - 1, Console.CursorTop);
              Console.Write(" ");
              Console.SetCursorPosition(Console.CursorLeft - 1, Console.CursorTop);
            }
            break;
          default:
            if (userInput.KeyChar != 0)
            {
              password.AppendChar(userInput.KeyChar);
              Console.Write("*");
            }
            break;
        }
      }
      Console.WriteLine();
      password.MakeReadOnly();
      return password;
    }
```

### <a name="get-the-number-of-new-messages-in-an-inbox"></a><span data-ttu-id="95c55-150">Obtenir le nombre de nouveaux messages dans une boîte de réception</span><span class="sxs-lookup"><span data-stu-id="95c55-150">Get the number of new messages in an Inbox</span></span>

<span data-ttu-id="95c55-p113">Parmi les opérations courantes qu'une application EWS peut effectuer, on peut citer l'obtention d'informations sur les messages électroniques, les rendez-vous, les réunions et sur les dossiers qui les stockent. Cet exemple obtient le nombre de messages résidant dans la boîte de réception d'un compte et affiche le nombre total de messages et le nombre de messages non lus. Il illustre les actions courantes suivantes pour les applications EWS :</span><span class="sxs-lookup"><span data-stu-id="95c55-p113">A common operation in an EWS application is to get information about email messages, appointments, meetings, and the folders that store them. This example gets the number of messages in an account's Inbox and displays the total number of messages and the number of unread messages. It demonstrates the following common actions for EWS applications:</span></span>
  
- <span data-ttu-id="95c55-154">Soumettre une demande EWS au serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="95c55-154">Making an EWS request to the Exchange server.</span></span>
    
- <span data-ttu-id="95c55-155">Analyse de la réponse XML renvoyée pour les informations demandées.</span><span class="sxs-lookup"><span data-stu-id="95c55-155">Parsing the returned XML response for the requested information.</span></span>
    
- <span data-ttu-id="95c55-156">Gestion des exceptions et messages d'erreur courants.</span><span class="sxs-lookup"><span data-stu-id="95c55-156">Handling common exceptions and error messages.</span></span>
    
<span data-ttu-id="95c55-p114">Ajoutez le code suivant à la méthode  `ShowNumberOfMessagesInInbox` qui a été générée après la méthode principale. Lorsque vous exécutez l'application, elle imprime le nombre de messages dans la boîte de réception du compte et le nombre de messages non lus dans la boîte de réception. Après avoir exécuté l'application, vous pouvez ouvrir le fichier GetStartedWithEWS.log pour afficher la requête XML qui a été envoyée au serveur Exchange et la réponse que le serveur a renvoyée.</span><span class="sxs-lookup"><span data-stu-id="95c55-p114">Add the following code to the  `ShowNumberOfMessagesInInbox` method that was stubbed out after the main method. When you run the application, it will print the number of messages in the account's Inbox and the number of unread messages in the Inbox. After you run the application, you can open the GetStartedWithEWS.log file to see the XML request that was sent to the Exchange server and the response that the server returned.</span></span> 
  
```cs
      /// This is the XML request that is sent to the Exchange server.
      var getFolderSOAPRequest =
"<?xml version=\"1.0\" encoding=\"utf-8\"?>\n" +
"<soap:Envelope xmlns:soap=\"https://schemas.xmlsoap.org/soap/envelope/\"\n" +
"   xmlns:t=\"https://schemas.microsoft.com/exchange/services/2006/types\">\n" +
"<soap:Header>\n" +
"    <t:RequestServerVersion Version=\"Exchange2007_SP1\" />\n" +
"  </soap:Header>\n" +
"  <soap:Body>\n" +
"    <GetFolder xmlns=\"https://schemas.microsoft.com/exchange/services/2006/messages\"\n" +
"               xmlns:t=\"https://schemas.microsoft.com/exchange/services/2006/types\">\n" +
"      <FolderShape>\n" +
"        <t:BaseShape>Default</t:BaseShape>\n" +
"      </FolderShape>\n" +
"      <FolderIds>\n" +
"        <t:DistinguishedFolderId Id=\"inbox\"/>\n" +
"      </FolderIds>\n" +
"    </GetFolder>\n" +
"  </soap:Body>\n" +
"</soap:Envelope>\n";
      // Write the get folder operation request to the console and log file.
      Tracing.WriteLine("Get folder operation request:");
      Tracing.WriteLine(getFolderSOAPRequest);
      var getFolderRequest = WebRequest.CreateHttp(Office365WebServicesURL);
      getFolderRequest.AllowAutoRedirect = false;
      getFolderRequest.Credentials = userCredentials;
      getFolderRequest.Method = "POST";
      getFolderRequest.ContentType = "text/xml";
      var requestWriter = new StreamWriter(getFolderRequest.GetRequestStream());
      requestWriter.Write(getFolderSOAPRequest);
      requestWriter.Close();
      try
      {
        var getFolderResponse = (HttpWebResponse)(getFolderRequest.GetResponse());
        if (getFolderResponse.StatusCode == HttpStatusCode.OK)
        {
          var responseStream = getFolderResponse.GetResponseStream();
          XElement responseEnvelope = XElement.Load(responseStream);
          if (responseEnvelope != null)
          {
            // Write the response to the console and log file.
            Tracing.WriteLine("Response:");
            StringBuilder stringBuilder = new StringBuilder();
            XmlWriterSettings settings = new XmlWriterSettings();
            settings.Indent = true;
            XmlWriter writer = XmlWriter.Create(stringBuilder, settings);
            responseEnvelope.Save(writer);
            writer.Close();
            Tracing.WriteLine(stringBuilder.ToString());
            // Check the response for error codes. If there is an error, throw an application exception.
            IEnumerable<XElement> errorCodes = from errorCode in responseEnvelope.Descendants
                                               ("{https://schemas.microsoft.com/exchange/services/2006/messages}ResponseCode")
                                               select errorCode;
            foreach (var errorCode in errorCodes)
            {
              if (errorCode.Value != "NoError")
              {
                switch (errorCode.Parent.Name.LocalName.ToString())
                {
                  case "Response":
                    string responseError = "Response-level error getting inbox information:\n" + errorCode.Value;
                    throw new ApplicationException(responseError);
                  case "UserResponse":
                    string userError = "User-level error getting inbox information:\n" + errorCode.Value;
                    throw new ApplicationException(userError);
                }
              }
            }
            // Process the response.
            IEnumerable<XElement> folders = from folderElement in
                                              responseEnvelope.Descendants
                                              ("{https://schemas.microsoft.com/exchange/services/2006/messages}Folders")
                                            select folderElement;
            foreach (var folder in folders)
            {
              Tracing.Write("Folder name:     ");
              var folderName = from folderElement in
                                 folder.Descendants
                                 ("{https://schemas.microsoft.com/exchange/services/2006/types}DisplayName")
                               select folderElement.Value;
              Tracing.WriteLine(folderName.ElementAt(0));
              Tracing.Write("Total messages:  ");
              var totalCount = from folderElement in
                                 folder.Descendants
                                   ("{https://schemas.microsoft.com/exchange/services/2006/types}TotalCount")
                               select folderElement.Value;
              Tracing.WriteLine(totalCount.ElementAt(0));
              Tracing.Write("Unread messages: ");
              var unreadCount = from folderElement in
                                 folder.Descendants
                                   ("{https://schemas.microsoft.com/exchange/services/2006/types}UnreadCount")
                               select folderElement.Value;
              Tracing.WriteLine(unreadCount.ElementAt(0));
            }
          }
        }
      }
      catch (WebException ex)
      {
        Tracing.WriteLine("Caught Web exception:");
        Tracing.WriteLine(ex.Message);
      }
      catch (ApplicationException ex)
      {
        Tracing.WriteLine("Caught application exception:");
        Tracing.WriteLine(ex.Message);
      }

```

### <a name="send-an-email-message"></a><span data-ttu-id="95c55-160">Envoyer un message électronique</span><span class="sxs-lookup"><span data-stu-id="95c55-160">Send an email message</span></span>

<span data-ttu-id="95c55-p115">Une autre opération courante pour une application EWS consiste à envoyer des messages électroniques ou des demandes de réunion. Cet exemple crée et envoie un message électronique à l’aide les informations d’identification utilisateur qui ont été entrées précédemment. Il illustre ces tâches d’application EWS courantes :</span><span class="sxs-lookup"><span data-stu-id="95c55-p115">Another common operation for an EWS application is to send email messages or meeting requests. This example creates and sends an email message using the user credentials that were entered earlier. It demonstrates these common EWS application tasks:</span></span>
  
- <span data-ttu-id="95c55-164">Création et envoi d'un courrier électronique.</span><span class="sxs-lookup"><span data-stu-id="95c55-164">Creating and sending an email.</span></span>
    
- <span data-ttu-id="95c55-165">Analyse de la réponse XML renvoyée pour déterminer si le message a été envoyé correctement.</span><span class="sxs-lookup"><span data-stu-id="95c55-165">Parsing the returned XML response to determine if the email was correctly sent.</span></span>
    
- <span data-ttu-id="95c55-166">Gestion des exceptions et messages d'erreur courants.</span><span class="sxs-lookup"><span data-stu-id="95c55-166">Handling common exceptions and error messages.</span></span>
    
<span data-ttu-id="95c55-p116">Ajoutez le code suivant à la méthode SendTestEmail qui a été générée après la méthode principale. Après avoir exécuté l’application, vous pouvez ouvrir le fichier GetStartedWithEWS.log pour afficher la requête XML qui a été envoyée au serveur Exchange et la réponse que le serveur a renvoyée.</span><span class="sxs-lookup"><span data-stu-id="95c55-p116">Add the following code to the SendTestEmail method that was stubbed out after the main method. After you run the application, you can open the GetStartedWithEWS.log file to see the XML request that was sent to the Exchange server and the response that the server returned.</span></span>
  
```cs
var createItemSOAPRequest =
      "<?xml version=\"1.0\" encoding=\"utf-8\"?>\n" +
      "<soap:Envelope xmlns:xsi=\"http://www.w3.org/2001/XMLSchema-instance\" \n" +
      "               xmlns:m=\"https://schemas.microsoft.com/exchange/services/2006/messages\" \n" +
      "               xmlns:t=\"https://schemas.microsoft.com/exchange/services/2006/types\" \n" +
      "               xmlns:soap=\"https://schemas.xmlsoap.org/soap/envelope/\">\n" +
      "  <soap:Header>\n" +
      "    <t:RequestServerVersion Version=\"Exchange2007_SP1\" />\n" +
      "  </soap:Header>\n" +
      "  <soap:Body>\n" +
      "    <m:CreateItem MessageDisposition=\"SendAndSaveCopy\">\n" +
      "      <m:SavedItemFolderId>\n" +
      "        <t:DistinguishedFolderId Id=\"sentitems\" />\n" +
      "      </m:SavedItemFolderId>\n" +
      "      <m:Items>\n" +
      "        <t:Message>\n" +
      "          <t:Subject>Company Soccer Team</t:Subject>\n" +
      "          <t:Body BodyType=\"HTML\">Are you interested in joining?</t:Body>\n" +
      "          <t:ToRecipients>\n" +
      "            <t:Mailbox>\n" +
      "              <t:EmailAddress>sadie@contoso.com</t:EmailAddress>\n" +
      "              </t:Mailbox>\n" +
      "          </t:ToRecipients>\n" +
      "        </t:Message>\n" +
      "      </m:Items>\n" +
      "    </m:CreateItem>\n" +
      "  </soap:Body>\n" +
      "</soap:Envelope>\n";
      // Write the create item operation request to the console and log file.
      Tracing.WriteLine("Get folder operation request:");
      Tracing.WriteLine(createItemSOAPRequest);
      var getFolderRequest = WebRequest.CreateHttp(Office365WebServicesURL);
      getFolderRequest.AllowAutoRedirect = false;
      getFolderRequest.Credentials = userCredentials;
      getFolderRequest.Method = "POST";
      getFolderRequest.ContentType = "text/xml";
      var requestWriter = new StreamWriter(getFolderRequest.GetRequestStream());
      requestWriter.Write(createItemSOAPRequest);
      requestWriter.Close();
      try
      {
        var getFolderResponse = (HttpWebResponse)(getFolderRequest.GetResponse());
        if (getFolderResponse.StatusCode == HttpStatusCode.OK)
        {
          var responseStream = getFolderResponse.GetResponseStream();
          XElement responseEnvelope = XElement.Load(responseStream);
          if (responseEnvelope != null)
          {
            // Write the response to the console and log file.
            Tracing.WriteLine("Response:");
            StringBuilder stringBuilder = new StringBuilder();
            XmlWriterSettings settings = new XmlWriterSettings();
            settings.Indent = true;
            XmlWriter writer = XmlWriter.Create(stringBuilder, settings);
            responseEnvelope.Save(writer);
            writer.Close();
            Tracing.WriteLine(stringBuilder.ToString());
            // Check the response for error codes. If there is an error, throw an application exception.
            IEnumerable<XElement> errorCodes = from errorCode in responseEnvelope.Descendants
                                               ("{https://schemas.microsoft.com/exchange/services/2006/messages}ResponseCode")
                                               select errorCode;
            foreach (var errorCode in errorCodes)
            {
              if (errorCode.Value != "NoError")
              {
                switch (errorCode.Parent.Name.LocalName.ToString())
                {
                  case "Response":
                    string responseError = "Response-level error getting inbox information:\n" + errorCode.Value;
                    throw new ApplicationException(responseError);
                  case "UserResponse":
                    string userError = "User-level error getting inbox information:\n" + errorCode.Value;
                    throw new ApplicationException(userError);
                }
              }
            }
            Tracing.WriteLine("Message sent successfully.");
          }
        }
      }
      catch (WebException ex)
      {
        Tracing.WriteLine("Caught Web exception:");
        Tracing.WriteLine(ex.Message);
      }
      catch (ApplicationException ex)
      {
        Tracing.WriteLine("Caught application exception:");
        Tracing.WriteLine(ex.Message);
      }
```

<a name="bk_next"></a>

## <a name="next-steps"></a><span data-ttu-id="95c55-169">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="95c55-169">Next steps</span></span>

<span data-ttu-id="95c55-p117">Maintenant que vous avez écrit votre première application EWS, vous êtes prêt à découvrir d'autres manières d'utiliser EWS. Voici quelques idées pour bien commencer :</span><span class="sxs-lookup"><span data-stu-id="95c55-p117">Now that you've written your first EWS application, you're ready to discover other ways to use EWS. Here are some ideas to get you started:</span></span>
  
- <span data-ttu-id="95c55-p118">Mettez en œuvre la [découverte automatique](autodiscover-for-exchange.md) dans votre application afin que votre application se connecte au serveur Exchange approprié en fonction de l'adresse de messagerie de l'utilisateur. Reportez-vous également à l'exemple [Exchange 2013 : obtenir les paramètres de l'utilisateur à l'aide de découverte automatique](https://code.msdn.microsoft.com/Exchange-2013-Get-user-7e22c86e).</span><span class="sxs-lookup"><span data-stu-id="95c55-p118">Implement [Autodiscover](autodiscover-for-exchange.md) in your application so that your application will connect to the correct Exchange server based on the user's email address. See also the [Exchange 2013: Get user settings with Autodiscover](https://code.msdn.microsoft.com/Exchange-2013-Get-user-7e22c86e) sample.</span></span> 
    
- <span data-ttu-id="95c55-174">Reportez-vous à la [Référence EWS](https://msdn.microsoft.com/library/2a873474-1bb2-4cb1-a556-40e8c4159f4a%28Office.15%29.aspx) pour plus d'informations sur EWS.</span><span class="sxs-lookup"><span data-stu-id="95c55-174">Look at the [EWS reference](https://msdn.microsoft.com/library/2a873474-1bb2-4cb1-a556-40e8c4159f4a%28Office.15%29.aspx) for more information about EWS.</span></span> 
    
- <span data-ttu-id="95c55-175">Reportez-vous à [Opérations EWS](https://msdn.microsoft.com/library/cf6fd871-9a65-4f34-8557-c8c71dd7ce09%28Office.15%29.aspx) pour plus d'informations sur les opérations disponibles.</span><span class="sxs-lookup"><span data-stu-id="95c55-175">See the [EWS operations](https://msdn.microsoft.com/library/cf6fd871-9a65-4f34-8557-c8c71dd7ce09%28Office.15%29.aspx) for information about the operations that are available.</span></span> 
    
- <span data-ttu-id="95c55-176">Utilisez [l'éditeur EWS](http://ewseditor.codeplex.com/) pour afficher le trafic SOAP envoyé vers et depuis le serveur.</span><span class="sxs-lookup"><span data-stu-id="95c55-176">Use [EWS Editor](http://ewseditor.codeplex.com/) to see the SOAP traffic sent to and from the server.</span></span> 
    
<span data-ttu-id="95c55-177">Si vous rencontrez des problèmes avec votre application, [publiez une question ou un commentaire dans le forum](https://social.technet.microsoft.com/Forums/exchange/home?forum=exchangesvrdevelopment) (et n'oubliez pas de lire la première publication).</span><span class="sxs-lookup"><span data-stu-id="95c55-177">If you run into any issues with your application, [try posting a question or comment in the forum](https://social.technet.microsoft.com/Forums/exchange/home?forum=exchangesvrdevelopment) (and don't forget to read the first post).</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="95c55-178">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="95c55-178">See also</span></span>

- [<span data-ttu-id="95c55-179">Commencer à utiliser les services web dans Exchange</span><span class="sxs-lookup"><span data-stu-id="95c55-179">Start using web services in Exchange</span></span>](start-using-web-services-in-exchange.md)   
- [<span data-ttu-id="95c55-180">Explorer l'API managée EWS, EWS et les services web dans Exchange</span><span class="sxs-lookup"><span data-stu-id="95c55-180">Explore the EWS Managed API, EWS, and web services in Exchange</span></span>](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) 
- [<span data-ttu-id="95c55-181">Vue d'ensemble de la conception client EWS pour Exchange</span><span class="sxs-lookup"><span data-stu-id="95c55-181">EWS client design overview for Exchange</span></span>](ews-client-design-overview-for-exchange.md)   
- [<span data-ttu-id="95c55-182">Développer des clients de service web pour Exchange</span><span class="sxs-lookup"><span data-stu-id="95c55-182">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)  
- [<span data-ttu-id="95c55-183">Prise en main des applications clientes d'API managée EWS</span><span class="sxs-lookup"><span data-stu-id="95c55-183">Get started with EWS Managed API client applications</span></span>](get-started-with-ews-managed-api-client-applications.md)
    
