---
title: Outils et ressources pour la résolution des problèmes des applications EWS pour Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.assetid: ee7fcd05-35d7-47bf-bac4-e719c49c11fe
description: Trouvez des ressources pour vous aider à résoudre les problèmes de votre API gérée EWS ou de votre application EWS.
localization_priority: Priority
ms.openlocfilehash: 8a65b06cf911cd033d7fe5fe1b4566a7496de784
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542581"
---
# <a name="tools-and-resources-for-troubleshooting-ews-applications-for-exchange"></a>Outils et ressources pour la résolution des problèmes des applications EWS pour Exchange

Trouvez des ressources pour vous aider à résoudre les problèmes de votre API gérée EWS ou de votre application EWS.
  
Les choses ne se passent pas toujours comme prévu. Parfois, les demandes EWS échouent ou fournissent des résultats inattendus. Cela peut être frustrant, surtout si la raison n’est pas évidente. Nous espérons que cela ne vous arrive jamais, mais si c’est le cas, cet article fournit des informations sur les outils et les ressources que vous pouvez utiliser pour vous aider à résoudre votre problème.
  
> [!NOTE]
> Cet article fournit des conseils généraux de résolution des problèmes et des sources d’informations de résolution de problèmes. Malheureusement, il n’est pas possible de fournir des étapes détaillées de résolution des problèmes. Pour obtenir de l’aide pour résoudre votre erreur spécifique, consultez [Étapes suivantes](#bk_NextSteps). 
  
## <a name="examine-the-soap-requests-and-responses"></a>Examiner les requêtes et réponses SOAP

Lorsque les choses ne fonctionnent pas correctement, il est vraiment utile de voir ce qui se passe. La première ligne de requête lors de l’examen d’un problème avec EWS ou l’API gérée EWS consiste à examiner les demandes que votre application envoie sur le réseau et les réponses que le serveur renvoie.
  
L’API gérée EWS facilite l’examen des requêtes et des réponses SOAP grâce à sa [fonctionnalité intégrée de suivi](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md). Si vous utilisez EWS, vous pouvez avoir ou non accès à des fonctionnalités de suivi similaires, selon la plateforme ou les classes que vous utilisez pour envoyer vos demandes. Toutefois, vous pouvez toujours utiliser un outil de suivi réseau tel que [Moniteur réseau](https://www.microsoft.com/download/details.aspx?id=4865) ou [Fiddler](http://www.telerik.com/fiddler) pour examiner le trafic réseau et afficher les charges utiles de demande et de réponse. 
  
En outre, vous pouvez [instrumenter les demandes de votre client](instrumenting-client-requests-for-ews-and-rest-in-exchange.md) pour améliorer les informations disponibles dans les demandes et les réponses. 
  
Une fois que vous avez les demandes et les réponses, demandez-vous ce qui suit : sont-elles correctes ? Les valeurs que votre application envoie sont-elles attendues ? Les réponses sont-ils logiques ?
  
## <a name="examine-error-codes"></a>Examiner les codes d’erreur

Parfois, le code d’erreur peut aller beaucoup plus loin dans la localisation du problème, même si, d’un coup d’œil, il semble peu logique. L’erreur indique-t-elle que votre client est [en cours de limitation](ews-throttling-in-exchange.md) ? Un appel à la découverte automatique pour [actualiser les informations de configuration](how-to-refresh-configuration-information-by-using-autodiscover.md) est-il peut-être à prendre en compte ? 
  
Pour plus d’informations sur le traitement des erreurs spécifiques, consultez les articles suivants :
  
- [Gestion des messages d'erreur de découverte automatique](handling-autodiscover-error-messages.md)
    
- [Gestion des erreurs liées à la notification dans EWS dans Exchange](handling-notification-related-errors-in-ews-in-exchange.md)
    
- [Gestion des erreurs liées à la synchronisation dans EWS dans Exchange](handling-synchronization-related-errors-in-ews-in-exchange.md)
    
- [Gestion des erreurs liées à la suppression dans EWS dans Exchange](handling-deletion-related-errors-in-ews-in-exchange.md)
    
## <a name="verify-versions"></a>Vérifier les versions

Plusieurs composants sont impliqués dans les opérations EWS et les versions de ces composants peuvent influencer les résultats.
  
**Tableau 1. Composants avec version qui peuvent affecter les processus EWS**

|**Composant**|**API managée par EWS**|**EWS**|**Notes**|
|:-----|:-----|:-----|:-----|
|Version du serveur demandée  <br/> |Propriété [ExchangeServiceBase.RequestedServerVersion](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.requestedserverversion%28v=exchg.80%29.aspx)  <br/> |Élément [RequestServerVersion](https://msdn.microsoft.com/library/af4032d5-42b3-463e-9d0a-8236d78e5b75%28Office.15%29.aspx)  <br/> |Cette valeur contrôle la version du schéma EWS utilisée pour traiter la demande EWS. Assurez-vous que la version de schéma spécifiée ici est logique pour la demande que vous envoyez. Certaines propriétés et opérations ne sont pas disponibles dans les versions antérieures du schéma.  <br/> |
|Version du serveur  <br/> |Propriété [ExchangeServiceBase.ServerInfo](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.serverinfo%28v=exchg.80%29.aspx)  <br/> |Élément [ServerVersionInfo](https://msdn.microsoft.com/library/c04a6872-ca27-432b-aac2-36b023d0afc6%28Office.15%29.aspx)  <br/> |Cette valeur est renvoyée par le serveur dans les réponses EWS et indique la version du serveur qui a traitée la réponse. Vérifiez que cette valeur est celle que vous attendez. Si possible, assurez-vous que le serveur Exchange exécute la mise à jour la plus récente pour votre version principale de Exchange.  <br/> |
|Version d’API managée par EWS  <br/> |Propriété de version de produit du fichier Microsoft.Exchange.WebServices.dll de données.  <br/> |Non applicable  <br/> |Si vous utilisez l’API gérée EWS, assurez-vous que vous utilisez [la version la plus récente](https://aka.ms/ews-managed-api-readme).  <br/> |
   
## <a name="verify-access"></a>Vérifier l’accès

EWS est activé par défaut, mais les valeurs par défaut [peuvent être modifiées](how-to-control-access-to-ews-in-exchange.md). Utilisez la cmdlet [Get-OrganizationConfig](https://technet.microsoft.com/library/bb124754.aspx) pour vous assurer qu’EWS est activé sur le serveur et la cmdlet [Get-CASMailbox](https://technet.microsoft.com/library/aa997571.aspx) pour vous assurer que EWS est activé pour la boîte aux lettres de l’utilisateur. Vérifiez également les deux réponses de cmdlet pour une liste autoriser ou bloquer d’EWS, et assurez-vous que votre application n’est pas bloquée pour utiliser EWS. 
  
Vous devez également vérifier que les [paramètres d’authentification par défaut](https://technet.microsoft.com/library/gg247612%28v=exchg.150%29.aspx) sur le répertoire virtuel EWS n’ont pas été modifiés. 
  
## <a name="try-another-ews-client"></a>Essayer un autre client EWS

Parfois, il est utile d’essayer la même demande à partir d’un autre client et de comparer les résultats. Si un autre client obtient des résultats différents, qu’est-ce qui est différent ? Déterminer ce qui est différent entre une demande réussie et une demande ayant échoué peut aider à expliquer pourquoi une demande particulière échoue.
  
Même si vous pouvez certainement écrire un autre client pour le test, vous n’en avez pas besoin ! [EWSEditor](http://ewseditor.codeplex.com/) est un exemple de client qui utilise l’API gérée EWS et EWS. Vous pouvez télécharger le client (y compris le code source) et l’utiliser pour essayer les mêmes demandes qui échouent dans votre application. 
  
## <a name="examine-iis-logs"></a>Examiner les journaux IIS

Si vous avez accès au serveur Exchange, la fonctionnalité de journalisation fournie par Internet Information Services (IIS) sur les serveurs d’accès au client peut fournir plus d’informations sur les défaillances. Toutefois, gardez à l’esprit que les journaux IIS ne seront utiles que si vous recevez une erreur HTTP.
  
IIS fournit deux méthodes de journalisation différentes : la [journalisation IIS](http://www.iis.net/learn/manage/provisioning-and-managing-iis/configure-logging-in-iis) et le [suivi des demandes qui ont échoué](http://www.iis.net/learn/troubleshoot/using-failed-request-tracing/troubleshooting-failed-requests-using-tracing-in-iis). Pour utiliser les journaux IIS, vous pouvez utiliser [Log Parser Studio](https://blogs.technet.com/b/exchange/archive/2012/03/07/introducing-log-parser-studio.aspx) qui inclut un certain nombre de requêtes EWS intégrées.
  
## <a name="next-steps"></a>Étapes suivantes
<a name="bk_NextSteps"> </a>

Maintenant que vous avez découvert les outils et les ressources que vous pouvez utiliser pour résoudre les problèmes, vous aurez peut-être besoin d’aide pour comprendre les informations fournies par ces outils. Voici quelques options pour obtenir de l’aide :
  
- [Forum Développement Exchange Server sur MSDN](https://social.msdn.microsoft.com/Forums/home?category=exchangeserver) : Posez une question à la communauté de développement MSDN Exchange Server. 
    
- [StackOverflow](http://stackoverflow.com/tags/ews) : posez une question de la communauté StackOverflow. N’oubliez pas de marquer votre billet avec « ews ». 
    
- [Support Microsoft :](https://support.microsoft.com/ph/730/en-us) contactez un professionnel du support Microsoft pour obtenir de l’aide. 
    
## <a name="see-also"></a>Voir aussi


Consultez les articles suivants :
  
- [Développer des clients de service web pour Exchange](develop-web-service-clients-for-exchange.md)
    
- [Suivi des demandes et des réponses pour dépanner les applications API managées EWS](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md)
    
- [Instrumentation des demandes de client pour EWS et REST dans Exchange](instrumenting-client-requests-for-ews-and-rest-in-exchange.md)
    
- [Limitation EWS dans Exchange](ews-throttling-in-exchange.md)
    
- [Actualiser les informations de configuration à l’aide de la découverte automatique](how-to-refresh-configuration-information-by-using-autodiscover.md)
    
- [Gestion des messages d'erreur de découverte automatique](handling-autodiscover-error-messages.md)
    
- [Gestion des erreurs liées à la notification dans EWS dans Exchange](handling-notification-related-errors-in-ews-in-exchange.md)
    
- [Gestion des erreurs liées à la synchronisation dans EWS dans Exchange](handling-synchronization-related-errors-in-ews-in-exchange.md)
    
- [Gestion des erreurs liées à la suppression dans EWS dans Exchange](handling-deletion-related-errors-in-ews-in-exchange.md)
    
- [Configuration de la journalisation dans IIS](http://www.iis.net/learn/manage/provisioning-and-managing-iis/configure-logging-in-iis)
    
- [Résolution des problèmes de demandes échouées à l’aide du suivi dans IIS 7](http://www.iis.net/learn/troubleshoot/using-failed-request-tracing/troubleshooting-failed-requests-using-tracing-in-iis)
    
- [Présentation : Log Parser Studio](https://blogs.technet.com/b/exchange/archive/2012/03/07/introducing-log-parser-studio.aspx)
    
- [Paramètres par défaut pour les répertoires virtuels Exchange](https://technet.microsoft.com/library/gg247612%28v=exchg.150%29.aspx)
    
Téléchargez ce qui suit :
  
- [Moniteur réseau Microsoft 3.4](https://www.microsoft.com/download/details.aspx?id=4865)
    
- [Fiddler](http://www.telerik.com/fiddler)
    
- [EWSEditor](http://ewseditor.codeplex.com/)
    
- [API gérée services web Exchange](https://www.nuget.org/packages/Microsoft.Exchange.WebServices/)
