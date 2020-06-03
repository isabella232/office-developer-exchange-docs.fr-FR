---
title: Valider un certificat de serveur pour l’API managée EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 1fe0b215-8340-4bc8-a6ce-4f591ca9e353
description: Découvrez comment créer et référencer une méthode de rappel de validation de certificat afin de pouvoir faire des demandes d’API managée EWS à un serveur Exchange.
localization_priority: Priority
ms.openlocfilehash: 195c51ca71890d6092e4182d23990bb528d37095
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456779"
---
# <a name="validate-a-server-certificate-for-the-ews-managed-api"></a><span data-ttu-id="32dcb-103">Valider un certificat de serveur pour l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="32dcb-103">Validate a server certificate for the EWS Managed API</span></span>

<span data-ttu-id="32dcb-104">Découvrez comment créer et référencer une méthode de rappel de validation de certificat afin de pouvoir faire des demandes d’API managée EWS à un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="32dcb-104">Learn how to create and reference a certificate validation callback method so that you can make EWS Managed API requests to an Exchange server.</span></span>
  
<span data-ttu-id="32dcb-105">Par défaut, les versions d’Exchange qui commencent par Exchange 2007 SP1 utilisent des certificats X509 auto-signés pour authentifier les appels à partir d’EWS.</span><span class="sxs-lookup"><span data-stu-id="32dcb-105">By default, versions of Exchange starting with Exchange 2007 SP1 use self-signed X509 certificates to authenticate calls from EWS.</span></span> <span data-ttu-id="32dcb-106">Lorsque vous utilisez l’API managée EWS, vous devez créer une méthode de rappel de validation de certificat ; dans le cas contraire, les demandes d’API managée EWS échouent.</span><span class="sxs-lookup"><span data-stu-id="32dcb-106">When you are using the EWS Managed API, you need to create a certificate validation callback method; otherwise, EWS Managed API requests will fail.</span></span> <span data-ttu-id="32dcb-107">Si vous utilisez le service de découverte automatique, l’appel à la méthode de découverte automatique de l’API managée EWS échouera avec une erreur **AutodiscoverLocalException** .</span><span class="sxs-lookup"><span data-stu-id="32dcb-107">If you are using the Autodiscover service, the call to the EWS Managed API Autodiscover method will fail with an **AutodiscoverLocalException** error.</span></span> <span data-ttu-id="32dcb-108">Si vous utilisez un proxy de service Web généré par le Web, vous devrez peut-être également créer une méthode de rappel de validation, en fonction de la façon dont le proxy est créé.</span><span class="sxs-lookup"><span data-stu-id="32dcb-108">If you are using a web-generated web service proxy, you might also have to create a validation callback method, depending on how the proxy is created.</span></span> 
  
## <a name="prerequisites-for-creating-a-validation-callback-method"></a><span data-ttu-id="32dcb-109">Conditions préalables à la création d’une méthode de rappel de validation</span><span class="sxs-lookup"><span data-stu-id="32dcb-109">Prerequisites for creating a validation callback method</span></span>
<span data-ttu-id="32dcb-110"><a name="bk_prereq"> </a></span><span class="sxs-lookup"><span data-stu-id="32dcb-110"><a name="bk_prereq"> </a></span></span>

<span data-ttu-id="32dcb-111">Pour configurer la validation d’un certificat de serveur, vérifiez que les conditions suivantes sont vraies :</span><span class="sxs-lookup"><span data-stu-id="32dcb-111">To set up to validate a server certificate, ensure that the following are true:</span></span> 
  
- <span data-ttu-id="32dcb-112">Votre serveur Exchange utilise un certificat auto-signé pour EWS.</span><span class="sxs-lookup"><span data-stu-id="32dcb-112">Your Exchange server is using a self-signed certificate for EWS.</span></span> <span data-ttu-id="32dcb-113">Si l’administrateur a installé un certificat valide qui effectue le suivi vers un certificat racine, il n’est pas nécessaire de créer une méthode de rappel de validation.</span><span class="sxs-lookup"><span data-stu-id="32dcb-113">If the administrator has installed a valid certificate that traces to a root certificate, you do not need to create a validation callback method.</span></span> 
    
