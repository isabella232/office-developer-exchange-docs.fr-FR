---
title: Outils et ressources pour la résolution des problèmes des applications EWS pour Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: ee7fcd05-35d7-47bf-bac4-e719c49c11fe
description: Trouvez des ressources pour vous aider à résoudre les problèmes des applications EWS API managées.
ms.openlocfilehash: d8d8ea736ca3b896642ad06f5987caeba8d8d059
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755073"
---
# <a name="tools-and-resources-for-troubleshooting-ews-applications-for-exchange"></a>Outils et ressources pour la résolution des problèmes des applications EWS pour Exchange

Trouvez des ressources pour vous aider à résoudre les problèmes des applications EWS API managées.
  
Éléments ne se déroule pas comme prévu. Parfois EWS demande échoue ou fournir des résultats inattendus. Cela peut être frustrant, surtout si la raison n’est pas évidente. J’espère que cela vous arrivera jamais, mais dans ce cas, cet article fournit des informations sur les outils et les ressources que vous pouvez utiliser pour aider à résoudre le problème.
  
> [!NOTE]
> Cet article fournit des conseils de résolution des problèmes généraux et les sources des informations de dépannage. Malheureusement il n’est pas possible d’attribuer des étapes de dépannage détaillées. Pour obtenir une assistance dépannage votre erreur spécifique, voir les [étapes suivantes](#bk_NextSteps). 
  
## <a name="examine-the-soap-requests-and-responses"></a>Examiner les demandes et réponses SOAP

Lorsque les choses ne fonctionnent pas correctement, il est très utile pour être en mesure de voir ce qui se passe. La première ligne de la recherche lorsque vous recherchez un problème avec EWS ou l’API managée EWS consiste à examiner les demandes de l’envoi de votre application sur le réseau et les réponses que le serveur envoie précédent.
  
L’API managée EWS facilite examen demandes et réponses SOAP avec son [intégré dans la fonctionnalité de suivi](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md). Si vous utilisez EWS, vous pouvez ou n’aurez pas accès à une fonctionnalité similaire suivi, en fonction de quel plateforme ou les classes qui vous permet d’envoyer vos demandes. Toutefois, vous pouvez toujours utiliser un outil de suivi réseau comme [Moniteur réseau](http://www.microsoft.com/en-us/download/details.aspx?id=4865) ou [Fiddler](http://www.telerik.com/fiddler) examiner le trafic réseau et d’afficher les charges de demande et de réponse. 
  
En outre, vous pouvez [instrument vos requêtes client](instrumenting-client-requests-for-ews-and-rest-in-exchange.md) afin d’améliorer les informations disponibles dans les demandes et réponses. 
  
Une fois que vous avez les demandes et les réponses, posez-vous les éléments suivants : font elles semblent correctes ? Sont les valeurs que votre application envoie attendue ? Les réponses ont sens ?
  
## <a name="examine-error-codes"></a>Examinez les codes d’erreur

Le code d’erreur peuvent-ils parfois permettent de localiser le problème, même si au premier coup de œil cela ne semble pas pertinent. L’erreur indique que votre client est [limitée](ews-throttling-in-exchange.md)? Un appel à la découverte automatique pour [Actualiser les informations de configuration](how-to-refresh-configuration-information-by-using-autodiscover.md) est peut-être dans l’ordre ? 
  
Pour plus d’informations sur la gestion des erreurs spécifiques, voir les articles suivants :
  
- [Gestion des messages d'erreur de découverte automatique](handling-autodiscover-error-messages.md)
    
- [Gestion des erreurs liées à la notification dans EWS dans Exchange](handling-notification-related-errors-in-ews-in-exchange.md)
    
- [Gestion des erreurs liées à la synchronisation dans EWS dans Exchange](handling-synchronization-related-errors-in-ews-in-exchange.md)
    
- [Gestion des erreurs liées aux suppression dans EWS dans Exchange](handling-deletion-related-errors-in-ews-in-exchange.md)
    
## <a name="verify-versions"></a>Vérifier les versions

Il existe un nombre de différents composants impliqués dans les opérations EWS et les versions de ces composants peuvent influer sur les résultats.
  
**Le tableau 1. Composants de versions susceptibles d’affecter les processus EWS**

|**Composant**|**API managée par EWS**|**EWS**|**Remarques**|
|:-----|:-----|:-----|:-----|
|Version du serveur demandée  <br/> |Propriété [ExchangeServiceBase.RequestedServerVersion](http://msdn.microsoft.com/EN-US/library/microsoft.exchange.webservices.data.exchangeservicebase.requestedserverversion%28v=exchg.80%29.aspx)  <br/> |Élément [RequestServerVersion](http://msdn.microsoft.com/library/af4032d5-42b3-463e-9d0a-8236d78e5b75%28Office.15%29.aspx)  <br/> |Cette valeur contrôle la version du schéma EWS est utilisée pour traiter la demande EWS. Assurez-vous que la version du schéma spécifiée dans ce champ est significatif pour la demande vous envoyez. Certaines propriétés et opérations ne sont pas disponibles dans les versions antérieures du schéma.  <br/> |
|La version du serveur  <br/> |Propriété [ExchangeServiceBase.ServerInfo](http://msdn.microsoft.com/EN-US/library/microsoft.exchange.webservices.data.exchangeservicebase.serverinfo%28v=exchg.80%29.aspx)  <br/> |Élément [ServerVersionInfo](http://msdn.microsoft.com/library/c04a6872-ca27-432b-aac2-36b023d0afc6%28Office.15%29.aspx)  <br/> |Cette valeur est retournée par le serveur dans les réponses EWS et indique la version du serveur qui a traité la réponse. Assurez-vous que cette valeur est ce que vous attendez. Si possible, assurez-vous que le serveur Exchange exécute la mise à jour les plus récent pour votre version majeure d’Exchange.  <br/> |
|La version de l’API managée EWS  <br/> |La propriété version de produit du fichier Microsoft.Exchange.WebServices.dll.  <br/> |Not applicable  <br/> |Si vous utilisez l’API managée EWS, assurez-vous que vous utilisez [la version la plus récente](http://aka.ms/ews-managed-api-readme).  <br/> |
   
## <a name="verify-access"></a>Vérifier l’accès

EWS est activée par défaut, mais [peut être modifié par défaut](how-to-control-access-to-ews-in-exchange.md). Utilisez l’applet de commande [Get-OrganizationConfig](http://technet.microsoft.com/en-us/library/bb124754.aspx) pour vous assurer que EWS est activée sur le serveur et l’applet de commande [Get-CASMailbox](http://technet.microsoft.com/en-us/library/aa997571.aspx) pour vous assurer que EWS est activé pour la boîte aux lettres de l’utilisateur. Vérifiez également les deux réponses de l’applet de commande pour un EWS autorisent ou bloquent la liste et vous assurer que votre application n’est pas bloquée à partir de l’aide de EWS. 
  
Vous devez également vérifier que les [paramètres d’authentification par défaut](http://technet.microsoft.com/en-us/library/gg247612%28v=exchg.150%29.aspx) dans le répertoire virtuel EWS n’ont pas été modifiés. 
  
## <a name="try-another-ews-client"></a>Essayer un autre client EWS

Il est parfois utile essayer la même requête à partir d’un autre client et comparer les résultats. Si un autre client obtient des résultats différents, quelle est la différence ? Déterminer quelle est la différence entre une demande réussie et une demande ayant échouée peut aider à expliquer pourquoi une requête particulière est défectueux.
  
Si vous pouvez écrire certainement un autre client pour le test, vous n’avez pas besoin ! [EWSEditor](http://ewseditor.codeplex.com/) est un exemple de client qui utilise les API managées EWS. Vous pouvez télécharger le client (y compris le code source) et l’utiliser pour essayer les mêmes requêtes sont défectueux dans votre application. 
  
## <a name="examine-iis-logs"></a>Examiner les journaux IIS

Si vous avez accès au serveur Exchange, la fonctionnalité de journalisation fournie par Internet Information Services (IIS) sur les serveurs d’accès au Client peut fournir plus d’informations sur les échecs. Toutefois, n’oubliez pas que les journaux IIS ne seront utiles si vous recevez une erreur HTTP.
  
IIS fournit deux méthodes de journalisation différentes : [échecs de demandes de suivi](http://www.iis.net/learn/troubleshoot/using-failed-request-tracing/troubleshooting-failed-requests-using-tracing-in-iis)et de [journalisation IIS](http://www.iis.net/learn/manage/provisioning-and-managing-iis/configure-logging-in-iis) . Pour travailler avec les journaux IIS, vous pouvez utiliser [Log Parser Studio](http://blogs.technet.com/b/exchange/archive/2012/03/07/introducing-log-parser-studio.aspx), qui comprend un nombre de requêtes EWS intégrées.
  
## <a name="next-steps"></a>Étapes suivantes
<a name="bk_NextSteps"> </a>

Maintenant que vous avez appris à utiliser les outils et les ressources que vous pouvez utiliser pour résoudre les problèmes, vous devrez comprendre les informations fournies par ces outils. Certaines options pour obtenir de l’aide sont les suivantes :
  
- [Forum de développement d’Exchange Server sur MSDN](http://social.msdn.microsoft.com/Forums/en-US/home?category=exchangeserver) : poser une question de la Communauté de développement MSDN Exchange Server. 
    
- [StackOverflow](http://stackoverflow.com/tags/ews) : poser une question de la Communauté StackOverflow. Veillez à ajouter une balise à votre publication avec « ews ». 
    
- [Prise en charge de Microsoft](http://support.microsoft.com/ph/730/en-us) , contactez le support technique Microsoft pour obtenir une assistance. 
    
## <a name="see-also"></a>Voir aussi


Voir les articles suivants :
  
- [Développer des clients de service web pour Exchange](develop-web-service-clients-for-exchange.md)
    
- [Suivi des demandes et réponses pour dépanner les applications de l’API managée EWS](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md)
    
- [L'instrumentation des demandes du client pour EWS et reste dans Exchange](instrumenting-client-requests-for-ews-and-rest-in-exchange.md)
    
- [Limitation EWS dans Exchange](ews-throttling-in-exchange.md)
    
- [Actualiser les informations de configuration à l’aide de découverte automatique](how-to-refresh-configuration-information-by-using-autodiscover.md)
    
- [Gestion des messages d'erreur de découverte automatique](handling-autodiscover-error-messages.md)
    
- [Gestion des erreurs liées à la notification dans EWS dans Exchange](handling-notification-related-errors-in-ews-in-exchange.md)
    
- [Gestion des erreurs liées à la synchronisation dans EWS dans Exchange](handling-synchronization-related-errors-in-ews-in-exchange.md)
    
- [Gestion des erreurs liées aux suppression dans EWS dans Exchange](handling-deletion-related-errors-in-ews-in-exchange.md)
    
- [Configuration de l’enregistrement dans IIS](http://www.iis.net/learn/manage/provisioning-and-managing-iis/configure-logging-in-iis)
    
- [Dépannage des échecs de demandes à l’aide de suivi dans IIS 7](http://www.iis.net/learn/troubleshoot/using-failed-request-tracing/troubleshooting-failed-requests-using-tracing-in-iis)
    
- [Présentation : Log Parser Studio](http://blogs.technet.com/b/exchange/archive/2012/03/07/introducing-log-parser-studio.aspx)
    
- [Paramètres par défaut des répertoires virtuels Exchange](http://technet.microsoft.com/en-us/library/gg247612%28v=exchg.150%29.aspx)
    
Télécharger les éléments suivants :
  
- [Moniteur réseau Microsoft 3.4](http://www.microsoft.com/en-us/download/details.aspx?id=4865)
    
- [Fiddler](http://www.telerik.com/fiddler)
    
- [EWSEditor](http://ewseditor.codeplex.com/)
    
- [API gérée Exchange Web Services](http://go.microsoft.com/fwlink/?LinkID=255472)
    

