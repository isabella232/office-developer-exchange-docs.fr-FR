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
# <a name="validate-a-server-certificate-for-the-ews-managed-api"></a>Valider un certificat de serveur pour l’API managée EWS

Découvrez comment créer et référencer une méthode de rappel de validation de certificat afin de pouvoir faire des demandes d’API managée EWS à un serveur Exchange.
  
Par défaut, les versions d’Exchange qui commencent par Exchange 2007 SP1 utilisent des certificats X509 auto-signés pour authentifier les appels à partir d’EWS. Lorsque vous utilisez l’API managée EWS, vous devez créer une méthode de rappel de validation de certificat ; dans le cas contraire, les demandes d’API managée EWS échouent. Si vous utilisez le service de découverte automatique, l’appel à la méthode de découverte automatique de l’API managée EWS échouera avec une erreur **AutodiscoverLocalException** . Si vous utilisez un proxy de service Web généré par le Web, vous devrez peut-être également créer une méthode de rappel de validation, en fonction de la façon dont le proxy est créé. 
  
## <a name="prerequisites-for-creating-a-validation-callback-method"></a>Conditions préalables à la création d’une méthode de rappel de validation
<a name="bk_prereq"> </a>

Pour configurer la validation d’un certificat de serveur, vérifiez que les conditions suivantes sont vraies : 
  
- Votre serveur Exchange utilise un certificat auto-signé pour EWS. Si l’administrateur a installé un certificat valide qui effectue le suivi vers un certificat racine, il n’est pas nécessaire de créer une méthode de rappel de validation. 
    
- Vous créez une application managée qui inclut une référence aux espaces de noms .NET Framework requis suivants : 
    
  - **System.Net**
  - **System .net. Security**  
  - **System. Security. Cryptography. X509Certificates**
    
## <a name="example-callback-method-to-validate-a-server-certificate-for-the-ews-managed-api"></a>Exemple : méthode de rappel pour valider un certificat de serveur pour l’API managée EWS
<a name="bk_example"> </a>

L’exemple de code suivant montre comment créer une méthode de rappel de validation de certificat x509 pour l’API managée EWS. Cette méthode valide un certificat x509 et renvoie uniquement la valeur true lorsque l’un des critères suivants est rempli : 
  
- Le certificat est valide et effectue le suivi vers un certificat racine valide.    
- Le certificat est valide et auto-signé par le serveur qui l’a renvoyé. 
    
> [!IMPORTANT]
> La méthode de rappel de validation de certificat dans cet exemple offre une sécurité suffisante pour le développement et le test des applications d’API managée EWS. Toutefois, il peut ne pas fournir une sécurité suffisante pour votre application déployée. Vous devez toujours vous assurer que la méthode de rappel de validation de certificat que vous utilisez répond aux exigences de sécurité de votre organisation. 
  
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

Vous utilisez la classe **ServicePointManager** dans l’espace de noms **System.net** .net pour raccorder une méthode de rappel de validation en définissant la propriété **ServerCertificateValidationCallback** . Vous pouvez utiliser un code semblable à l’exemple de code suivant pour définir la propriété **ServerCertificateValidationCallback** . 
  
```cs
ServicePointManager.ServerCertificateValidationCallback = CertificateValidationCallBack;

```

## <a name="next-steps"></a>Étapes suivantes
<a name="bk_example"> </a>

Une fois que vous avez créé la méthode de rappel de validation pour l’API managée EWS, vous pouvez utiliser le service de découverte automatique pour obtenir les points de connexion et les paramètres utilisateur et de domaine à partir d’un serveur Exchange. Pour plus d’informations, voir les articles suivants :
  
- [Utiliser la découverte automatique pour trouver des points de connexion](how-to-use-autodiscover-to-find-connection-points.md)
    
- [Obtenir les paramètres de l'utilisateur Exchange à l'aide de découverte automatique](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)
    
- [Obtenir des paramètres de domaine à partir d’un serveur Exchange](how-to-get-domain-settings-from-an-exchange-server.md)
    
## <a name="see-also"></a>Voir aussi

- [Configuration de votre application EWS](setting-up-your-ews-application.md)  
- [Commencer à utiliser les services web dans Exchange](start-using-web-services-in-exchange.md)
    

