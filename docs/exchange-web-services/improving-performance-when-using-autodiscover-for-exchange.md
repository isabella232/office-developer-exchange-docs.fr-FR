---
title: Amélioration des performances lors de l'utilisation de la fonctionnalité de découverte automatique pour Exchange
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: e65ff6b2-3810-43ad-9728-27308891b193
description: Découvrez comment améliorer les performances du processus de découverte automatique dans votre application.
ms.openlocfilehash: c0920f71c230f63658dfa8d29b34ca75bb796db0
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59520996"
---
# <a name="improving-performance-when-using-autodiscover-for-exchange"></a>Amélioration des performances lors de l'utilisation de la fonctionnalité de découverte automatique pour Exchange

Ce document peut contenir des informations liées aux fonctionnalités ou produits préliminaires qui sont sujettes à modifications avant la sortie de la version définitive. Ce document est fourni "tel quel" à titre indicatif et Microsoft exclut toute garantie, expresse ou implicite, en ce qui concerne ce document. Découvrez comment améliorer les performances du processus de découverte automatique dans votre application.
  
Il existe un grand nombre de raisons telles que la découverte automatique. Configuration de votre application pour se connecter à Exchange sans intervention de l'utilisateur est parfait ! Si vous êtes en train de lire cet article, vous savez probablement déjà toutes les raisons d'utiliser et d'amour de découverte automatique, afin que nous ne les avez répertoriés ici. Au lieu de cela, nous allons parler à un inconvénient : performances.
  
Découverte automatique n'est pas fondamentalement un processus lent, mais il n'est pas fondamentalement fast soit. Le [processus de découverte automatique](autodiscover-for-exchange.md) implique un grand nombre d'activité réseau, et qui présente un grand nombre de risque de délais. Le processus de découverte automatique comprend trois phases ; les trois sont susceptibles d'affecter les performances : 
  
- Définition du pool de candidats de découverte automatique du point de terminaison  pour les applications qui s'exécutent sur des ordinateurs à un domaine, cela peut impliquer des [recherches de SCP](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md), ce qui implique la communication avec les Services de domaine Active Directory (AD DS).
    
- Vous essayez de chaque candidat  cela nécessite une demande/réponse HTTP à chaque point de terminaison du candidat.
    
- Test d'autres alternatives  lorsque les candidats dans votre pool de candidat de point de terminaison de découverte automatique ne pas produire des résultats, vous pouvez effectuer une demande GET non authentifiée (demande/réponse HTTP) et une recherche DNS.
    
Sur la surface cela ne semble pas beaucoup. Toutefois, imaginons un scénario où le pool de candidat de point de terminaison de découverte automatique est plus d'un ou deux URL, et vous ne trouvez pas une travail 1 jusqu'à ce que la dernière URL dans votre pool. Le délai peut devenir un peu plus évident. Par conséquent, quelles sont les possibilités ?
  
## <a name="consider-the-need-for-scp-lookup"></a>Envisager la nécessité de recherche SCP

Lorsque les objets SCP sont présentes et correctement configurés, ils peuvent accélérer le processus de découverte automatique. Dans d'autres cas, toutefois, elles peuvent ralentir il. Si SCP n'est pas utilisée dans votre environnement, passez à la partie de recherche SCP entière du processus de découverte automatique pour économiser du temps.
  
L'API managée EWS facilite cette tâche : définissez simplement la propriété [ExchangeService.EnableScpLookup](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.enablescplookup%28v=exchg.80%29.aspx) à **false** avant d'appeler la méthode [ExchangeService.AutodiscoverUrl](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.autodiscoverurl%28v=exchg.80%29.aspx) . Si vous utilisez la classe [AutodiscoverService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.autodiscover.autodiscoverservice%28v=exchg.80%29.aspx) , définissez la propriété [AutodiscoverService.EnableScpLookup](https://msdn.microsoft.com/library/microsoft.exchange.webservices.autodiscover.autodiscoverservice.enablescplookup%28v=exchg.80%29.aspx) à **false** avant d'appeler une de ses méthodes. 
  
## <a name="use-autodiscover-less-often"></a>Utiliser la découverte automatique moins souvent

Découverte automatique n'est pas conçue pour être utilisée fréquemment utiliser par les applications. L'intention de découverte automatique est une application peut utiliser pour découvrir les informations de configuration, puis mettre en cache ces informations pendant une période de temps. Si vous n'êtes pas en cache les informations de configuration, songez à ajouter à votre application pour réduire le nombre de fois que vous utilisez la découverte automatique la mise en cache.
  
Même si vous mettez en cache déjà, évaluez la durée pendant laquelle vous mettez en cache les informations de configuration. La norme est pour [Actualiser les informations de découverte automatique toutes les 24 heures](how-to-refresh-configuration-information-by-using-autodiscover.md), mais vous ne pourrez pas étendre ce moment-là. Vous devez tester avec vos environnements cibles et élaborer un « time-to-live » pour votre configuration fonctionne pour vous.
  
## <a name="minimize-requested-data"></a>Réduire les données demandées

Si vous utilisez la classe **AutodiscoverService** dans l'API managée EWS, ou de l'opération [Opération GetUserSettings (SOAP)](https://msdn.microsoft.com/library/758d965c-ef63-4de4-9120-e293abf14ff8%28Office.15%29.aspx) via SOAP, vous disposez d'un contrôle direct sur les paramètres sont retournés dans la réponse. Bien que vous pouvez demander un certain paramètres, sans doute que votre application doit uniquement un petit nombre d'entre eux. Tous les paramètres que vous demandez nécessitent plus de traitement sur le serveur, ce qui signifie davantage de temps en attente d'une réponse. Évaluer les paramètres que vous demandez et d'éliminer celles que vous n'avez pas besoin. 
  
Si vous utilisez la méthode **ExchangeService.AutodiscoverUrl** dans l'API managée EWS, vous ne pouvez pas modifier les paramètres que vous demandez. Toutefois, cette méthode est déjà assez efficace ; il demande uniquement les paramètres **ExternalEwsUrl** et **InternalEwsUrl** à partir de l' [énumération de UserSettingName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.autodiscover.usersettingname%28v=exchg.80%29.aspx).
  
Si vous utilisez le service de découverte automatique POX, [vous ne pouvez pas demander des propriétés spécifiques](autodiscover-for-exchange.md#bk_Options).
  
## <a name="see-also"></a>Voir aussi


- [Découverte automatique pour Exchange](autodiscover-for-exchange.md)
    
- [Trouver des points de terminaison de découverte automatique à l’aide de la recherche SCP dans Exchange](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md)
    
- [Actualiser les informations de configuration à l’aide de la découverte automatique](how-to-refresh-configuration-information-by-using-autodiscover.md)
    
- [Classe de ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)
    
- [Classe de AutodiscoverService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.autodiscover.autodiscoverservice%28v=exchg.80%29.aspx)
    

