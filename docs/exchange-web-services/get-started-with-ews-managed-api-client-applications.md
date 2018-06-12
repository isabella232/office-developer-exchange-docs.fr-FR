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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19754794"
---
# <a name="get-started-with-ews-managed-api-client-applications"></a>Prise en main des applications clientes d'API managée EWS

Ce document peut contenir des informations liées aux fonctionnalités ou produits préliminaires qui sont sujettes à modifications avant la sortie de la version définitive. Ce document est fourni "tel quel" à titre indicatif et Microsoft exclut toute garantie, expresse ou implicite, en ce qui concerne ce document. Développer une application cliente de messagerie Hello World simple pour Exchange à l'aide de l'API managée EWS. 
  
L'[API managée EWS](http://aka.ms/ews-managed-api-readme) fournit un modèle objet intuitif et facile à utiliser pour envoyer et recevoir des messages du service web à partir d'applications clientes, d'applications de portail et d'applications de service. Vous pouvez accéder à presque toutes les informations stockées dans une boîte aux lettres de serveur Exchange Online, Exchange Online dans le cadre d'Office 365 ou Exchange à l'aide de l'API managée EWS. Vous pouvez utiliser les informations de cet article pour développer votre première application cliente d'API managée EWS. 
  
> [!NOTE]
> [!REMARQUE]  L'API managée EWS est maintenant disponible en tant que projet open source sur [GitHub](https://github.com/officedev/ews-managed-api). Vous pouvez utiliser la bibliothèque open source afin de : >  participer aux résolutions de bogues et aux améliorations apportées à l'API ; >  obtenir des correctifs et des améliorations avant qu'ils soient disponibles dans une version officielle ; >  accéder à l'implémentation la plus complète et la plus à jour de l'API, afin de l'utiliser comme référence ou pour créer des bibliothèques sur de nouvelles plateformes. >  Vos [contributions](https://github.com/OfficeDev/ews-managed-api/blob/master/CONTRIBUTING.md) via GitHub sont les bienvenues. 
  
## <a name="youll-need-an-exchange-server"></a>Besoin d'un serveur Exchange
<a name="NeedExchange"> </a>

Si vous avez déjà un compte de boîte aux lettres Exchange, vous pouvez ignorer cette section. Dans le cas contraire, vous pouvez configurer une boîte aux lettres Exchange pour votre première application cliente EWS par le biais des méthodes suivantes :
  
- En obtenant un [site de développement Office 365](http://msdn.microsoft.com/en-us/library/office/fp179924.aspx) (recommandé). Il s'agit de la manière la plus rapide de configurer une boîte aux lettres Exchange. 
    
- En téléchargeant [Exchange Server](http://office.microsoft.com/en-us/exchange/microsoft-exchange-try-or-buy-exchange-we-can-help-you-decide-FX103746846.aspx?WT%2Eintid1=ODC%5FENUS%5FFX103472230%5FXT103965589).
    
Après avoir vérifié que vous pouvez envoyer et recevoir des messages électroniques à partir d'Exchange, vous êtes prêt à configurer votre environnement de développement. Vous pouvez utiliser le client web Exchange [Outlook Web App](http://technet.microsoft.com/en-us/library/jj657718%28v=exchg.150%29.aspx) pour vérifier que vous pouvez envoyer des messages électroniques. 
  
## <a name="set-up-your-development-environment"></a>Configuration de votre environnement de développement
<a name="Setup"> </a>

Assurez-vous que vous avez accès aux éléments suivants :
  
- Toute version de [Visual Studio](http://www.visualstudio.com/en-us/downloads/download-visual-studio-vs.aspx) prenant en charge .NET Framework 4. Nous vous recommandons d'utiliser Visual Studio même si vous n'en avez pas techniquement besoin (car vous pouvez utiliser un compilateur C#). 
    
- L'[API managée EWS](http://aka.ms/ews-managed-api-readme). Vous pouvez utiliser la version 32 ou 64 bits, en fonction de votre système. Utilisez l'emplacement d'installation par défaut. 
    
## <a name="create-your-first-ews-managed-api-application"></a>Création de votre première application d'API managée EWS
<a name="Create"> </a>

Ces étapes supposent que vous configurez un site de développement Office 365. Si vous avez téléchargé et installé Exchange, vous devez [installer un certificat valide](http://technet.microsoft.com/en-us/library/bb310769%28v=exchg.141%29.aspx) sur votre serveur Exchange, ou [implémenter un rappel de validation de certificat](how-to-validate-a-server-certificate-for-the-ews-managed-api.md) pour un certificat auto-signé fourni par défaut. Notez également que ces étapes peuvent varier légèrement selon la version de Visual Studio que vous utilisez. 
  
### <a name="step-1-create-a-project-in-visual-studio"></a>Étape 1 : création d'un projet dans Visual Studio

1. Dans Visual Studio, dans le menu **Fichier**, sélectionnez **Nouveau**, puis **Projet**. La boîte de dialogue **Nouveau projet** s'ouvre. 
    
2. Créez une **application console C#**. Dans le volet **Modèles**, choisissez **Visual C#**, puis **Application console**. 
    
3. Nommez le projet HelloWorld, puis cliquez sur **OK**.
    
Visual Studio crée le projet et ouvre la fenêtre de document de code Program.cs.

### <a name="step-2-add-a-reference-to-the-ews-managed-api"></a>Étape 2 : ajout d'une référence à l'API managée EWS

1. Si la fenêtre **Explorateur de solutions** est déjà ouverte, ignorez cette étape et passez à l'étape 2. Pour ouvrir la fenêtre **Explorateur de solutions**, sous le menu **Affichage**, choisissez **Explorateur de solutions**. 
    
2. Dans l' **Explorateur de solutions** et le projet **HelloWorld**, ouvrez le menu contextuel (clic droit) de **Références** et choisissez **Ajouter une référence**. Une boîte de dialogue pour la gestion des références du projet s'ouvre. 
    
3. Choisissez l'option **Parcourir**. Accédez à l'emplacement dans lequel vous avez installé le DLL d'API managée EWS. Le chemin par défaut défini par l'installateur est le suivant : C:\Program Files\Microsoft\Exchange\Web Services\<version>\. Le chemin peut varier en fonction de la version de Microsoft.Exchange.WebServices.dll que vous avez téléchargée (32 ou 64 bits). Choisissez **Microsoft.Exchange.WebServices.dll** et sélectionnez **OK** ou **Ajouter**. Cette action permet d'ajouter la référence d'API managée EWS à votre projet. 
    
4. Si vous utilisez API managée EWS 2.0, modifiez le projet HelloWorld de façon à ce qu'il cible .NET Framework 4. D'autres versions de l'API managée EWS peuvent utiliser une version cible différente de .NET Framework.
    
5. Vérifiez que vous utilisez la version cible appropriée de .NET Framework. Ouvrez le menu contextuel (clic droit) pour votre projet **HelloWorld** dans l' **Explorateur de solutions**, puis choisissez **Propriétés**. Vérifiez que **.NET Framework 4** est sélectionné dans la zone de liste déroulante **Version cible de .NET Framework**. 
    
Maintenant que votre projet est configuré et que vous avez créé une référence à l'API managée EWS, vous êtes prêt à créer votre première application. Pour simplifier les choses, ajoutez votre code au fichier Program.cs. Lire la [référence l’assembly d’API managées](how-to-reference-the-ews-managed-api-assembly.md) pour plus d’informations sur la référence à l’API managée EWS. À l'étape suivante, vous allez développer le code de base pour écrire la plupart des applications clientes d'API managée EWS. 
### <a name="step-3-set-up-url-redirection-validation-for-autodiscover"></a>Étape 3 : configuration de la validation de la redirection d'URL pour la découverte automatique

- Ajoutez la méthode de rappel de validation de redirection suivante après la méthode **Main(string[] args)**. Cette action permet de vérifier si les URL redirigées renvoyées par la [découverte automatique](autodiscover-for-exchange.md) représentent un point de terminaison HTTPS. 
    
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

Ce rappel de validation est transmis à l'objet **ExchangeService** à l'étape 4. Vous en avez besoin de façon à ce que votre application approuve et suive les redirections de la découverte automatique. Les résultats de la redirection de la découverte automatique fournissent le point de terminaison EWS de votre application. 

### <a name="step-4-prepare-the-exchangeservice-object"></a>Étape 4 : préparation de l'objet ExchangeService

1. Ajoutez une référence de directive **using** à l'API managée EWS. Ajoutez le code suivant après la dernière directive **using** dans la partie supérieure de Program.cs. 
    
   ```cs
    using Microsoft.Exchange.WebServices.Data;
   ```

2. Dans la méthode **Main**, instanciez l'objet [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) avec la version de service que vous souhaitez cibler. Cet exemple cible la version la plus ancienne du schéma EWS. 
    
   ```cs
    ExchangeService service = new ExchangeService(ExchangeVersion.Exchange2007_SP1);
   ```

3. Si vous ciblez un serveur Exchange local et que votre client est joint au domaine, passez à l'étape 4. Si votre client cible une boîte aux lettres de site de développement Office 365 ou Exchange Online, vous devez transmettre des informations d'identification explicites. Ajoutez le code suivant après l'instanciation de l'objet **ExchangeService** et définissez les informations d'identification de votre compte de boîte aux lettres. Le nom d'utilisateur doit être le nom de l'utilisateur principal. Passez à l'étape 5. 
    
   ```cs
    service.Credentials = new WebCredentials("user1@contoso.com", "password");
   ```

4. Les clients joints au domaine qui ciblent un serveur Exchange local peuvent utiliser les informations d'identification par défaut de l'utilisateur connecté, en supposant que les informations d'identification sont associées à une boîte aux lettres. Ajoutez le code suivant après l'instanciation de l'objet **ExchangeService**. 
    
   ```cs
    service.UseDefaultCredentials = true;
   ```

   Si votre client cible une boîte aux lettres de site de développement Exchange Online ou Office 365, vérifiez que l'élément [UseDefaultCredentials](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.usedefaultcredentials%28v=exchg.80%29.aspx) est défini sur **false**, qui est la valeur par défaut. Votre client est prêt à effectuer le premier appel vers le service de découverte automatique pour obtenir l'URL de service pour les appels vers le service EWS.
    
5. La méthode **AutodiscoverUrl** sur l'objet **ExchangeService** effectue une série d'appels vers le service de découverte automatique pour obtenir l'URL de service. Si cet appel de méthode aboutit, la propriété d'URL sur l'objet **ExchangeService** sera définie avec l'URL de service. Transmettez l'adresse de messagerie de l'utilisateur et l'élément **RedirectionUrlValidationCallback** à la méthode **AutodiscoverUrl**. Ajoutez le code suivant après la spécification des informations d'identification à l'étape 3 ou 4. Remplacez  `user1@contoso.com` par votre adresse électronique afin que le service de découverte automatique détecte votre point de terminaison EWS. 
    
   ```cs
    service.AutodiscoverUrl("user1@contoso.com", RedirectionUrlValidationCallback);
   ```

À ce stade, votre client est configuré pour émettre des appels à EWS pour accéder aux données de boîtes aux lettres. Si vous exécutez votre code maintenant, vous pouvez vérifier que l'appel de méthode **AutodiscoverUrl** a fonctionné en examinant le contenu de la propriété [ExchangeService.Url](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx). Si cette propriété contient une URL, votre appel a abouti. Cela signifie que votre application s'est correctement authentifiée auprès du service et qu'elle a découvert le point de terminaison EWS de votre boîte aux lettres. Vous êtes maintenant prêt à émettre vos premiers appels vers EWS. Pour plus d’informations sur la définition de l’URL EWS, lisez [la valeur de l’URL du service à l’aide de l’API managées EWS](how-to-set-the-ews-service-url-by-using-the-ews-managed-api.md) . 

### <a name="step-6-create-your-first-hello-world-email-message"></a>Étape 6 : création de votre premier message électronique Hello World

1. Après l'appel de méthode **AutodiscoverUrl**, instanciez un nouvel objet **EmailMessage** et transmettez l'objet de service que vous avez créé. 
    
   ```cs
    EmailMessage email = new EmailMessage(service);
   ```

   Vous disposez désormais d'un message électronique sur lequel la liaison de service est définie. Les appels émis sur l'objet **EmailMessage** sont destinés à ce service. 
    
2. À présent, définissez la ligne du destinataire du message électronique (To:). Pour ce faire, modifiez l'élément  `user1@contoso.com` afin d'utiliser votre adresse SMTP. 
    
   ```cs
    email.ToRecipients.Add("user1@contoso.com");
   ```

3. Définissez l'objet et le corps du message électronique.
    
   ```cs
    email.Subject = "HelloWorld";
    email.Body = new MessageBody("This is the first email I've sent by using the EWS Managed API.");
   ```

4. Vous êtes maintenant prêt à envoyer votre premier message électronique à l'aide de l'API managée EWS. La méthode **Send** appelle le service et soumet le message électronique pour livraison. Lisez [communiquer avec EWS à l’aide de l’API managée EWS](how-to-communicate-with-ews-by-using-the-ews-managed-api.md) pour en savoir plus sur les autres méthodes que vous pouvez utiliser pour communiquer avec Exchange. 
    
   ```cs
    email.Send();
   ```

5. Vous êtes prêt à exécuter votre application Hello World. Dans Visual Studio, sélectionnez **F5**. Une fenêtre de console vide s'ouvre. Vous ne verrez rien dans la fenêtre de console le temps que votre application s'authentifie, suive les redirections de la découverte automatique et effectue son premier appel pour créer un message électronique que vous envoyez à vous-même. Si vous souhaitez voir les appels en cours, ajoutez les deux lignes suivantes de code avant d'appeler la méthode **AutodiscoverUrl**. Appuyez ensuite sur F5. Cette action permet de [transmettre les requêtes et les réponses EWS](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md) dans la fenêtre de console. 
    
   ```cs
    service.TraceEnabled = true;
    service.TraceFlags = TraceFlags.All;
   ```

Vous disposez maintenant d'une application cliente d'API managée EWS qui fonctionne. Pour plus de commodité, l'exemple suivant comporte l'intégralité du code que vous avez ajouté à Program.cs pour créer votre application Hello World.

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

## <a name="next-steps"></a>Étapes suivantes
<a name="Next"> </a>

Si vous êtes prêt à aller plus loin avec votre première application cliente d'API managée EWS, consultez les ressources suivantes :
  
- [Exchange 2013 : 101 exemples de code](http://code.msdn.microsoft.com/exchange/Exchange-2013-101-Code-3c38582c)
    
- [Dossiers et éléments](folders-and-items-in-ews-in-exchange.md)
    
- [EWSEditor](http://ewseditor.codeplex.com/)
    
Si vous rencontrez des problèmes avec votre application, [publiez une question ou un commentaire dans le forum](http://social.technet.microsoft.com/Forums/exchange/en-US/home?forum=exchangesvrdevelopment) (et n'oubliez pas de lire la meilleure publication). 
  
## <a name="in-this-section"></a>Dans cette section
<a name="Next"> </a>

- [Référence de l’assembly de l’API managée EWS](how-to-reference-the-ews-managed-api-assembly.md)
    
- [Définir l’URL du service EWS à l’aide de l’API managée EWS](how-to-set-the-ews-service-url-by-using-the-ews-managed-api.md)
    
- [Communiquer avec EWS à l’aide de l’API managée EWS](how-to-communicate-with-ews-by-using-the-ews-managed-api.md)
    
## <a name="see-also"></a>Voir aussi

- [Commencer à utiliser les services web dans Exchange](start-using-web-services-in-exchange.md)    
- [Vue d'ensemble de la conception client EWS pour Exchange](ews-client-design-overview-for-exchange.md)    
- [Développer des clients de service web pour Exchange](develop-web-service-clients-for-exchange.md)   
- [Suivi des demandes et réponses pour dépanner les applications de l’API managée EWS](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md)
    

