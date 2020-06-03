---
title: Outils et ressources pour la résolution des applications EWS pour Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.assetid: ee7fcd05-35d7-47bf-bac4-e719c49c11fe
description: Trouvez des ressources qui vous aideront à dépanner votre API managée EWS ou votre application EWS.
localization_priority: Priority
ms.openlocfilehash: 7c7cbe8c93edec5ad99df079c6eb96286c1ba063
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463740"
---
# <a name="tools-and-resources-for-troubleshooting-ews-applications-for-exchange"></a>Outils et ressources pour la résolution des applications EWS pour Exchange

Trouvez des ressources qui vous aideront à dépanner votre API managée EWS ou votre application EWS.
  
Les choses ne sont pas toujours aussi planifiées. Parfois, les requêtes EWS échouent ou fournissent des résultats inattendus. Cela peut être frustrant, surtout si la raison n’est pas évidente. Nous espérons que cela ne vous arrivera jamais, mais si c’est le cas, cet article fournit des informations sur les outils et les ressources que vous pouvez utiliser pour vous aider à résoudre votre problème.
  
> [!NOTE]
> Cet article fournit des conseils et sources de dépannage généraux pour obtenir des informations de résolution des problèmes. Malheureusement, il n’est pas possible d’indiquer des étapes de résolution des problèmes détaillées. Pour obtenir de l’aide sur la résolution des erreurs, consultez la section [étapes suivantes](#bk_NextSteps). 
  
## <a name="examine-the-soap-requests-and-responses"></a>Examiner les demandes et les réponses SOAP

Lorsque les éléments ne fonctionnent pas correctement, il est vraiment utile de pouvoir voir ce qui se passe. La première ligne de consultation lors de l’enquête sur un problème avec EWS ou l’API managée EWS consiste à examiner les demandes que votre application envoie sur le réseau et les réponses renvoyées par le serveur.
  
L’API managée EWS facilite l’examen des demandes et des réponses SOAP grâce à sa [fonctionnalité de suivi intégrée](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md). Si vous utilisez EWS, il se peut que vous ayez ou non accès à une fonctionnalité de suivi similaire, en fonction de la plateforme ou des classes que vous utilisez pour envoyer vos demandes. Toutefois, vous pouvez toujours utiliser un outil de suivi réseau tel que le [Moniteur réseau](https://www.microsoft.com/download/details.aspx?id=4865) ou [Fiddler](http://www.telerik.com/fiddler) pour examiner le trafic réseau et afficher les charges utiles de demande et de réponse. 
  
En outre, vous pouvez [instrumenter vos demandes client](instrumenting-client-requests-for-ews-and-rest-in-exchange.md) pour améliorer les informations disponibles dans les demandes et les réponses. 
  
Une fois que vous avez les demandes et les réponses, posez-vous les questions suivantes : est-ce qu’elles semblent correctes ? Les valeurs envoyées par votre application sont-elles prévues ? Les réponses ont-elles un sens ?
  
## <a name="examine-error-codes"></a>Examiner les codes d’erreur

Parfois, le code d’erreur peut être très utile pour identifier le problème, même si, à première vue, il ne semble pas logique. L’erreur indique-t-elle que votre client est [limité](ews-throttling-in-exchange.md)? Un appel à la découverte automatique pour [Actualiser les informations de configuration](how-to-refresh-configuration-information-by-using-autodiscover.md) est peut-être dans l’ordre ? 
  
Pour plus d’informations sur la gestion des erreurs spécifiques, consultez les articles suivants :
  
- [Gestion des messages d'erreur de découverte automatique](handling-autodiscover-error-messages.md)
    
- [Gestion des erreurs liées à la notification dans EWS dans Exchange](handling-notification-related-errors-in-ews-in-exchange.md)
    
- [Gestion des erreurs liées à la synchronisation dans EWS dans Exchange](handling-synchronization-related-errors-in-ews-in-exchange.md)
    
- [Gestion des erreurs liées à la suppression dans EWS dans Exchange](handling-deletion-related-errors-in-ews-in-exchange.md)
    
## <a name="verify-versions"></a>Vérifier les versions

Il existe un certain nombre de composants différents impliqués dans les opérations EWS et les versions de ces composants peuvent influencer les résultats.
  
**Tableau 1. Composants avec version pouvant affecter les processus EWS**

|**Composant**|**API managée EWS**|**EWS**|**Remarques**|
|:-----|:-----|:-----|:-----|
|Version du serveur demandée  <br/> |Propriété [ExchangeServiceBase. RequestedServerVersion](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.requestedserverversion%28v=exchg.80%29.aspx)  <br/> |Élément [RequestServerVersion](https://msdn.microsoft.com/library/af4032d5-42b3-463e-9d0a-8236d78e5b75%28Office.15%29.aspx)  <br/> |Cette valeur détermine la version du schéma EWS qui est utilisée pour traiter la demande EWS. Assurez-vous que la version de schéma spécifiée ici est pertinente pour la demande que vous envoyez. Certaines propriétés et opérations ne sont pas disponibles dans les versions antérieures du schéma.  <br/> |
|La version du serveur  <br/> |Propriété [ExchangeServiceBase. informations](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.serverinfo%28v=exchg.80%29.aspx)  <br/> |Élément [ServerVersionInfo](https://msdn.microsoft.com/library/c04a6872-ca27-432b-aac2-36b023d0afc6%28Office.15%29.aspx)  <br/> |Cette valeur est renvoyée par le serveur dans les réponses EWS et indique la version du serveur qui a traité la réponse. Assurez-vous que cette valeur est celle que vous attendez. Si possible, assurez-vous que le serveur Exchange exécute la mise à jour la plus récente pour votre version principale d’Exchange.  <br/> |
|Version de l’API managée EWS  <br/> |Propriété de version du produit du fichier Microsoft. Exchange. WebServices. dll.  <br/> |Non applicable  <br/> |Si vous utilisez l’API managée EWS, assurez-vous que vous utilisez [la version la plus récente](https://aka.ms/ews-managed-api-readme).  <br/> |
   
## <a name="verify-access"></a>Vérifier l’accès

EWS est activé par défaut, mais les [valeurs par défaut peuvent être modifiées](how-to-control-access-to-ews-in-exchange.md). Utilisez la cmdlet [Get-OrganizationConfig](https://technet.microsoft.com/library/bb124754.aspx) pour vous assurer que EWS est activé sur le serveur, et la cmdlet [Get-CASMailbox](https://technet.microsoft.com/library/aa997571.aspx) pour s’assurer que EWS est activé pour la boîte aux lettres de l’utilisateur. Vérifiez également les deux réponses de cmdlet pour une liste verte ou une liste rouge EWS, et assurez-vous que votre application n’est pas bloquée via EWS. 
  
Vous devez également vérifier que les [paramètres d’authentification par défaut](https://technet.microsoft.com/library/gg247612%28v=exchg.150%29.aspx) sur le répertoire virtuel EWS n’ont pas été modifiés. 
  
## <a name="try-another-ews-client"></a>Essayer un autre client EWS

Parfois, il est utile d’essayer la même demande à partir d’un autre client et de comparer les résultats. Si un autre client obtient des résultats différents, qu’est-ce qui est différent ? Déterminer les différences entre une demande réussie et une demande ayant échoué peut vous aider à expliquer pourquoi une requête particulière est défectueuse.
  
Bien que vous puissiez certainement écrire un autre client pour le test, vous n’avez pas besoin de le faire ! [EWSEditor](http://ewseditor.codeplex.com/) est un exemple de client qui utilise l’API managée EWS et EWS. Vous pouvez télécharger le client (y compris le code source) et l’utiliser pour essayer les mêmes requêtes qui échouent dans votre application. 
  
## <a name="examine-iis-logs"></a>Examiner les journaux IIS

Si vous avez accès au serveur Exchange, les fonctionnalités de journalisation fournies par les services Internet (IIS) sur les serveurs d’accès au client peuvent fournir des informations supplémentaires sur les échecs. Toutefois, gardez à l’esprit que les journaux IIS ne seront utiles que si vous recevez une erreur HTTP.
  
Les services Internet (IIS) fournissent deux méthodes de journalisation : [le suivi des demandes ayant échoué](http://www.iis.net/learn/troubleshoot/using-failed-request-tracing/troubleshooting-failed-requests-using-tracing-in-iis)et la [journalisation IIS](http://www.iis.net/learn/manage/provisioning-and-managing-iis/configure-logging-in-iis) . Pour utiliser les journaux IIS, vous pouvez utiliser [Log Parser Studio](https://blogs.technet.com/b/exchange/archive/2012/03/07/introducing-log-parser-studio.aspx), qui inclut un certain nombre de requêtes EWS intégrées.
  
## <a name="next-steps"></a>Étapes suivantes
<a name="bk_NextSteps"> </a>

À présent que vous avez appris à connaître les outils et les ressources que vous pouvez utiliser pour résoudre les problèmes, vous aurez peut-être besoin de comprendre les informations fournies par ces outils. Voici quelques options permettant d’obtenir de l’aide :
  
- [Forum de développement Exchange Server sur MSDN](https://social.msdn.microsoft.com/Forums/home?category=exchangeserver) : Posez une question à la communauté de développement Exchange Server MSDN. 
    
- [StackOverflow](http://stackoverflow.com/tags/ews) : Posez une question sur la communauté StackOverflow. N’oubliez pas de baliser votre billet avec « EWS ». 
    
- [Support Microsoft](https://support.microsoft.com/ph/730/en-us) : contactez un professionnel du support technique Microsoft pour obtenir de l’aide. 
    
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
    
- [Dépannage des demandes ayant échoué à l’aide du suivi dans IIS 7](http://www.iis.net/learn/troubleshoot/using-failed-request-tracing/troubleshooting-failed-requests-using-tracing-in-iis)
    
- [Présentation : Log Parser Studio](https://blogs.technet.com/b/exchange/archive/2012/03/07/introducing-log-parser-studio.aspx)
    
- [Paramètres par défaut des répertoires virtuels Exchange](https://technet.microsoft.com/library/gg247612%28v=exchg.150%29.aspx)
    
Téléchargez les éléments suivants :
  
- [Moniteur réseau Microsoft 3.4](https://www.microsoft.com/download/details.aspx?id=4865)
    
- [Fiddler](http://www.telerik.com/fiddler)
    
- [EWSEditor](http://ewseditor.codeplex.com/)
    
- [API gérée Exchange Web Services](https://go.microsoft.com/fwlink/?LinkID=255472)
    

