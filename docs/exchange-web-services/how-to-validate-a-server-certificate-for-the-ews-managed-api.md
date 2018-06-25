---
title: Valider un certificat de serveur pour l’API managée EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 1fe0b215-8340-4bc8-a6ce-4f591ca9e353
description: Découvrez comment créer et faire référence à une méthode de rappel de validation de certificat afin que vous pouvez effectuer des demandes d’API managées à un serveur Exchange.
ms.openlocfilehash: 13d7c51e55308b9e9997697a075c8a9e6b4f10d0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754951"
---
# <a name="validate-a-server-certificate-for-the-ews-managed-api"></a><span data-ttu-id="10213-103">Valider un certificat de serveur pour l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="10213-103">Validate a server certificate for the EWS Managed API</span></span>

<span data-ttu-id="10213-104">Découvrez comment créer et faire référence à une méthode de rappel de validation de certificat afin que vous pouvez effectuer des demandes d’API managées à un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="10213-104">Learn how to create and reference a certificate validation callback method so that you can make EWS Managed API requests to an Exchange server.</span></span>
  
<span data-ttu-id="10213-105">Par défaut, les versions d’Exchange commençant par Exchange 2007 SP1 utilisent X509 signé automatiquement des certificats pour authentifier les appels EWS.</span><span class="sxs-lookup"><span data-stu-id="10213-105">By default, versions of Exchange starting with Exchange 2007 SP1 use self-signed X509 certificates to authenticate calls from EWS.</span></span> <span data-ttu-id="10213-106">Lorsque vous utilisez l’API managée EWS, vous devez créer une méthode de rappel de validation de certificat ; dans le cas contraire, les demandes d’API managées échouera.</span><span class="sxs-lookup"><span data-stu-id="10213-106">When you are using the EWS Managed API, you need to create a certificate validation callback method; otherwise, EWS Managed API requests will fail.</span></span> <span data-ttu-id="10213-107">Si vous utilisez le service de découverte automatique, l’appel à la méthode Autodiscover des API gérée EWS échoue avec une erreur **AutodiscoverLocalException** .</span><span class="sxs-lookup"><span data-stu-id="10213-107">If you are using the Autodiscover service, the call to the EWS Managed API Autodiscover method will fail with an **AutodiscoverLocalException** error.</span></span> <span data-ttu-id="10213-108">Si vous utilisez un proxy de service web généré par le web, vous devrez également créer une méthode de rappel de validation, selon la façon dont le serveur proxy est créé.</span><span class="sxs-lookup"><span data-stu-id="10213-108">If you are using a web-generated web service proxy, you might also have to create a validation callback method, depending on how the proxy is created.</span></span> 
  
## <a name="prerequisites-for-creating-a-validation-callback-method"></a><span data-ttu-id="10213-109">Conditions requises pour créer une méthode de rappel de validation</span><span class="sxs-lookup"><span data-stu-id="10213-109">Prerequisites for creating a validation callback method</span></span>
<span data-ttu-id="10213-110"><a name="bk_prereq"> </a></span><span class="sxs-lookup"><span data-stu-id="10213-110"></span></span>

<span data-ttu-id="10213-111">Pour configurer pour valider un certificat de serveur, assurez-vous que les conditions suivantes sont remplies :</span><span class="sxs-lookup"><span data-stu-id="10213-111">To set up to validate a server certificate, ensure that the following are true:</span></span> 
  
- <span data-ttu-id="10213-112">Votre serveur Exchange utilise un certificat auto-signé pour EWS.</span><span class="sxs-lookup"><span data-stu-id="10213-112">Your Exchange server is using a self-signed certificate for EWS.</span></span> <span data-ttu-id="10213-113">Si l’administrateur a installé un certificat valide qui authentifie à un certificat racine, il est inutile créer une méthode de rappel de validation.</span><span class="sxs-lookup"><span data-stu-id="10213-113">If the administrator has installed a valid certificate that traces to a root certificate, you do not need to create a validation callback method.</span></span> 
    
- <span data-ttu-id="10213-114">Vous créez une application managée qui inclut une référence à l’espace de noms .NET Framework requises suivantes :</span><span class="sxs-lookup"><span data-stu-id="10213-114">You are creating a managed application that includes a reference to the following required .NET Framework namespaces:</span></span> 
    
  - <span data-ttu-id="10213-115">**System.Net**</span><span class="sxs-lookup"><span data-stu-id="10213-115">**System.Net**</span></span>
  - <span data-ttu-id="10213-116">**System.Net.Security**</span><span class="sxs-lookup"><span data-stu-id="10213-116">**System.Net.Security**</span></span>  
  - <span data-ttu-id="10213-117">**System.Security.Cryptography.X509Certificates**</span><span class="sxs-lookup"><span data-stu-id="10213-117">**System.Security.Cryptography.X509Certificates**</span></span>
    
## <a name="example-callback-method-to-validate-a-server-certificate-for-the-ews-managed-api"></a><span data-ttu-id="10213-118">Exemple : De méthode de rappel pour valider un certificat de serveur pour l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="10213-118">Example: Callback method to validate a server certificate for the EWS Managed API</span></span>
<span data-ttu-id="10213-119"><a name="bk_example"> </a></span><span class="sxs-lookup"><span data-stu-id="10213-119"></span></span>

