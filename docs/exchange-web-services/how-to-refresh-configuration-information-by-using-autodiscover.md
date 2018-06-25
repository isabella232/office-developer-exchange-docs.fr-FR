---
title: Actualiser les informations de configuration à l’aide de découverte automatique
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: c2f3c6a5-e8ea-4375-b41a-686a6f238d33
description: Découvrez comment et quand pour actualiser les informations de configuration de votre connexion à Exchange à l’aide de découverte automatique.
ms.openlocfilehash: ef3b61781cbafa6e7b873336a050c0b8c33a28ec
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754954"
---
# <a name="refresh-configuration-information-by-using-autodiscover"></a>Actualiser les informations de configuration à l’aide de découverte automatique

Découvrez comment et quand pour actualiser les informations de configuration de votre connexion à Exchange à l’aide de découverte automatique.
  
Lorsque votre application EWS s’exécute pour la première fois, découverte automatique fournit un excellent moyen pour collecter les informations que nécessaires pour pouvoir se connecter à la boîte aux lettres Exchange de l’utilisateur. Mais la découverte automatique n’est pas seulement pour la première utilisation. À l’aide de la découverte automatique sur une base régulière peut aider votre application connectée en l’activant pour répondre aux modifications dans le déploiement d’Exchange.
  
## <a name="cache-autodiscover-endpoint-and-ews-settings"></a>Cache du point de terminaison de découverte automatique et paramètres EWS
<a name="bk_CacheSettings"> </a>

Tout en nous conseillé d’utiliser la découverte automatique régulièrement, vous utilisez comment régulièrement il exige certains. Idéalement, vous pouvez équilibrer répondre rapidement aux modifications dans l’environnement par rapport à la génération de trop de trafic réseau inutile. Lorsque votre application reçoit une réponse positive de découverte automatique pour la première fois, vous devez enregistrer les informations suivantes afin que vous n’êtes pas obligé de Répétez le processus de découverte automatique chaque fois que vous envoyez une demande EWS.
  
**Le tableau 1. Informations de cache pour les demandes de découverte automatique**

|**Paramètre de cache**|**Valide pour...**|**Détails**|
|:-----|:-----|:-----|
|Point de terminaison de découverte automatique  <br/> |Dans la mesure où elle fonctionne.  <br/> |Lorsque vous enregistrez le point de terminaison de découverte automatique qui a renvoyé une réponse positive, vous n’êtes pas obligé de Répétez le processus de [génération d’une liste de points de terminaison de découverte automatique](how-to-generate-a-list-of-autodiscover-endpoints.md) et à les essayer jusqu'à ce que vous obtenez une réponse positive.<br/><br/> **Remarque**: l’API managées ne gère pas le point de terminaison de découverte automatique de la mise en cache.           |
|URL EWS et tous les autres paramètres sont récupérées à partir de la réponse de découverte automatique  <br/> |24 heures  <br/> |En enregistrant le URL EWS et autres des paramètres liés, vous ne disposez pas d' [Envoyer une nouvelle demande de découverte automatique](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) pour chaque demande EWS ou si votre application redémarre. Toutefois, même si une URL EWS fonctionne pour vos utilisateurs, un serveur peut être disponible et plus efficace.<br/><br/> Par exemple, boîte aux lettres de l’utilisateur a peut-être été déplacée vers un nouveau serveur de boîtes aux lettres, entraînant un nouveau point de terminaison EWS par défaut. Nous vous recommandons d’actualiser vos paramètres de l’utilisateur en envoyant une nouvelle demande de découverte automatique après que 24 heures se sont écoulées depuis votre dernière demande de découverte automatique. Ce temps peut être ajustée pour satisfaire les besoins de votre application.  <br/> |
   
## <a name="refresh-cached-configuration-information"></a>Actualiser les informations de configuration mises en cache
<a name="bk_RefreshConfig"> </a>

Maintenant que vous avez mis en cache, examinons comment vous pouvez conserver ce cache vierge. Nous vous recommandons d’actualiser vos informations de mise en cache lorsque :
  
- Expiration de la période de validité de l’information.
    
