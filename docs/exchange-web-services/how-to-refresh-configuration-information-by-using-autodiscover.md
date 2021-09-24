---
title: Actualiser les informations de configuration à l’aide de la découverte automatique
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: c2f3c6a5-e8ea-4375-b41a-686a6f238d33
description: Découvrez comment et quand actualiser les informations de configuration de votre Exchange à l’aide de la découverte automatique.
ms.openlocfilehash: 0ec6910fcd8ab66085de2414f02a4f78419ec78b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513114"
---
# <a name="refresh-configuration-information-by-using-autodiscover"></a>Actualiser les informations de configuration à l’aide de la découverte automatique

Découvrez comment et quand actualiser les informations de configuration de votre Exchange à l’aide de la découverte automatique.
  
Lorsque votre application EWS s’exécute pour la première fois, la découverte automatique vous offre un excellent moyen de collecter les informations dont vous avez besoin pour vous connecter à la boîte aux lettres Exchange de votre utilisateur. Toutefois, la découverte automatique n’est pas seulement pour la première utilisation. L’utilisation régulière de la découverte automatique peut aider à maintenir votre application connectée en lui permettant de répondre aux modifications apportées au Exchange déploiement.
  
## <a name="cache-autodiscover-endpoint-and-ews-settings"></a>Mettre en cache le point de terminaison de découverte automatique et les paramètres EWS
<a name="bk_CacheSettings"> </a>

Bien qu’il soit recommandé d’utiliser la découverte automatique régulièrement, il est recommandé d’en tenir compte. Dans l’idéal, vous pouvez trouver un équilibre entre répondre rapidement aux modifications de l’environnement et générer trop de trafic réseau inutile. Lorsque votre application obtient une réponse de découverte automatique réussie pour la première fois, vous devez enregistrer les informations suivantes afin de ne pas avoir à répéter le processus de découverte automatique chaque fois que vous envoyez une demande EWS.
  
**Tableau 1. Informations à mettre en cache pour les demandes de découverte automatique**

|**Paramètre de mise en cache**|**Valide pour...**|**Détails**|
|:-----|:-----|:-----|
|Point de terminaison de découverte automatique  <br/> |Tant que cela fonctionne  <br/> |Lorsque vous enregistrez le point de terminaison de découverte automatique qui a [](how-to-generate-a-list-of-autodiscover-endpoints.md) renvoyé une réponse réussie, vous n’avez pas besoin de répéter le processus de génération d’une liste de points de terminaison de découverte automatique et d’essai jusqu’à ce que vous receviez une réponse réussie.<br/><br/> **REMARQUE**: l’API gérée EWS ne prend pas en charge la mise en cache du point de terminaison de découverte automatique.           |
|URL EWS et autres paramètres récupérés à partir de la réponse de découverte automatique  <br/> |Une semaine  <br/> |En saving the EWS URL and other related settings, you do not have to [send a new Autodiscover request](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) for each EWS request or if your application restarts. Toutefois, même si une URL EWS fonctionne pour votre utilisateur, un serveur peut être disponible plus optimal.<br/><br/> Par exemple, la boîte aux lettres de l’utilisateur peut avoir été déplacée vers un nouveau serveur de boîtes aux lettres, ce qui a pour résultat un nouveau point de terminaison EWS préféré. Nous vous recommandons d’actualiser vos paramètres utilisateur en envoyant une nouvelle demande de découverte automatique après une semaine écoulée depuis votre dernière demande de découverte automatique. Ce délai peut être ajusté pour répondre aux exigences de votre application.  <br/> |
   
## <a name="refresh-cached-configuration-information"></a>Actualiser les informations de configuration mises en cache
<a name="bk_RefreshConfig"> </a>

Maintenant que vous avez les informations mises en cache, examinons comment vous pouvez conserver ce cache à jour. Nous vous recommandons d’actualiser vos informations mises en cache lorsque :
  
- La période de validité des informations expire.
    