- <span data-ttu-id="32dcb-114">Vous créez une application managée qui inclut une référence aux espaces de noms .NET Framework requis suivants :</span><span class="sxs-lookup"><span data-stu-id="32dcb-114">You are creating a managed application that includes a reference to the following required .NET Framework namespaces:</span></span> 
    
  - <span data-ttu-id="32dcb-115">**System.Net**</span><span class="sxs-lookup"><span data-stu-id="32dcb-115">**System.Net**</span></span>
  - <span data-ttu-id="32dcb-116">**System .net. Security**</span><span class="sxs-lookup"><span data-stu-id="32dcb-116">**System.Net.Security**</span></span>  
  - <span data-ttu-id="32dcb-117">**System. Security. Cryptography. X509Certificates**</span><span class="sxs-lookup"><span data-stu-id="32dcb-117">**System.Security.Cryptography.X509Certificates**</span></span>
    
## <a name="example-callback-method-to-validate-a-server-certificate-for-the-ews-managed-api"></a><span data-ttu-id="32dcb-118">Exemple : méthode de rappel pour valider un certificat de serveur pour l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="32dcb-118">Example: Callback method to validate a server certificate for the EWS Managed API</span></span>
<span data-ttu-id="32dcb-119"><a name="bk_example"> </a></span><span class="sxs-lookup"><span data-stu-id="32dcb-119"><a name="bk_example"> </a></span></span>

<span data-ttu-id="32dcb-120">L’exemple de code suivant montre comment créer une méthode de rappel de validation de certificat x509 pour l’API managée EWS.</span><span class="sxs-lookup"><span data-stu-id="32dcb-120">The following code example shows how to create an X509 certificate validation callback method for the EWS Managed API.</span></span> <span data-ttu-id="32dcb-121">Cette méthode valide un certificat x509 et renvoie uniquement la valeur true lorsque l’un des critères suivants est rempli :</span><span class="sxs-lookup"><span data-stu-id="32dcb-121">This method will validate an X509 certificate and only return true when either of the following criteria are met:</span></span> 
  
- <span data-ttu-id="32dcb-122">Le certificat est valide et effectue le suivi vers un certificat racine valide.</span><span class="sxs-lookup"><span data-stu-id="32dcb-122">The certificate is valid and traces back to a valid root certificate.</span></span>    
- <span data-ttu-id="32dcb-123">Le certificat est valide et auto-signé par le serveur qui l’a renvoyé.</span><span class="sxs-lookup"><span data-stu-id="32dcb-123">The certificate is valid and is self-signed by the server that returned it.</span></span> 
    
> [!IMPORTANT]
> <span data-ttu-id="32dcb-124">La méthode de rappel de validation de certificat dans cet exemple offre une sécurité suffisante pour le développement et le test des applications d’API managée EWS.</span><span class="sxs-lookup"><span data-stu-id="32dcb-124">The certificate validation callback method in this example provides sufficient security for development and testing of EWS Managed API applications.</span></span> <span data-ttu-id="32dcb-125">Toutefois, il peut ne pas fournir une sécurité suffisante pour votre application déployée.</span><span class="sxs-lookup"><span data-stu-id="32dcb-125">However, it might not provide sufficient security for your deployed application.</span></span> <span data-ttu-id="32dcb-126">Vous devez toujours vous assurer que la méthode de rappel de validation de certificat que vous utilisez répond aux exigences de sécurité de votre organisation.</span><span class="sxs-lookup"><span data-stu-id="32dcb-126">You should always make sure that the certificate validation callback method that you use meets the security requirements of your organization.</span></span> 
  