<span data-ttu-id="10213-120">L’exemple de code suivant montre comment créer un X509 méthode de rappel de validation de certificat pour l’API managée EWS.</span><span class="sxs-lookup"><span data-stu-id="10213-120">The following code example shows how to create an X509 certificate validation callback method for the EWS Managed API.</span></span> <span data-ttu-id="10213-121">Cette méthode est validée un X509 du certificat et retourne true uniquement si un des critères suivants sont remplie :</span><span class="sxs-lookup"><span data-stu-id="10213-121">This method will validate an X509 certificate and only return true when either of the following criteria are met:</span></span> 
  
- <span data-ttu-id="10213-122">Le certificat est valide et traces retour à un certificat racine valide.</span><span class="sxs-lookup"><span data-stu-id="10213-122">The certificate is valid and traces back to a valid root certificate.</span></span>    
- <span data-ttu-id="10213-123">Le certificat est valide et est auto-signé par le serveur qui a renvoyé.</span><span class="sxs-lookup"><span data-stu-id="10213-123">The certificate is valid and is self-signed by the server that returned it.</span></span> 
    
> [!IMPORTANT]
> <span data-ttu-id="10213-124">La méthode de rappel de validation de certificat dans cet exemple fournit une sécurité suffisante pour le développement et le test des applications d’API managées.</span><span class="sxs-lookup"><span data-stu-id="10213-124">The certificate validation callback method in this example provides sufficient security for development and testing of EWS Managed API applications.</span></span> <span data-ttu-id="10213-125">Toutefois, il ne peut pas fournir une sécurité suffisante pour votre application déployée.</span><span class="sxs-lookup"><span data-stu-id="10213-125">However, it might not provide sufficient security for your deployed application.</span></span> <span data-ttu-id="10213-126">Vous assurer que la méthode de rappel de validation de certificat que vous utilisez répond aux exigences de sécurité de votre organisation.</span><span class="sxs-lookup"><span data-stu-id="10213-126">You should always make sure that the certificate validation callback method that you use meets the security requirements of your organization.</span></span> 
  
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

<span data-ttu-id="10213-127">Vous utilisez la classe **ServicePointManager** dans l’espace de noms .NET **System.Net** pour connecter une méthode de rappel de validation en définissant la propriété **ServerCertificateValidationCallback** .</span><span class="sxs-lookup"><span data-stu-id="10213-127">You use the **ServicePointManager** class in the .NET **System.Net** namespace to hook up a validation callback method by setting the **ServerCertificateValidationCallback** property.</span></span> <span data-ttu-id="10213-128">Vous pouvez utiliser le code similaire à l’exemple de code suivant pour définir la propriété **ServerCertificateValidationCallback** .</span><span class="sxs-lookup"><span data-stu-id="10213-128">You can use code similar to the following code example to set the **ServerCertificateValidationCallback** property.</span></span> 
  
```cs
ServicePointManager.ServerCertificateValidationCallback = CertificateValidationCallBack;

```

## <a name="next-steps"></a><span data-ttu-id="10213-129">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="10213-129">Next steps</span></span>
<span data-ttu-id="10213-130"><a name="bk_example"> </a></span><span class="sxs-lookup"><span data-stu-id="10213-130"></span></span>

<span data-ttu-id="10213-131">Une fois que vous avez créé la méthode de rappel de validation pour l’API managée EWS, vous pouvez utiliser le service de découverte automatique pour obtenir des points de connexion et les utilisateurs et les paramètres de domaine à partir d’un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="10213-131">After you have created the validation callback method for the EWS Managed API, you can use the Autodiscover service to get connection points and user and domain settings from an Exchange server.</span></span> <span data-ttu-id="10213-132">Pour plus d’informations, voir les articles suivants :</span><span class="sxs-lookup"><span data-stu-id="10213-132">For more information, see the following articles:</span></span>
  
- [<span data-ttu-id="10213-133">Utiliser la découverte automatique pour rechercher les points de connexion</span><span class="sxs-lookup"><span data-stu-id="10213-133">Use Autodiscover to find connection points</span></span>](how-to-use-autodiscover-to-find-connection-points.md)
    
- [<span data-ttu-id="10213-134">Obtenir les paramètres de l’utilisateur Exchange à l’aide de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="10213-134">Get user settings from Exchange by using Autodiscover</span></span>](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)
    
- [<span data-ttu-id="10213-135">Obtenir les paramètres de domaine à partir d’un serveur Exchange</span><span class="sxs-lookup"><span data-stu-id="10213-135">Get domain settings from an Exchange server</span></span>](how-to-get-domain-settings-from-an-exchange-server.md)
    
## <a name="see-also"></a><span data-ttu-id="10213-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="10213-136">See also</span></span>

- [<span data-ttu-id="10213-137">La configuration de vos applications EWS</span><span class="sxs-lookup"><span data-stu-id="10213-137">Setting up your EWS application</span></span>](setting-up-your-ews-application.md)  
- [<span data-ttu-id="10213-138">Commencer à utiliser les services web dans Exchange</span><span class="sxs-lookup"><span data-stu-id="10213-138">Start using web services in Exchange</span></span>](start-using-web-services-in-exchange.md)
    

