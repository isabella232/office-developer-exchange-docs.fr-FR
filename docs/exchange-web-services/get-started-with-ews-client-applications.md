---
title: Prise en main des applications clientes EWS
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: e6fd5c23-0ba5-4a7b-bdde-4a553447069f
description: Créez votre première application en utilisant Exchange Web Services (EWS) dans Exchange.
ms.openlocfilehash: 911495c74f4c74114a86b1a3a98c9200db338b34
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754791"
---
# <a name="get-started-with-ews-client-applications"></a>Prise en main des applications clientes EWS

Ce document peut contenir des informations liées aux fonctionnalités ou produits préliminaires qui sont sujettes à modifications avant la sortie de la version définitive. Ce document est fourni "tel quel" à titre indicatif et Microsoft exclut toute garantie, expresse ou implicite, en ce qui concerne ce document. Créez votre première application en utilisant Exchange Web Services (EWS) dans Exchange.
  
EWS est un service complet que vos applications peuvent utiliser pour accéder à presque toutes les informations stockées dans une boîte aux lettres Exchange Online, Exchange Online dans le cadre d'Office 365 ou Exchange en local. EWS utilise les protocoles web standard pour fournir un accès à un serveur Exchange ; les bibliothèques telles que l'[API managée EWS](get-started-with-ews-managed-api-client-applications.md) encapsulent les opérations EWS pour fournir une interface orientée objet. Une fois que vous aurez exécuté les exemples de cet article, vous maîtriserez les concepts de base d'EWS. 
  
Vous pouvez appeler les opérations EWS à partir de n'importe quel système d'exploitation ou langage, car les requêtes et réponses EWS utilisent le protocole SOAP. Les exemples de cet article sont écrits à l'aide de C# et utilisent .NET Framework [HttpWebRequest](https://msdn.microsoft.com/library/System.Net.HttpWebRequest.aspx) et [HttpWebResponse](https://msdn.microsoft.com/library/System.Net.HttpWebResponse.aspx) des objets ; toutefois, la partie importante du code est le code XML utilisé pour établir la demande EWS et la réponse XML renvoyée par le serveur. Les exemples de code mettent en évidence les transactions XML et ne traitent pas le code XML. 
  
## <a name="youll-need-an-exchange-server"></a>Besoin d'un serveur Exchange

Si vous avez déjà un compte de boîte aux lettres Exchange, vous pouvez ignorer cette étape. Dans le cas contraire, vous pouvez configurer une boîte aux lettres Exchange pour votre première application EWS par le biais des méthodes suivantes :
  