```cs
      private static bool CertificateValidationCallBack(
         object sender,
         System.Security.Cryptography.X509Certificates.X509Certificate certificate,
         System.Security.Cryptography.X509Certificates.X509Chain chain,
         System.Net.Security.SslPolicyErrors sslPolicyErrors)
    {
      // If the certificate is a valid, signed certificate, return true.
      if (sslPolicyErrors == System.Net.Security.SslPolicyErrors.None)
      {
        return true;
      }
      // If there are errors in the certificate chain, look at each error to determine the cause.
      if ((sslPolicyErrors &amp; System.Net.Security.SslPolicyErrors.RemoteCertificateChainErrors) != 0)
      {
        if (chain != null &amp;&amp; chain.ChainStatus != null)
        {
          foreach (System.Security.Cryptography.X509Certificates.X509ChainStatus status in chain.ChainStatus)
          {
            if ((certificate.Subject == certificate.Issuer) &amp;&amp;
               (status.Status == System.Security.Cryptography.X509Certificates.X509ChainStatusFlags.UntrustedRoot))
            {
              // Self-signed certificates with an untrusted root are valid. 
              continue;
            }
            else
            {
              if (status.Status != System.Security.Cryptography.X509Certificates.X509ChainStatusFlags.NoError)
              {
                // If there are any other errors in the certificate chain, the certificate is invalid,
             // so the method returns false.
                return false;
              }
            }
          }
        }
        // When processing reaches this line, the only errors in the certificate chain are 
    // untrusted root errors for self-signed certificates. These certificates are valid
    // for default Exchange server installations, so return true.
        return true;
      }
      else
      {
     // In all other cases, return false.
        return false;
      }
    }

```

<span data-ttu-id="32dcb-127">Vous utilisez la classe **ServicePointManager** dans l’espace de noms **System.net** .net pour raccorder une méthode de rappel de validation en définissant la propriété **ServerCertificateValidationCallback** .</span><span class="sxs-lookup"><span data-stu-id="32dcb-127">You use the **ServicePointManager** class in the .NET **System.Net** namespace to hook up a validation callback method by setting the **ServerCertificateValidationCallback** property.</span></span> <span data-ttu-id="32dcb-128">Vous pouvez utiliser un code semblable à l’exemple de code suivant pour définir la propriété **ServerCertificateValidationCallback** .</span><span class="sxs-lookup"><span data-stu-id="32dcb-128">You can use code similar to the following code example to set the **ServerCertificateValidationCallback** property.</span></span> 
  
```cs
ServicePointManager.ServerCertificateValidationCallback = CertificateValidationCallBack;

```

## <a name="next-steps"></a><span data-ttu-id="32dcb-129">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="32dcb-129">Next steps</span></span>
<span data-ttu-id="32dcb-130"><a name="bk_example"> </a></span><span class="sxs-lookup"><span data-stu-id="32dcb-130"><a name="bk_example"> </a></span></span>

<span data-ttu-id="32dcb-131">Une fois que vous avez créé la méthode de rappel de validation pour l’API managée EWS, vous pouvez utiliser le service de découverte automatique pour obtenir les points de connexion et les paramètres utilisateur et de domaine à partir d’un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="32dcb-131">After you have created the validation callback method for the EWS Managed API, you can use the Autodiscover service to get connection points and user and domain settings from an Exchange server.</span></span> <span data-ttu-id="32dcb-132">Pour plus d’informations, voir les articles suivants :</span><span class="sxs-lookup"><span data-stu-id="32dcb-132">For more information, see the following articles:</span></span>
  
- [<span data-ttu-id="32dcb-133">Utiliser la découverte automatique pour trouver des points de connexion</span><span class="sxs-lookup"><span data-stu-id="32dcb-133">Use Autodiscover to find connection points</span></span>](how-to-use-autodiscover-to-find-connection-points.md)
    
- [<span data-ttu-id="32dcb-134">Obtenir les paramètres de l'utilisateur Exchange à l'aide de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="32dcb-134">Get user settings from Exchange by using Autodiscover</span></span>](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)
    
- [<span data-ttu-id="32dcb-135">Obtenir des paramètres de domaine à partir d’un serveur Exchange</span><span class="sxs-lookup"><span data-stu-id="32dcb-135">Get domain settings from an Exchange server</span></span>](how-to-get-domain-settings-from-an-exchange-server.md)
    
## <a name="see-also"></a><span data-ttu-id="32dcb-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="32dcb-136">See also</span></span>

- [<span data-ttu-id="32dcb-137">Configuration de votre application EWS</span><span class="sxs-lookup"><span data-stu-id="32dcb-137">Setting up your EWS application</span></span>](setting-up-your-ews-application.md)  
- [<span data-ttu-id="32dcb-138">Commencer à utiliser les services web dans Exchange</span><span class="sxs-lookup"><span data-stu-id="32dcb-138">Start using web services in Exchange</span></span>](start-using-web-services-in-exchange.md)
    