- Des [erreurs liées à la connexion](#bk_ConnectionErrors) se produit. 
    
Pour actualiser vos informations de mise en cache, envoyez une demande de découverte automatique pour un point de terminaison de découverte automatique mis en cache et procédez comme suit :
  
- Si la demande réussit, comparer le point de terminaison EWS dans la réponse avec un point de terminaison EWS mis en cache et procédez comme suit :
    
  - Si elles sont différentes, utilisez le nouveau point de terminaison EWS. Si vous êtes l’actualisation pour récupérer d’une erreur, réessayez la demande a échoué avec le nouveau point de terminaison.
    
  - Si elles sont les mêmes, continuer à utiliser le point de terminaison EWS d’origine. Si vous êtes l’actualisation pour récupérer d’une erreur, gérer l’erreur comme il convient.
    
- En cas d’échec de la demande, démarrer le [processus de découverte automatique](autodiscover-for-exchange.md) à partir du début. Une fois que vous obtenez une réponse positive, remplacez le point de terminaison de découverte automatique mis en cache par le point de terminaison de découverte automatique qui a réussi et continue à utiliser le nouveau point de terminaison EWS. Si vous n’obtenez pas une réponse positive, continuer à utiliser le point de terminaison de découverte automatique d’origine et le point de terminaison EWS. Si vous êtes l’actualisation pour récupérer d’une erreur, gérer l’erreur comme il convient. 
    
L’illustration suivante fournit une représentation visuelle de ce processus.
  
**La figure 1. Processus d’actualisation des informations de configuration à l’aide de découverte automatique**

![Diagramme schématique indiquant comment la découverte automatique actualise les informations de configuration.](media/Ex15_Autodiscover_Refresh_Flowchart.png)
  
### <a name="connection-related-errors"></a>Erreurs liées à la connexion
<a name="bk_ConnectionErrors"> </a>

L’actualisation de vos informations de configuration de mise en cache peut aider avec des erreurs, mais pas toutes. 
  
**Le tableau 2. Erreurs adressées par l’actualisation de votre cache**

|**Erreur**|**Implémentation de l’API managée EWS**|**Remarques**|
|:-----|:-----|:-----|
|Erreurs d’échec de réseau ou DNS<br/><br/> Exemple : Nom d’hôte est introuvable.  <br/> |[ServiceRemoteException](https://msdn.microsoft.com/library/Microsoft.Exchange.WebServices.Data.ServiceRemoteException.aspx) <br/> |Une erreur indiquant que le serveur est introuvable ou ne peut pas être joint peut être résolue en essayant de découverte automatique. <br/><br/> Votre point de terminaison EWS mis en cache peut-être ne plus être valide, et la découverte automatique peut être en mesure de vous pointez vers le nouveau serveur.  <br/> |
|Erreurs d’état HTTP<br/><br/> Exemple : 503 Service indisponible  <br/> |[ServiceRemoteException](https://msdn.microsoft.com/library/Microsoft.Exchange.WebServices.Data.ServiceRemoteException.aspx) <br/> |Erreurs d’état HTTP peuvent se produire pour différentes raisons.<br/><br/> Toutefois, il est conseillé d’essayer de découverte automatique pour voir si un nouveau point de terminaison EWS est disponible pour l’utilisateur.  <br/> |
|Codes d’erreur EWS <br/><br/> Exemple : ErrorConnectionFailed <br/> |[ResponseCodeType](https://msdn.microsoft.com/library/Microsoft.Exchange.WebServices.Data.ResponseCodeType.aspx) <br/> | La plupart des codes d’erreur EWS ne justifient l’actualisation de vos informations de configuration.<br/><br/> Toutefois, les éléments suivants spécifiquement indiquent que les informations de configuration doivent être mis à jour :<br/>- **ErrorConnectionFailed** <br/>- **ErrorMailboxMoveInProgress** <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Découverte automatique pour Exchange](autodiscover-for-exchange.md)  
- [Générer une liste des points de terminaison de découverte automatique](how-to-generate-a-list-of-autodiscover-endpoints.md)   
- [Obtenir les paramètres de l’utilisateur Exchange à l’aide de découverte automatique](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)
    