- En obtenant un [site de développement Office 365](http://msdn.microsoft.com/en-us/library/office/fp179924.aspx) (recommandé). Il s'agit de la manière la plus rapide d'obtenir une boîte aux lettres Exchange.
    
- En téléchargeant [Exchange Server](http://office.microsoft.com/en-us/exchange/microsoft-exchange-try-or-buy-exchange-we-can-help-you-decide-FX103746846.aspx?WT%2Eintid1=ODC%5FENUS%5FFX103472230%5FXT103965589).
    
Après avoir vérifié que vous pouvez envoyer et recevoir des messages électroniques à partir de votre serveur Exchange, vous êtes prêt à configurer votre environnement de développement. Vous pouvez utiliser l'application web Outlook pour vérifier que vous pouvez envoyer des messages électroniques.
  
Vous devez également connaître l'URL du point de terminaison EWS du serveur. Dans une application de production, vous devez utiliser la [découverte automatique](autodiscover-for-exchange.md) pour déterminer l'URL EWS. Les exemples de cet article utilisent l'URL du point de terminaison Office 365 EWS, https://outlook.office365.com/EWS/Exchange.asmx. La section [Étapes suivantes](#bk_next) comporte des liens vers des informations complémentaires sur la découverte automatique que vous pouvez consulter lorsque vous êtes prêt. 
  
Si vous testez votre application à l'aide d'un serveur Exchange qui comporte le certificat auto-signé par défaut, vous devez créer une [méthode de validation de certificats](how-to-validate-a-server-certificate-for-the-ews-managed-api.md) répondant aux exigences de sécurité de votre organisation. 
  
## <a name="set-up-your-development-environment"></a>Configuration de votre environnement de développement

Les outils que vous utilisez pour créer votre première application EWS dépendent de votre système d'exploitation et de votre langage, selon vos goûts personnels principalement. Si vous voulez suivre les exemples C# de cet article, vous avez besoin des éléments suivants : 
  
- Toute version de Visual Studio qui prend en charge .NET Framework 4.0. 
    
- Une connexion Internet que votre ordinateur de développement peut utiliser pour contacter votre serveur Exchange. Si vous pouvez utiliser Outlook Web App avec un nom DNS plutôt qu'avec une adresse IP pour vous connecter à votre serveur Exchange, la configuration est opérationnelle.
    
## <a name="create-your-first-ews-application"></a>Création de votre première application EWS

L'application EWS que vous allez créer illustre deux scénarios courants d'utilisation d'EWS :
  
1. Obtenir des informations à partir d'une boîte aux lettres Exchange et afficher ces informations à l'utilisateur.
    
2. Effectuer une action, comme envoyer un courrier électronique et vérifier la réponse pour voir si l'action a réussi.
    
Nous allons commencer.
  
### <a name="set-up-the-solution"></a>Configurer la solution

Commencez par créer une solution d'application console à l'aide de Visual Studio. Lorsque la solution est prête, créez un objet nommé Tracing.cs. Utilisez cet objet pour écrire des informations sur la console et un fichier journal afin de pouvoir consulter les résultats après l'exécution de votre code. Collez le code suivant dans le fichier Tracing.cs.
  
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

Ouvrez ensuite le fichier Program.cs. Copiez le reste du code de l'exemple dans ce fichier.
  
Tout d'abord, configurez le shell du programme. Le programme : 
  
1. Crée un fichier journal afin que la demande et la réponse puissent être écrites sur le disque pour consultation ultérieure.
    
2. Obtient l'adresse de messagerie et le mot de passe du compte auquel vous accédez.
    
3. Appelle les méthodes de l'échantillon.
    
Remplacez la méthode  `Main` dans Program.cs par le code suivant. 
  
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

La dernière chose que vous devez faire est d'ajouter la méthode statique  `GetPasswordFromConsole`. Cette méthode retourne un objet [SecureString](https://msdn.microsoft.com/library/System.Security.SecureString.aspx) qui contient un mot de passe tapé à la console. 
  
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

### <a name="get-the-number-of-new-messages-in-an-inbox"></a>Obtenir le nombre de nouveaux messages dans une boîte de réception

Parmi les opérations courantes qu'une application EWS peut effectuer, on peut citer l'obtention d'informations sur les messages électroniques, les rendez-vous, les réunions et sur les dossiers qui les stockent. Cet exemple obtient le nombre de messages résidant dans la boîte de réception d'un compte et affiche le nombre total de messages et le nombre de messages non lus. Il illustre les actions courantes suivantes pour les applications EWS :
  
- Soumettre une demande EWS au serveur Exchange.
    
- Analyse de la réponse XML renvoyée pour les informations demandées.
    
- Gestion des exceptions et messages d'erreur courants.
    
Ajoutez le code suivant à la méthode  `ShowNumberOfMessagesInInbox` qui a été générée après la méthode principale. Lorsque vous exécutez l'application, elle imprime le nombre de messages dans la boîte de réception du compte et le nombre de messages non lus dans la boîte de réception. Après avoir exécuté l'application, vous pouvez ouvrir le fichier GetStartedWithEWS.log pour afficher la requête XML qui a été envoyée au serveur Exchange et la réponse que le serveur a renvoyée. 
  
```cs
      /// This is the XML request that is sent to the Exchange server.
      var getFolderSOAPRequest =
"<?xml version=\"1.0\" encoding=\"utf-8\"?>\n" +
"<soap:Envelope xmlns:soap=\"http://schemas.xmlsoap.org/soap/envelope/\"\n" +
"   xmlns:t=\"http://schemas.microsoft.com/exchange/services/2006/types\">\n" +
"<soap:Header>\n" +
"    <t:RequestServerVersion Version=\"Exchange2007_SP1\" />\n" +
"  </soap:Header>\n" +
"  <soap:Body>\n" +
"    <GetFolder xmlns=\"http://schemas.microsoft.com/exchange/services/2006/messages\"\n" +
"               xmlns:t=\"http://schemas.microsoft.com/exchange/services/2006/types\">\n" +
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
                                               ("{http://schemas.microsoft.com/exchange/services/2006/messages}ResponseCode")
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
                                              ("{http://schemas.microsoft.com/exchange/services/2006/messages}Folders")
                                            select folderElement;
            foreach (var folder in folders)
            {
              Tracing.Write("Folder name:     ");
              var folderName = from folderElement in
                                 folder.Descendants
                                 ("{http://schemas.microsoft.com/exchange/services/2006/types}DisplayName")
                               select folderElement.Value;
              Tracing.WriteLine(folderName.ElementAt(0));
              Tracing.Write("Total messages:  ");
              var totalCount = from folderElement in
                                 folder.Descendants
                                   ("{http://schemas.microsoft.com/exchange/services/2006/types}TotalCount")
                               select folderElement.Value;
              Tracing.WriteLine(totalCount.ElementAt(0));
              Tracing.Write("Unread messages: ");
              var unreadCount = from folderElement in
                                 folder.Descendants
                                   ("{http://schemas.microsoft.com/exchange/services/2006/types}UnreadCount")
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

### <a name="send-an-email-message"></a>Envoyer un message électronique

Une autre opération courante pour une application EWS consiste à envoyer des messages électroniques ou des demandes de réunion. Cet exemple crée et envoie un message électronique à l'aide les informations d'identification utilisateur qui ont été entrées précédemment. Il illustre ces tâches d'application EWS courantes :
  
- Création et envoi d'un courrier électronique.
    
- Analyse de la réponse XML renvoyée pour déterminer si le message a été envoyé correctement.
    
- Gestion des exceptions et messages d'erreur courants.
    
Ajoutez le code suivant à la méthode SendTestEmail qui a été générée après la méthode principale. Après avoir exécuté l'application, vous pouvez ouvrir le fichier GetStartedWithEWS.log pour afficher la requête XML qui a été envoyée au serveur Exchange et la réponse que le serveur a renvoyée.
  
```cs
var createItemSOAPRequest =
      "<?xml version=\"1.0\" encoding=\"utf-8\"?>\n" +
      "<soap:Envelope xmlns:xsi=\"http://www.w3.org/2001/XMLSchema-instance\" \n" +
      "               xmlns:m=\"http://schemas.microsoft.com/exchange/services/2006/messages\" \n" +
      "               xmlns:t=\"http://schemas.microsoft.com/exchange/services/2006/types\" \n" +
      "               xmlns:soap=\"http://schemas.xmlsoap.org/soap/envelope/\">\n" +
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
                                               ("{http://schemas.microsoft.com/exchange/services/2006/messages}ResponseCode")
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

## <a name="next-steps"></a>Étapes suivantes

Maintenant que vous avez écrit votre première application EWS, vous êtes prêt à découvrir d'autres manières d'utiliser EWS. Voici quelques idées pour bien commencer :
  
- Mettez en œuvre la [découverte automatique](autodiscover-for-exchange.md) dans votre application afin que votre application se connecte au serveur Exchange approprié en fonction de l'adresse de messagerie de l'utilisateur. Reportez-vous également à l'exemple [Exchange 2013 : obtenir les paramètres de l'utilisateur à l'aide de découverte automatique](http://code.msdn.microsoft.com/Exchange-2013-Get-user-7e22c86e). 
    
- Reportez-vous à la [Référence EWS](http://msdn.microsoft.com/library/2a873474-1bb2-4cb1-a556-40e8c4159f4a%28Office.15%29.aspx) pour plus d'informations sur EWS. 
    
- Reportez-vous à [Opérations EWS](http://msdn.microsoft.com/library/cf6fd871-9a65-4f34-8557-c8c71dd7ce09%28Office.15%29.aspx) pour plus d'informations sur les opérations disponibles. 
    
- Utilisez [l'éditeur EWS](http://ewseditor.codeplex.com/) pour afficher le trafic SOAP envoyé vers et depuis le serveur. 
    
Si vous rencontrez des problèmes avec votre application, [publiez une question ou un commentaire dans le forum](http://social.technet.microsoft.com/Forums/exchange/en-US/home?forum=exchangesvrdevelopment) (et n'oubliez pas de lire la première publication). 
  
## <a name="see-also"></a>Voir aussi

- [Commencer à utiliser les services web dans Exchange](start-using-web-services-in-exchange.md)   
- [Explorer l'API managée EWS, EWS et les services web dans Exchange](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) 
- [Vue d'ensemble de la conception client EWS pour Exchange](ews-client-design-overview-for-exchange.md)   
- [Développer des clients de service web pour Exchange](develop-web-service-clients-for-exchange.md)  
- [Prise en main des applications clientes d'API managée EWS](get-started-with-ews-managed-api-client-applications.md)
    