- Une [erreur liée à la connexion](#bk_ConnectionErrors) se produit ET vos informations mises en cache ont été actualisées pour la dernière fois il y a plus d’une heure.
    
Pour actualiser vos informations mises en cache, envoyez une demande de découverte automatique à un point de terminaison de découverte automatique mis en cache et faites les choses suivantes :
  
- Si la demande réussit, comparez le point de terminaison EWS dans la réponse au point de terminaison EWS mis en cache, puis faites ce qui suit :
    
  - S’ils sont différents, utilisez le nouveau point de terminaison EWS. Si vous l’actualisation pour récupérer à partir d’une erreur, réessayez la demande ayant échoué avec le nouveau point de terminaison.
    
  - S’ils sont identiques, continuez à utiliser le point de terminaison EWS d’origine. Si vous l’actualisation pour récupérer à partir d’une erreur, traitez l’erreur selon le cas.
    
- Si la demande échoue, démarrez le processus de [découverte automatique](autodiscover-for-exchange.md) à partir du début. Une fois que vous avez réussi, remplacez le point de terminaison de découverte automatique mis en cache par le point de terminaison de découverte automatique qui a réussi et continuez à utiliser le nouveau point de terminaison EWS. Si vous n’obtenez pas de réponse réussie, continuez à utiliser le point de terminaison de découverte automatique d’origine et le point de terminaison EWS. Si vous l’actualisation pour récupérer à partir d’une erreur, traitez l’erreur selon le cas. 
    
La figure suivante fournit une représentation visuelle de ce processus.
  
**Figure 1. Processus d’actualisation des informations de configuration à l’aide de la découverte automatique**

![Diagramme schématique indiquant comment la découverte automatique actualise les informations de configuration.](media/Ex15_Autodiscover_Refresh_Flowchart.png)
  
### <a name="connection-related-errors"></a>Erreurs liées à la connexion
<a name="bk_ConnectionErrors"> </a>

L’actualisation de vos informations de configuration mises en cache peut vous aider à corriger certaines erreurs, mais pas toutes. 
  
**Tableau 2. Erreurs traitées par l’actualisation de votre cache**

|**Erreur**|**Implémentation de l’API gérée EWS**|**Remarques**|
|:-----|:-----|:-----|
|Erreurs DNS ou de défaillance du réseau<br/><br/> Exemple : Nom d’hôte in trouvé.  <br/> |[ServiceRemoteException](https://docs.microsoft.com/dotnet/api/microsoft.exchange.webservices.data.serviceremoteexception?view=exchange-ews-api) <br/> |Toute erreur qui indique que le serveur est introuvable ou introuvable peut être résolue par une tentative de découverte automatique. <br/><br/> Votre point de terminaison EWS mis en cache n’est peut-être plus valide et la découverte automatique peut vous faire pointer vers le nouveau serveur.  <br/> |
|Erreurs d’état HTTP<br/><br/> Exemple : Service 503 indisponible  <br/> |[ServiceRemoteException](https://docs.microsoft.com/dotnet/api/microsoft.exchange.webservices.data.serviceremoteexception?view=exchange-ews-api) <br/> |Les erreurs d’état HTTP peuvent se produire pour de nombreuses raisons différentes.<br/><br/> Toutefois, il est bon d’essayer la découverte automatique pour voir si un nouveau point de terminaison EWS est disponible pour l’utilisateur.  <br/> |
|Codes d’erreur EWS <br/><br/> Exemple : ErrorConnectionFailed <br/> |[ResponseCodeType](../web-service-reference/responsecode.md) <br/> | La plupart des codes d’erreur EWS ne justifient pas l’actualisation de vos informations de configuration.<br/><br/> Toutefois, les éléments suivants indiquent spécifiquement que les informations de configuration doivent être mises à jour :<br/>- **ErrorConnectionFailed** <br/>- **ErrorMailboxMoveInProgress** <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Découverte automatique pour Exchange](autodiscover-for-exchange.md)  
- [Générer une liste de points de terminaison de découverte automatique](how-to-generate-a-list-of-autodiscover-endpoints.md)   
- [Obtenir les paramètres de l'utilisateur Exchange à l'aide de découverte automatique](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)
    

