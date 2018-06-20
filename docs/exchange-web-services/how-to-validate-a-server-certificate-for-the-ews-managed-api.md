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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19754951"
---
# <a name="validate-a-server-certificate-for-the-ews-managed-api"></a>Valider un certificat de serveur pour l’API managée EWS

Découvrez comment créer et faire référence à une méthode de rappel de validation de certificat afin que vous pouvez effectuer des demandes d’API managées à un serveur Exchange.
  
Par défaut, les versions d’Exchange commençant par Exchange 2007 SP1 utilisent X509 signé automatiquement des certificats pour authentifier les appels EWS. Lorsque vous utilisez l’API managée EWS, vous devez créer une méthode de rappel de validation de certificat ; dans le cas contraire, les demandes d’API managées échouera. Si vous utilisez le service de découverte automatique, l’appel à la méthode Autodiscover des API gérée EWS échoue avec une erreur **AutodiscoverLocalException** . Si vous utilisez un proxy de service web généré par le web, vous devrez également créer une méthode de rappel de validation, selon la façon dont le serveur proxy est créé. 
  
## <a name="prerequisites-for-creating-a-validation-callback-method"></a>Conditions requises pour créer une méthode de rappel de validation
<a name="bk_prereq"> </a>

Pour configurer pour valider un certificat de serveur, assurez-vous que les conditions suivantes sont remplies : 
  
- Votre serveur Exchange utilise un certificat auto-signé pour EWS. Si l’administrateur a installé un certificat valide qui authentifie à un certificat racine, il est inutile créer une méthode de rappel de validation. 
    
- Vous créez une application managée qui inclut une référence à l’espace de noms .NET Framework requises suivantes : 
    
  - **System.Net**
  - **System.Net.Security**  
  - **System.Security.Cryptography.X509Certificates**
    
## <a name="example-callback-method-to-validate-a-server-certificate-for-the-ews-managed-api"></a>Exemple : De méthode de rappel pour valider un certificat de serveur pour l’API managée EWS
<a name="bk_example"> </a>

L’exemple de code suivant montre comment créer un X509 méthode de rappel de validation de certificat pour l’API managée EWS. Cette méthode est validée un X509 du certificat et retourne true uniquement si un des critères suivants sont remplie : 
  
- Le certificat est valide et traces retour à un certificat racine valide.    
- Le certificat est valide et est auto-signé par le serveur qui a renvoyé. 
    
> [!IMPORTANT]
> La méthode de rappel de validation de certificat dans cet exemple fournit une sécurité suffisante pour le développement et le test des applications d’API managées. Toutefois, il ne peut pas fournir une sécurité suffisante pour votre application déployée. Vous assurer que la méthode de rappel de validation de certificat que vous utilisez répond aux exigences de sécurité de votre organisation. 
  
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

Vous utilisez la classe **ServicePointManager** dans l’espace de noms .NET **System.Net** pour connecter une méthode de rappel de validation en définissant la propriété **ServerCertificateValidationCallback** . Vous pouvez utiliser le code similaire à l’exemple de code suivant pour définir la propriété **ServerCertificateValidationCallback** . 
  
```cs
ServicePointManager.ServerCertificateValidationCallback = CertificateValidationCallBack;

```

## <a name="next-steps"></a>Étapes suivantes
<a name="bk_example"> </a>

Une fois que vous avez créé la méthode de rappel de validation pour l’API managée EWS, vous pouvez utiliser le service de découverte automatique pour obtenir des points de connexion et les utilisateurs et les paramètres de domaine à partir d’un serveur Exchange. Pour plus d’informations, voir les articles suivants :
  
- [Utiliser la découverte automatique pour rechercher les points de connexion](how-to-use-autodiscover-to-find-connection-points.md)
    
- [Obtenir les paramètres de l’utilisateur Exchange à l’aide de découverte automatique](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)
    
- [Obtenir les paramètres de domaine à partir d’un serveur Exchange](how-to-get-domain-settings-from-an-exchange-server.md)
    
## <a name="see-also"></a>Voir aussi

- [La configuration de vos applications EWS](setting-up-your-ews-application.md)  
- [Commencer à utiliser les services web dans Exchange](start-using-web-services-in-exchange.md)
    

